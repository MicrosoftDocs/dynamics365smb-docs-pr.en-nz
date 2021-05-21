---
title: Define a WIP Method and Monitor Job Progress| Microsoft Docs
description: Describes how you can create a work in progress (WIP) method and calculate WIP to estimate the financial value of jobs while they are ongoing.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: project management, KPI, work in process, work in progress
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: fac1c041108cacfcabf18b04d128949d05e1d283
ms.sourcegitcommit: 93c8681054b059cec38cb29b86de20be37980676
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 04/23/2021
ms.locfileid: "5938137"
---
# <a name="monitor-job-progress-and-performance"></a><span data-ttu-id="0c32b-103">Monitor Job Progress and Performance</span><span class="sxs-lookup"><span data-stu-id="0c32b-103">Monitor Job Progress and Performance</span></span>
<span data-ttu-id="0c32b-104">As a job progresses, materials, resources, and other expenses are consumed and must be posted to the job.</span><span class="sxs-lookup"><span data-stu-id="0c32b-104">As a job progresses, materials, resources, and other expenses are consumed and must be posted to the job.</span></span> <span data-ttu-id="0c32b-105">Work in Progress (WIP) is a feature that enables you to estimate the financial value of jobs in the general ledger while the jobs are ongoing.</span><span class="sxs-lookup"><span data-stu-id="0c32b-105">Work in Process (WIP) is a feature that enables you to estimate the financial value of jobs in the general ledger while the jobs are ongoing.</span></span> <span data-ttu-id="0c32b-106">In many cases, you might post expenses for a job before invoicing a job.</span><span class="sxs-lookup"><span data-stu-id="0c32b-106">In many cases, you might post expenses for a job before invoicing a job.</span></span> <span data-ttu-id="0c32b-107">When only expenses have been posted, your financial statement will be inaccurate.</span><span class="sxs-lookup"><span data-stu-id="0c32b-107">When only expenses have been posted, your financial statement will be inaccurate.</span></span> <span data-ttu-id="0c32b-108">For more information, see [Understanding WIP Methods](projects-understanding-wip.md).</span><span class="sxs-lookup"><span data-stu-id="0c32b-108">For more information, see [Understanding WIP Methods](projects-understanding-wip.md).</span></span>

<span data-ttu-id="0c32b-109">To track the value in the general ledger, you can calculate WIP and post the value to the general ledger.</span><span class="sxs-lookup"><span data-stu-id="0c32b-109">To track the value in the general ledger, you can calculate WIP and post the value to the general ledger.</span></span>

<span data-ttu-id="0c32b-110">You can calculate WIP based on the following:</span><span class="sxs-lookup"><span data-stu-id="0c32b-110">You can calculate WIP based on the following:</span></span>

* <span data-ttu-id="0c32b-111">Cost Value</span><span class="sxs-lookup"><span data-stu-id="0c32b-111">Cost Value</span></span>
* <span data-ttu-id="0c32b-112">Sales Value</span><span class="sxs-lookup"><span data-stu-id="0c32b-112">Sales Value</span></span>
* <span data-ttu-id="0c32b-113">Recognisable Cost</span><span class="sxs-lookup"><span data-stu-id="0c32b-113">Recognizable Cost</span></span>
* <span data-ttu-id="0c32b-114">Percentage of Completion</span><span class="sxs-lookup"><span data-stu-id="0c32b-114">Percentage of Completion</span></span>
* <span data-ttu-id="0c32b-115">Completed Contract</span><span class="sxs-lookup"><span data-stu-id="0c32b-115">Completed Contract</span></span>

<span data-ttu-id="0c32b-116">If you want to view the result using a different method, you can change the method and calculate WIP again.</span><span class="sxs-lookup"><span data-stu-id="0c32b-116">If you want to view the result using a different method, you can change the method and calculate WIP again.</span></span> <span data-ttu-id="0c32b-117">There is no limit to the number of times that you calculate WIP.</span><span class="sxs-lookup"><span data-stu-id="0c32b-117">There is no limit to the number of times that you calculate WIP.</span></span> <span data-ttu-id="0c32b-118">WIP is only calculated, it does not get posted to the general ledger.</span><span class="sxs-lookup"><span data-stu-id="0c32b-118">WIP is only calculated, it does not get posted to the general ledger.</span></span> <span data-ttu-id="0c32b-119">After you have calculated WIP, you can post to the general ledger.</span><span class="sxs-lookup"><span data-stu-id="0c32b-119">After you have calculated WIP, you can post to the general ledger.</span></span>

