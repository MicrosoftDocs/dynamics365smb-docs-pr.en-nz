---
title: About Planning Functionality | Microsoft Docs
description: The planning system takes all demand and supply data into account, nets the results, and creates suggestions for balancing the supply to meet the demand.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 35b67b7f77571b570245ebdb26c49458d3f83e39
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "5386890"
---
# <a name="about-planning-functionality"></a><span data-ttu-id="27f72-103">About Planning Functionality</span><span class="sxs-lookup"><span data-stu-id="27f72-103">About Planning Functionality</span></span>

<span data-ttu-id="27f72-104">The planning system takes all demand and supply data into account, nets the results, and creates suggestions for balancing the supply to meet the demand.</span><span class="sxs-lookup"><span data-stu-id="27f72-104">The planning system takes all demand and supply data into account, nets the results, and creates suggestions for balancing the supply to meet the demand.</span></span>  

<span data-ttu-id="27f72-105">For detailed information, see [Design Details: Supply Planning](design-details-supply-planning.md).</span><span class="sxs-lookup"><span data-stu-id="27f72-105">For detailed information, see [Design Details: Supply Planning](design-details-supply-planning.md).</span></span>  

> [!NOTE]  
> <span data-ttu-id="27f72-106">For all the fields that are mentioned in this topic, read the tooltip to understand their function.</span><span class="sxs-lookup"><span data-stu-id="27f72-106">For all the fields that are mentioned in this topic, read the tooltip to understand their function.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="demand-and-supply"></a><span data-ttu-id="27f72-107">Demand and Supply</span><span class="sxs-lookup"><span data-stu-id="27f72-107">Demand and Supply</span></span>

<span data-ttu-id="27f72-108">Planning has two elements: demand and supply.</span><span class="sxs-lookup"><span data-stu-id="27f72-108">Planning has two elements: demand and supply.</span></span> <span data-ttu-id="27f72-109">These must be held in balance to ensure that the demand is met in a timely and cost-efficient manner.</span><span class="sxs-lookup"><span data-stu-id="27f72-109">These must be held in balance to ensure that the demand is met in a timely and cost-efficient manner.</span></span>  

- <span data-ttu-id="27f72-110">Demand is the common term used for any kind of gross requirement such as a sales order, service order, component need from assembly or production orders, outbound transfer, blanket order or forecast.</span><span class="sxs-lookup"><span data-stu-id="27f72-110">Demand is the common term used for any kind of gross requirement such as a sales order, service order, component need from assembly or production orders, outbound transfer, blanket order or forecast.</span></span> <span data-ttu-id="27f72-111">In addition to these, application allows some other technical types of demand - such as a negative production or purchase order, negative inventory, and purchase return.</span><span class="sxs-lookup"><span data-stu-id="27f72-111">In addition to these, application allows some other technical types of demand - such as a negative production or purchase order, negative inventory, and purchase return.</span></span>  
- <span data-ttu-id="27f72-112">Supply is the common word used for any kind of replenishment such as inventory, a purchase order, assembly order, production order, or inbound transfer.</span><span class="sxs-lookup"><span data-stu-id="27f72-112">Supply is the common word used for any kind of replenishment such as inventory, a purchase order, assembly order, production order, or inbound transfer.</span></span> <span data-ttu-id="27f72-113">Correspondingly, there can be a negative sales or service order, negative component need or sales return – all of which in some way also represent supply.</span><span class="sxs-lookup"><span data-stu-id="27f72-113">Correspondingly, there can be a negative sales or service order, negative component need or sales return – all of which in some way also represent supply.</span></span>  

<span data-ttu-id="27f72-114">Another goal of the planning system is to ensure that the inventory does not grow unnecessarily.</span><span class="sxs-lookup"><span data-stu-id="27f72-114">Another goal of the planning system is to ensure that the inventory does not grow unnecessarily.</span></span> <span data-ttu-id="27f72-115">In the case of decreasing demand, the planning system will suggest that you postpone, decrease in quantity, or cancel existing replenishment orders.</span><span class="sxs-lookup"><span data-stu-id="27f72-115">In the case of decreasing demand, the planning system will suggest that you postpone, decrease in quantity, or cancel existing replenishment orders.</span></span>  

## <a name="planning-calculation"></a><span data-ttu-id="27f72-116">Planning Calculation</span><span class="sxs-lookup"><span data-stu-id="27f72-116">Planning Calculation</span></span>

