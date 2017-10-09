---
title: Design Details - Staying Under the Overflow Level | Microsoft Docs
description: When using Maximum Qty. and Fixed Reorder Qty., the planning system focuses on the projected inventory in the given time-bucket only. This means that the planning system may suggest superfluous supply when negative demand or positive supply changes occur outside of the given time bucket.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/06/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: bbfafc41f22a5582b90683bdacf8135e78e46843
ms.contentlocale: en-nz
ms.lasthandoff: 09/22/2017

---
# <a name="design-details-staying-under-the-overflow-level"></a><span data-ttu-id="2a71a-104">Design Details: Staying under the Overflow Level</span><span class="sxs-lookup"><span data-stu-id="2a71a-104">Design Details: Staying under the Overflow Level</span></span>
<span data-ttu-id="2a71a-105">When using the Maximum Qty. and Fixed Reorder Qty. policies, the planning system focuses on the projected inventory in the given time-bucket only.</span><span class="sxs-lookup"><span data-stu-id="2a71a-105">When using the Maximum Qty. and Fixed Reorder Qty. policies, the planning system focuses on the projected inventory in the given time-bucket only.</span></span> <span data-ttu-id="2a71a-106">This means that the planning system may suggest superfluous supply when negative demand or positive supply changes occur outside of the given time bucket.</span><span class="sxs-lookup"><span data-stu-id="2a71a-106">This means that the planning system may suggest superfluous supply when negative demand or positive supply changes occur outside of the given time bucket.</span></span> <span data-ttu-id="2a71a-107">If, for this reason, a superfluous supply is suggested, the planning system calculates which quantity the supply should be decreased to (or deleted) to avoid the superfluous supply.</span><span class="sxs-lookup"><span data-stu-id="2a71a-107">If, for this reason, a superfluous supply is suggested, the planning system calculates which quantity the supply should be decreased to (or deleted) to avoid the superfluous supply.</span></span> <span data-ttu-id="2a71a-108">This quantity is called the “overflow level.”</span><span class="sxs-lookup"><span data-stu-id="2a71a-108">This quantity is called the “overflow level.”</span></span> <span data-ttu-id="2a71a-109">The overflow is communicated as a planning line with a **Change Qty. (Decrease)** or **Cancel** action and the following warning message:</span><span class="sxs-lookup"><span data-stu-id="2a71a-109">The overflow is communicated as a planning line with a **Change Qty. (Decrease)** or **Cancel** action and the following warning message:</span></span>  

<span data-ttu-id="2a71a-110">*Attention: The projected inventory [xx] is higher than the overflow level [xx] on the Due Date [xx].*</span><span class="sxs-lookup"><span data-stu-id="2a71a-110">*Attention: The projected inventory [xx] is higher than the overflow level [xx] on the Due Date [xx].*</span></span>  

<span data-ttu-id="2a71a-111">![Inventory overflow level](media/supplyplanning_2_overflow1_new.png "supplyplanning_2_overflow1_new")</span><span class="sxs-lookup"><span data-stu-id="2a71a-111">![Inventory overflow level](media/supplyplanning_2_overflow1_new.png "supplyplanning_2_overflow1_new")</span></span>  

##  <a name="calculating-the-overflow-level"></a><span data-ttu-id="2a71a-112">Calculating the Overflow Level</span><span class="sxs-lookup"><span data-stu-id="2a71a-112">Calculating the Overflow Level</span></span>  
<span data-ttu-id="2a71a-113">The overflow level is calculated in different ways depending on planning setup.</span><span class="sxs-lookup"><span data-stu-id="2a71a-113">The overflow level is calculated in different ways depending on planning setup.</span></span>  

### <a name="maximum-qty-reordering-policy"></a><span data-ttu-id="2a71a-114">Maximum Qty. reordering policy</span><span class="sxs-lookup"><span data-stu-id="2a71a-114">Maximum Qty. reordering policy</span></span>  
<span data-ttu-id="2a71a-115">Overflow level = Maximum Inventory</span><span class="sxs-lookup"><span data-stu-id="2a71a-115">Overflow level = Maximum Inventory</span></span>  

