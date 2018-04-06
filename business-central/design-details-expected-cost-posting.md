---
title: Design Details - Expected Cost Posting | Microsoft Docs
description: "Expected costs represent the estimation of, for example, a purchased item’s cost that you record before you receive the invoice for the item."
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
ms.openlocfilehash: 50ac9cbb946fedc687eb5ea1373c99d68f3d322b
ms.contentlocale: en-nz
ms.lasthandoff: 03/22/2018

---
# <a name="design-details-expected-cost-posting"></a><span data-ttu-id="9160e-103">Design Details: Expected Cost Posting</span><span class="sxs-lookup"><span data-stu-id="9160e-103">Design Details: Expected Cost Posting</span></span>
<span data-ttu-id="9160e-104">Expected costs represent the estimation of, for example, a purchased item’s cost that you record before you receive the invoice for the item.</span><span class="sxs-lookup"><span data-stu-id="9160e-104">Expected costs represent the estimation of, for example, a purchased item’s cost that you record before you receive the invoice for the item.</span></span>  

 <span data-ttu-id="9160e-105">You can post expected cost to inventory and to the general ledger.</span><span class="sxs-lookup"><span data-stu-id="9160e-105">You can post expected cost to inventory and to the general ledger.</span></span> <span data-ttu-id="9160e-106">When you post a quantity that is only received or shipped but not invoiced, then a value entry is created with the expected cost.</span><span class="sxs-lookup"><span data-stu-id="9160e-106">When you post a quantity that is only received or shipped but not invoiced, then a value entry is created with the expected cost.</span></span> <span data-ttu-id="9160e-107">This expected cost affects the inventory value, but is not posted to the general ledger unless you set up the system up to do so.</span><span class="sxs-lookup"><span data-stu-id="9160e-107">This expected cost affects the inventory value, but is not posted to the general ledger unless you set up the system up to do so.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="9160e-108">Expected costs are only managed for item transactions.</span><span class="sxs-lookup"><span data-stu-id="9160e-108">Expected costs are only managed for item transactions.</span></span> <span data-ttu-id="9160e-109">Expected costs are not for immaterial transaction types, such as capacity and item charges.</span><span class="sxs-lookup"><span data-stu-id="9160e-109">Expected costs are not for immaterial transaction types, such as capacity and item charges.</span></span>  

 <span data-ttu-id="9160e-110">If only the quantity part of an inventory increase has been posted, then the inventory value in the general ledger does not change unless you have selected the **Expected Cost Posting to G/L** check box in the **Inventory Setup** window.</span><span class="sxs-lookup"><span data-stu-id="9160e-110">If only the quantity part of an inventory increase has been posted, then the inventory value in the general ledger does not change unless you have selected the **Expected Cost Posting to G/L** check box in the **Inventory Setup** window.</span></span> <span data-ttu-id="9160e-111">In that case, the expected cost is posted to interim accounts at the time of receipt.</span><span class="sxs-lookup"><span data-stu-id="9160e-111">In that case, the expected cost is posted to interim accounts at the time of receipt.</span></span> <span data-ttu-id="9160e-112">After the receipt has been fully invoiced, the interim accounts are then balanced and the actual cost is posted to the inventory account.</span><span class="sxs-lookup"><span data-stu-id="9160e-112">After the receipt has been fully invoiced, the interim accounts are then balanced and the actual cost is posted to the inventory account.</span></span>  

 <span data-ttu-id="9160e-113">To support reconciliation and traceability work, the invoiced value entry shows the expected cost amount that has been posted to balance the interim accounts.</span><span class="sxs-lookup"><span data-stu-id="9160e-113">To support reconciliation and traceability work, the invoiced value entry shows the expected cost amount that has been posted to balance the interim accounts.</span></span>  

## <a name="example"></a><span data-ttu-id="9160e-114">Example</span><span class="sxs-lookup"><span data-stu-id="9160e-114">Example</span></span>  
 <span data-ttu-id="9160e-115">The following example shows expected cost if the **Automatic Cost Posting** check box and the **Expected Cost Posting to G/L** check box are selected in the **Inventory Setup** window.</span><span class="sxs-lookup"><span data-stu-id="9160e-115">The following example shows expected cost if the **Automatic Cost Posting** check box and the **Expected Cost Posting to G/L** check box are selected in the **Inventory Setup** window.</span></span>  

 <span data-ttu-id="9160e-116">You post a purchase order as received.</span><span class="sxs-lookup"><span data-stu-id="9160e-116">You post a purchase order as received.</span></span> <span data-ttu-id="9160e-117">The expected cost is LCY 95.00.</span><span class="sxs-lookup"><span data-stu-id="9160e-117">The expected cost is LCY 95.00.</span></span>  

 <span data-ttu-id="9160e-118">**Value Entries**</span><span class="sxs-lookup"><span data-stu-id="9160e-118">**Value Entries**</span></span>  