<span data-ttu-id="27f72-117">The planning system is driven by anticipated and actual customer demand, as well as inventory reordering parameters.</span><span class="sxs-lookup"><span data-stu-id="27f72-117">The planning system is driven by anticipated and actual customer demand, as well as inventory reordering parameters.</span></span> <span data-ttu-id="27f72-118">Running the planning calculation will result in application suggesting specific actions (Action Messages) to take concerning possible replenishment from vendors, transfers between warehouses, or production.</span><span class="sxs-lookup"><span data-stu-id="27f72-118">Running the planning calculation will result in application suggesting specific actions (Action Messages) to take concerning possible replenishment from vendors, transfers between warehouses, or production.</span></span> <span data-ttu-id="27f72-119">If replenishment orders already exist, the suggested actions could be to increase or expedite the orders to meet the changes in demand.</span><span class="sxs-lookup"><span data-stu-id="27f72-119">If replenishment orders already exist, the suggested actions could be to increase or expedite the orders to meet the changes in demand.</span></span>  

<span data-ttu-id="27f72-120">The basis of the planning routine is in the gross-to-net calculation.</span><span class="sxs-lookup"><span data-stu-id="27f72-120">The basis of the planning routine is in the gross-to-net calculation.</span></span> <span data-ttu-id="27f72-121">Net requirements drive planned order releases, which are scheduled based on the routing information (manufactured items) or the item card lead time (purchased items).</span><span class="sxs-lookup"><span data-stu-id="27f72-121">Net requirements drive planned order releases, which are scheduled based on the routing information (manufactured items) or the item card lead time (purchased items).</span></span> <span data-ttu-id="27f72-122">Planned order release quantities are based on the planning calculation, and are affected by the parameters set on the individual item cards.</span><span class="sxs-lookup"><span data-stu-id="27f72-122">Planned order release quantities are based on the planning calculation, and are affected by the parameters set on the individual item cards.</span></span>  

## <a name="planning-with-manual-transfer-orders"></a><span data-ttu-id="27f72-123">Planning with Manual Transfer Orders</span><span class="sxs-lookup"><span data-stu-id="27f72-123">Planning with Manual Transfer Orders</span></span>

<span data-ttu-id="27f72-124">As you can see from the **Replenishment System** field on a SKU card, the planning system can be set up to create transfer orders to balance supply and demand across locations.</span><span class="sxs-lookup"><span data-stu-id="27f72-124">As you can see from the **Replenishment System** field on a SKU card, the planning system can be set up to create transfer orders to balance supply and demand across locations.</span></span>  

<span data-ttu-id="27f72-125">In addition to such automatic transfer orders, you may sometimes need to perform a general move of inventory quantities to another location, irrespective of existing demand.</span><span class="sxs-lookup"><span data-stu-id="27f72-125">In addition to such automatic transfer orders, you may sometimes need to perform a general move of inventory quantities to another location, irrespective of existing demand.</span></span> <span data-ttu-id="27f72-126">For this purpose you would manually create a transfer order for the quantity to move.</span><span class="sxs-lookup"><span data-stu-id="27f72-126">For this purpose you would manually create a transfer order for the quantity to move.</span></span> <span data-ttu-id="27f72-127">To ensure that the planning system does not try to manipulate this manual transfer order, you must set the **Planning Flexibility** on the transfer line(s) to None.</span><span class="sxs-lookup"><span data-stu-id="27f72-127">To ensure that the planning system does not try to manipulate this manual transfer order, you must set the **Planning Flexibility** on the transfer line(s) to None.</span></span>  

<span data-ttu-id="27f72-128">Contrarily, if you do want the planning system to adjust the transfer order quantities and dates to existing demand, you must set the **Planning Flexibility** field to the default value, Unlimited.</span><span class="sxs-lookup"><span data-stu-id="27f72-128">Contrarily, if you do want the planning system to adjust the transfer order quantities and dates to existing demand, you must set the **Planning Flexibility** field to the default value, Unlimited.</span></span>

## <a name="planning-parameters"></a><span data-ttu-id="27f72-129">Planning Parameters</span><span class="sxs-lookup"><span data-stu-id="27f72-129">Planning Parameters</span></span>