## <a name="to-create-a-job-wip-method"></a><span data-ttu-id="0c32b-120">To create a job WIP method</span><span class="sxs-lookup"><span data-stu-id="0c32b-120">To create a job WIP method</span></span>
<span data-ttu-id="0c32b-121">You can create a job WIP method that reflects the needs of your organisation.</span><span class="sxs-lookup"><span data-stu-id="0c32b-121">You can create a job WIP method that reflects the needs of your organization.</span></span> <span data-ttu-id="0c32b-122">After you have created it, you can set it as the default job WIP calculation method that will be used in your organisation.</span><span class="sxs-lookup"><span data-stu-id="0c32b-122">After you have created it, you can set it as the default job WIP calculation method that will be used in your organization.</span></span>  

> [!NOTE]
> <span data-ttu-id="0c32b-123">After you have used your new method to create WIP entries, you cannot delete the method or modify it.</span><span class="sxs-lookup"><span data-stu-id="0c32b-123">After you have used your new method to create WIP entries, you cannot delete the method or modify it.</span></span>  

1. <span data-ttu-id="0c32b-124">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Job WIP Methods**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="0c32b-124">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Job WIP Methods**, and then choose the related link.</span></span>  
2. <span data-ttu-id="0c32b-125">Choose the **New** action, and then fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="0c32b-125">Choose the **New** action, and then fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  
3. <span data-ttu-id="0c32b-126">Close the page.</span><span class="sxs-lookup"><span data-stu-id="0c32b-126">Close the page.</span></span>   
4. <span data-ttu-id="0c32b-127">To make this new method the default, choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Jobs Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="0c32b-127">To make this new method the default, choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Jobs Setup**, and then choose the related link.</span></span>  
5. <span data-ttu-id="0c32b-128">In the **Default WIP Method** field, choose the method from the list.</span><span class="sxs-lookup"><span data-stu-id="0c32b-128">In the **Default WIP Method** field, choose the method from the list.</span></span>

## <a name="to-define-a-wip-method-for-a-job"></a><span data-ttu-id="0c32b-129">To define a WIP method for a job</span><span class="sxs-lookup"><span data-stu-id="0c32b-129">To define a WIP method for a job</span></span>
<span data-ttu-id="0c32b-130">When you create a new job, you must specify which job WIP method that applies.</span><span class="sxs-lookup"><span data-stu-id="0c32b-130">When you create a new job, you must specify which job WIP method that applies.</span></span> <span data-ttu-id="0c32b-131">In some cases, which Job WIP method that you can use has been set up for you as a default.</span><span class="sxs-lookup"><span data-stu-id="0c32b-131">In some cases, which Job WIP method that you can use has been set up for you as a default.</span></span>

1. <span data-ttu-id="0c32b-132">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Jobs**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="0c32b-132">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Jobs**, and then choose the related link.</span></span>
2. <span data-ttu-id="0c32b-133">Choose the **New** action.</span><span class="sxs-lookup"><span data-stu-id="0c32b-133">Choose the **New** action.</span></span> <span data-ttu-id="0c32b-134">For more information, see [Create Jobs](projects-how-create-jobs.md).</span><span class="sxs-lookup"><span data-stu-id="0c32b-134">For more information, see [Create Jobs](projects-how-create-jobs.md).</span></span>  
3. <span data-ttu-id="0c32b-135">On the **Job Card** page, in the **WIP Method** field, select a WIP method from the list.</span><span class="sxs-lookup"><span data-stu-id="0c32b-135">On the **Job Card** page, in the **WIP Method** field, select a WIP method from the list.</span></span> <span data-ttu-id="0c32b-136">If a default method has been defined, you can select another option if needed.</span><span class="sxs-lookup"><span data-stu-id="0c32b-136">If a default method has been defined, you can select another option if needed.</span></span>  

## <a name="to-calculate-wip"></a><span data-ttu-id="0c32b-137">To calculate WIP</span><span class="sxs-lookup"><span data-stu-id="0c32b-137">To calculate WIP</span></span>
<span data-ttu-id="0c32b-138">You can determine the WIP amount that is to be posted to balance sheet accounts for the period end reporting.</span><span class="sxs-lookup"><span data-stu-id="0c32b-138">You can determine the WIP amount that is to be posted to balance sheet accounts for the period end reporting.</span></span> <span data-ttu-id="0c32b-139">You use the **Job Calculate WIP** batch job to do this.</span><span class="sxs-lookup"><span data-stu-id="0c32b-139">You use the **Job Calculate WIP** batch job to do this.</span></span>  

