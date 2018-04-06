---
title: Design Details | Microsoft Docs
description: This content contains detailed technical information about complex application features in Finance and Operations, Business edition.
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b34f276a764f0e828fbc1f015429df9852242a4c
ms.openlocfilehash: 9c8ba2d7c2acaeb4c5c683f2f365e474e4f7bfce
ms.contentlocale: en-nz
ms.lasthandoff: 03/22/2018

---
# <a name="design-details"></a><span data-ttu-id="56299-103">Design Details</span><span class="sxs-lookup"><span data-stu-id="56299-103">Design Details</span></span>
<span data-ttu-id="56299-104">This content contains detailed technical information about complex application features in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="56299-104">This content contains detailed technical information about complex application features in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  

 <span data-ttu-id="56299-105">Design details content is aimed at implementers, developers, and super users who need deeper insight to implement, customise, or set up the features in question.</span><span class="sxs-lookup"><span data-stu-id="56299-105">Design details content is aimed at implementers, developers, and super users who need deeper insight to implement, customize, or set up the features in question.</span></span>  

|<span data-ttu-id="56299-106">**To**</span><span class="sxs-lookup"><span data-stu-id="56299-106">**To**</span></span>|<span data-ttu-id="56299-107">**See**</span><span class="sxs-lookup"><span data-stu-id="56299-107">**See**</span></span>|  
|------------|-------------|  
|<span data-ttu-id="56299-108">Learn about the design for storing and posting dimensions, including code examples on how to migrate and upgrade dimension code.</span><span class="sxs-lookup"><span data-stu-id="56299-108">Learn about the design for storing and posting dimensions, including code examples on how to migrate and upgrade dimension code.</span></span>|[<span data-ttu-id="56299-109">Design Details: Dimension Set Entries</span><span class="sxs-lookup"><span data-stu-id="56299-109">Design Details: Dimension Set Entries</span></span>](design-details-dimension-set-entries.md)|  
|<span data-ttu-id="56299-110">Learn how the planning system works and how to adjust the algorithms to meet planning requirements in different environments.</span><span class="sxs-lookup"><span data-stu-id="56299-110">Learn how the planning system works and how to adjust the algorithms to meet planning requirements in different environments.</span></span>|[<span data-ttu-id="56299-111">Design Details: Supply Planning</span><span class="sxs-lookup"><span data-stu-id="56299-111">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)|  
|<span data-ttu-id="56299-112">Understand mechanisms in the costing engine, such as costing method and cost adjustment, and which accounting principles they are designed for.</span><span class="sxs-lookup"><span data-stu-id="56299-112">Understand mechanisms in the costing engine, such as costing method and cost adjustment, and which accounting principles they are designed for.</span></span>|[<span data-ttu-id="56299-113">Design Details: Inventory Costing</span><span class="sxs-lookup"><span data-stu-id="56299-113">Design Details: Inventory Costing</span></span>](design-details-inventory-costing.md)|  
|<span data-ttu-id="56299-114">Learn about central principles behind advanced and basic warehouse features and how they integrate with other supply chain features.</span><span class="sxs-lookup"><span data-stu-id="56299-114">Learn about central principles behind advanced and basic warehouse features and how they integrate with other supply chain features.</span></span>|[<span data-ttu-id="56299-115">Design Details: Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="56299-115">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)|  
|<span data-ttu-id="56299-116">Learn about historic and the current design of item tracking functionality and how it integrates with the reservation system to include serial/lot numbers in availability calculations.</span><span class="sxs-lookup"><span data-stu-id="56299-116">Learn about historic and the current design of item tracking functionality and how it integrates with the reservation system to include serial/lot numbers in availability calculations.</span></span>|[<span data-ttu-id="56299-117">Design Details: Item Tracking</span><span class="sxs-lookup"><span data-stu-id="56299-117">Design Details: Item Tracking</span></span>](design-details-item-tracking.md)|  
|<span data-ttu-id="56299-118">Learn about the General Journal Posting Line feature, including recent simplifications to the design of codeunit 12.</span><span class="sxs-lookup"><span data-stu-id="56299-118">Learn about the General Journal Posting Line feature, including recent simplifications to the design of codeunit 12.</span></span>|[<span data-ttu-id="56299-119">Design Details: General Journal Post Line</span><span class="sxs-lookup"><span data-stu-id="56299-119">Design Details: General Journal Post Line</span></span>](design-details-general-journal-post-line.md)|  

## <a name="see-also"></a><span data-ttu-id="56299-120">See Also</span><span class="sxs-lookup"><span data-stu-id="56299-120">See Also</span></span>  
 <span data-ttu-id="56299-121">[Planning](production-planning.md) </span><span class="sxs-lookup"><span data-stu-id="56299-121">[Planning](production-planning.md) </span></span>  
 <span data-ttu-id="56299-122">[Managing Inventory Costs](finance-manage-inventory-costs.md) </span><span class="sxs-lookup"><span data-stu-id="56299-122">[Managing Inventory Costs](finance-manage-inventory-costs.md) </span></span>  
 <span data-ttu-id="56299-123">[Warehouse Management](warehouse-manage-warehouse.md) </span><span class="sxs-lookup"><span data-stu-id="56299-123">[Warehouse Management](warehouse-manage-warehouse.md) </span></span>  
 [<span data-ttu-id="56299-124">Setting Up Complex Application Areas Using Best Practices</span><span class="sxs-lookup"><span data-stu-id="56299-124">Setting Up Complex Application Areas Using Best Practices</span></span>](set-up-complex-application-areas-using-best-practices.md)  
 <span data-ttu-id="56299-125">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="56299-125">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

 ## [!INCLUDE[d365fin](includes/free_trial_md.md)]  
 ## [!INCLUDE[d365fin](includes/training_link_md.md)]