|<span data-ttu-id="9160e-119">Posting Date</span><span class="sxs-lookup"><span data-stu-id="9160e-119">Posting Date</span></span>|<span data-ttu-id="9160e-120">Entry Type</span><span class="sxs-lookup"><span data-stu-id="9160e-120">Entry Type</span></span>|<span data-ttu-id="9160e-121">Cost Amount (Expected)</span><span class="sxs-lookup"><span data-stu-id="9160e-121">Cost Amount (Expected)</span></span>|<span data-ttu-id="9160e-122">Expected Cost Posted to G/L</span><span class="sxs-lookup"><span data-stu-id="9160e-122">Expected Cost Posted to G/L</span></span>|<span data-ttu-id="9160e-123">Expected Cost</span><span class="sxs-lookup"><span data-stu-id="9160e-123">Expected Cost</span></span>|<span data-ttu-id="9160e-124">Item Ledger Entry No.</span><span class="sxs-lookup"><span data-stu-id="9160e-124">Item Ledger Entry No.</span></span>|<span data-ttu-id="9160e-125">Entry No.</span><span class="sxs-lookup"><span data-stu-id="9160e-125">Entry No.</span></span>|  
|------------------|----------------|------------------------------|----------------------------------|-------------------|---------------------------|---------------|  
|<span data-ttu-id="9160e-126">01-01-20</span><span class="sxs-lookup"><span data-stu-id="9160e-126">01-01-20</span></span>|<span data-ttu-id="9160e-127">Direct Cost</span><span class="sxs-lookup"><span data-stu-id="9160e-127">Direct Cost</span></span>|<span data-ttu-id="9160e-128">95.00</span><span class="sxs-lookup"><span data-stu-id="9160e-128">95.00</span></span>|<span data-ttu-id="9160e-129">95.00</span><span class="sxs-lookup"><span data-stu-id="9160e-129">95.00</span></span>|<span data-ttu-id="9160e-130">Yes</span><span class="sxs-lookup"><span data-stu-id="9160e-130">Yes</span></span>|<span data-ttu-id="9160e-131">1</span><span class="sxs-lookup"><span data-stu-id="9160e-131">1</span></span>|<span data-ttu-id="9160e-132">1</span><span class="sxs-lookup"><span data-stu-id="9160e-132">1</span></span>|  

 <span data-ttu-id="9160e-133">**Relation Entries in the G/L – Item Ledger Relation Table**</span><span class="sxs-lookup"><span data-stu-id="9160e-133">**Relation Entries in the G/L – Item Ledger Relation Table**</span></span>  

|<span data-ttu-id="9160e-134">G/L Entry No.</span><span class="sxs-lookup"><span data-stu-id="9160e-134">G/L Entry No.</span></span>|<span data-ttu-id="9160e-135">Value Entry No.</span><span class="sxs-lookup"><span data-stu-id="9160e-135">Value Entry No.</span></span>|<span data-ttu-id="9160e-136">G/L Register No.</span><span class="sxs-lookup"><span data-stu-id="9160e-136">G/L Register No.</span></span>|  
|--------------------|---------------------|-----------------------|  
|<span data-ttu-id="9160e-137">1</span><span class="sxs-lookup"><span data-stu-id="9160e-137">1</span></span>|<span data-ttu-id="9160e-138">1</span><span class="sxs-lookup"><span data-stu-id="9160e-138">1</span></span>|<span data-ttu-id="9160e-139">1</span><span class="sxs-lookup"><span data-stu-id="9160e-139">1</span></span>|  
|<span data-ttu-id="9160e-140">2</span><span class="sxs-lookup"><span data-stu-id="9160e-140">2</span></span>|<span data-ttu-id="9160e-141">1</span><span class="sxs-lookup"><span data-stu-id="9160e-141">1</span></span>|<span data-ttu-id="9160e-142">1</span><span class="sxs-lookup"><span data-stu-id="9160e-142">1</span></span>|  

 <span data-ttu-id="9160e-143">**General Ledger Entries**</span><span class="sxs-lookup"><span data-stu-id="9160e-143">**General Ledger Entries**</span></span>  

