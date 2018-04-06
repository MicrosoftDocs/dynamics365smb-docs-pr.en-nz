---
title: Record and Adjust Resource Usage and Prices| Microsoft Docs
description: Describes how you can record the resource usage or consumption associated with a job, to keep track and manage costs, prices, and work types.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: project management, capacity, staff
ms.date: 01/25/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: f86fed1b300df98ef120e2f91fdd0785670d04f1
ms.contentlocale: en-nz
ms.lasthandoff: 03/22/2018

---
# <a name="use-resources-for-jobs"></a><span data-ttu-id="eb2e1-103">Use Resources for Jobs</span><span class="sxs-lookup"><span data-stu-id="eb2e1-103">Use Resources for Jobs</span></span>
<span data-ttu-id="eb2e1-104">You record the usage of resources in the job journal to keep track of costs, prices, and the work types that are linked to jobs.</span><span class="sxs-lookup"><span data-stu-id="eb2e1-104">You record the usage of resources in the job journal to keep track of costs, prices, and the work types that are linked to jobs.</span></span> <span data-ttu-id="eb2e1-105">For more information, see [Record Usage for Jobs](projects-how-record-job-usage.md).</span><span class="sxs-lookup"><span data-stu-id="eb2e1-105">For more information, see [Record Usage for Jobs](projects-how-record-job-usage.md).</span></span>

<span data-ttu-id="eb2e1-106">You can also post the usage of a resource in a resource journal.</span><span class="sxs-lookup"><span data-stu-id="eb2e1-106">You can also post the usage of a resource in a resource journal.</span></span> <span data-ttu-id="eb2e1-107">Entries posted in a resource journal have no effect on the general ledger.</span><span class="sxs-lookup"><span data-stu-id="eb2e1-107">Entries posted in a resource journal have no effect on the general ledger.</span></span>

## <a name="to-assign-resources-to-jobs"></a><span data-ttu-id="eb2e1-108">To assign resources to jobs</span><span class="sxs-lookup"><span data-stu-id="eb2e1-108">To assign resources to jobs</span></span>
<span data-ttu-id="eb2e1-109">You assign resources to jobs by creating job planning lines for the job.</span><span class="sxs-lookup"><span data-stu-id="eb2e1-109">You assign resources to jobs by creating job planning lines for the job.</span></span> <span data-ttu-id="eb2e1-110">For more information, see [Create Jobs](projects-how-create-jobs.md).</span><span class="sxs-lookup"><span data-stu-id="eb2e1-110">For more information, see [Create Jobs](projects-how-create-jobs.md).</span></span>

## <a name="to-record-resource-usage-for-a-job"></a><span data-ttu-id="eb2e1-111">To record resource usage for a job</span><span class="sxs-lookup"><span data-stu-id="eb2e1-111">To record resource usage for a job</span></span>
1. <span data-ttu-id="eb2e1-112">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Job Journals**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="eb2e1-112">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Job Journals**, and then choose the related link.</span></span>
2. <span data-ttu-id="eb2e1-113">Open a relevant job journal batch, and then fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="eb2e1-113">Open a relevant job journal batch, and then fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. <span data-ttu-id="eb2e1-114">When the journal is complete, choose the **Post** action.</span><span class="sxs-lookup"><span data-stu-id="eb2e1-114">When the journal is complete, choose the **Post** action.</span></span>

## <a name="to-adjust-resource-prices"></a><span data-ttu-id="eb2e1-115">To adjust resource prices</span><span class="sxs-lookup"><span data-stu-id="eb2e1-115">To adjust resource prices</span></span>
<span data-ttu-id="eb2e1-116">If you want to change costs or prices for a large number of resources, you can use a batch job.</span><span class="sxs-lookup"><span data-stu-id="eb2e1-116">If you want to change costs or prices for a large number of resources, you can use a batch job.</span></span>  

1. <span data-ttu-id="eb2e1-117">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Adjust Resource Costs/Prices**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="eb2e1-117">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Adjust Resource Costs/Prices**, and then choose the related link.</span></span>
2. <span data-ttu-id="eb2e1-118">Fill in the fields on a line as necessary, and then choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="eb2e1-118">Fill in the fields on a line as necessary, and then choose the **OK** button.</span></span>

> [!NOTE]  
>   <span data-ttu-id="eb2e1-119">This batch job does not create or adjust alternate costs or prices for resources.</span><span class="sxs-lookup"><span data-stu-id="eb2e1-119">This batch job does not create or adjust alternate costs or prices for resources.</span></span> <span data-ttu-id="eb2e1-120">It only changes the contents of the field on the resource card for the **Adjust Field** field that you selected in the batch job.</span><span class="sxs-lookup"><span data-stu-id="eb2e1-120">It only changes the contents of the field on the resource card for the **Adjust Field** field that you selected in the batch job.</span></span> <span data-ttu-id="eb2e1-121">The adjustment will take effect immediately for resources, so check your adjustment factors before you run the batch job.</span><span class="sxs-lookup"><span data-stu-id="eb2e1-121">The adjustment will take effect immediately for resources, so check your adjustment factors before you run the batch job.</span></span>