> [!NOTE]  
>  <span data-ttu-id="2a71a-116">If a minimum order quantity exists, then it will be added as follows: Overflow level = Maximum Inventory + Minimum Order Quantity.</span><span class="sxs-lookup"><span data-stu-id="2a71a-116">If a minimum order quantity exists, then it will be added as follows: Overflow level = Maximum Inventory + Minimum Order Quantity.</span></span>  

### <a name="fixed-reorder-qty-reordering-policy"></a><span data-ttu-id="2a71a-117">Fixed Reorder Qty. reordering policy</span><span class="sxs-lookup"><span data-stu-id="2a71a-117">Fixed Reorder Qty. reordering policy</span></span>  
<span data-ttu-id="2a71a-118">Overflow level = Reorder Quantity + Reorder Point</span><span class="sxs-lookup"><span data-stu-id="2a71a-118">Overflow level = Reorder Quantity + Reorder Point</span></span>  

> [!NOTE]  
>  <span data-ttu-id="2a71a-119">If the minimum order quantity is higher than the reorder point, then it will replace as follows: Overflow Level = Reorder Quantity + Minimum Order Quantity</span><span class="sxs-lookup"><span data-stu-id="2a71a-119">If the minimum order quantity is higher than the reorder point, then it will replace as follows: Overflow Level = Reorder Quantity + Minimum Order Quantity</span></span>  

### <a name="order-multiple"></a><span data-ttu-id="2a71a-120">Order Multiple</span><span class="sxs-lookup"><span data-stu-id="2a71a-120">Order Multiple</span></span>  
<span data-ttu-id="2a71a-121">If an order multiple exists, then it will adjust the overflow level for both Maximum Qty. and Fixed Reorder Qty. reordering policies.</span><span class="sxs-lookup"><span data-stu-id="2a71a-121">If an order multiple exists, then it will adjust the overflow level for both Maximum Qty. and Fixed Reorder Qty. reordering policies.</span></span>  

##  <a name="creating-the-planning-line-with-overflow-warning"></a><span data-ttu-id="2a71a-122">Creating the Planning Line with Overflow Warning</span><span class="sxs-lookup"><span data-stu-id="2a71a-122">Creating the Planning Line with Overflow Warning</span></span>  
<span data-ttu-id="2a71a-123">When an existing supply causes the projected inventory to be higher than the overflow level at the end of a time bucket, a planning line is created.</span><span class="sxs-lookup"><span data-stu-id="2a71a-123">When an existing supply causes the projected inventory to be higher than the overflow level at the end of a time bucket, a planning line is created.</span></span> <span data-ttu-id="2a71a-124">To warn about the potential superfluous supply, the planning line has a warning message, the **Accept Action Message** field is not selected, and the action message is either Cancel or Change Qty.</span><span class="sxs-lookup"><span data-stu-id="2a71a-124">To warn about the potential superfluous supply, the planning line has a warning message, the **Accept Action Message** field is not selected, and the action message is either Cancel or Change Qty.</span></span>  

### <a name="calculating-the-planning-line-quantity"></a><span data-ttu-id="2a71a-125">Calculating the Planning Line Quantity</span><span class="sxs-lookup"><span data-stu-id="2a71a-125">Calculating the Planning Line Quantity</span></span>  
<span data-ttu-id="2a71a-126">Planning Line Quantity = Current Supply Quantity – (Projected Inventory – Overflow Level)</span><span class="sxs-lookup"><span data-stu-id="2a71a-126">Planning Line Quantity = Current Supply Quantity – (Projected Inventory – Overflow Level)</span></span>  

> [!NOTE]  
>  <span data-ttu-id="2a71a-127">As with all warning lines, any maximum/minimum order quantity or order multiple will be ignored.</span><span class="sxs-lookup"><span data-stu-id="2a71a-127">As with all warning lines, any maximum/minimum order quantity or order multiple will be ignored.</span></span>  

### <a name="defining-the-action-message-type"></a><span data-ttu-id="2a71a-128">Defining the Action Message Type</span><span class="sxs-lookup"><span data-stu-id="2a71a-128">Defining the Action Message Type</span></span>  