|<span data-ttu-id="9160e-144">Posting Date</span><span class="sxs-lookup"><span data-stu-id="9160e-144">Posting Date</span></span>|<span data-ttu-id="9160e-145">G/L Account</span><span class="sxs-lookup"><span data-stu-id="9160e-145">G/L Account</span></span>|<span data-ttu-id="9160e-146">Account No. (En-US Demo)</span><span class="sxs-lookup"><span data-stu-id="9160e-146">Account No. (En-US Demo)</span></span>|<span data-ttu-id="9160e-147">Amount</span><span class="sxs-lookup"><span data-stu-id="9160e-147">Amount</span></span>|<span data-ttu-id="9160e-148">Entry No.</span><span class="sxs-lookup"><span data-stu-id="9160e-148">Entry No.</span></span>|  
|------------------|------------------|---------------------------------|------------|---------------|  
|<span data-ttu-id="9160e-149">01-01-20</span><span class="sxs-lookup"><span data-stu-id="9160e-149">01-01-20</span></span>|<span data-ttu-id="9160e-150">Inventory Accrual Account (Interim)</span><span class="sxs-lookup"><span data-stu-id="9160e-150">Inventory Accrual Account (Interim)</span></span>|<span data-ttu-id="9160e-151">5530</span><span class="sxs-lookup"><span data-stu-id="9160e-151">5530</span></span>|<span data-ttu-id="9160e-152">-95.00</span><span class="sxs-lookup"><span data-stu-id="9160e-152">-95.00</span></span>|<span data-ttu-id="9160e-153">2</span><span class="sxs-lookup"><span data-stu-id="9160e-153">2</span></span>|  
|<span data-ttu-id="9160e-154">01-01-20</span><span class="sxs-lookup"><span data-stu-id="9160e-154">01-01-20</span></span>|<span data-ttu-id="9160e-155">Inventory Account (Interim)</span><span class="sxs-lookup"><span data-stu-id="9160e-155">Inventory Account (Interim)</span></span>|<span data-ttu-id="9160e-156">2131</span><span class="sxs-lookup"><span data-stu-id="9160e-156">2131</span></span>|<span data-ttu-id="9160e-157">95.00</span><span class="sxs-lookup"><span data-stu-id="9160e-157">95.00</span></span>|<span data-ttu-id="9160e-158">1</span><span class="sxs-lookup"><span data-stu-id="9160e-158">1</span></span>|  

 <span data-ttu-id="9160e-159">At a later date, you post the purchase order as invoiced.</span><span class="sxs-lookup"><span data-stu-id="9160e-159">At a later date, you post the purchase order as invoiced.</span></span> <span data-ttu-id="9160e-160">The invoiced cost is LCY 100.00.</span><span class="sxs-lookup"><span data-stu-id="9160e-160">The invoiced cost is LCY 100.00.</span></span>  

 <span data-ttu-id="9160e-161">**Value Entries**</span><span class="sxs-lookup"><span data-stu-id="9160e-161">**Value Entries**</span></span>  

|<span data-ttu-id="9160e-162">Posting Date</span><span class="sxs-lookup"><span data-stu-id="9160e-162">Posting Date</span></span>|<span data-ttu-id="9160e-163">Cost Amount (Actual)</span><span class="sxs-lookup"><span data-stu-id="9160e-163">Cost Amount (Actual)</span></span>|<span data-ttu-id="9160e-164">Cost Amount (Expected)</span><span class="sxs-lookup"><span data-stu-id="9160e-164">Cost Amount (Expected)</span></span>|<span data-ttu-id="9160e-165">Cost Posted to G/L</span><span class="sxs-lookup"><span data-stu-id="9160e-165">Cost Posted to G/L</span></span>|<span data-ttu-id="9160e-166">Expected Cost</span><span class="sxs-lookup"><span data-stu-id="9160e-166">Expected Cost</span></span>|<span data-ttu-id="9160e-167">Item Ledger Entry No.</span><span class="sxs-lookup"><span data-stu-id="9160e-167">Item Ledger Entry No.</span></span>|<span data-ttu-id="9160e-168">Entry No.</span><span class="sxs-lookup"><span data-stu-id="9160e-168">Entry No.</span></span>|  
|------------------|----------------------------|------------------------------|-------------------------|-------------------|---------------------------|---------------|  
|<span data-ttu-id="9160e-169">01-15-20</span><span class="sxs-lookup"><span data-stu-id="9160e-169">01-15-20</span></span>|<span data-ttu-id="9160e-170">100.00</span><span class="sxs-lookup"><span data-stu-id="9160e-170">100.00</span></span>|<span data-ttu-id="9160e-171">-95.00</span><span class="sxs-lookup"><span data-stu-id="9160e-171">-95.00</span></span>|<span data-ttu-id="9160e-172">100.00</span><span class="sxs-lookup"><span data-stu-id="9160e-172">100.00</span></span>|<span data-ttu-id="9160e-173">No</span><span class="sxs-lookup"><span data-stu-id="9160e-173">No</span></span>|<span data-ttu-id="9160e-174">1</span><span class="sxs-lookup"><span data-stu-id="9160e-174">1</span></span>|<span data-ttu-id="9160e-175">2</span><span class="sxs-lookup"><span data-stu-id="9160e-175">2</span></span>|  

 <span data-ttu-id="9160e-176">**Relation Entries in the G/L – Item Ledger Relation Table**</span><span class="sxs-lookup"><span data-stu-id="9160e-176">**Relation Entries in the G/L – Item Ledger Relation Table**</span></span>  