1. <span data-ttu-id="0c32b-140">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Job Calculate WIP**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="0c32b-140">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Job Calculate WIP**, and then choose the related link.</span></span>  
2. <span data-ttu-id="0c32b-141">Choose the **Calculate WIP** action.</span><span class="sxs-lookup"><span data-stu-id="0c32b-141">Choose the **Calculate WIP** action.</span></span>
3. <span data-ttu-id="0c32b-142">On the **Job Calculate WIP** page, fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="0c32b-142">On the **Job Calculate WIP** page, fill in the fields as necessary.</span></span>
4. <span data-ttu-id="0c32b-143">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="0c32b-143">Choose the **OK** button.</span></span>  

> [!NOTE]  
>   <span data-ttu-id="0c32b-144">The batch job only calculates the WIP.</span><span class="sxs-lookup"><span data-stu-id="0c32b-144">The batch job only calculates the WIP.</span></span> <span data-ttu-id="0c32b-145">It is not posted to the general ledger.</span><span class="sxs-lookup"><span data-stu-id="0c32b-145">It is not posted to the general ledger.</span></span> <span data-ttu-id="0c32b-146">To do so, you must run the **Post WIP to G/L** batch job when you have calculated the WIP.</span><span class="sxs-lookup"><span data-stu-id="0c32b-146">To do so, you must run the **Post WIP to G/L** batch job when you have calculated the WIP.</span></span> <span data-ttu-id="0c32b-147">For more information, see the following procedure.</span><span class="sxs-lookup"><span data-stu-id="0c32b-147">For more information, see the following procedure.</span></span>

## <a name="to-post-wip"></a><span data-ttu-id="0c32b-148">To post WIP</span><span class="sxs-lookup"><span data-stu-id="0c32b-148">To post WIP</span></span>
<span data-ttu-id="0c32b-149">When you have calculated WIP, you can post it to balance sheet accounts for the period end reporting.</span><span class="sxs-lookup"><span data-stu-id="0c32b-149">When you have calculated WIP, you can post it to balance sheet accounts for the period end reporting.</span></span> <span data-ttu-id="0c32b-150">You use the **Job Post WIP to G/L** batch job to do this.</span><span class="sxs-lookup"><span data-stu-id="0c32b-150">You use the **Job Post WIP to G/L** batch job to do this.</span></span>

1. <span data-ttu-id="0c32b-151">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Job Post WIP to G/L**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="0c32b-151">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Job Post WIP to G/L**, and then choose the related link.</span></span>  
2. <span data-ttu-id="0c32b-152">On the **Job Post WIP to G/L** page, fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="0c32b-152">On the **Job Post WIP to G/L** page, fill in the fields as necessary.</span></span>  
3. <span data-ttu-id="0c32b-153">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="0c32b-153">Choose the **OK** button.</span></span>

## <a name="to-calculate-and-post-job-completion-entries"></a><span data-ttu-id="0c32b-154">To calculate and post job completion entries</span><span class="sxs-lookup"><span data-stu-id="0c32b-154">To calculate and post job completion entries</span></span>
<span data-ttu-id="0c32b-155">When you have completed all activities for a job, including usage posting and invoicing, you must update the job to have a **Status** of **Completed**.</span><span class="sxs-lookup"><span data-stu-id="0c32b-155">When you have completed all activities for a job, including usage posting and invoicing, you must update the job to have a **Status** of **Completed**.</span></span> <span data-ttu-id="0c32b-156">Then, you must reverse any WIP that has been posted to the general ledger.</span><span class="sxs-lookup"><span data-stu-id="0c32b-156">Then, you must reverse any WIP that has been posted to the general ledger.</span></span>