<span data-ttu-id="27f72-130">The planning parameters control when, how much, and how to replenish based on the various settings on the item card (or stockkeeping unit - SKU), and the manufacturing setup.</span><span class="sxs-lookup"><span data-stu-id="27f72-130">The planning parameters control when, how much, and how to replenish based on the various settings on the item card (or stockkeeping unit - SKU), and the manufacturing setup.</span></span>  

<span data-ttu-id="27f72-131">The following planning parameters exist on the item or SKU card:</span><span class="sxs-lookup"><span data-stu-id="27f72-131">The following planning parameters exist on the item or SKU card:</span></span>  

- <span data-ttu-id="27f72-132">Dampener Period</span><span class="sxs-lookup"><span data-stu-id="27f72-132">Dampener Period</span></span>  
- <span data-ttu-id="27f72-133">Dampener Quantity</span><span class="sxs-lookup"><span data-stu-id="27f72-133">Dampener Quantity</span></span>  
- <span data-ttu-id="27f72-134">Reordering Policy</span><span class="sxs-lookup"><span data-stu-id="27f72-134">Reordering Policy</span></span>  
- <span data-ttu-id="27f72-135">Reorder Point</span><span class="sxs-lookup"><span data-stu-id="27f72-135">Reorder Point</span></span>
- <span data-ttu-id="27f72-136">Maximum Inventory</span><span class="sxs-lookup"><span data-stu-id="27f72-136">Maximum Inventory</span></span>  
- <span data-ttu-id="27f72-137">Overflow Level</span><span class="sxs-lookup"><span data-stu-id="27f72-137">Overflow Level</span></span>  
- <span data-ttu-id="27f72-138">Time Bucket</span><span class="sxs-lookup"><span data-stu-id="27f72-138">Time Bucket</span></span>  
- <span data-ttu-id="27f72-139">Lot Accumulation Period</span><span class="sxs-lookup"><span data-stu-id="27f72-139">Lot Accumulation Period</span></span>  
- <span data-ttu-id="27f72-140">Rescheduling Period</span><span class="sxs-lookup"><span data-stu-id="27f72-140">Rescheduling Period</span></span>  
- <span data-ttu-id="27f72-141">Reorder Quantity</span><span class="sxs-lookup"><span data-stu-id="27f72-141">Reorder Quantity</span></span>  
- <span data-ttu-id="27f72-142">Safety Lead Time</span><span class="sxs-lookup"><span data-stu-id="27f72-142">Safety Lead Time</span></span>  
- <span data-ttu-id="27f72-143">Safety Stock Quantity</span><span class="sxs-lookup"><span data-stu-id="27f72-143">Safety Stock Quantity</span></span>  
- <span data-ttu-id="27f72-144">Assembly Policy</span><span class="sxs-lookup"><span data-stu-id="27f72-144">Assembly Policy</span></span>  
- <span data-ttu-id="27f72-145">Manufacturing Policy</span><span class="sxs-lookup"><span data-stu-id="27f72-145">Manufacturing Policy</span></span>  

<span data-ttu-id="27f72-146">The following order modifiers exist on the item or SKU card:</span><span class="sxs-lookup"><span data-stu-id="27f72-146">The following order modifiers exist on the item or SKU card:</span></span>  

- <span data-ttu-id="27f72-147">Minimum Order Quantity</span><span class="sxs-lookup"><span data-stu-id="27f72-147">Minimum Order Quantity</span></span>  
- <span data-ttu-id="27f72-148">Maximum Order Quantity</span><span class="sxs-lookup"><span data-stu-id="27f72-148">Maximum Order Quantity</span></span>  
- <span data-ttu-id="27f72-149">Order Multiple</span><span class="sxs-lookup"><span data-stu-id="27f72-149">Order Multiple</span></span>  

<span data-ttu-id="27f72-150">Global planning setup fields on the **Manufacturing Setup** page include:</span><span class="sxs-lookup"><span data-stu-id="27f72-150">Global planning setup fields on the **Manufacturing Setup** page include:</span></span>  