|<span data-ttu-id="9160e-177">G/L Entry No.</span><span class="sxs-lookup"><span data-stu-id="9160e-177">G/L Entry No.</span></span>|<span data-ttu-id="9160e-178">Value Entry No.</span><span class="sxs-lookup"><span data-stu-id="9160e-178">Value Entry No.</span></span>|<span data-ttu-id="9160e-179">G/L Register No.</span><span class="sxs-lookup"><span data-stu-id="9160e-179">G/L Register No.</span></span>|  
|--------------------|---------------------|-----------------------|  
|<span data-ttu-id="9160e-180">3</span><span class="sxs-lookup"><span data-stu-id="9160e-180">3</span></span>|<span data-ttu-id="9160e-181">2</span><span class="sxs-lookup"><span data-stu-id="9160e-181">2</span></span>|<span data-ttu-id="9160e-182">2</span><span class="sxs-lookup"><span data-stu-id="9160e-182">2</span></span>|  
|<span data-ttu-id="9160e-183">4</span><span class="sxs-lookup"><span data-stu-id="9160e-183">4</span></span>|<span data-ttu-id="9160e-184">2</span><span class="sxs-lookup"><span data-stu-id="9160e-184">2</span></span>|<span data-ttu-id="9160e-185">2</span><span class="sxs-lookup"><span data-stu-id="9160e-185">2</span></span>|  
|<span data-ttu-id="9160e-186">5</span><span class="sxs-lookup"><span data-stu-id="9160e-186">5</span></span>|<span data-ttu-id="9160e-187">2</span><span class="sxs-lookup"><span data-stu-id="9160e-187">2</span></span>|<span data-ttu-id="9160e-188">2</span><span class="sxs-lookup"><span data-stu-id="9160e-188">2</span></span>|  
|<span data-ttu-id="9160e-189">6</span><span class="sxs-lookup"><span data-stu-id="9160e-189">6</span></span>|<span data-ttu-id="9160e-190">2</span><span class="sxs-lookup"><span data-stu-id="9160e-190">2</span></span>|<span data-ttu-id="9160e-191">2</span><span class="sxs-lookup"><span data-stu-id="9160e-191">2</span></span>|  

 <span data-ttu-id="9160e-192">**General Ledger Entries**</span><span class="sxs-lookup"><span data-stu-id="9160e-192">**General Ledger Entries**</span></span>  

