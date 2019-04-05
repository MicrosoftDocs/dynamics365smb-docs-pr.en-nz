---
title: Design Details | Microsoft Docs
description: This content contains detailed technical information about complex application features in Business Central.
author: SorenGP
documentationcenter: ''
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2018
ms.author: sgroespe
ms.openlocfilehash: f374daae5d7135324ef4fc3da4845a992aa0ccb5
ms.sourcegitcommit: 1bcfaa99ea302e6b84b8361ca02730b135557fc1
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 03/08/2019
ms.locfileid: "822104"
---
# <a name="design-details"></a><span data-ttu-id="c2393-103">Design Details</span><span class="sxs-lookup"><span data-stu-id="c2393-103">Design Details</span></span>
<span data-ttu-id="c2393-104">This content contains detailed technical information about complex application features in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="c2393-104">This content contains detailed technical information about complex application features in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  

 <span data-ttu-id="c2393-105">Design details content is aimed at implementers, developers, and super users who need deeper insight to implement, customise, or set up the features in question.</span><span class="sxs-lookup"><span data-stu-id="c2393-105">Design details content is aimed at implementers, developers, and super users who need deeper insight to implement, customize, or set up the features in question.</span></span>  

|<span data-ttu-id="c2393-106">**To**</span><span class="sxs-lookup"><span data-stu-id="c2393-106">**To**</span></span>|<span data-ttu-id="c2393-107">**See**</span><span class="sxs-lookup"><span data-stu-id="c2393-107">**See**</span></span>|  
|------------|-------------|  
|<span data-ttu-id="c2393-108">Learn about the design for storing and posting dimensions, including code examples on how to migrate and upgrade dimension code.</span><span class="sxs-lookup"><span data-stu-id="c2393-108">Learn about the design for storing and posting dimensions, including code examples on how to migrate and upgrade dimension code.</span></span>|[<span data-ttu-id="c2393-109">Design Details: Dimension Set Entries</span><span class="sxs-lookup"><span data-stu-id="c2393-109">Design Details: Dimension Set Entries</span></span>](design-details-dimension-set-entries.md)|  
|<span data-ttu-id="c2393-110">Learn how the planning system works and how to adjust the algorithms to meet planning requirements in different environments.</span><span class="sxs-lookup"><span data-stu-id="c2393-110">Learn how the planning system works and how to adjust the algorithms to meet planning requirements in different environments.</span></span>|[<span data-ttu-id="c2393-111">Design Details: Supply Planning</span><span class="sxs-lookup"><span data-stu-id="c2393-111">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)|  
|<span data-ttu-id="c2393-112">Understand mechanisms in the costing engine, such as costing method and cost adjustment, and which accounting principles they are designed for.</span><span class="sxs-lookup"><span data-stu-id="c2393-112">Understand mechanisms in the costing engine, such as costing method and cost adjustment, and which accounting principles they are designed for.</span></span>|[<span data-ttu-id="c2393-113">Design Details: Inventory Costing</span><span class="sxs-lookup"><span data-stu-id="c2393-113">Design Details: Inventory Costing</span></span>](design-details-inventory-costing.md)|  
|<span data-ttu-id="c2393-114">Learn about central principles behind advanced and basic warehouse features and how they integrate with other supply chain features.</span><span class="sxs-lookup"><span data-stu-id="c2393-114">Learn about central principles behind advanced and basic warehouse features and how they integrate with other supply chain features.</span></span>|[<span data-ttu-id="c2393-115">Design Details: Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="c2393-115">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)|  
|<span data-ttu-id="c2393-116">Learn about historic and the current design of item tracking functionality and how it integrates with the reservation system to include serial/lot numbers in availability calculations.</span><span class="sxs-lookup"><span data-stu-id="c2393-116">Learn about historic and the current design of item tracking functionality and how it integrates with the reservation system to include serial/lot numbers in availability calculations.</span></span>|[<span data-ttu-id="c2393-117">Design Details: Item Tracking</span><span class="sxs-lookup"><span data-stu-id="c2393-117">Design Details: Item Tracking</span></span>](design-details-item-tracking.md)|  
|<span data-ttu-id="c2393-118">Learn about the General Journal Posting Line feature, including recent simplifications to the design of codeunit 12.</span><span class="sxs-lookup"><span data-stu-id="c2393-118">Learn about the General Journal Posting Line feature, including recent simplifications to the design of codeunit 12.</span></span>|[<span data-ttu-id="c2393-119">Design Details: General Journal Post Line</span><span class="sxs-lookup"><span data-stu-id="c2393-119">Design Details: General Journal Post Line</span></span>](design-details-general-journal-post-line.md)|  

## <a name="see-also"></a><span data-ttu-id="c2393-120">See Also</span><span class="sxs-lookup"><span data-stu-id="c2393-120">See Also</span></span>  
 <span data-ttu-id="c2393-121">[Planning](production-planning.md) </span><span class="sxs-lookup"><span data-stu-id="c2393-121">[Planning](production-planning.md) </span></span>  
 <span data-ttu-id="c2393-122">[Managing Inventory Costs](finance-manage-inventory-costs.md) </span><span class="sxs-lookup"><span data-stu-id="c2393-122">[Managing Inventory Costs](finance-manage-inventory-costs.md) </span></span>  
 <span data-ttu-id="c2393-123">[Warehouse Management](warehouse-manage-warehouse.md) </span><span class="sxs-lookup"><span data-stu-id="c2393-123">[Warehouse Management](warehouse-manage-warehouse.md) </span></span>  
 [<span data-ttu-id="c2393-124">Setting Up Complex Application Areas Using Best Practices</span><span class="sxs-lookup"><span data-stu-id="c2393-124">Setting Up Complex Application Areas Using Best Practices</span></span>](set-up-complex-application-areas-using-best-practices.md)  
 <span data-ttu-id="c2393-125">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="c2393-125">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

 ## [!INCLUDE[d365fin](includes/free_trial_md.md)]  
  