- <span data-ttu-id="27f72-151">Dynamic Low-Level Code</span><span class="sxs-lookup"><span data-stu-id="27f72-151">Dynamic Low-Level Code</span></span>  
- <span data-ttu-id="27f72-152">Current Demand Forecast</span><span class="sxs-lookup"><span data-stu-id="27f72-152">Current Demand Forecast</span></span>  
- <span data-ttu-id="27f72-153">Use Forecast on Locations</span><span class="sxs-lookup"><span data-stu-id="27f72-153">Use Forecast on Locations</span></span>  
- <span data-ttu-id="27f72-154">Default Safety Lead Time</span><span class="sxs-lookup"><span data-stu-id="27f72-154">Default Safety Lead Time</span></span>  
- <span data-ttu-id="27f72-155">Blank Overflow Level</span><span class="sxs-lookup"><span data-stu-id="27f72-155">Blank Overflow Level</span></span>  
- <span data-ttu-id="27f72-156">Combined MPS/MRP Calculation</span><span class="sxs-lookup"><span data-stu-id="27f72-156">Combined MPS/MRP Calculation</span></span>
- <span data-ttu-id="27f72-157">Components at Location</span><span class="sxs-lookup"><span data-stu-id="27f72-157">Components at Location</span></span>  
- <span data-ttu-id="27f72-158">Default Dampener Period</span><span class="sxs-lookup"><span data-stu-id="27f72-158">Default Dampener Period</span></span>  
- <span data-ttu-id="27f72-159">Default Dampener Quantity</span><span class="sxs-lookup"><span data-stu-id="27f72-159">Default Dampener Quantity</span></span>  

<span data-ttu-id="27f72-160">For more information, see [Design Details: Planning Parameters](design-details-planning-parameters.md)</span><span class="sxs-lookup"><span data-stu-id="27f72-160">For more information, see [Design Details: Planning Parameters](design-details-planning-parameters.md)</span></span>  

## <a name="other-important-planning-fields"></a><span data-ttu-id="27f72-161">Other Important Planning Fields</span><span class="sxs-lookup"><span data-stu-id="27f72-161">Other Important Planning Fields</span></span>

### <a name="planning-flexibility"></a><span data-ttu-id="27f72-162">Planning Flexibility</span><span class="sxs-lookup"><span data-stu-id="27f72-162">Planning Flexibility</span></span>

<span data-ttu-id="27f72-163">On most supply orders, such as production orders, you can select **Unlimited** or **None** in the **Planning Flexibility** field on the lines.</span><span class="sxs-lookup"><span data-stu-id="27f72-163">On most supply orders, such as production orders, you can select **Unlimited** or **None** in the **Planning Flexibility** field on the lines.</span></span>

<span data-ttu-id="27f72-164">This specifies whether the supply represented by the production order line is considered by the planning system when calculating action messages.</span><span class="sxs-lookup"><span data-stu-id="27f72-164">This specifies whether the supply represented by the production order line is considered by the planning system when calculating action messages.</span></span>
<span data-ttu-id="27f72-165">If the field contains **Unlimited**, then the planning system includes the line when calculating action messages.</span><span class="sxs-lookup"><span data-stu-id="27f72-165">If the field contains **Unlimited**, then the planning system includes the line when calculating action messages.</span></span> <span data-ttu-id="27f72-166">If the field contains **None**, then the line is firm and unchangeable, and the planning system does not include the line when calculating action messages.</span><span class="sxs-lookup"><span data-stu-id="27f72-166">If the field contains **None**, then the line is firm and unchangeable, and the planning system does not include the line when calculating action messages.</span></span>

### <a name="warning"></a><span data-ttu-id="27f72-167">Warning</span><span class="sxs-lookup"><span data-stu-id="27f72-167">Warning</span></span>

<span data-ttu-id="27f72-168">The **Warning** information field on the **Planning Worksheet** page informs you of any planning line created for an unusual situation with a text, which the user can choose to read additional information.</span><span class="sxs-lookup"><span data-stu-id="27f72-168">The **Warning** information field on the **Planning Worksheet** page informs you of any planning line created for an unusual situation with a text, which the user can choose to read additional information.</span></span> <span data-ttu-id="27f72-169">The following warning types exist:</span><span class="sxs-lookup"><span data-stu-id="27f72-169">The following warning types exist:</span></span>

- <span data-ttu-id="27f72-170">Emergency</span><span class="sxs-lookup"><span data-stu-id="27f72-170">Emergency</span></span>
- <span data-ttu-id="27f72-171">Exception</span><span class="sxs-lookup"><span data-stu-id="27f72-171">Exception</span></span>
- <span data-ttu-id="27f72-172">Attention</span><span class="sxs-lookup"><span data-stu-id="27f72-172">Attention</span></span>
- <span data-ttu-id="27f72-173">Emergency</span><span class="sxs-lookup"><span data-stu-id="27f72-173">Emergency</span></span>

