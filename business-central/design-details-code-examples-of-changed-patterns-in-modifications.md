---
title: Design Details - Closing Demand and Supply | Microsoft Docs
description: When the supply balancing procedures have been performed, there are three possible end situations.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 2be48e11d562f469ab9ef5ac156fdeb46ea51107
ms.contentlocale: en-nz
ms.lasthandoff: 03/22/2018

---
# <a name="design-details-closing-demand-and-supply"></a><span data-ttu-id="76e83-103">Design Details: Closing Demand and Supply</span><span class="sxs-lookup"><span data-stu-id="76e83-103">Design Details: Closing Demand and Supply</span></span>
<span data-ttu-id="76e83-104">When the supply balancing procedures have been performed, there are three possible end situations:</span><span class="sxs-lookup"><span data-stu-id="76e83-104">When the supply balancing procedures have been performed, there are three possible end situations:</span></span>  

-   <span data-ttu-id="76e83-105">The required quantity and date of the demand events have been met and the planning for them can be closed.</span><span class="sxs-lookup"><span data-stu-id="76e83-105">The required quantity and date of the demand events have been met and the planning for them can be closed.</span></span> <span data-ttu-id="76e83-106">The supply event is still open and may be able to cover the next demand, so the balancing procedure can start over with the current supply event and the next demand.</span><span class="sxs-lookup"><span data-stu-id="76e83-106">The supply event is still open and may be able to cover the next demand, so the balancing procedure can start over with the current supply event and the next demand.</span></span>  

-   <span data-ttu-id="76e83-107">The supply order cannot be modified to cover all of the demand.</span><span class="sxs-lookup"><span data-stu-id="76e83-107">The supply order cannot be modified to cover all of the demand.</span></span> <span data-ttu-id="76e83-108">The demand event is still open, with some uncovered quantity that may be covered by the next supply event.</span><span class="sxs-lookup"><span data-stu-id="76e83-108">The demand event is still open, with some uncovered quantity that may be covered by the next supply event.</span></span> <span data-ttu-id="76e83-109">Thus the current supply event is closed, so the balancing act can start over with the current demand and the next supply event.</span><span class="sxs-lookup"><span data-stu-id="76e83-109">Thus the current supply event is closed, so the balancing act can start over with the current demand and the next supply event.</span></span>  

-   <span data-ttu-id="76e83-110">All of the demand has been covered; there is no subsequent demand (or there has been no demand at all).</span><span class="sxs-lookup"><span data-stu-id="76e83-110">All of the demand has been covered; there is no subsequent demand (or there has been no demand at all).</span></span> <span data-ttu-id="76e83-111">If there is any surplus supply, it may be decreased (or cancelled) and then closed.</span><span class="sxs-lookup"><span data-stu-id="76e83-111">If there is any surplus supply, it may be decreased (or canceled) and then closed.</span></span> <span data-ttu-id="76e83-112">It is possible that additional supply events exist further along in the chain, and they should also be cancelled.</span><span class="sxs-lookup"><span data-stu-id="76e83-112">It is possible that additional supply events exist further along in the chain, and they should also be canceled.</span></span>  

 <span data-ttu-id="76e83-113">Last, the planning system will create an order tracking link between the supply and the demand.</span><span class="sxs-lookup"><span data-stu-id="76e83-113">Last, the planning system will create an order tracking link between the supply and the demand.</span></span>  