-   <span data-ttu-id="2a71a-129">If the planning line quantity is higher than 0, then the action message is Change Qty.</span><span class="sxs-lookup"><span data-stu-id="2a71a-129">If the planning line quantity is higher than 0, then the action message is Change Qty.</span></span>  
-   <span data-ttu-id="2a71a-130">If the planning line quantity is equal to or lower than 0, then the action message is Cancel</span><span class="sxs-lookup"><span data-stu-id="2a71a-130">If the planning line quantity is equal to or lower than 0, then the action message is Cancel</span></span>  

### <a name="composing-the-warning-message"></a><span data-ttu-id="2a71a-131">Composing the Warning Message</span><span class="sxs-lookup"><span data-stu-id="2a71a-131">Composing the Warning Message</span></span>  
<span data-ttu-id="2a71a-132">In case of overflow, the **Untracked Planning Elements** window displays a warning message with the following information:</span><span class="sxs-lookup"><span data-stu-id="2a71a-132">In case of overflow, the **Untracked Planning Elements** window displays a warning message with the following information:</span></span>  

-   <span data-ttu-id="2a71a-133">The projected inventory level that triggered the warning</span><span class="sxs-lookup"><span data-stu-id="2a71a-133">The projected inventory level that triggered the warning</span></span>  
-   <span data-ttu-id="2a71a-134">The calculated overflow level</span><span class="sxs-lookup"><span data-stu-id="2a71a-134">The calculated overflow level</span></span>  
-   <span data-ttu-id="2a71a-135">The due date of the supply event.</span><span class="sxs-lookup"><span data-stu-id="2a71a-135">The due date of the supply event.</span></span>  

<span data-ttu-id="2a71a-136">Example: “The projected inventory 120 is higher than the overflow level 60 on 28-01-11”</span><span class="sxs-lookup"><span data-stu-id="2a71a-136">Example: “The projected inventory 120 is higher than the overflow level 60 on 28-01-11”</span></span>  

## <a name="scenario"></a><span data-ttu-id="2a71a-137">Scenario</span><span class="sxs-lookup"><span data-stu-id="2a71a-137">Scenario</span></span>  
<span data-ttu-id="2a71a-138">In this scenario, a customer changes a sales order from 70 to 40 pieces between two planning runs.</span><span class="sxs-lookup"><span data-stu-id="2a71a-138">In this scenario, a customer changes a sales order from 70 to 40 pieces between two planning runs.</span></span> <span data-ttu-id="2a71a-139">The overflow feature sets in to reduce the purchase that was suggested for the initial sales quantity.</span><span class="sxs-lookup"><span data-stu-id="2a71a-139">The overflow feature sets in to reduce the purchase that was suggested for the initial sales quantity.</span></span>  

### <a name="item-setup"></a><span data-ttu-id="2a71a-140">Item setup</span><span class="sxs-lookup"><span data-stu-id="2a71a-140">Item setup</span></span>  

|<span data-ttu-id="2a71a-141">Reordering Policy</span><span class="sxs-lookup"><span data-stu-id="2a71a-141">Reordering Policy</span></span>|<span data-ttu-id="2a71a-142">Maximum Qty.</span><span class="sxs-lookup"><span data-stu-id="2a71a-142">Maximum Qty.</span></span>|  
|-----------------------|------------------|  
|<span data-ttu-id="2a71a-143">Maximum Order Quantity</span><span class="sxs-lookup"><span data-stu-id="2a71a-143">Maximum Order Quantity</span></span>|<span data-ttu-id="2a71a-144">100</span><span class="sxs-lookup"><span data-stu-id="2a71a-144">100</span></span>|  
|<span data-ttu-id="2a71a-145">Reorder Point</span><span class="sxs-lookup"><span data-stu-id="2a71a-145">Reorder Point</span></span>|<span data-ttu-id="2a71a-146">50</span><span class="sxs-lookup"><span data-stu-id="2a71a-146">50</span></span>|  
|<span data-ttu-id="2a71a-147">Inventory</span><span class="sxs-lookup"><span data-stu-id="2a71a-147">Inventory</span></span>|<span data-ttu-id="2a71a-148">80</span><span class="sxs-lookup"><span data-stu-id="2a71a-148">80</span></span>|  