<span data-ttu-id="27f72-174">The emergency warning is displayed in two situations:</span><span class="sxs-lookup"><span data-stu-id="27f72-174">The emergency warning is displayed in two situations:</span></span>

- <span data-ttu-id="27f72-175">The inventory is negative on the planning starting date.</span><span class="sxs-lookup"><span data-stu-id="27f72-175">The inventory is negative on the planning starting date.</span></span>
- <span data-ttu-id="27f72-176">Back-dated supply or demand events exist.</span><span class="sxs-lookup"><span data-stu-id="27f72-176">Back-dated supply or demand events exist.</span></span>

<span data-ttu-id="27f72-177">If an item's inventory is negative on the planning starting date, the planning system suggests an emergency supply order for the negative quantity to arrive on the planning starting date.</span><span class="sxs-lookup"><span data-stu-id="27f72-177">If an item's inventory is negative on the planning starting date, the planning system suggests an emergency supply order for the negative quantity to arrive on the planning starting date.</span></span> <span data-ttu-id="27f72-178">The warning text states the starting date and the quantity of the emergency order.</span><span class="sxs-lookup"><span data-stu-id="27f72-178">The warning text states the starting date and the quantity of the emergency order.</span></span>

<span data-ttu-id="27f72-179">Any document lines with due dates before the planning starting date are consolidated into one emergency supply order for the item to arrive on the planning starting date.</span><span class="sxs-lookup"><span data-stu-id="27f72-179">Any document lines with due dates before the planning starting date are consolidated into one emergency supply order for the item to arrive on the planning starting date.</span></span>

### <a name="exception"></a><span data-ttu-id="27f72-180">Exception</span><span class="sxs-lookup"><span data-stu-id="27f72-180">Exception</span></span>

<span data-ttu-id="27f72-181">The exception warning is displayed if the projected available inventory drops below the safety stock quantity.</span><span class="sxs-lookup"><span data-stu-id="27f72-181">The exception warning is displayed if the projected available inventory drops below the safety stock quantity.</span></span>

<span data-ttu-id="27f72-182">The planning system will suggest a supply order to meet the demand on its due date.</span><span class="sxs-lookup"><span data-stu-id="27f72-182">The planning system will suggest a supply order to meet the demand on its due date.</span></span> <span data-ttu-id="27f72-183">The warning text states the item's safety stock quantity and the date on which it is violated.</span><span class="sxs-lookup"><span data-stu-id="27f72-183">The warning text states the item's safety stock quantity and the date on which it is violated.</span></span>

<span data-ttu-id="27f72-184">Violating the safety stock level is considered an exception because it should not occur if the reorder point has been set correctly.</span><span class="sxs-lookup"><span data-stu-id="27f72-184">Violating the safety stock level is considered an exception because it should not occur if the reorder point has been set correctly.</span></span>

> [!NOTE]
> <span data-ttu-id="27f72-185">Supply on planning lines with Exception warnings is normally not modified according to planning parameters.</span><span class="sxs-lookup"><span data-stu-id="27f72-185">Supply on planning lines with Exception warnings is normally not modified according to planning parameters.</span></span> <span data-ttu-id="27f72-186">Instead, the planning system only suggests a supply to cover the exact demand quantity.</span><span class="sxs-lookup"><span data-stu-id="27f72-186">Instead, the planning system only suggests a supply to cover the exact demand quantity.</span></span> <span data-ttu-id="27f72-187">However, you can set the planning run up to respect certain planning parameters for planning lines with certain warnings.</span><span class="sxs-lookup"><span data-stu-id="27f72-187">However, you can set the planning run up to respect certain planning parameters for planning lines with certain warnings.</span></span> <span data-ttu-id="27f72-188">For more information, see the description for the **Respect Planning Parameters for Exception Warnings** field in the [Run Full Planning, MPS or MRP](production-how-to-run-mps-and-mrp.md) article.</span><span class="sxs-lookup"><span data-stu-id="27f72-188">For more information, see the description for the **Respect Planning Parameters for Exception Warnings** field in the [Run Full Planning, MPS or MRP](production-how-to-run-mps-and-mrp.md) article.</span></span>

### <a name="attention"></a><span data-ttu-id="27f72-189">Attention</span><span class="sxs-lookup"><span data-stu-id="27f72-189">Attention</span></span>