## <a name="creating-the-planning-line-suggested-action"></a><span data-ttu-id="76e83-114">Creating the Planning Line (Suggested Action)</span><span class="sxs-lookup"><span data-stu-id="76e83-114">Creating the Planning Line (Suggested Action)</span></span>  
 <span data-ttu-id="76e83-115">If any action – New, Change Quantity, Reschedule, Reschedule and Change Quantity, or Cancel – is suggested to revise the supply order, the planning system creates a planning line in the planning worksheet.</span><span class="sxs-lookup"><span data-stu-id="76e83-115">If any action – New, Change Quantity, Reschedule, Reschedule and Change Quantity, or Cancel – is suggested to revise the supply order, the planning system creates a planning line in the planning worksheet.</span></span> <span data-ttu-id="76e83-116">Due to order tracking, the planning line is created not only when the supply event is closed, but also if the demand event is closed, even though the supply event is still open and may be subject to additional changes when the next demand event is processed.</span><span class="sxs-lookup"><span data-stu-id="76e83-116">Due to order tracking, the planning line is created not only when the supply event is closed, but also if the demand event is closed, even though the supply event is still open and may be subject to additional changes when the next demand event is processed.</span></span> <span data-ttu-id="76e83-117">This means that when first created, the planning line may be changed again.</span><span class="sxs-lookup"><span data-stu-id="76e83-117">This means that when first created, the planning line may be changed again.</span></span>  

 <span data-ttu-id="76e83-118">To minimise database access when handling production orders, the planning line can be maintained in three levels, while aiming to perform the least demanding maintenance level:</span><span class="sxs-lookup"><span data-stu-id="76e83-118">To minimize database access when handling production orders, the planning line can be maintained in three levels, while aiming to perform the least demanding maintenance level:</span></span>  

-   <span data-ttu-id="76e83-119">Create only the planning line with the current due date and quantity but without the routing and components.</span><span class="sxs-lookup"><span data-stu-id="76e83-119">Create only the planning line with the current due date and quantity but without the routing and components.</span></span>  

-   <span data-ttu-id="76e83-120">Include routing: the planned routing is laid out including calculation of starting and ending dates and times.</span><span class="sxs-lookup"><span data-stu-id="76e83-120">Include routing: the planned routing is laid out including calculation of starting and ending dates and times.</span></span> <span data-ttu-id="76e83-121">This is demanding in terms of database accesses.</span><span class="sxs-lookup"><span data-stu-id="76e83-121">This is demanding in terms of database accesses.</span></span> <span data-ttu-id="76e83-122">To determine the ending and due dates, it may be necessary to calculate this even if the supply event has not been closed (in the case of forward scheduling).</span><span class="sxs-lookup"><span data-stu-id="76e83-122">To determine the ending and due dates, it may be necessary to calculate this even if the supply event has not been closed (in the case of forward scheduling).</span></span>  

-   <span data-ttu-id="76e83-123">Include BOM explosion: this can wait until just before the supply event is closed.</span><span class="sxs-lookup"><span data-stu-id="76e83-123">Include BOM explosion: this can wait until just before the supply event is closed.</span></span>  

 <span data-ttu-id="76e83-124">This concludes the descriptions of how demand and supply is loaded, prioritised, and balanced by the planning system.</span><span class="sxs-lookup"><span data-stu-id="76e83-124">This concludes the descriptions of how demand and supply is loaded, prioritized, and balanced by the planning system.</span></span> <span data-ttu-id="76e83-125">In integration with this supply planning activity, the system must ensure that the required inventory level of each planned item is maintained according to its reordering policies.</span><span class="sxs-lookup"><span data-stu-id="76e83-125">In integration with this supply planning activity, the system must ensure that the required inventory level of each planned item is maintained according to its reordering policies.</span></span>  

## <a name="see-also"></a><span data-ttu-id="76e83-126">See Also</span><span class="sxs-lookup"><span data-stu-id="76e83-126">See Also</span></span>  
 <span data-ttu-id="76e83-127">[Design Details: Balancing Demand and Supply](design-details-balancing-demand-and-supply.md) </span><span class="sxs-lookup"><span data-stu-id="76e83-127">[Design Details: Balancing Demand and Supply](design-details-balancing-demand-and-supply.md) </span></span>  
 <span data-ttu-id="76e83-128">[Design Details: Central Concepts of the Planning System](design-details-central-concepts-of-the-planning-system.md) </span><span class="sxs-lookup"><span data-stu-id="76e83-128">[Design Details: Central Concepts of the Planning System](design-details-central-concepts-of-the-planning-system.md) </span></span>  
 [<span data-ttu-id="76e83-129">Design Details: Supply Planning</span><span class="sxs-lookup"><span data-stu-id="76e83-129">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)

