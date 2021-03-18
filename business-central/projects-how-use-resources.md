---
title: Record and Adjust Resource Usage and Prices| Microsoft Docs
description: Describes how you can record the resource usage or consumption associated with a job, to keep track and manage costs, prices, and work types.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: project management, capacity, staff
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 48d7615ec32424400133c9dbf6b63c46d450f019
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "5388390"
---
# <a name="use-resources-for-jobs"></a><span data-ttu-id="cec47-103">Use Resources for Jobs</span><span class="sxs-lookup"><span data-stu-id="cec47-103">Use Resources for Jobs</span></span>
<span data-ttu-id="cec47-104">You record the usage of resources in the job journal to keep track of costs, prices, and the work types that are linked to jobs.</span><span class="sxs-lookup"><span data-stu-id="cec47-104">You record the usage of resources in the job journal to keep track of costs, prices, and the work types that are linked to jobs.</span></span> <span data-ttu-id="cec47-105">For more information, see [Record Usage for Jobs](projects-how-record-job-usage.md).</span><span class="sxs-lookup"><span data-stu-id="cec47-105">For more information, see [Record Usage for Jobs](projects-how-record-job-usage.md).</span></span>

> [!NOTE]
> <span data-ttu-id="cec47-106">You can also purchase external resources, for example, to invoice a vendor for work delivered.</span><span class="sxs-lookup"><span data-stu-id="cec47-106">You can also purchase external resources, for example, to invoice a vendor for work delivered.</span></span> <span data-ttu-id="cec47-107">For more information, see [Record Purchases](purchasing-how-record-purchases.md).</span><span class="sxs-lookup"><span data-stu-id="cec47-107">For more information, see [Record Purchases](purchasing-how-record-purchases.md).</span></span>

<span data-ttu-id="cec47-108">You can also post the usage of a resource in a resource journal.</span><span class="sxs-lookup"><span data-stu-id="cec47-108">You can also post the usage of a resource in a resource journal.</span></span> <span data-ttu-id="cec47-109">Entries posted in a resource journal have no effect on the general ledger.</span><span class="sxs-lookup"><span data-stu-id="cec47-109">Entries posted in a resource journal have no effect on the general ledger.</span></span>

## <a name="to-assign-resources-to-jobs"></a><span data-ttu-id="cec47-110">To assign resources to jobs</span><span class="sxs-lookup"><span data-stu-id="cec47-110">To assign resources to jobs</span></span>
<span data-ttu-id="cec47-111">You assign resources to jobs by creating job planning lines for the job.</span><span class="sxs-lookup"><span data-stu-id="cec47-111">You assign resources to jobs by creating job planning lines for the job.</span></span> <span data-ttu-id="cec47-112">For more information, see [Create Jobs](projects-how-create-jobs.md).</span><span class="sxs-lookup"><span data-stu-id="cec47-112">For more information, see [Create Jobs](projects-how-create-jobs.md).</span></span>

## <a name="to-record-resource-usage-for-a-job"></a><span data-ttu-id="cec47-113">To record resource usage for a job</span><span class="sxs-lookup"><span data-stu-id="cec47-113">To record resource usage for a job</span></span>
1. <span data-ttu-id="cec47-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Job Journals**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="cec47-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Job Journals**, and then choose the related link.</span></span>
2. <span data-ttu-id="cec47-115">Open a relevant job journal batch, and then fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="cec47-115">Open a relevant job journal batch, and then fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. <span data-ttu-id="cec47-116">When the journal is complete, choose the **Post** action.</span><span class="sxs-lookup"><span data-stu-id="cec47-116">When the journal is complete, choose the **Post** action.</span></span>

## <a name="to-adjust-resource-prices"></a><span data-ttu-id="cec47-117">To adjust resource prices</span><span class="sxs-lookup"><span data-stu-id="cec47-117">To adjust resource prices</span></span>
<span data-ttu-id="cec47-118">If you want to change costs or prices for a large number of resources, you can use a batch job.</span><span class="sxs-lookup"><span data-stu-id="cec47-118">If you want to change costs or prices for a large number of resources, you can use a batch job.</span></span>  

1. <span data-ttu-id="cec47-119">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Adjust Resource Costs/Prices**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="cec47-119">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Adjust Resource Costs/Prices**, and then choose the related link.</span></span>
2. <span data-ttu-id="cec47-120">Fill in the fields on a line as necessary, and then choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="cec47-120">Fill in the fields on a line as necessary, and then choose the **OK** button.</span></span>

> [!NOTE]  
>   <span data-ttu-id="cec47-121">This batch job does not create or adjust alternate costs or prices for resources.</span><span class="sxs-lookup"><span data-stu-id="cec47-121">This batch job does not create or adjust alternate costs or prices for resources.</span></span> <span data-ttu-id="cec47-122">It only changes the contents of the field on the resource card for the **Adjust Field** field that you selected in the batch job.</span><span class="sxs-lookup"><span data-stu-id="cec47-122">It only changes the contents of the field on the resource card for the **Adjust Field** field that you selected in the batch job.</span></span> <span data-ttu-id="cec47-123">The adjustment will take effect immediately for resources, so check your adjustment factors before you run the batch job.</span><span class="sxs-lookup"><span data-stu-id="cec47-123">The adjustment will take effect immediately for resources, so check your adjustment factors before you run the batch job.</span></span>

