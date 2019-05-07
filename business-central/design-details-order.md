---
title: Design Details - Order | Microsoft Docs
description: This topic provides information about order-to-order links in a make-to-order environment.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: design, order
ms.date: 04/01/2019
ms.author: sgroespe
redirect_url: design-details-handling-reordering-policies
ms.openlocfilehash: 3a0014a80bd4f1f6c786638ddec23a1852c9a635
ms.sourcegitcommit: bd78a5d990c9e83174da1409076c22df8b35eafd
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 03/31/2019
ms.locfileid: "913864"
---
# <a name="design-details-order"></a><span data-ttu-id="31631-103">Design Details: Order</span><span class="sxs-lookup"><span data-stu-id="31631-103">Design Details: Order</span></span>
<span data-ttu-id="31631-104">In a make-to-order environment, an item is purchased or produced to exclusively cover a specific demand.</span><span class="sxs-lookup"><span data-stu-id="31631-104">In a make-to-order environment, an item is purchased or produced to exclusively cover a specific demand.</span></span> <span data-ttu-id="31631-105">Typically it relates to A-items, and the motivation for choosing the order reordering policy can be that the demand is infrequent, the lead-time is insignificant, or the required attributes vary.</span><span class="sxs-lookup"><span data-stu-id="31631-105">Typically it relates to A-items, and the motivation for choosing the order reordering policy can be that the demand is infrequent, the lead-time is insignificant, or the required attributes vary.</span></span>  

<span data-ttu-id="31631-106">The program creates an order-to-order link, which acts as a preliminary connection between the supply, a supply order or inventory, and the demand that it is going to fulfill.</span><span class="sxs-lookup"><span data-stu-id="31631-106">The program creates an order-to-order link, which acts as a preliminary connection between the supply, a supply order or inventory, and the demand that it is going to fulfill.</span></span>  

<span data-ttu-id="31631-107">Apart from using the Order policy, the order-to-order link can be applied during planning in the following ways:</span><span class="sxs-lookup"><span data-stu-id="31631-107">Apart from using the Order policy, the order-to-order link can be applied during planning in the following ways:</span></span>  

* <span data-ttu-id="31631-108">When using the Make-to-Order manufacturing policy to create multi-level or project type production orders (producing needed components on the same production order).</span><span class="sxs-lookup"><span data-stu-id="31631-108">When using the Make-to-Order manufacturing policy to create multi-level or project type production orders (producing needed components on the same production order).</span></span>  
* <span data-ttu-id="31631-109">When using the Sales Order Planning feature to create a production order from a sales order.</span><span class="sxs-lookup"><span data-stu-id="31631-109">When using the Sales Order Planning feature to create a production order from a sales order.</span></span>  

<span data-ttu-id="31631-110">Even if a manufacturing company considers itself as a make-to-order environment, it might be best to use a Lot-for-Lot reordering policy if the items are pure standard without variation in attributes.</span><span class="sxs-lookup"><span data-stu-id="31631-110">Even if a manufacturing company considers itself as a make-to-order environment, it might be best to use a Lot-for-Lot reordering policy if the items are pure standard without variation in attributes.</span></span> <span data-ttu-id="31631-111">As a result, the system will use unplanned inventory and only accumulates sales orders with the same shipment date or within a defined time bucket.</span><span class="sxs-lookup"><span data-stu-id="31631-111">As a result, the system will use unplanned inventory and only accumulates sales orders with the same shipment date or within a defined time bucket.</span></span>  

## <a name="order-to-order-links-and-past-due-dates"></a><span data-ttu-id="31631-112">Order-to-Order Links and Past Due Dates</span><span class="sxs-lookup"><span data-stu-id="31631-112">Order-to-Order Links and Past Due Dates</span></span>  
<span data-ttu-id="31631-113">Unlike most supply-demand sets, linked orders with due dates before the planning starting date are fully planned for by the system.</span><span class="sxs-lookup"><span data-stu-id="31631-113">Unlike most supply-demand sets, linked orders with due dates before the planning starting date are fully planned for by the system.</span></span> <span data-ttu-id="31631-114">The business reason for this exception is that specific demand-supply sets must be synchronised through to execution.</span><span class="sxs-lookup"><span data-stu-id="31631-114">The business reason for this exception is that specific demand-supply sets must be synchronized through to execution.</span></span> <span data-ttu-id="31631-115">For more information about the frozen zone that applies to most demand-supply types, see [Design Details: Dealing with Orders Before the Planning Starting Date](design-details-dealing-with-orders-before-the-planning-starting-date.md).</span><span class="sxs-lookup"><span data-stu-id="31631-115">For more information about the frozen zone that applies to most demand-supply types, see [Design Details: Dealing with Orders Before the Planning Starting Date](design-details-dealing-with-orders-before-the-planning-starting-date.md).</span></span>  

## <a name="see-also"></a><span data-ttu-id="31631-116">See Also</span><span class="sxs-lookup"><span data-stu-id="31631-116">See Also</span></span>  
<span data-ttu-id="31631-117">[Design Details: Reordering Policies](design-details-reordering-policies.md) </span><span class="sxs-lookup"><span data-stu-id="31631-117">[Design Details: Reordering Policies](design-details-reordering-policies.md) </span></span>  
<span data-ttu-id="31631-118">[Design Details: Planning Parameters](design-details-planning-parameters.md) </span><span class="sxs-lookup"><span data-stu-id="31631-118">[Design Details: Planning Parameters](design-details-planning-parameters.md) </span></span>  
<span data-ttu-id="31631-119">[Design Details: Handling Reordering Policies](design-details-handling-reordering-policies.md) </span><span class="sxs-lookup"><span data-stu-id="31631-119">[Design Details: Handling Reordering Policies](design-details-handling-reordering-policies.md) </span></span>  
[<span data-ttu-id="31631-120">Design Details: Supply Planning</span><span class="sxs-lookup"><span data-stu-id="31631-120">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)