|<span data-ttu-id="9160e-193">Posting Date</span><span class="sxs-lookup"><span data-stu-id="9160e-193">Posting Date</span></span>|<span data-ttu-id="9160e-194">G/L Account</span><span class="sxs-lookup"><span data-stu-id="9160e-194">G/L Account</span></span>|<span data-ttu-id="9160e-195">Account No. (En-US Demo)</span><span class="sxs-lookup"><span data-stu-id="9160e-195">Account No. (En-US Demo)</span></span>|<span data-ttu-id="9160e-196">Amount</span><span class="sxs-lookup"><span data-stu-id="9160e-196">Amount</span></span>|<span data-ttu-id="9160e-197">Entry No.</span><span class="sxs-lookup"><span data-stu-id="9160e-197">Entry No.</span></span>|  
|------------------|------------------|---------------------------------|------------|---------------|  
|<span data-ttu-id="9160e-198">01-15-20</span><span class="sxs-lookup"><span data-stu-id="9160e-198">01-15-20</span></span>|<span data-ttu-id="9160e-199">Inventory Accrual Account (Interim)</span><span class="sxs-lookup"><span data-stu-id="9160e-199">Inventory Accrual Account (Interim)</span></span>|<span data-ttu-id="9160e-200">5530</span><span class="sxs-lookup"><span data-stu-id="9160e-200">5530</span></span>|<span data-ttu-id="9160e-201">95.00</span><span class="sxs-lookup"><span data-stu-id="9160e-201">95.00</span></span>|<span data-ttu-id="9160e-202">4</span><span class="sxs-lookup"><span data-stu-id="9160e-202">4</span></span>|  
|<span data-ttu-id="9160e-203">01-15-20</span><span class="sxs-lookup"><span data-stu-id="9160e-203">01-15-20</span></span>|<span data-ttu-id="9160e-204">Inventory Account (Interim)</span><span class="sxs-lookup"><span data-stu-id="9160e-204">Inventory Account (Interim)</span></span>|<span data-ttu-id="9160e-205">2131</span><span class="sxs-lookup"><span data-stu-id="9160e-205">2131</span></span>|<span data-ttu-id="9160e-206">-95.00</span><span class="sxs-lookup"><span data-stu-id="9160e-206">-95.00</span></span>|<span data-ttu-id="9160e-207">3</span><span class="sxs-lookup"><span data-stu-id="9160e-207">3</span></span>|  
|<span data-ttu-id="9160e-208">01-15-20</span><span class="sxs-lookup"><span data-stu-id="9160e-208">01-15-20</span></span>|<span data-ttu-id="9160e-209">Direct Cost Applied Account</span><span class="sxs-lookup"><span data-stu-id="9160e-209">Direct Cost Applied Account</span></span>|<span data-ttu-id="9160e-210">7291</span><span class="sxs-lookup"><span data-stu-id="9160e-210">7291</span></span>|<span data-ttu-id="9160e-211">-100</span><span class="sxs-lookup"><span data-stu-id="9160e-211">-100</span></span>|<span data-ttu-id="9160e-212">6</span><span class="sxs-lookup"><span data-stu-id="9160e-212">6</span></span>|  
|<span data-ttu-id="9160e-213">01-15-20</span><span class="sxs-lookup"><span data-stu-id="9160e-213">01-15-20</span></span>|<span data-ttu-id="9160e-214">Inventory Account</span><span class="sxs-lookup"><span data-stu-id="9160e-214">Inventory Account</span></span>|<span data-ttu-id="9160e-215">2130</span><span class="sxs-lookup"><span data-stu-id="9160e-215">2130</span></span>|<span data-ttu-id="9160e-216">100</span><span class="sxs-lookup"><span data-stu-id="9160e-216">100</span></span>|<span data-ttu-id="9160e-217">5</span><span class="sxs-lookup"><span data-stu-id="9160e-217">5</span></span>|  

## <a name="see-also"></a><span data-ttu-id="9160e-218">See Also</span><span class="sxs-lookup"><span data-stu-id="9160e-218">See Also</span></span>
 <span data-ttu-id="9160e-219">[Design Details: Inventory Costing](design-details-inventory-costing.md) </span><span class="sxs-lookup"><span data-stu-id="9160e-219">[Design Details: Inventory Costing](design-details-inventory-costing.md) </span></span>  
 <span data-ttu-id="9160e-220">[Design Details: Cost Adjustment](design-details-cost-adjustment.md) </span><span class="sxs-lookup"><span data-stu-id="9160e-220">[Design Details: Cost Adjustment](design-details-cost-adjustment.md) </span></span>  
 <span data-ttu-id="9160e-221">[Design Details: Reconciliation with the General Ledger](design-details-reconciliation-with-the-general-ledger.md) </span><span class="sxs-lookup"><span data-stu-id="9160e-221">[Design Details: Reconciliation with the General Ledger](design-details-reconciliation-with-the-general-ledger.md) </span></span>  
 <span data-ttu-id="9160e-222">[Design Details: Inventory Posting](design-details-inventory-posting.md) </span><span class="sxs-lookup"><span data-stu-id="9160e-222">[Design Details: Inventory Posting](design-details-inventory-posting.md) </span></span>  
 [<span data-ttu-id="9160e-223">Design Details: Variance</span><span class="sxs-lookup"><span data-stu-id="9160e-223">Design Details: Variance</span></span>](design-details-variance.md)  
 [<span data-ttu-id="9160e-224">Managing Inventory Costs</span><span class="sxs-lookup"><span data-stu-id="9160e-224">Managing Inventory Costs</span></span>](finance-manage-inventory-costs.md)  
 [<span data-ttu-id="9160e-225">Finance</span><span class="sxs-lookup"><span data-stu-id="9160e-225">Finance</span></span>](finance.md)  
 <span data-ttu-id="9160e-226">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="9160e-226">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