## <a name="to-get-resource-price-change-suggestions-based-on-existing-alternate-prices"></a><span data-ttu-id="cec47-124">To get resource price change suggestions based on existing alternate prices</span><span class="sxs-lookup"><span data-stu-id="cec47-124">To get resource price change suggestions based on existing alternate prices</span></span>
<span data-ttu-id="cec47-125">If you have already set up alternate resource price for some resources, you can use a batch job to set up multiple alternate resource prices.</span><span class="sxs-lookup"><span data-stu-id="cec47-125">If you have already set up alternate resource price for some resources, you can use a batch job to set up multiple alternate resource prices.</span></span>

1. <span data-ttu-id="cec47-126">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Resource Price Changes**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="cec47-126">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Resource Price Changes**, and then choose the related link.</span></span>
2. <span data-ttu-id="cec47-127">Choose the **Suggest Res. Price Chg. (Price)** action, and then fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="cec47-127">Choose the **Suggest Res. Price Chg. (Price)** action, and then fill in the fields as necessary.</span></span>
3. <span data-ttu-id="cec47-128">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="cec47-128">Choose the **OK** button.</span></span>  
4. <span data-ttu-id="cec47-129">When the batch job is finished, the **Resource Price Changes** page shows the results of the batch job.</span><span class="sxs-lookup"><span data-stu-id="cec47-129">When the batch job is finished, the **Resource Price Changes** page shows the results of the batch job.</span></span>

## <a name="to-get-resource-price-change-suggestions-based-on-standard-prices"></a><span data-ttu-id="cec47-130">To get resource price change suggestions based on standard prices</span><span class="sxs-lookup"><span data-stu-id="cec47-130">To get resource price change suggestions based on standard prices</span></span>
<span data-ttu-id="cec47-131">If you want to set up multiple alternate resource prices based on the standard prices on the resource cards, you can use a batch job.</span><span class="sxs-lookup"><span data-stu-id="cec47-131">If you want to set up multiple alternate resource prices based on the standard prices on the resource cards, you can use a batch job.</span></span>  

1. <span data-ttu-id="cec47-132">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Resource Price Changes**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="cec47-132">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Resource Price Changes**, and then choose the related link.</span></span>
2. <span data-ttu-id="cec47-133">Choose the **Suggest Res. Price Chg. (Res.)** action, and then fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="cec47-133">Choose the **Suggest Res. Price Chg. (Res.)** action, and then fill in the fields as necessary.</span></span>  
3. <span data-ttu-id="cec47-134">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="cec47-134">Choose the **OK** button.</span></span>  
4. <span data-ttu-id="cec47-135">When the batch job is finished, open the **Resource Price Changes** page to see the results of the batch job.</span><span class="sxs-lookup"><span data-stu-id="cec47-135">When the batch job is finished, open the **Resource Price Changes** page to see the results of the batch job.</span></span>

## <a name="to-get-resource-price-change-suggestions-based-on-alternate-prices"></a><span data-ttu-id="cec47-136">To get resource price change suggestions based on alternate prices</span><span class="sxs-lookup"><span data-stu-id="cec47-136">To get resource price change suggestions based on alternate prices</span></span>
<span data-ttu-id="cec47-137">If you have already set up alternate resource price for some resources, you can use a batch job to set up multiple alternate resource prices.</span><span class="sxs-lookup"><span data-stu-id="cec47-137">If you have already set up alternate resource price for some resources, you can use a batch job to set up multiple alternate resource prices.</span></span>

1. <span data-ttu-id="cec47-138">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Suggest Res. Price Chg. (Price)**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="cec47-138">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Suggest Res. Price Chg. (Price)**, and then choose the related link.</span></span>  
2. <span data-ttu-id="cec47-139">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="cec47-139">Fill in the fields as necessary.</span></span>
3. <span data-ttu-id="cec47-140">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="cec47-140">Choose the **OK** button.</span></span>  
4. <span data-ttu-id="cec47-141">When the batch job is finished, open the **Resource Price Changes** page to see the results of the batch job.</span><span class="sxs-lookup"><span data-stu-id="cec47-141">When the batch job is finished, open the **Resource Price Changes** page to see the results of the batch job.</span></span>

## <a name="see-also"></a><span data-ttu-id="cec47-142">See Also</span><span class="sxs-lookup"><span data-stu-id="cec47-142">See Also</span></span>
[<span data-ttu-id="cec47-143">Project Management</span><span class="sxs-lookup"><span data-stu-id="cec47-143">Project Management</span></span>](projects-manage-projects.md)  
[<span data-ttu-id="cec47-144">Finance</span><span class="sxs-lookup"><span data-stu-id="cec47-144">Finance</span></span>](finance.md)  
<span data-ttu-id="cec47-145">[Purchasing](purchasing-manage-purchasing.md)       </span><span class="sxs-lookup"><span data-stu-id="cec47-145">[Purchasing](purchasing-manage-purchasing.md)       </span></span>  
<span data-ttu-id="cec47-146">[Sales](sales-manage-sales.md)   </span><span class="sxs-lookup"><span data-stu-id="cec47-146">[Sales](sales-manage-sales.md)   </span></span>  
<span data-ttu-id="cec47-147">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="cec47-147">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>  


[!INCLUDE[footer-include](includes/footer-banner.md)]