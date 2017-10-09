---
title: How to Update Standard Costs | Microsoft Docs
description: You must periodically update the standard costs of components and roll the new costs up to the parent item.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/09/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 57da88de6a3bbb22cea7c12a2b579206ca5d7766
ms.contentlocale: en-nz
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-update-standard-costs"></a><span data-ttu-id="379c8-103">How to: Update Standard Costs</span><span class="sxs-lookup"><span data-stu-id="379c8-103">How to: Update Standard Costs</span></span>
<span data-ttu-id="379c8-104">You must periodically update the standard costs of components and roll the new costs up to the parent item.</span><span class="sxs-lookup"><span data-stu-id="379c8-104">You must periodically update the standard costs of components and roll the new costs up to the parent item.</span></span> <span data-ttu-id="379c8-105">The process typically consists of the following four steps:</span><span class="sxs-lookup"><span data-stu-id="379c8-105">The process typically consists of the following four steps:</span></span>  

1.  <span data-ttu-id="379c8-106">Update costs at the component and capacity levels.</span><span class="sxs-lookup"><span data-stu-id="379c8-106">Update costs at the component and capacity levels.</span></span> <span data-ttu-id="379c8-107">For more information, see the **Suggest Item Standard Cost** batch job.</span><span class="sxs-lookup"><span data-stu-id="379c8-107">For more information, see the **Suggest Item Standard Cost** batch job.</span></span>  
2.  <span data-ttu-id="379c8-108">Consolidate and roll up the component and capacity costs to calculate the total manufacturing or assembly cost of the items.</span><span class="sxs-lookup"><span data-stu-id="379c8-108">Consolidate and roll up the component and capacity costs to calculate the total manufacturing or assembly cost of the items.</span></span>  
3.  <span data-ttu-id="379c8-109">Implement the standard costs that are entered when you run the previous batch jobs.</span><span class="sxs-lookup"><span data-stu-id="379c8-109">Implement the standard costs that are entered when you run the previous batch jobs.</span></span> <span data-ttu-id="379c8-110">The standard costs do not take effect until they are implemented.</span><span class="sxs-lookup"><span data-stu-id="379c8-110">The standard costs do not take effect until they are implemented.</span></span> <span data-ttu-id="379c8-111">For more information, see Implement Standard Cost Changes.</span><span class="sxs-lookup"><span data-stu-id="379c8-111">For more information, see Implement Standard Cost Changes.</span></span>  
4.  <span data-ttu-id="379c8-112">Implement the changes to update the **Unit Cost** field on the item card and perform inventory revaluation.</span><span class="sxs-lookup"><span data-stu-id="379c8-112">Implement the changes to update the **Unit Cost** field on the item card and perform inventory revaluation.</span></span> <span data-ttu-id="379c8-113">For more information, see [How to: Revalue Inventory](inventory-how-revalue-inventory.md).</span><span class="sxs-lookup"><span data-stu-id="379c8-113">For more information, see [How to: Revalue Inventory](inventory-how-revalue-inventory.md).</span></span>  

<span data-ttu-id="379c8-114">For more information, see [About Calculating Standard Cost](finance-about-calculating-standard-cost.md).</span><span class="sxs-lookup"><span data-stu-id="379c8-114">For more information, see [About Calculating Standard Cost](finance-about-calculating-standard-cost.md).</span></span>  
## <a name="to-update-standard-costs"></a><span data-ttu-id="379c8-115">To update standard costs</span><span class="sxs-lookup"><span data-stu-id="379c8-115">To update standard costs</span></span>  
1.  <span data-ttu-id="379c8-116">Run the **Adjust Cost-Item Entries** batch job.</span><span class="sxs-lookup"><span data-stu-id="379c8-116">Run the **Adjust Cost-Item Entries** batch job.</span></span>  
2.  <span data-ttu-id="379c8-117">Run the **Post Inventory Cost to G/L** batch job.</span><span class="sxs-lookup"><span data-stu-id="379c8-117">Run the **Post Inventory Cost to G/L** batch job.</span></span>  
3.  <span data-ttu-id="379c8-118">Open the **Standard Cost Worksheet** and use one or more of the following functions:</span><span class="sxs-lookup"><span data-stu-id="379c8-118">Open the **Standard Cost Worksheet** and use one or more of the following functions:</span></span>  

    1.  <span data-ttu-id="379c8-119">Run the **Suggest Item Standard Cost** batch job.</span><span class="sxs-lookup"><span data-stu-id="379c8-119">Run the **Suggest Item Standard Cost** batch job.</span></span>  
    2.  <span data-ttu-id="379c8-120">Review the results and make changes as necessary.</span><span class="sxs-lookup"><span data-stu-id="379c8-120">Review the results and make changes as necessary.</span></span>  
    3.  <span data-ttu-id="379c8-121">Run the **Suggest Capacity Standard Cost** batch job.</span><span class="sxs-lookup"><span data-stu-id="379c8-121">Run the **Suggest Capacity Standard Cost** batch job.</span></span>  
    4.  <span data-ttu-id="379c8-122">Review the results and make changes as necessary.</span><span class="sxs-lookup"><span data-stu-id="379c8-122">Review the results and make changes as necessary.</span></span>
    5. <span data-ttu-id="379c8-123">Run the **Roll Up Standard Cost** batch job.</span><span class="sxs-lookup"><span data-stu-id="379c8-123">Run the **Roll Up Standard Cost** batch job.</span></span>
    6.  <span data-ttu-id="379c8-124">Review the results and make changes as necessary.</span><span class="sxs-lookup"><span data-stu-id="379c8-124">Review the results and make changes as necessary.</span></span>
    7.  <span data-ttu-id="379c8-125">Run the **Implement Standard Cost Changes** batch job.</span><span class="sxs-lookup"><span data-stu-id="379c8-125">Run the **Implement Standard Cost Changes** batch job.</span></span>  
4.  <span data-ttu-id="379c8-126">Review and post the **Revaluation Journal** window, which has been populated with entries from the previous steps in this process.</span><span class="sxs-lookup"><span data-stu-id="379c8-126">Review and post the **Revaluation Journal** window, which has been populated with entries from the previous steps in this process.</span></span>  

## <a name="see-also"></a><span data-ttu-id="379c8-127">See Also</span><span class="sxs-lookup"><span data-stu-id="379c8-127">See Also</span></span>  
 <span data-ttu-id="379c8-128">[About Calculating Standard Cost](finance-about-calculating-standard-cost.md) </span><span class="sxs-lookup"><span data-stu-id="379c8-128">[About Calculating Standard Cost](finance-about-calculating-standard-cost.md) </span></span>  
 <span data-ttu-id="379c8-129">[Managing Inventory Costs](finance-manage-inventory-costs.md) </span><span class="sxs-lookup"><span data-stu-id="379c8-129">[Managing Inventory Costs](finance-manage-inventory-costs.md) </span></span>  
 <span data-ttu-id="379c8-130">[Design Details: Costing Methods](design-details-costing-methods.md) [[Finance](finance.md)]</span><span class="sxs-lookup"><span data-stu-id="379c8-130">[Design Details: Costing Methods](design-details-costing-methods.md) [[Finance](finance.md)]</span></span>  
 <span data-ttu-id="379c8-131">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="379c8-131">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  