<span data-ttu-id="27f72-190">The attention warning is displayed in two situations:</span><span class="sxs-lookup"><span data-stu-id="27f72-190">The attention warning is displayed in two situations:</span></span>

- <span data-ttu-id="27f72-191">The planning starting date is earlier than the work date.</span><span class="sxs-lookup"><span data-stu-id="27f72-191">The planning starting date is earlier than the work date.</span></span>
- <span data-ttu-id="27f72-192">The planning line suggests to change a released purchase or production order.</span><span class="sxs-lookup"><span data-stu-id="27f72-192">The planning line suggests to change a released purchase or production order.</span></span>

> [!NOTE]
> <span data-ttu-id="27f72-193">In planning lines with warnings, the **Accept Action Message** field is not selected, because the planner is expected to further investigate these lines before carrying out the plan.</span><span class="sxs-lookup"><span data-stu-id="27f72-193">In planning lines with warnings, the **Accept Action Message** field is not selected, because the planner is expected to further investigate these lines before carrying out the plan.</span></span>

## <a name="planning-worksheets-and-requisition-worksheets"></a><span data-ttu-id="27f72-194">Planning worksheets and requisition worksheets</span><span class="sxs-lookup"><span data-stu-id="27f72-194">Planning worksheets and requisition worksheets</span></span>

<span data-ttu-id="27f72-195">As described in [Planning](production-planning.md), you can choose between two worksheets for most planning activities, the planning worksheet and the requisition worksheet.</span><span class="sxs-lookup"><span data-stu-id="27f72-195">As described in [Planning](production-planning.md), you can choose between two worksheets for most planning activities, the planning worksheet and the requisition worksheet.</span></span> <span data-ttu-id="27f72-196">Most processes are described based on the planning worksheet, but there are a couple of scenarios where the requisition worksheet is preferred.</span><span class="sxs-lookup"><span data-stu-id="27f72-196">Most processes are described based on the planning worksheet, but there are a couple of scenarios where the requisition worksheet is preferred.</span></span>

### <a name="requisition-worksheet"></a><span data-ttu-id="27f72-197">Requisition worksheet</span><span class="sxs-lookup"><span data-stu-id="27f72-197">Requisition worksheet</span></span>

<span data-ttu-id="27f72-198">The **Requisition Worksheet** page lists items that you want to order.</span><span class="sxs-lookup"><span data-stu-id="27f72-198">The **Requisition Worksheet** page lists items that you want to order.</span></span> <span data-ttu-id="27f72-199">You can enter items in the worksheet in the following ways:</span><span class="sxs-lookup"><span data-stu-id="27f72-199">You can enter items in the worksheet in the following ways:</span></span>

- <span data-ttu-id="27f72-200">Enter the items manually in the worksheet and fill in the relevant fields.</span><span class="sxs-lookup"><span data-stu-id="27f72-200">Enter the items manually in the worksheet and fill in the relevant fields.</span></span>

- <span data-ttu-id="27f72-201">Use the **Calculate Plan** batch job.</span><span class="sxs-lookup"><span data-stu-id="27f72-201">Use the **Calculate Plan** batch job.</span></span> <span data-ttu-id="27f72-202">This calculates a replenishment plan for items and stockkeeping units that have been set up with a replenishment system of **Purchase** or **Transfer**.</span><span class="sxs-lookup"><span data-stu-id="27f72-202">This calculates a replenishment plan for items and stockkeeping units that have been set up with a replenishment system of **Purchase** or **Transfer**.</span></span> <span data-ttu-id="27f72-203">When you use this batch job, the program automatically fills in the **Action Message** field with a suggestion for an action you can take to replenish the item.</span><span class="sxs-lookup"><span data-stu-id="27f72-203">When you use this batch job, the program automatically fills in the **Action Message** field with a suggestion for an action you can take to replenish the item.</span></span> <span data-ttu-id="27f72-204">This could be increasing the item quantity on an existing order or creating a new order, for example.</span><span class="sxs-lookup"><span data-stu-id="27f72-204">This could be increasing the item quantity on an existing order or creating a new order, for example.</span></span>