## <a name="to-get-resource-price-change-suggestions-based-on-existing-alternate-prices"></a><span data-ttu-id="eb2e1-122">To get resource price change suggestions based on existing alternate prices</span><span class="sxs-lookup"><span data-stu-id="eb2e1-122">To get resource price change suggestions based on existing alternate prices</span></span>
<span data-ttu-id="eb2e1-123">If you have already set up alternate resource price for some resources, you can use a batch job to set up multiple alternate resource prices.</span><span class="sxs-lookup"><span data-stu-id="eb2e1-123">If you have already set up alternate resource price for some resources, you can use a batch job to set up multiple alternate resource prices.</span></span>

1. <span data-ttu-id="eb2e1-124">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Resource Price Changes**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="eb2e1-124">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Resource Price Changes**, and then choose the related link.</span></span>
2. <span data-ttu-id="eb2e1-125">Choose the **Suggest Res. Price Chg. (Price)** action, and then fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="eb2e1-125">Choose the **Suggest Res. Price Chg. (Price)** action, and then fill in the fields as necessary.</span></span>
3. <span data-ttu-id="eb2e1-126">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="eb2e1-126">Choose the **OK** button.</span></span>  
4. <span data-ttu-id="eb2e1-127">When the batch job is finished, the **Resource Price Changes** window shows the results of the batch job.</span><span class="sxs-lookup"><span data-stu-id="eb2e1-127">When the batch job is finished, the **Resource Price Changes** window shows the results of the batch job.</span></span>

## <a name="to-get-resource-price-change-suggestions-based-on-standard-prices"></a><span data-ttu-id="eb2e1-128">To get resource price change suggestions based on standard prices</span><span class="sxs-lookup"><span data-stu-id="eb2e1-128">To get resource price change suggestions based on standard prices</span></span>
<span data-ttu-id="eb2e1-129">If you want to set up multiple alternate resource prices based on the standard prices on the resource cards, you can use a batch job.</span><span class="sxs-lookup"><span data-stu-id="eb2e1-129">If you want to set up multiple alternate resource prices based on the standard prices on the resource cards, you can use a batch job.</span></span>  

1. <span data-ttu-id="eb2e1-130">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Resource Price Changes**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="eb2e1-130">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Resource Price Changes**, and then choose the related link.</span></span>
2. <span data-ttu-id="eb2e1-131">Choose the **Suggest Res. Price Chg. (Res.)** action, and then fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="eb2e1-131">Choose the **Suggest Res. Price Chg. (Res.)** action, and then fill in the fields as necessary.</span></span>  
3. <span data-ttu-id="eb2e1-132">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="eb2e1-132">Choose the **OK** button.</span></span>  
4. <span data-ttu-id="eb2e1-133">When the batch job is finished, open the **Resource Price Changes** window to see the results of the batch job.</span><span class="sxs-lookup"><span data-stu-id="eb2e1-133">When the batch job is finished, open the **Resource Price Changes** window to see the results of the batch job.</span></span>

## <a name="to-get-resource-price-change-suggestions-based-on-alternate-prices"></a><span data-ttu-id="eb2e1-134">To get resource price change suggestions based on alternate prices</span><span class="sxs-lookup"><span data-stu-id="eb2e1-134">To get resource price change suggestions based on alternate prices</span></span>
<span data-ttu-id="eb2e1-135">If you have already set up alternate resource price for some resources, you can use a batch job to set up multiple alternate resource prices.</span><span class="sxs-lookup"><span data-stu-id="eb2e1-135">If you have already set up alternate resource price for some resources, you can use a batch job to set up multiple alternate resource prices.</span></span>

1. <span data-ttu-id="eb2e1-136">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Suggest Res. Price Chg. (Price)**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="eb2e1-136">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Suggest Res. Price Chg. (Price)**, and then choose the related link.</span></span>  
2. <span data-ttu-id="eb2e1-137">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="eb2e1-137">Fill in the fields as necessary.</span></span>
3. <span data-ttu-id="eb2e1-138">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="eb2e1-138">Choose the **OK** button.</span></span>  
4. <span data-ttu-id="eb2e1-139">When the batch job is finished, open the **Resource Price Changes** window to see the results of the batch job.</span><span class="sxs-lookup"><span data-stu-id="eb2e1-139">When the batch job is finished, open the **Resource Price Changes** window to see the results of the batch job.</span></span>

## <a name="see-also"></a><span data-ttu-id="eb2e1-140">See Also</span><span class="sxs-lookup"><span data-stu-id="eb2e1-140">See Also</span></span>
[<span data-ttu-id="eb2e1-141">Project Management</span><span class="sxs-lookup"><span data-stu-id="eb2e1-141">Project Management</span></span>](projects-manage-projects.md)  
[<span data-ttu-id="eb2e1-142">Finance</span><span class="sxs-lookup"><span data-stu-id="eb2e1-142">Finance</span></span>](finance.md)  
<span data-ttu-id="eb2e1-143">[Purchasing](purchasing-manage-purchasing.md)       </span><span class="sxs-lookup"><span data-stu-id="eb2e1-143">[Purchasing](purchasing-manage-purchasing.md)       </span></span>  
<span data-ttu-id="eb2e1-144">[Sales](sales-manage-sales.md)   </span><span class="sxs-lookup"><span data-stu-id="eb2e1-144">[Sales](sales-manage-sales.md)   </span></span>  
<span data-ttu-id="eb2e1-145">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="eb2e1-145">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  