### <a name="situation-before-sales-decrease"></a><span data-ttu-id="2a71a-149">Situation before sales decrease</span><span class="sxs-lookup"><span data-stu-id="2a71a-149">Situation before sales decrease</span></span>  

|<span data-ttu-id="2a71a-150">Event</span><span class="sxs-lookup"><span data-stu-id="2a71a-150">Event</span></span>|<span data-ttu-id="2a71a-151">Change Qty.</span><span class="sxs-lookup"><span data-stu-id="2a71a-151">Change Qty.</span></span>|<span data-ttu-id="2a71a-152">Projected Inventory</span><span class="sxs-lookup"><span data-stu-id="2a71a-152">Projected Inventory</span></span>|  
|-----------|-----------------|-------------------------|  
|<span data-ttu-id="2a71a-153">Day one</span><span class="sxs-lookup"><span data-stu-id="2a71a-153">Day one</span></span>|<span data-ttu-id="2a71a-154">None</span><span class="sxs-lookup"><span data-stu-id="2a71a-154">None</span></span>|<span data-ttu-id="2a71a-155">80</span><span class="sxs-lookup"><span data-stu-id="2a71a-155">80</span></span>|  
|<span data-ttu-id="2a71a-156">Sale</span><span class="sxs-lookup"><span data-stu-id="2a71a-156">Sale</span></span>|<span data-ttu-id="2a71a-157">-70</span><span class="sxs-lookup"><span data-stu-id="2a71a-157">-70</span></span>|<span data-ttu-id="2a71a-158">10</span><span class="sxs-lookup"><span data-stu-id="2a71a-158">10</span></span>|  
|<span data-ttu-id="2a71a-159">End of time bucket</span><span class="sxs-lookup"><span data-stu-id="2a71a-159">End of time bucket</span></span>|<span data-ttu-id="2a71a-160">None</span><span class="sxs-lookup"><span data-stu-id="2a71a-160">None</span></span>|<span data-ttu-id="2a71a-161">10</span><span class="sxs-lookup"><span data-stu-id="2a71a-161">10</span></span>|  
|<span data-ttu-id="2a71a-162">Suggest new purchase order</span><span class="sxs-lookup"><span data-stu-id="2a71a-162">Suggest new purchase order</span></span>|<span data-ttu-id="2a71a-163">+90</span><span class="sxs-lookup"><span data-stu-id="2a71a-163">+90</span></span>|<span data-ttu-id="2a71a-164">100</span><span class="sxs-lookup"><span data-stu-id="2a71a-164">100</span></span>|  

### <a name="situation-after-sales-decrease"></a><span data-ttu-id="2a71a-165">Situation after sales decrease</span><span class="sxs-lookup"><span data-stu-id="2a71a-165">Situation after sales decrease</span></span>  

|<span data-ttu-id="2a71a-166">Change</span><span class="sxs-lookup"><span data-stu-id="2a71a-166">Change</span></span>|<span data-ttu-id="2a71a-167">Change Qty.</span><span class="sxs-lookup"><span data-stu-id="2a71a-167">Change Qty.</span></span>|<span data-ttu-id="2a71a-168">Projected Inventory</span><span class="sxs-lookup"><span data-stu-id="2a71a-168">Projected Inventory</span></span>|  
|------------|-----------------|-------------------------|  
|<span data-ttu-id="2a71a-169">Day one</span><span class="sxs-lookup"><span data-stu-id="2a71a-169">Day one</span></span>|<span data-ttu-id="2a71a-170">None</span><span class="sxs-lookup"><span data-stu-id="2a71a-170">None</span></span>|<span data-ttu-id="2a71a-171">80</span><span class="sxs-lookup"><span data-stu-id="2a71a-171">80</span></span>|  
|<span data-ttu-id="2a71a-172">Sale</span><span class="sxs-lookup"><span data-stu-id="2a71a-172">Sale</span></span>|<span data-ttu-id="2a71a-173">-40</span><span class="sxs-lookup"><span data-stu-id="2a71a-173">-40</span></span>|<span data-ttu-id="2a71a-174">40</span><span class="sxs-lookup"><span data-stu-id="2a71a-174">40</span></span>|  
|<span data-ttu-id="2a71a-175">Purchase</span><span class="sxs-lookup"><span data-stu-id="2a71a-175">Purchase</span></span>|<span data-ttu-id="2a71a-176">+90</span><span class="sxs-lookup"><span data-stu-id="2a71a-176">+90</span></span>|<span data-ttu-id="2a71a-177">130</span><span class="sxs-lookup"><span data-stu-id="2a71a-177">130</span></span>|  
|<span data-ttu-id="2a71a-178">End of time bucket</span><span class="sxs-lookup"><span data-stu-id="2a71a-178">End of time bucket</span></span>|<span data-ttu-id="2a71a-179">None</span><span class="sxs-lookup"><span data-stu-id="2a71a-179">None</span></span>|<span data-ttu-id="2a71a-180">130</span><span class="sxs-lookup"><span data-stu-id="2a71a-180">130</span></span>|  
|<span data-ttu-id="2a71a-181">Suggest to decrease purchase</span><span class="sxs-lookup"><span data-stu-id="2a71a-181">Suggest to decrease purchase</span></span><br /><br /> <span data-ttu-id="2a71a-182">order from 90 to 60</span><span class="sxs-lookup"><span data-stu-id="2a71a-182">order from 90 to 60</span></span>|<span data-ttu-id="2a71a-183">-30</span><span class="sxs-lookup"><span data-stu-id="2a71a-183">-30</span></span>|<span data-ttu-id="2a71a-184">100</span><span class="sxs-lookup"><span data-stu-id="2a71a-184">100</span></span>|  