- <span data-ttu-id="27f72-205">If you have used the **Calculate Plan** batch job from the **Planning Worksheet** page to calculate a replenishment plan, you can use the **Carry Out Action Message** batch job to copy purchase and transfer order proposals from the planning worksheet to the requisition worksheet.</span><span class="sxs-lookup"><span data-stu-id="27f72-205">If you have used the **Calculate Plan** batch job from the **Planning Worksheet** page to calculate a replenishment plan, you can use the **Carry Out Action Message** batch job to copy purchase and transfer order proposals from the planning worksheet to the requisition worksheet.</span></span> <span data-ttu-id="27f72-206">This is practical if separate users are responsible for handling production orders and purchase/transfer orders.</span><span class="sxs-lookup"><span data-stu-id="27f72-206">This is practical if separate users are responsible for handling production orders and purchase/transfer orders.</span></span>

- <span data-ttu-id="27f72-207">You can use the **Drop Shipment** action to fill in the requisition worksheet lines.</span><span class="sxs-lookup"><span data-stu-id="27f72-207">You can use the **Drop Shipment** action to fill in the requisition worksheet lines.</span></span> <span data-ttu-id="27f72-208">This action uses the **Get Sales Orders** batch job to determine the sales order lines that you want to designate for a drop shipment.</span><span class="sxs-lookup"><span data-stu-id="27f72-208">This action uses the **Get Sales Orders** batch job to determine the sales order lines that you want to designate for a drop shipment.</span></span>

- <span data-ttu-id="27f72-209">You can use the **Special Order** action to fill in the requisition worksheet lines.</span><span class="sxs-lookup"><span data-stu-id="27f72-209">You can use the **Special Order** action to fill in the requisition worksheet lines.</span></span> <span data-ttu-id="27f72-210">This action uses the **Get Sales Orders** batch job to determine the sales order lines that you want to designate for a special order.</span><span class="sxs-lookup"><span data-stu-id="27f72-210">This action uses the **Get Sales Orders** batch job to determine the sales order lines that you want to designate for a special order.</span></span>

<span data-ttu-id="27f72-211">Requisition worksheet lines contain detailed information about the items that need to be reordered.</span><span class="sxs-lookup"><span data-stu-id="27f72-211">Requisition worksheet lines contain detailed information about the items that need to be reordered.</span></span> <span data-ttu-id="27f72-212">You can edit and delete the lines to adjust your replenishment plan, and you can further process the lines by using the **Carry Out Action Message** batch job.</span><span class="sxs-lookup"><span data-stu-id="27f72-212">You can edit and delete the lines to adjust your replenishment plan, and you can further process the lines by using the **Carry Out Action Message** batch job.</span></span>

<span data-ttu-id="27f72-213">For details about planning with locations and transfers, see [Planning With or Without Locations](production-planning-with-without-locations.md).</span><span class="sxs-lookup"><span data-stu-id="27f72-213">For details about planning with locations and transfers, see [Planning With or Without Locations](production-planning-with-without-locations.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="27f72-214">See Also</span><span class="sxs-lookup"><span data-stu-id="27f72-214">See Also</span></span>

[<span data-ttu-id="27f72-215">Design Details: Supply Planning</span><span class="sxs-lookup"><span data-stu-id="27f72-215">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)  
[<span data-ttu-id="27f72-216">Planning</span><span class="sxs-lookup"><span data-stu-id="27f72-216">Planning</span></span>](production-planning.md)  
[<span data-ttu-id="27f72-217">Setting Up Manufacturing</span><span class="sxs-lookup"><span data-stu-id="27f72-217">Setting Up Manufacturing</span></span>](production-configure-production-processes.md)  
[<span data-ttu-id="27f72-218">Manufacturing</span><span class="sxs-lookup"><span data-stu-id="27f72-218">Manufacturing</span></span>](production-manage-manufacturing.md)  
[<span data-ttu-id="27f72-219">Inventory</span><span class="sxs-lookup"><span data-stu-id="27f72-219">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="27f72-220">Purchasing</span><span class="sxs-lookup"><span data-stu-id="27f72-220">Purchasing</span></span>](purchasing-manage-purchasing.md)  
[<span data-ttu-id="27f72-221">Setup Best Practices: Supply Planning</span><span class="sxs-lookup"><span data-stu-id="27f72-221">Setup Best Practices: Supply Planning</span></span>](setup-best-practices-supply-planning.md)  
<span data-ttu-id="27f72-222">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="27f72-222">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>


[!INCLUDE[footer-include](includes/footer-banner.md)]