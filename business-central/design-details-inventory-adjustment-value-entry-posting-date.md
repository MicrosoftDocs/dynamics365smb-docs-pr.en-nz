---
title: Posting date on value entries
description: Learn how the Adjust Cost - Item Entries batch job identifies and assigns a posting date to the value entries that the batch job is about to create.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 11/23/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: c95432ec1cf24aaaedf0fad5a2746ace9705e2e3
ms.contentlocale: en-nz
ms.lasthandoff: 03/22/2018

---
# <a name="design-details-posting-date-on-adjustment-value-entry"></a><span data-ttu-id="5e27c-103">Design Details: Posting Date on Adjustment Value Entry</span><span class="sxs-lookup"><span data-stu-id="5e27c-103">Design Details: Posting Date on Adjustment Value Entry</span></span>
<span data-ttu-id="5e27c-104">This article provides guidance for users of the Inventory Costing functionality in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="5e27c-104">This article provides guidance for users of the Inventory Costing functionality in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="5e27c-105">The specific article is providing guidance in how the **Adjust Cost - Item Entries** batch job identifies and assigns a posting date to the value entries that the batch job is about to create.</span><span class="sxs-lookup"><span data-stu-id="5e27c-105">The specific article is providing guidance in how the **Adjust Cost - Item Entries** batch job identifies and assigns a posting date to the value entries that the batch job is about to create.</span></span>  

<span data-ttu-id="5e27c-106">First the concept of the process is reviewed, how the batch job identifies and assigns the Posting Date to the Value Entry to be created.</span><span class="sxs-lookup"><span data-stu-id="5e27c-106">First the concept of the process is reviewed, how the batch job identifies and assigns the Posting Date to the Value Entry to be created.</span></span> <span data-ttu-id="5e27c-107">Thereafter there are some scenarios shared that we in the support team come across from time to time and finally there is a summary of the concepts used from version 3.0.</span><span class="sxs-lookup"><span data-stu-id="5e27c-107">Thereafter there are some scenarios shared that we in the support team come across from time to time and finally there is a summary of the concepts used from version 3.0.</span></span>  

## <a name="the-concept"></a><span data-ttu-id="5e27c-108">The Concept</span><span class="sxs-lookup"><span data-stu-id="5e27c-108">The Concept</span></span>  
<span data-ttu-id="5e27c-109">From version 5.0, the **Adjust Cost – Item Entries** batch job assigns a posting date to the value entry it is about to create in the following steps:</span><span class="sxs-lookup"><span data-stu-id="5e27c-109">From version 5.0, the **Adjust Cost – Item Entries** batch job assigns a posting date to the value entry it is about to create in the following steps:</span></span>  

1.  <span data-ttu-id="5e27c-110">Initially the Posting Date of the entry to be created is the same date as the entry it adjusts.</span><span class="sxs-lookup"><span data-stu-id="5e27c-110">Initially the Posting Date of the entry to be created is the same date as the entry it adjusts.</span></span>  

2.  <span data-ttu-id="5e27c-111">The Posting Date is validated against Inventory Periods and/or General Ledger Setup.</span><span class="sxs-lookup"><span data-stu-id="5e27c-111">The Posting Date is validated against Inventory Periods and/or General Ledger Setup.</span></span>  

3.  <span data-ttu-id="5e27c-112">Assignment of Posting Date; If the initial Posting Date is not within allowed posting date range the batch job will assign an allowed Posting Date from either General Ledger Setup or Inventory Period.</span><span class="sxs-lookup"><span data-stu-id="5e27c-112">Assignment of Posting Date; If the initial Posting Date is not within allowed posting date range the batch job will assign an allowed Posting Date from either General Ledger Setup or Inventory Period.</span></span> <span data-ttu-id="5e27c-113">If both Inventory Periods and allowed posting dates in General Ledger Setup are defined, the later date of the two will be assigned to the Adjustment Value Entry.</span><span class="sxs-lookup"><span data-stu-id="5e27c-113">If both Inventory Periods and allowed posting dates in General Ledger Setup are defined, the later date of the two will be assigned to the Adjustment Value Entry.</span></span>  

 <span data-ttu-id="5e27c-114">Let’s review this process more in practice.</span><span class="sxs-lookup"><span data-stu-id="5e27c-114">Let’s review this process more in practice.</span></span> <span data-ttu-id="5e27c-115">Assume we have an Item Ledger Entry of Sale.</span><span class="sxs-lookup"><span data-stu-id="5e27c-115">Assume we have an Item Ledger Entry of Sale.</span></span> <span data-ttu-id="5e27c-116">The item was shipped on September 5th, 2013 and it was invoiced the day after.</span><span class="sxs-lookup"><span data-stu-id="5e27c-116">The item was shipped on September 5th, 2013 and it was invoiced the day after.</span></span>  

<span data-ttu-id="5e27c-117">![Item Ledger Entry: Date format: YYYY MM DD](media/helene/TechArticleAdjustcost1.png "TechArticleAdjustcost1")</span><span class="sxs-lookup"><span data-stu-id="5e27c-117">![Item Ledger Entry: Date format: YYYY MM DD](media/helene/TechArticleAdjustcost1.png "TechArticleAdjustcost1")</span></span>  

<span data-ttu-id="5e27c-118">Below, the first Value Entry (379) represents the shipment and carry the same Posting Date as the parent Item ledger Entry.</span><span class="sxs-lookup"><span data-stu-id="5e27c-118">Below, the first Value Entry (379) represents the shipment and carry the same Posting Date as the parent Item ledger Entry.</span></span>  

<span data-ttu-id="5e27c-119">The second Value Entry (381) represents the invoice.</span><span class="sxs-lookup"><span data-stu-id="5e27c-119">The second Value Entry (381) represents the invoice.</span></span>  

 <span data-ttu-id="5e27c-120">The third Value Entry (391) is an Adjustment of the invoicing Value Entry (381)</span><span class="sxs-lookup"><span data-stu-id="5e27c-120">The third Value Entry (391) is an Adjustment of the invoicing Value Entry (381)</span></span>  

 <span data-ttu-id="5e27c-121">![Item Ledger Entry: Date format: YYYY MM DD](media/helene/TechArticleAdjustcost2.png "TechArticleAdjustcost2")</span><span class="sxs-lookup"><span data-stu-id="5e27c-121">![Item Ledger Entry: Date format: YYYY MM DD](media/helene/TechArticleAdjustcost2.png "TechArticleAdjustcost2")</span></span>  

 <span data-ttu-id="5e27c-122">Step 1: Adjustment Value Entry to be created is assigned same Posting Date as the entry it adjusts, illustrated above by Value entry 391.</span><span class="sxs-lookup"><span data-stu-id="5e27c-122">Step 1: Adjustment Value Entry to be created is assigned same Posting Date as the entry it adjusts, illustrated above by Value entry 391.</span></span>  

 <span data-ttu-id="5e27c-123">Step 2: Validation of initial assigned Posting Date.</span><span class="sxs-lookup"><span data-stu-id="5e27c-123">Step 2: Validation of initial assigned Posting Date.</span></span>  

<span data-ttu-id="5e27c-124">The **Adjust Cost – Item Entries** batch job determines if the initial Posting Date of the Adjustment Value Entry is within allowed posting date range based upon Inventory Periods and/or General Ledger Setup.</span><span class="sxs-lookup"><span data-stu-id="5e27c-124">The **Adjust Cost – Item Entries** batch job determines if the initial Posting Date of the Adjustment Value Entry is within allowed posting date range based upon Inventory Periods and/or General Ledger Setup.</span></span>  

 <span data-ttu-id="5e27c-125">Let’s review the above mentioned Sale by adding setup of allowed posting date ranges.</span><span class="sxs-lookup"><span data-stu-id="5e27c-125">Let’s review the above mentioned Sale by adding setup of allowed posting date ranges.</span></span>  

 <span data-ttu-id="5e27c-126">Inventory Periods:</span><span class="sxs-lookup"><span data-stu-id="5e27c-126">Inventory Periods:</span></span>  