### <a name="resulting-planning-lines"></a><span data-ttu-id="2a71a-185">Resulting Planning Lines</span><span class="sxs-lookup"><span data-stu-id="2a71a-185">Resulting Planning Lines</span></span>  
 <span data-ttu-id="2a71a-186">One planning line (warning) is created to reduce the purchase with 30 from 90 to 60 to keep the projected inventory on 100 according to the overflow level.</span><span class="sxs-lookup"><span data-stu-id="2a71a-186">One planning line (warning) is created to reduce the purchase with 30 from 90 to 60 to keep the projected inventory on 100 according to the overflow level.</span></span>  

<span data-ttu-id="2a71a-187">![Plan according to overflow level](media/nav_app_supply_planning_2_overflow2.png "nav_app_supply_planning_2_overflow2")</span><span class="sxs-lookup"><span data-stu-id="2a71a-187">![Plan according to overflow level](media/nav_app_supply_planning_2_overflow2.png "nav_app_supply_planning_2_overflow2")</span></span>  

> [!NOTE]  
>  <span data-ttu-id="2a71a-188">Without the Overflow feature, no warning is created if the projected inventory level is above maximum inventory.</span><span class="sxs-lookup"><span data-stu-id="2a71a-188">Without the Overflow feature, no warning is created if the projected inventory level is above maximum inventory.</span></span> <span data-ttu-id="2a71a-189">This could cause a superfluous supply of 30.</span><span class="sxs-lookup"><span data-stu-id="2a71a-189">This could cause a superfluous supply of 30.</span></span>  

## <a name="see-also"></a><span data-ttu-id="2a71a-190">See Also</span><span class="sxs-lookup"><span data-stu-id="2a71a-190">See Also</span></span>  
<span data-ttu-id="2a71a-191">[Design Details: Reordering Policies](design-details-reordering-policies.md) </span><span class="sxs-lookup"><span data-stu-id="2a71a-191">[Design Details: Reordering Policies](design-details-reordering-policies.md) </span></span>  
<span data-ttu-id="2a71a-192">[Design Details: Planning Parameters](design-details-planning-parameters.md) </span><span class="sxs-lookup"><span data-stu-id="2a71a-192">[Design Details: Planning Parameters](design-details-planning-parameters.md) </span></span>  
<span data-ttu-id="2a71a-193">[Design Details: Handling Reordering Policies](design-details-handling-reordering-policies.md) </span><span class="sxs-lookup"><span data-stu-id="2a71a-193">[Design Details: Handling Reordering Policies](design-details-handling-reordering-policies.md) </span></span>  
[<span data-ttu-id="2a71a-194">Design Details: Supply Planning</span><span class="sxs-lookup"><span data-stu-id="2a71a-194">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)