1. <span data-ttu-id="0c32b-157">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Jobs**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="0c32b-157">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Jobs**, and then choose the related link.</span></span>  
2. <span data-ttu-id="0c32b-158">Select an open job, and then choose the **Edit** action.</span><span class="sxs-lookup"><span data-stu-id="0c32b-158">Select an open job, and then choose the **Edit** action.</span></span>
3. <span data-ttu-id="0c32b-159">In the **Status** field, select **Completed**.</span><span class="sxs-lookup"><span data-stu-id="0c32b-159">In the **Status** field, select **Completed**.</span></span>
4. <span data-ttu-id="0c32b-160">Follow the assistance steps to calculate and post WIP.</span><span class="sxs-lookup"><span data-stu-id="0c32b-160">Follow the assistance steps to calculate and post WIP.</span></span> <span data-ttu-id="0c32b-161">Alternatively, follows steps 5 and 6 to do so manually.</span><span class="sxs-lookup"><span data-stu-id="0c32b-161">Alternatively, follows steps 5 and 6 to do so manually.</span></span>  
5. <span data-ttu-id="0c32b-162">Choose the **Calculate WIP** action.</span><span class="sxs-lookup"><span data-stu-id="0c32b-162">Choose the **Calculate WIP** action.</span></span>
6. <span data-ttu-id="0c32b-163">On the **Job Calculate WIP** page, fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="0c32b-163">On the **Job Calculate WIP** page, fill in the fields as necessary.</span></span>  

     <span data-ttu-id="0c32b-164">The job WIP entries created by running the batch job will have the **Job Complete** check box selected to show that they are completion entries.</span><span class="sxs-lookup"><span data-stu-id="0c32b-164">The job WIP entries created by running the batch job will have the **Job Complete** check box selected to show that they are completion entries.</span></span>  
7. <span data-ttu-id="0c32b-165">Choose the **Job Post WIP to G/L** action.</span><span class="sxs-lookup"><span data-stu-id="0c32b-165">Choose the **Job Post WIP to G/L** action.</span></span>
8. <span data-ttu-id="0c32b-166">On the **Job Post WIP to G/L** page, fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="0c32b-166">On the **Job Post WIP to G/L** page, fill in the fields as necessary.</span></span>  

     <span data-ttu-id="0c32b-167">The job WIP general ledger entries created by running the batch job will have the **Job Complete** check box selected to show they are completion entries.</span><span class="sxs-lookup"><span data-stu-id="0c32b-167">The job WIP general ledger entries created by running the batch job will have the **Job Complete** check box selected to show they are completion entries.</span></span>

## <a name="to-view-job-ledger-entries"></a><span data-ttu-id="0c32b-168">To view job ledger entries</span><span class="sxs-lookup"><span data-stu-id="0c32b-168">To view job ledger entries</span></span>
<span data-ttu-id="0c32b-169">All job-related entries are recorded in job registers and are numbered sequentially, starting with 1.</span><span class="sxs-lookup"><span data-stu-id="0c32b-169">All job-related entries are recorded in job registers and are numbered sequentially, starting with 1.</span></span> <span data-ttu-id="0c32b-170">From the job register, you can get an overview of all job ledger entries.</span><span class="sxs-lookup"><span data-stu-id="0c32b-170">From the job register, you can get an overview of all job ledger entries.</span></span>    

1. <span data-ttu-id="0c32b-171">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Job Registers**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="0c32b-171">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Job Registers**, and then choose the related link.</span></span>
2. <span data-ttu-id="0c32b-172">Select a relevant register, and then choose **Job Ledger** action.</span><span class="sxs-lookup"><span data-stu-id="0c32b-172">Select a relevant register, and then choose **Job Ledger** action.</span></span>

<span data-ttu-id="0c32b-173">On the **Job Ledger Entries** page you can review the entries that are associated with any job.</span><span class="sxs-lookup"><span data-stu-id="0c32b-173">On the **Job Ledger Entries** page you can review the entries that are associated with any job.</span></span>  

## <a name="see-also"></a><span data-ttu-id="0c32b-174">See Also</span><span class="sxs-lookup"><span data-stu-id="0c32b-174">See Also</span></span>
<span data-ttu-id="0c32b-175">[Managing Projects](projects-manage-projects.md)
[Managing Inventory Costs](finance-manage-inventory-costs.md) </span><span class="sxs-lookup"><span data-stu-id="0c32b-175">[Managing Projects](projects-manage-projects.md)
[Managing Inventory Costs](finance-manage-inventory-costs.md) </span></span>  
[<span data-ttu-id="0c32b-176">Finance</span><span class="sxs-lookup"><span data-stu-id="0c32b-176">Finance</span></span>](finance.md)  
<span data-ttu-id="0c32b-177">[Purchasing](purchasing-manage-purchasing.md)       </span><span class="sxs-lookup"><span data-stu-id="0c32b-177">[Purchasing](purchasing-manage-purchasing.md)       </span></span>  
<span data-ttu-id="0c32b-178">[Sales](sales-manage-sales.md)    </span><span class="sxs-lookup"><span data-stu-id="0c32b-178">[Sales](sales-manage-sales.md)    </span></span>  
<span data-ttu-id="0c32b-179">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="0c32b-179">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>  


[!INCLUDE[footer-include](includes/footer-banner.md)]