<span data-ttu-id="5e27c-127">![Adjust cost &#45;Item entries data](media/helene/TechArticleAdjustcost3.png "TechArticleAdjustcost3")</span><span class="sxs-lookup"><span data-stu-id="5e27c-127">![Adjust cost &#45;Item entries data](media/helene/TechArticleAdjustcost3.png "TechArticleAdjustcost3")</span></span>

 <span data-ttu-id="5e27c-128">First allowed posting date is the first day in the first open period.</span><span class="sxs-lookup"><span data-stu-id="5e27c-128">First allowed posting date is the first day in the first open period.</span></span> <span data-ttu-id="5e27c-129">September 1st, 2013.</span><span class="sxs-lookup"><span data-stu-id="5e27c-129">September 1st, 2013.</span></span>  

 <span data-ttu-id="5e27c-130">General Ledger Setup:</span><span class="sxs-lookup"><span data-stu-id="5e27c-130">General Ledger Setup:</span></span>  

<span data-ttu-id="5e27c-131">![Adjust cost &#45;Item entries data](media/helene/TechArticleAdjustcost4.png "TechArticleAdjustcost4")</span><span class="sxs-lookup"><span data-stu-id="5e27c-131">![Adjust cost &#45;Item entries data](media/helene/TechArticleAdjustcost4.png "TechArticleAdjustcost4")</span></span>

 <span data-ttu-id="5e27c-132">First allowed posting date is the date stated in field Allow Posting From: September 10th, 2013.</span><span class="sxs-lookup"><span data-stu-id="5e27c-132">First allowed posting date is the date stated in field Allow Posting From: September 10th, 2013.</span></span>  

 <span data-ttu-id="5e27c-133">If both Inventory Periods and allowed posting dates in General Ledger Setup are defined, the later date of the two will define the allowed posting date range.</span><span class="sxs-lookup"><span data-stu-id="5e27c-133">If both Inventory Periods and allowed posting dates in General Ledger Setup are defined, the later date of the two will define the allowed posting date range.</span></span>  

 <span data-ttu-id="5e27c-134">Step 3: Assignment of an allowed posting date;</span><span class="sxs-lookup"><span data-stu-id="5e27c-134">Step 3: Assignment of an allowed posting date;</span></span>  

 <span data-ttu-id="5e27c-135">The initial assigned Posting Date was September 6th as illustrated in step 1.</span><span class="sxs-lookup"><span data-stu-id="5e27c-135">The initial assigned Posting Date was September 6th as illustrated in step 1.</span></span> <span data-ttu-id="5e27c-136">However, in the 2nd step the Adjust Cost – Item entries batch job identifies that earliest allowed Posting Date is September 10th and thereby assigns September 10th to the Adjustment Value Entry, below.</span><span class="sxs-lookup"><span data-stu-id="5e27c-136">However, in the 2nd step the Adjust Cost – Item entries batch job identifies that earliest allowed Posting Date is September 10th and thereby assigns September 10th to the Adjustment Value Entry, below.</span></span>  

 <span data-ttu-id="5e27c-137">![Adjust cost &#45;Item entries data](media/helene/TechArticleAdjustcost5.png "TechArticleAdjustcost5")</span><span class="sxs-lookup"><span data-stu-id="5e27c-137">![Adjust cost &#45;Item entries data](media/helene/TechArticleAdjustcost5.png "TechArticleAdjustcost5")</span></span>

 <span data-ttu-id="5e27c-138">We have now reviewed the concept for assigning Posting Dates to Value Entries created by the Adjust Cost - Item entries batch job.</span><span class="sxs-lookup"><span data-stu-id="5e27c-138">We have now reviewed the concept for assigning Posting Dates to Value Entries created by the Adjust Cost - Item entries batch job.</span></span>  

 <span data-ttu-id="5e27c-139">Let’s continue to review some scenarios that we in the support team comes across from time to time in relation to assigned Posting Dates in the Adjust Cost – Item entries batch job and related setups.</span><span class="sxs-lookup"><span data-stu-id="5e27c-139">Let’s continue to review some scenarios that we in the support team comes across from time to time in relation to assigned Posting Dates in the Adjust Cost – Item entries batch job and related setups.</span></span>  

## <a name="scenarios"></a><span data-ttu-id="5e27c-140">Scenarios</span><span class="sxs-lookup"><span data-stu-id="5e27c-140">Scenarios</span></span>  

### <a name="scenario-i-posting-date-is-not-within-your-range-of-allowed-posting-dates"></a><span data-ttu-id="5e27c-141">Scenario I: “Posting Date is not within your range of allowed posting dates…”</span><span class="sxs-lookup"><span data-stu-id="5e27c-141">Scenario I: “Posting Date is not within your range of allowed posting dates…”</span></span>  
 <span data-ttu-id="5e27c-142">This is a scenario where a user is experiencing mentioned error message when the Adjust Cost – Item entries batch job is run.</span><span class="sxs-lookup"><span data-stu-id="5e27c-142">This is a scenario where a user is experiencing mentioned error message when the Adjust Cost – Item entries batch job is run.</span></span>  

 <span data-ttu-id="5e27c-143">In the previous section, describing the concept of assigning posting dates, the intention of the Adjust Cost – Item entries batch job is to create a Value Entry with Posting Date September 10th.</span><span class="sxs-lookup"><span data-stu-id="5e27c-143">In the previous section, describing the concept of assigning posting dates, the intention of the Adjust Cost – Item entries batch job is to create a Value Entry with Posting Date September 10th.</span></span>  

<span data-ttu-id="5e27c-144">![Adjust cost &#45;Item entries data](media/helene/TechArticleAdjustcost6.png "TechArticleAdjustcost6")</span><span class="sxs-lookup"><span data-stu-id="5e27c-144">![Adjust cost &#45;Item entries data](media/helene/TechArticleAdjustcost6.png "TechArticleAdjustcost6")</span></span>

 <span data-ttu-id="5e27c-145">We follow up on the User Setup:</span><span class="sxs-lookup"><span data-stu-id="5e27c-145">We follow up on the User Setup:</span></span>  

<span data-ttu-id="5e27c-146">![Adjust cost &#45;Item entries data](media/helene/TechArticleAdjustcost7.png "TechArticleAdjustcost7")</span><span class="sxs-lookup"><span data-stu-id="5e27c-146">![Adjust cost &#45;Item entries data](media/helene/TechArticleAdjustcost7.png "TechArticleAdjustcost7")</span></span>

 <span data-ttu-id="5e27c-147">The user in this case has an allowed posting date range from September 11th to September 30th and is thereby not allowed to post the Adjustment Value Entry with Posting Date September 10th.</span><span class="sxs-lookup"><span data-stu-id="5e27c-147">The user in this case has an allowed posting date range from September 11th to September 30th and is thereby not allowed to post the Adjustment Value Entry with Posting Date September 10th.</span></span>  

<span data-ttu-id="5e27c-148">![Adjust cost &#45;Item entries data](media/helene/TechArticleAdjustcost8.png "TechArticleAdjustcost8")</span><span class="sxs-lookup"><span data-stu-id="5e27c-148">![Adjust cost &#45;Item entries data](media/helene/TechArticleAdjustcost8.png "TechArticleAdjustcost8")</span></span>

 <span data-ttu-id="5e27c-149">Knowledge Base article [952996](https://mbs2.microsoft.com/Knowledgebase/kbdisplay.aspx?WTNTZSMNWUKNTMMYXUPYZQPOUXNXSPSYOQQYYMLUQLOYYMWP) discusses additional scenarios related to mentioned error message.</span><span class="sxs-lookup"><span data-stu-id="5e27c-149">Knowledge Base article [952996](https://mbs2.microsoft.com/Knowledgebase/kbdisplay.aspx?WTNTZSMNWUKNTMMYXUPYZQPOUXNXSPSYOQQYYMLUQLOYYMWP) discusses additional scenarios related to mentioned error message.</span></span>  

### <a name="scenario-ii-posting-date-on-adjustment-value-entry-versus-posting-date-on-entry-causing-the-adjustment-such-as-revaluation-or-item-charge"></a><span data-ttu-id="5e27c-150">Scenario II: Posting Date on Adjustment Value Entry versus Posting Date on entry causing the adjustment such as Revaluation or Item charge.</span><span class="sxs-lookup"><span data-stu-id="5e27c-150">Scenario II: Posting Date on Adjustment Value Entry versus Posting Date on entry causing the adjustment such as Revaluation or Item charge.</span></span>  

### <a name="revaluation-scenario"></a><span data-ttu-id="5e27c-151">Revaluation scenario:</span><span class="sxs-lookup"><span data-stu-id="5e27c-151">Revaluation scenario:</span></span>  
 <span data-ttu-id="5e27c-152">Prerequisites:</span><span class="sxs-lookup"><span data-stu-id="5e27c-152">Prerequisites:</span></span>  

 <span data-ttu-id="5e27c-153">Inventory setup:</span><span class="sxs-lookup"><span data-stu-id="5e27c-153">Inventory setup:</span></span>  

-   <span data-ttu-id="5e27c-154">Automatic Cost Posting = Yes</span><span class="sxs-lookup"><span data-stu-id="5e27c-154">Automatic Cost Posting = Yes</span></span>  

-   <span data-ttu-id="5e27c-155">Automatic Cost Adjustment=Always</span><span class="sxs-lookup"><span data-stu-id="5e27c-155">Automatic Cost Adjustment=Always</span></span>  

-   <span data-ttu-id="5e27c-156">Average Cost Calc. Type=item</span><span class="sxs-lookup"><span data-stu-id="5e27c-156">Average Cost Calc. Type=item</span></span>  

-   <span data-ttu-id="5e27c-157">Average Cost Period=Day</span><span class="sxs-lookup"><span data-stu-id="5e27c-157">Average Cost Period=Day</span></span>  

 <span data-ttu-id="5e27c-158">General Ledger Setup:</span><span class="sxs-lookup"><span data-stu-id="5e27c-158">General Ledger Setup:</span></span>  

-   <span data-ttu-id="5e27c-159">Allow Posting From = January 1st, 2014</span><span class="sxs-lookup"><span data-stu-id="5e27c-159">Allow Posting From = January 1st, 2014</span></span>  

-   <span data-ttu-id="5e27c-160">Allow Posting To = empty</span><span class="sxs-lookup"><span data-stu-id="5e27c-160">Allow Posting To = empty</span></span>  

 <span data-ttu-id="5e27c-161">User Setup:</span><span class="sxs-lookup"><span data-stu-id="5e27c-161">User Setup:</span></span>  

-   <span data-ttu-id="5e27c-162">Allow Posting From = December 1st, 2013.</span><span class="sxs-lookup"><span data-stu-id="5e27c-162">Allow Posting From = December 1st, 2013.</span></span>  

-   <span data-ttu-id="5e27c-163">Allow Posting to = empty</span><span class="sxs-lookup"><span data-stu-id="5e27c-163">Allow Posting to = empty</span></span>  

##### <a name="to-test-the-scenario"></a><span data-ttu-id="5e27c-164">To test the scenario</span><span class="sxs-lookup"><span data-stu-id="5e27c-164">To test the scenario</span></span>  

1.  <span data-ttu-id="5e27c-165">Create item TEST:</span><span class="sxs-lookup"><span data-stu-id="5e27c-165">Create item TEST:</span></span>  

     <span data-ttu-id="5e27c-166">Base unit of measure = PCS</span><span class="sxs-lookup"><span data-stu-id="5e27c-166">Base unit of measure = PCS</span></span>  

     <span data-ttu-id="5e27c-167">Costing Method = Average</span><span class="sxs-lookup"><span data-stu-id="5e27c-167">Costing Method = Average</span></span>  

     <span data-ttu-id="5e27c-168">Select optional posting groups.</span><span class="sxs-lookup"><span data-stu-id="5e27c-168">Select optional posting groups.</span></span>  

2.  <span data-ttu-id="5e27c-169">Open Item Journal, create and post a line as follows:</span><span class="sxs-lookup"><span data-stu-id="5e27c-169">Open Item Journal, create and post a line as follows:</span></span>  

     <span data-ttu-id="5e27c-170">Posting Date = December 15th, 2013</span><span class="sxs-lookup"><span data-stu-id="5e27c-170">Posting Date = December 15th, 2013</span></span>  

     <span data-ttu-id="5e27c-171">Item = TEST</span><span class="sxs-lookup"><span data-stu-id="5e27c-171">Item = TEST</span></span>  

     <span data-ttu-id="5e27c-172">Entry Type = Purchase</span><span class="sxs-lookup"><span data-stu-id="5e27c-172">Entry Type = Purchase</span></span>  

     <span data-ttu-id="5e27c-173">Quantity = 100</span><span class="sxs-lookup"><span data-stu-id="5e27c-173">Quantity = 100</span></span>  

     <span data-ttu-id="5e27c-174">Unit Amount = 10</span><span class="sxs-lookup"><span data-stu-id="5e27c-174">Unit Amount = 10</span></span>  

3.  <span data-ttu-id="5e27c-175">Open Item Journal, create and post a line as follows:</span><span class="sxs-lookup"><span data-stu-id="5e27c-175">Open Item Journal, create and post a line as follows:</span></span>  

     <span data-ttu-id="5e27c-176">Date = December 20th, 2013</span><span class="sxs-lookup"><span data-stu-id="5e27c-176">Date = December 20th, 2013</span></span>  

     <span data-ttu-id="5e27c-177">Item = TEST</span><span class="sxs-lookup"><span data-stu-id="5e27c-177">Item = TEST</span></span>  

     <span data-ttu-id="5e27c-178">Entry Type = Negative Adjustment</span><span class="sxs-lookup"><span data-stu-id="5e27c-178">Entry Type = Negative Adjustment</span></span>  

     <span data-ttu-id="5e27c-179">Quantity = 2</span><span class="sxs-lookup"><span data-stu-id="5e27c-179">Quantity = 2</span></span>  

4.  <span data-ttu-id="5e27c-180">Open Item Journal, create and post a line as follows:</span><span class="sxs-lookup"><span data-stu-id="5e27c-180">Open Item Journal, create and post a line as follows:</span></span>  

     <span data-ttu-id="5e27c-181">Date = January 15th, 2014</span><span class="sxs-lookup"><span data-stu-id="5e27c-181">Date = January 15th, 2014</span></span>  

     <span data-ttu-id="5e27c-182">Item = TEST</span><span class="sxs-lookup"><span data-stu-id="5e27c-182">Item = TEST</span></span>  

     <span data-ttu-id="5e27c-183">Entry Type = Negative Adjustment</span><span class="sxs-lookup"><span data-stu-id="5e27c-183">Entry Type = Negative Adjustment</span></span>  

     <span data-ttu-id="5e27c-184">Quantity = 3</span><span class="sxs-lookup"><span data-stu-id="5e27c-184">Quantity = 3</span></span>  

5.  <span data-ttu-id="5e27c-185">Open Revaluation Journal, create and post a line as follows:</span><span class="sxs-lookup"><span data-stu-id="5e27c-185">Open Revaluation Journal, create and post a line as follows:</span></span>  

     <span data-ttu-id="5e27c-186">Item = TEST</span><span class="sxs-lookup"><span data-stu-id="5e27c-186">Item = TEST</span></span>  

     <span data-ttu-id="5e27c-187">Applies-to Entry = select Purchase entry posted at step 2.</span><span class="sxs-lookup"><span data-stu-id="5e27c-187">Applies-to Entry = select Purchase entry posted at step 2.</span></span> <span data-ttu-id="5e27c-188">The Posting Date of the revaluation will be the same as the entry it adjusts.</span><span class="sxs-lookup"><span data-stu-id="5e27c-188">The Posting Date of the revaluation will be the same as the entry it adjusts.</span></span>  

     <span data-ttu-id="5e27c-189">Unit Cost Revalued = 40</span><span class="sxs-lookup"><span data-stu-id="5e27c-189">Unit Cost Revalued = 40</span></span>  

 <span data-ttu-id="5e27c-190">The following Item Ledger and Value Entries have been posted:</span><span class="sxs-lookup"><span data-stu-id="5e27c-190">The following Item Ledger and Value Entries have been posted:</span></span>  

<span data-ttu-id="5e27c-191">![Adjust cost &#45;Item entries data](media/helene/TechArticleAdjustcost9.png "TechArticleAdjustcost9")</span><span class="sxs-lookup"><span data-stu-id="5e27c-191">![Adjust cost &#45;Item entries data](media/helene/TechArticleAdjustcost9.png "TechArticleAdjustcost9")</span></span>

 <span data-ttu-id="5e27c-192">![Adjust cost &#45;Item entries data](media/helene/TechArticleAdjustcost10.png "TechArticleAdjustcost10")</span><span class="sxs-lookup"><span data-stu-id="5e27c-192">![Adjust cost &#45;Item entries data](media/helene/TechArticleAdjustcost10.png "TechArticleAdjustcost10")</span></span>

 <span data-ttu-id="5e27c-193">The Adjust Cost – Item entries batch job has recognised a change in cost and adjusted the Negative Adjustments.</span><span class="sxs-lookup"><span data-stu-id="5e27c-193">The Adjust Cost – Item entries batch job has recognized a change in cost and adjusted the Negative Adjustments.</span></span>  

 <span data-ttu-id="5e27c-194">**Review of Posting Dates on created Adjustment Value Entries:** The earliest allowed Posting Date the Adjust Cost - Item Entries batch job has to relate to is January 1st, 2014 as stated in the General Ledger Setup.</span><span class="sxs-lookup"><span data-stu-id="5e27c-194">**Review of Posting Dates on created Adjustment Value Entries:** The earliest allowed Posting Date the Adjust Cost - Item Entries batch job has to relate to is January 1st, 2014 as stated in the General Ledger Setup.</span></span>  

 <span data-ttu-id="5e27c-195">**Negative Adjustment in step 3:** assigned Posting Date is January 1st, provided by General Ledger Setup.</span><span class="sxs-lookup"><span data-stu-id="5e27c-195">**Negative Adjustment in step 3:** assigned Posting Date is January 1st, provided by General Ledger Setup.</span></span> <span data-ttu-id="5e27c-196">The Posting Date of the Value Entry in scope for adjustment is December 20, 2013.</span><span class="sxs-lookup"><span data-stu-id="5e27c-196">The Posting Date of the Value Entry in scope for adjustment is December 20, 2013.</span></span> <span data-ttu-id="5e27c-197">According to General Ledger Setup the date is not within allowed posting date range.</span><span class="sxs-lookup"><span data-stu-id="5e27c-197">According to General Ledger Setup the date is not within allowed posting date range.</span></span> <span data-ttu-id="5e27c-198">Therefore the Posting Date stated in the Allow Posting From field in the General Ledger Setup is assigned to the Adjustment Value Entry.</span><span class="sxs-lookup"><span data-stu-id="5e27c-198">Therefore the Posting Date stated in the Allow Posting From field in the General Ledger Setup is assigned to the Adjustment Value Entry.</span></span>  

 <span data-ttu-id="5e27c-199">**Negative Adjustment in step 4:** assigned Posting Date is January 15th.</span><span class="sxs-lookup"><span data-stu-id="5e27c-199">**Negative Adjustment in step 4:** assigned Posting Date is January 15th.</span></span> <span data-ttu-id="5e27c-200">The Value Entry in scope of adjustment has Posting Date January 15th, which is within the allowed posting date range according to General Ledger Setup.</span><span class="sxs-lookup"><span data-stu-id="5e27c-200">The Value Entry in scope of adjustment has Posting Date January 15th, which is within the allowed posting date range according to General Ledger Setup.</span></span>  

 <span data-ttu-id="5e27c-201">The adjustment made for the Negative Adjustment in step 3 causes discussion.</span><span class="sxs-lookup"><span data-stu-id="5e27c-201">The adjustment made for the Negative Adjustment in step 3 causes discussion.</span></span> <span data-ttu-id="5e27c-202">The favorable Posting Date for the Adjustment Value Entry would have been December 20th or at least within December as the revaluation causing the change in COGS was posted in December.</span><span class="sxs-lookup"><span data-stu-id="5e27c-202">The favorable Posting Date for the Adjustment Value Entry would have been December 20th or at least within December as the revaluation causing the change in COGS was posted in December.</span></span>  

 <span data-ttu-id="5e27c-203">To achieve adjustment in December of the Negative Adjustment in step 3, the General Ledger Setup, Allow Posting From field, need to state a date in December.</span><span class="sxs-lookup"><span data-stu-id="5e27c-203">To achieve adjustment in December of the Negative Adjustment in step 3, the General Ledger Setup, Allow Posting From field, need to state a date in December.</span></span>  

 <span data-ttu-id="5e27c-204">**Conclusion:**</span><span class="sxs-lookup"><span data-stu-id="5e27c-204">**Conclusion:**</span></span>  

 <span data-ttu-id="5e27c-205">With the experiences from this scenario, considering most suitable setup of allowed posting date range for a company, the following might be useful: As long as changes in inventory value is allowed to be posted in a period, December in this case, the setup the company uses for allowed posting date ranges should be aligned with this decision.</span><span class="sxs-lookup"><span data-stu-id="5e27c-205">With the experiences from this scenario, considering most suitable setup of allowed posting date range for a company, the following might be useful: As long as changes in inventory value is allowed to be posted in a period, December in this case, the setup the company uses for allowed posting date ranges should be aligned with this decision.</span></span> <span data-ttu-id="5e27c-206">The Allow Posting From in the General Ledger Setup, stating December 1st  would allow the revaluation made in December to be forwarded to affected outbound entries in the same period.</span><span class="sxs-lookup"><span data-stu-id="5e27c-206">The Allow Posting From in the General Ledger Setup, stating December 1st  would allow the revaluation made in December to be forwarded to affected outbound entries in the same period.</span></span>  

 <span data-ttu-id="5e27c-207">User groups not allowed to post in December but in January, which was probably intended to be limited by the General Ledger Setup in this scenario, should instead be addressed via the User setup.</span><span class="sxs-lookup"><span data-stu-id="5e27c-207">User groups not allowed to post in December but in January, which was probably intended to be limited by the General Ledger Setup in this scenario, should instead be addressed via the User setup.</span></span>  

### <a name="item-charge-scenario"></a><span data-ttu-id="5e27c-208">Item charge scenario:</span><span class="sxs-lookup"><span data-stu-id="5e27c-208">Item charge scenario:</span></span>  
 <span data-ttu-id="5e27c-209">Prerequisites:</span><span class="sxs-lookup"><span data-stu-id="5e27c-209">Prerequisites:</span></span>  

 <span data-ttu-id="5e27c-210">Inventory setup:</span><span class="sxs-lookup"><span data-stu-id="5e27c-210">Inventory setup:</span></span>  

-   <span data-ttu-id="5e27c-211">Automatic Cost Posting = Yes</span><span class="sxs-lookup"><span data-stu-id="5e27c-211">Automatic Cost Posting = Yes</span></span>  

-   <span data-ttu-id="5e27c-212">Automatic Cost Adjustment=Always</span><span class="sxs-lookup"><span data-stu-id="5e27c-212">Automatic Cost Adjustment=Always</span></span>  

-   <span data-ttu-id="5e27c-213">Average Cost Calc. Type=item</span><span class="sxs-lookup"><span data-stu-id="5e27c-213">Average Cost Calc. Type=item</span></span>  

-   <span data-ttu-id="5e27c-214">Average Cost Period=Day</span><span class="sxs-lookup"><span data-stu-id="5e27c-214">Average Cost Period=Day</span></span>  

 <span data-ttu-id="5e27c-215">General Ledger Setup:</span><span class="sxs-lookup"><span data-stu-id="5e27c-215">General Ledger Setup:</span></span>  

-   <span data-ttu-id="5e27c-216">Allow Posting From = December 1st, 2013.</span><span class="sxs-lookup"><span data-stu-id="5e27c-216">Allow Posting From = December 1st, 2013.</span></span>  

-   <span data-ttu-id="5e27c-217">Allow Posting To = empty</span><span class="sxs-lookup"><span data-stu-id="5e27c-217">Allow Posting To = empty</span></span>  

 <span data-ttu-id="5e27c-218">User Setup:</span><span class="sxs-lookup"><span data-stu-id="5e27c-218">User Setup:</span></span>  

-   <span data-ttu-id="5e27c-219">Allow Posting From = December 1st, 2013.</span><span class="sxs-lookup"><span data-stu-id="5e27c-219">Allow Posting From = December 1st, 2013.</span></span>  

-   <span data-ttu-id="5e27c-220">Allow Posting to = empty</span><span class="sxs-lookup"><span data-stu-id="5e27c-220">Allow Posting to = empty</span></span>  

##### <a name="to-test-the-scenario"></a><span data-ttu-id="5e27c-221">To test the scenario</span><span class="sxs-lookup"><span data-stu-id="5e27c-221">To test the scenario</span></span>  

1.  <span data-ttu-id="5e27c-222">Create item charge:</span><span class="sxs-lookup"><span data-stu-id="5e27c-222">Create item charge:</span></span>  

     <span data-ttu-id="5e27c-223">Base unit of measure = PCS</span><span class="sxs-lookup"><span data-stu-id="5e27c-223">Base unit of measure = PCS</span></span>  

     <span data-ttu-id="5e27c-224">Costing Method = Average</span><span class="sxs-lookup"><span data-stu-id="5e27c-224">Costing Method = Average</span></span>  

     <span data-ttu-id="5e27c-225">Select optional posting groups.</span><span class="sxs-lookup"><span data-stu-id="5e27c-225">Select optional posting groups.</span></span>  

2.  <span data-ttu-id="5e27c-226">Create new purchase order</span><span class="sxs-lookup"><span data-stu-id="5e27c-226">Create new purchase order</span></span>  

     <span data-ttu-id="5e27c-227">Buy-from Vendor No.: 10000</span><span class="sxs-lookup"><span data-stu-id="5e27c-227">Buy-from Vendor No.: 10000</span></span>  

     <span data-ttu-id="5e27c-228">Posting Date = December 15th, 2013</span><span class="sxs-lookup"><span data-stu-id="5e27c-228">Posting Date = December 15th, 2013</span></span>  

     <span data-ttu-id="5e27c-229">Vendor Invoice No.: 1234</span><span class="sxs-lookup"><span data-stu-id="5e27c-229">Vendor Invoice No.: 1234</span></span>  

     <span data-ttu-id="5e27c-230">On the purchase order line:</span><span class="sxs-lookup"><span data-stu-id="5e27c-230">On the purchase order line:</span></span>  

     <span data-ttu-id="5e27c-231">Item = CHARGE</span><span class="sxs-lookup"><span data-stu-id="5e27c-231">Item = CHARGE</span></span>  

     <span data-ttu-id="5e27c-232">Quantity = 1</span><span class="sxs-lookup"><span data-stu-id="5e27c-232">Quantity = 1</span></span>  

     <span data-ttu-id="5e27c-233">Direct Unit Cost = 100</span><span class="sxs-lookup"><span data-stu-id="5e27c-233">Direct Unit Cost = 100</span></span>  

     <span data-ttu-id="5e27c-234">Post Receive and Invoice.</span><span class="sxs-lookup"><span data-stu-id="5e27c-234">Post Receive and Invoice.</span></span>  

3.  <span data-ttu-id="5e27c-235">Create new sales order:</span><span class="sxs-lookup"><span data-stu-id="5e27c-235">Create new sales order:</span></span>  

     <span data-ttu-id="5e27c-236">Sell-to Customer No.: 10000</span><span class="sxs-lookup"><span data-stu-id="5e27c-236">Sell-to Customer No.: 10000</span></span>  

     <span data-ttu-id="5e27c-237">Posting Date = December 16th, 2013</span><span class="sxs-lookup"><span data-stu-id="5e27c-237">Posting Date = December 16th, 2013</span></span>  

     <span data-ttu-id="5e27c-238">On the sales order line:</span><span class="sxs-lookup"><span data-stu-id="5e27c-238">On the sales order line:</span></span>  

     <span data-ttu-id="5e27c-239">Item = CHARGE</span><span class="sxs-lookup"><span data-stu-id="5e27c-239">Item = CHARGE</span></span>  

     <span data-ttu-id="5e27c-240">Quantity = 1</span><span class="sxs-lookup"><span data-stu-id="5e27c-240">Quantity = 1</span></span>  

     <span data-ttu-id="5e27c-241">Unit Price = 135</span><span class="sxs-lookup"><span data-stu-id="5e27c-241">Unit Price = 135</span></span>  

     <span data-ttu-id="5e27c-242">Post Ship and Invoice.</span><span class="sxs-lookup"><span data-stu-id="5e27c-242">Post Ship and Invoice.</span></span>  

4.  <span data-ttu-id="5e27c-243">General Ledger Setup:</span><span class="sxs-lookup"><span data-stu-id="5e27c-243">General Ledger Setup:</span></span>  

     <span data-ttu-id="5e27c-244">Allow Posting From = January 1st, 2014</span><span class="sxs-lookup"><span data-stu-id="5e27c-244">Allow Posting From = January 1st, 2014</span></span>  

     <span data-ttu-id="5e27c-245">Allow Posting To = blank</span><span class="sxs-lookup"><span data-stu-id="5e27c-245">Allow Posting To = blank</span></span>  

5.  <span data-ttu-id="5e27c-246">Create new purchase order:</span><span class="sxs-lookup"><span data-stu-id="5e27c-246">Create new purchase order:</span></span>  

     <span data-ttu-id="5e27c-247">Buy-from Vendor No.: 10000</span><span class="sxs-lookup"><span data-stu-id="5e27c-247">Buy-from Vendor No.: 10000</span></span>  

     <span data-ttu-id="5e27c-248">Posting Date = January 2nd, 2014</span><span class="sxs-lookup"><span data-stu-id="5e27c-248">Posting Date = January 2nd, 2014</span></span>  

     <span data-ttu-id="5e27c-249">Vendor Invoice No.: 2345</span><span class="sxs-lookup"><span data-stu-id="5e27c-249">Vendor Invoice No.: 2345</span></span>  

     <span data-ttu-id="5e27c-250">On the purchase order line:</span><span class="sxs-lookup"><span data-stu-id="5e27c-250">On the purchase order line:</span></span>  

     <span data-ttu-id="5e27c-251">Item Charge = JB-FREIGHT</span><span class="sxs-lookup"><span data-stu-id="5e27c-251">Item Charge = JB-FREIGHT</span></span>  

     <span data-ttu-id="5e27c-252">Quantity = 1</span><span class="sxs-lookup"><span data-stu-id="5e27c-252">Quantity = 1</span></span>  

     <span data-ttu-id="5e27c-253">Direct Unit Cost = 3</span><span class="sxs-lookup"><span data-stu-id="5e27c-253">Direct Unit Cost = 3</span></span>  

     <span data-ttu-id="5e27c-254">Assign Item Charge to Purchase Receipt from step 2.</span><span class="sxs-lookup"><span data-stu-id="5e27c-254">Assign Item Charge to Purchase Receipt from step 2.</span></span>  

     <span data-ttu-id="5e27c-255">Post Receipt and Invoice.</span><span class="sxs-lookup"><span data-stu-id="5e27c-255">Post Receipt and Invoice.</span></span>  

     <span data-ttu-id="5e27c-256">![Adjust cost &#45;Item entries data](media/helene/TechArticleAdjustcost11.png "TechArticleAdjustcost11")</span><span class="sxs-lookup"><span data-stu-id="5e27c-256">![Adjust cost &#45;Item entries data](media/helene/TechArticleAdjustcost11.png "TechArticleAdjustcost11")</span></span>

6.  <span data-ttu-id="5e27c-257">On work date January 3rd a purchase invoice arrives, containing an additional item charge to the purchase made in step 2.</span><span class="sxs-lookup"><span data-stu-id="5e27c-257">On work date January 3rd a purchase invoice arrives, containing an additional item charge to the purchase made in step 2.</span></span> <span data-ttu-id="5e27c-258">This invoice has document date December 30th and is therefore posted with Posting Date December 30th, 2013.</span><span class="sxs-lookup"><span data-stu-id="5e27c-258">This invoice has document date December 30th and is therefore posted with Posting Date December 30th, 2013.</span></span>  

     <span data-ttu-id="5e27c-259">Create new purchase order:</span><span class="sxs-lookup"><span data-stu-id="5e27c-259">Create new purchase order:</span></span>  

     <span data-ttu-id="5e27c-260">Buy-from Vendor No.: 10000</span><span class="sxs-lookup"><span data-stu-id="5e27c-260">Buy-from Vendor No.: 10000</span></span>  

     <span data-ttu-id="5e27c-261">Posting Date = December 30th, 2013</span><span class="sxs-lookup"><span data-stu-id="5e27c-261">Posting Date = December 30th, 2013</span></span>  

     <span data-ttu-id="5e27c-262">Vendor Invoice No.: 3456</span><span class="sxs-lookup"><span data-stu-id="5e27c-262">Vendor Invoice No.: 3456</span></span>  

     <span data-ttu-id="5e27c-263">On the purchase order line:</span><span class="sxs-lookup"><span data-stu-id="5e27c-263">On the purchase order line:</span></span>  

     <span data-ttu-id="5e27c-264">Item Charge = JB-FREIGHT</span><span class="sxs-lookup"><span data-stu-id="5e27c-264">Item Charge = JB-FREIGHT</span></span>  

     <span data-ttu-id="5e27c-265">Quantity = 1</span><span class="sxs-lookup"><span data-stu-id="5e27c-265">Quantity = 1</span></span>  

     <span data-ttu-id="5e27c-266">Direct Unit Cost = 2</span><span class="sxs-lookup"><span data-stu-id="5e27c-266">Direct Unit Cost = 2</span></span>  

     <span data-ttu-id="5e27c-267">Assign Item Charge to Purchase Receipt from step 2</span><span class="sxs-lookup"><span data-stu-id="5e27c-267">Assign Item Charge to Purchase Receipt from step 2</span></span>  

     <span data-ttu-id="5e27c-268">Post Receipt and Invoice.</span><span class="sxs-lookup"><span data-stu-id="5e27c-268">Post Receipt and Invoice.</span></span>  

   <span data-ttu-id="5e27c-269">![Adjust cost &#45;Item entries data](media/helene/TechArticleAdjustcost12.png "TechArticleAdjustcost12")</span><span class="sxs-lookup"><span data-stu-id="5e27c-269">![Adjust cost &#45;Item entries data](media/helene/TechArticleAdjustcost12.png "TechArticleAdjustcost12")</span></span>

 <span data-ttu-id="5e27c-270">Inventory Valuation report is printed as of Date December 31st , 2013</span><span class="sxs-lookup"><span data-stu-id="5e27c-270">Inventory Valuation report is printed as of Date December 31st , 2013</span></span>  

<span data-ttu-id="5e27c-271">![Adjust cost &#45;Item entries data](media/helene/TechArticleAdjustcost13.png "TechArticleAdjustcost13")</span><span class="sxs-lookup"><span data-stu-id="5e27c-271">![Adjust cost &#45;Item entries data](media/helene/TechArticleAdjustcost13.png "TechArticleAdjustcost13")</span></span>

 <span data-ttu-id="5e27c-272">**Summary of scenario:**</span><span class="sxs-lookup"><span data-stu-id="5e27c-272">**Summary of scenario:**</span></span>  

 <span data-ttu-id="5e27c-273">The described scenario ends up with an Inventory Valuation report demonstrating Quantity = 0 while the Value = 2.</span><span class="sxs-lookup"><span data-stu-id="5e27c-273">The described scenario ends up with an Inventory Valuation report demonstrating Quantity = 0 while the Value = 2.</span></span> <span data-ttu-id="5e27c-274">The Item charge posted in step 11 is part of the Inventory Increase value of December while the Inventory Decrease of the same period is not affected.</span><span class="sxs-lookup"><span data-stu-id="5e27c-274">The Item charge posted in step 11 is part of the Inventory Increase value of December while the Inventory Decrease of the same period is not affected.</span></span>  

 <span data-ttu-id="5e27c-275">Having the General Ledger Setup stating Allow Posting From January 1st was a good thing for the first Item charge.</span><span class="sxs-lookup"><span data-stu-id="5e27c-275">Having the General Ledger Setup stating Allow Posting From January 1st was a good thing for the first Item charge.</span></span> <span data-ttu-id="5e27c-276">The costs of the Inventory Increase and Decrease was recorded in the same period.</span><span class="sxs-lookup"><span data-stu-id="5e27c-276">The costs of the Inventory Increase and Decrease was recorded in the same period.</span></span> <span data-ttu-id="5e27c-277">For the second Item charge however, the General Ledger Setup causes the change in COGS to be recognised in the period after.</span><span class="sxs-lookup"><span data-stu-id="5e27c-277">For the second Item charge however, the General Ledger Setup causes the change in COGS to be recognized in the period after.</span></span>  

 <span data-ttu-id="5e27c-278">**Conclusion:**</span><span class="sxs-lookup"><span data-stu-id="5e27c-278">**Conclusion:**</span></span>  

 <span data-ttu-id="5e27c-279">It’s a challenge to have the Inventory Valuation report to demonstrate Quantity = 0 while the Value <> 0.</span><span class="sxs-lookup"><span data-stu-id="5e27c-279">It’s a challenge to have the Inventory Valuation report to demonstrate Quantity = 0 while the Value <> 0.</span></span> <span data-ttu-id="5e27c-280">In this case it’s also more difficult to express the optimal settings, having purchase invoices arriving the same day but addressing different periods or even fiscal years.</span><span class="sxs-lookup"><span data-stu-id="5e27c-280">In this case it’s also more difficult to express the optimal settings, having purchase invoices arriving the same day but addressing different periods or even fiscal years.</span></span> <span data-ttu-id="5e27c-281">Crossing to a new fiscal year usually requires some planning and as part of that the insight of Adjust Cost – Item entries process, recognising COGS, is to be considered.</span><span class="sxs-lookup"><span data-stu-id="5e27c-281">Crossing to a new fiscal year usually requires some planning and as part of that the insight of Adjust Cost – Item entries process, recognizing COGS, is to be considered.</span></span>  

 <span data-ttu-id="5e27c-282">In this scenario one option could have been to have the General Ledger Setup, field Allow Posting From, stating a date in December for a couple of more days and the posting of the first item charge postponed to allow all costs for the previous period/fiscal year to be recognised for the period they belong to first, having the Adjust Cost – Item entries batch job run and thereafter move the allowed posting date to the new period\/fiscal year.</span><span class="sxs-lookup"><span data-stu-id="5e27c-282">In this scenario one option could have been to have the General Ledger Setup, field Allow Posting From, stating a date in December for a couple of more days and the posting of the first item charge postponed to allow all costs for the previous period/fiscal year to be recognized for the period they belong to first, having the Adjust Cost – Item entries batch job run and thereafter move the allowed posting date to the new period\/fiscal year.</span></span> <span data-ttu-id="5e27c-283">The first item charge with posting date January 2nd could then be posted.</span><span class="sxs-lookup"><span data-stu-id="5e27c-283">The first item charge with posting date January 2nd could then be posted.</span></span>  

## <a name="history-of-adjust-cost--item-entries-batch-job"></a><span data-ttu-id="5e27c-284">History of Adjust Cost – Item entries batch job</span><span class="sxs-lookup"><span data-stu-id="5e27c-284">History of Adjust Cost – Item entries batch job</span></span>  
 <span data-ttu-id="5e27c-285">Below is a summary of the concept assigning Posting Dates to Adjustment Value Entries by the Adjust Cost – Item entries batch job since version 3.0.</span><span class="sxs-lookup"><span data-stu-id="5e27c-285">Below is a summary of the concept assigning Posting Dates to Adjustment Value Entries by the Adjust Cost – Item entries batch job since version 3.0.</span></span>  

### <a name="from-version-30370a"></a><span data-ttu-id="5e27c-286">From version 3.0..3.70.A</span><span class="sxs-lookup"><span data-stu-id="5e27c-286">From version 3.0..3.70.A</span></span>  
 <span data-ttu-id="5e27c-287">In the request form of the Adjust Cost - Item Entries batch job there is a Posting Date to be entered by the user.</span><span class="sxs-lookup"><span data-stu-id="5e27c-287">In the request form of the Adjust Cost - Item Entries batch job there is a Posting Date to be entered by the user.</span></span> <span data-ttu-id="5e27c-288">The batch job runs through all necessary changes and creates value entries with the posting date entered in the request form.</span><span class="sxs-lookup"><span data-stu-id="5e27c-288">The batch job runs through all necessary changes and creates value entries with the posting date entered in the request form.</span></span> <span data-ttu-id="5e27c-289">Suggested posting date to use is today’s date.</span><span class="sxs-lookup"><span data-stu-id="5e27c-289">Suggested posting date to use is today’s date.</span></span>  

### <a name="version-370b40"></a><span data-ttu-id="5e27c-290">Version 3.70.B..4.0</span><span class="sxs-lookup"><span data-stu-id="5e27c-290">Version 3.70.B..4.0</span></span>  
 <span data-ttu-id="5e27c-291">In the request form of the Adjust Cost - Item Entries batch job there is a Closed Period Entry Posting Date to be entered by the user.</span><span class="sxs-lookup"><span data-stu-id="5e27c-291">In the request form of the Adjust Cost - Item Entries batch job there is a Closed Period Entry Posting Date to be entered by the user.</span></span> <span data-ttu-id="5e27c-292">The batch job runs through all necessary changes and creates value entries with the posting date of the parent item ledger entry (shipment date of the sale that the adjustment address).</span><span class="sxs-lookup"><span data-stu-id="5e27c-292">The batch job runs through all necessary changes and creates value entries with the posting date of the parent item ledger entry (shipment date of the sale that the adjustment address).</span></span> <span data-ttu-id="5e27c-293">If the posting date of the parent item ledger entry is not within allowed posting date range the posting date stated as Closed Period Entry Posting Date will be assigned the Adjustment Value Entry.</span><span class="sxs-lookup"><span data-stu-id="5e27c-293">If the posting date of the parent item ledger entry is not within allowed posting date range the posting date stated as Closed Period Entry Posting Date will be assigned the Adjustment Value Entry.</span></span> <span data-ttu-id="5e27c-294">A date is considered to be in a closed period when it is earlier than the date in the Allow Posting From field in the General Ledger Setup.</span><span class="sxs-lookup"><span data-stu-id="5e27c-294">A date is considered to be in a closed period when it is earlier than the date in the Allow Posting From field in the General Ledger Setup.</span></span>  

### <a name="from-version-50"></a><span data-ttu-id="5e27c-295">From version 5.0:</span><span class="sxs-lookup"><span data-stu-id="5e27c-295">From version 5.0:</span></span>  
 <span data-ttu-id="5e27c-296">There is no longer a posting date to be stated in the request form of the Adjust Cost - Item entries batch job.</span><span class="sxs-lookup"><span data-stu-id="5e27c-296">There is no longer a posting date to be stated in the request form of the Adjust Cost - Item entries batch job.</span></span> <span data-ttu-id="5e27c-297">The batch job runs through all necessary changes and creates value entries with the posting date of the value entry it adjusts.</span><span class="sxs-lookup"><span data-stu-id="5e27c-297">The batch job runs through all necessary changes and creates value entries with the posting date of the value entry it adjusts.</span></span> <span data-ttu-id="5e27c-298">If the posting date is not within allowed posting date range the posting date in the Allow Posting From field in the General Ledger Setup, OR if the Inventory periods are used, the later date of the two will be used.</span><span class="sxs-lookup"><span data-stu-id="5e27c-298">If the posting date is not within allowed posting date range the posting date in the Allow Posting From field in the General Ledger Setup, OR if the Inventory periods are used, the later date of the two will be used.</span></span> <span data-ttu-id="5e27c-299">See described concept above.</span><span class="sxs-lookup"><span data-stu-id="5e27c-299">See described concept above.</span></span>  

## <a name="history-of-post-inventory-cost-to-gl-batch-job"></a><span data-ttu-id="5e27c-300">History of Post Inventory cost to G/L batch job</span><span class="sxs-lookup"><span data-stu-id="5e27c-300">History of Post Inventory cost to G/L batch job</span></span>  
 <span data-ttu-id="5e27c-301">The Post Inventory Cost to G/L batch job is closely related to the Adjust Cost – Item entries batch job why the history of this batch job is summarised and shared here as well.</span><span class="sxs-lookup"><span data-stu-id="5e27c-301">The Post Inventory Cost to G/L batch job is closely related to the Adjust Cost – Item entries batch job why the history of this batch job is summarized and shared here as well.</span></span>  

### <a name="from-version-30370a"></a><span data-ttu-id="5e27c-302">From version 3.0..3.70.A</span><span class="sxs-lookup"><span data-stu-id="5e27c-302">From version 3.0..3.70.A</span></span>  
 <span data-ttu-id="5e27c-303">In the request form of the Post Inventory Cost to G/L there is a Posting Date to be entered by the user.</span><span class="sxs-lookup"><span data-stu-id="5e27c-303">In the request form of the Post Inventory Cost to G/L there is a Posting Date to be entered by the user.</span></span> <span data-ttu-id="5e27c-304">The batch job runs through all value entries within the filter, if any, and creates General Ledger Entries with Posting Date entered in the request form.</span><span class="sxs-lookup"><span data-stu-id="5e27c-304">The batch job runs through all value entries within the filter, if any, and creates General Ledger Entries with Posting Date entered in the request form.</span></span>  

### <a name="version-370b40"></a><span data-ttu-id="5e27c-305">Version 3.70.B..4.0</span><span class="sxs-lookup"><span data-stu-id="5e27c-305">Version 3.70.B..4.0</span></span>  
 <span data-ttu-id="5e27c-306">In the request form of the Post Inventory Cost to G/L the Closed Period Entry Posting Date field is available.</span><span class="sxs-lookup"><span data-stu-id="5e27c-306">In the request form of the Post Inventory Cost to G/L the Closed Period Entry Posting Date field is available.</span></span> <span data-ttu-id="5e27c-307">The program uses the date you enter in this field as the posting date for the general ledger entries it creates for value entries whose posting dates are in closed accounting periods.</span><span class="sxs-lookup"><span data-stu-id="5e27c-307">The program uses the date you enter in this field as the posting date for the general ledger entries it creates for value entries whose posting dates are in closed accounting periods.</span></span> <span data-ttu-id="5e27c-308">Otherwise, the general ledger entries will have the same posting date as the original value entries.</span><span class="sxs-lookup"><span data-stu-id="5e27c-308">Otherwise, the general ledger entries will have the same posting date as the original value entries.</span></span> <span data-ttu-id="5e27c-309">A date is considered to be in a closed period when it is earlier than the date in the Allow Posting From field in the General Ledger Setup.</span><span class="sxs-lookup"><span data-stu-id="5e27c-309">A date is considered to be in a closed period when it is earlier than the date in the Allow Posting From field in the General Ledger Setup.</span></span> <span data-ttu-id="5e27c-310">If posting to G\/L Per Posting Group, the general ledger entries will have the posting date that is specified in the Posting Date field in the request form.</span><span class="sxs-lookup"><span data-stu-id="5e27c-310">If posting to G\/L Per Posting Group, the general ledger entries will have the posting date that is specified in the Posting Date field in the request form.</span></span>  

 <span data-ttu-id="5e27c-311">In version 3 and 4 the batch job scans all value entries to detect if there are any value entries where Cost Amount (Actual) differs from Cost Posted to G/L.</span><span class="sxs-lookup"><span data-stu-id="5e27c-311">In version 3 and 4 the batch job scans all value entries to detect if there are any value entries where Cost Amount (Actual) differs from Cost Posted to G/L.</span></span> <span data-ttu-id="5e27c-312">If there is a difference detected the differing amount will be posted in a G/L entry.</span><span class="sxs-lookup"><span data-stu-id="5e27c-312">If there is a difference detected the differing amount will be posted in a G/L entry.</span></span> <span data-ttu-id="5e27c-313">If expected cost posting is used corresponding fields are processed in the same way.</span><span class="sxs-lookup"><span data-stu-id="5e27c-313">If expected cost posting is used corresponding fields are processed in the same way.</span></span>  

<span data-ttu-id="5e27c-314">![Adjust cost &#45;Item entries data](media/helene/TechArticleAdjustcost14.png "TechArticleAdjustcost14")</span><span class="sxs-lookup"><span data-stu-id="5e27c-314">![Adjust cost &#45;Item entries data](media/helene/TechArticleAdjustcost14.png "TechArticleAdjustcost14")</span></span>

### <a name="from-version-50"></a><span data-ttu-id="5e27c-315">From version 5.0:</span><span class="sxs-lookup"><span data-stu-id="5e27c-315">From version 5.0:</span></span>  
 <span data-ttu-id="5e27c-316">There is no longer a posting date to be stated in the request form of the Post Inventory Cost to G/L batch job.</span><span class="sxs-lookup"><span data-stu-id="5e27c-316">There is no longer a posting date to be stated in the request form of the Post Inventory Cost to G/L batch job.</span></span> <span data-ttu-id="5e27c-317">The G/L entry is created with the same Posting Date as the related value entry.</span><span class="sxs-lookup"><span data-stu-id="5e27c-317">The G/L entry is created with the same Posting Date as the related value entry.</span></span> <span data-ttu-id="5e27c-318">In order to complete the batch job the allowed posting date range must allow the Posting Date of the created G/L entry.</span><span class="sxs-lookup"><span data-stu-id="5e27c-318">In order to complete the batch job the allowed posting date range must allow the Posting Date of the created G/L entry.</span></span> <span data-ttu-id="5e27c-319">If not, the allowed posting date range must be temporarily re-opened by changing or removing the dates in the Allow Posting From and To fields in the General Ledger Setup.</span><span class="sxs-lookup"><span data-stu-id="5e27c-319">If not, the allowed posting date range must be temporarily re-opened by changing or removing the dates in the Allow Posting From and To fields in the General Ledger Setup.</span></span> <span data-ttu-id="5e27c-320">To avoid reconciliation issues it is required that Posting Date of the G/L Entry corresponds to the Posting Date of the Value Entry.</span><span class="sxs-lookup"><span data-stu-id="5e27c-320">To avoid reconciliation issues it is required that Posting Date of the G/L Entry corresponds to the Posting Date of the Value Entry.</span></span>  

 <span data-ttu-id="5e27c-321">The batch job scans Table 5811 - Post Value Entry to G/L, to identify the Value Entries in scope for posting to General Ledger.</span><span class="sxs-lookup"><span data-stu-id="5e27c-321">The batch job scans Table 5811 - Post Value Entry to G/L, to identify the Value Entries in scope for posting to General Ledger.</span></span> <span data-ttu-id="5e27c-322">After successful run the table is emptied.</span><span class="sxs-lookup"><span data-stu-id="5e27c-322">After successful run the table is emptied.</span></span>  

 <span data-ttu-id="5e27c-323">Any feedback to how this process and documentation can be further developed is very welcome.</span><span class="sxs-lookup"><span data-stu-id="5e27c-323">Any feedback to how this process and documentation can be further developed is very welcome.</span></span>  

 <span data-ttu-id="5e27c-324">Helene Holmin</span><span class="sxs-lookup"><span data-stu-id="5e27c-324">Helene Holmin</span></span>  

 <span data-ttu-id="5e27c-325">Dynamics NAV Escalation Engineer</span><span class="sxs-lookup"><span data-stu-id="5e27c-325">Dynamics NAV Escalation Engineer</span></span>  

## <a name="see-also"></a><span data-ttu-id="5e27c-326">See Also</span><span class="sxs-lookup"><span data-stu-id="5e27c-326">See Also</span></span>  
[<span data-ttu-id="5e27c-327">Design Details: Inventory Costing</span><span class="sxs-lookup"><span data-stu-id="5e27c-327">Design Details: Inventory Costing</span></span>](design-details-inventory-costing.md)  
[<span data-ttu-id="5e27c-328">Design Details: Item Application</span><span class="sxs-lookup"><span data-stu-id="5e27c-328">Design Details: Item Application</span></span>](design-details-item-application.md)  

