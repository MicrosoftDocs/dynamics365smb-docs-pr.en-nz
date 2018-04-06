---
title: How to Plan Order by Order | Microsoft Docs
description: This planning task can be performed in the **Order Planning** window, which displays all new demand along with availability information and suggestions for supply. It provides the visibility and tools needed to effectively plan demand from sales lines and component lines and then create different types of supply orders directly.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/06/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 7a519025bd7bed4bb2974c3e7fb5f044ac35dcf4
ms.contentlocale: en-nz
ms.lasthandoff: 03/22/2018

---
# <a name="plan-for-new-demand-order-by-order"></a><span data-ttu-id="1b435-104">Plan for New Demand Order by Order</span><span class="sxs-lookup"><span data-stu-id="1b435-104">Plan for New Demand Order by Order</span></span>
<span data-ttu-id="1b435-105">This planning task can be performed in the **Order Planning** window, which displays all new demand along with availability information and suggestions for supply.</span><span class="sxs-lookup"><span data-stu-id="1b435-105">This planning task can be performed in the **Order Planning** window, which displays all new demand along with availability information and suggestions for supply.</span></span> <span data-ttu-id="1b435-106">It provides the visibility and tools needed to effectively plan demand from sales lines and component lines and then create different types of supply orders directly.</span><span class="sxs-lookup"><span data-stu-id="1b435-106">It provides the visibility and tools needed to effectively plan demand from sales lines and component lines and then create different types of supply orders directly.</span></span>  

<span data-ttu-id="1b435-107">You can enter the **Order Planning** window in two ways depending on your focus: From an order that you want to plan for specifically or in batch mode because you want to plan for all and any new demand.</span><span class="sxs-lookup"><span data-stu-id="1b435-107">You can enter the **Order Planning** window in two ways depending on your focus: From an order that you want to plan for specifically or in batch mode because you want to plan for all and any new demand.</span></span>  


## <a name="to-plan-for-new-production-order-demand"></a><span data-ttu-id="1b435-108">To plan for new production order demand</span><span class="sxs-lookup"><span data-stu-id="1b435-108">To plan for new production order demand</span></span>  
1.  <span data-ttu-id="1b435-109">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Planned Production Orders**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="1b435-109">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Planned Production Orders**, and then choose the related link.</span></span> <span data-ttu-id="1b435-110">(You can perform these steps for planned, firm planned, or released production orders).</span><span class="sxs-lookup"><span data-stu-id="1b435-110">(You can perform these steps for planned, firm planned, or released production orders).</span></span>
2.  <span data-ttu-id="1b435-111">Open the production order you want to plan for, and then choose the **Planning** action.</span><span class="sxs-lookup"><span data-stu-id="1b435-111">Open the production order you want to plan for, and then choose the **Planning** action.</span></span>  
3.  <span data-ttu-id="1b435-112">In the **Order Planning** window, choose the **Calculate Plan** action.</span><span class="sxs-lookup"><span data-stu-id="1b435-112">In the **Order Planning** window, choose the **Calculate Plan** action.</span></span>  

<span data-ttu-id="1b435-113">The window displays planning lines according to the view filter **Production Demand**, meaning unfulfilled component lines of all existing production orders.</span><span class="sxs-lookup"><span data-stu-id="1b435-113">The window displays planning lines according to the view filter **Production Demand**, meaning unfulfilled component lines of all existing production orders.</span></span> <span data-ttu-id="1b435-114">Demand for only the one production order is not shown because it is necessary to plan for one production order with an overview of demand for potentially earlier components lines.</span><span class="sxs-lookup"><span data-stu-id="1b435-114">Demand for only the one production order is not shown because it is necessary to plan for one production order with an overview of demand for potentially earlier components lines.</span></span> <span data-ttu-id="1b435-115">Planning lines for the production order in context are expanded.</span><span class="sxs-lookup"><span data-stu-id="1b435-115">Planning lines for the production order in context are expanded.</span></span>  

## <a name="to-plan-for-any-new-demand"></a><span data-ttu-id="1b435-116">To plan for any new demand</span><span class="sxs-lookup"><span data-stu-id="1b435-116">To plan for any new demand</span></span>  
1. <span data-ttu-id="1b435-117">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Order Planning**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="1b435-117">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Order Planning**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="1b435-118">In the **Order Planning** window, choose the **Calculate Plan** action.</span><span class="sxs-lookup"><span data-stu-id="1b435-118">In the **Order Planning** window, choose the **Calculate Plan** action.</span></span>
3.  <span data-ttu-id="1b435-119">Choose the **Expand (+)** button in front of the date in the **Demand Date** field to see the underlying planning lines that represent demand lines with insufficient availability.</span><span class="sxs-lookup"><span data-stu-id="1b435-119">Choose the **Expand (+)** button in front of the date in the **Demand Date** field to see the underlying planning lines that represent demand lines with insufficient availability.</span></span>  
4.  <span data-ttu-id="1b435-120">For each expanded planning line, that is, demand line, you can see values in information fields at the bottom of the window.</span><span class="sxs-lookup"><span data-stu-id="1b435-120">For each expanded planning line, that is, demand line, you can see values in information fields at the bottom of the window.</span></span>  

    |<span data-ttu-id="1b435-121">Option</span><span class="sxs-lookup"><span data-stu-id="1b435-121">Option</span></span>|<span data-ttu-id="1b435-122">Description</span><span class="sxs-lookup"><span data-stu-id="1b435-122">Description</span></span>|  
    |----------------------------------|---------------------------------------|  
    |<span data-ttu-id="1b435-123">**Qty. on Other Locations**</span><span class="sxs-lookup"><span data-stu-id="1b435-123">**Qty. on Other Locations**</span></span>|<span data-ttu-id="1b435-124">Shows if the item exists on another location.</span><span class="sxs-lookup"><span data-stu-id="1b435-124">Shows if the item exists on another location.</span></span> <span data-ttu-id="1b435-125">You can then look up and select it.</span><span class="sxs-lookup"><span data-stu-id="1b435-125">You can then look up and select it.</span></span>|  
    |<span data-ttu-id="1b435-126">**Substitutes Exist**</span><span class="sxs-lookup"><span data-stu-id="1b435-126">**Substitutes Exist**</span></span>|<span data-ttu-id="1b435-127">Shows if a substitute item is created for the item.</span><span class="sxs-lookup"><span data-stu-id="1b435-127">Shows if a substitute item is created for the item.</span></span> <span data-ttu-id="1b435-128">You can then look up and select it.</span><span class="sxs-lookup"><span data-stu-id="1b435-128">You can then look up and select it.</span></span> <span data-ttu-id="1b435-129">Note that this feature only applies to components, that is, from demand lines of type **Production**.</span><span class="sxs-lookup"><span data-stu-id="1b435-129">Note that this feature only applies to components, that is, from demand lines of type **Production**.</span></span>|  
    |<span data-ttu-id="1b435-130">**Quantity Available**</span><span class="sxs-lookup"><span data-stu-id="1b435-130">**Quantity Available**</span></span>|<span data-ttu-id="1b435-131">Shows the total availability of the item, that is, the Projected Available Balance.</span><span class="sxs-lookup"><span data-stu-id="1b435-131">Shows the total availability of the item, that is, the Projected Available Balance.</span></span>|  
    |<span data-ttu-id="1b435-132">**Earliest Date Available**</span><span class="sxs-lookup"><span data-stu-id="1b435-132">**Earliest Date Available**</span></span>|<span data-ttu-id="1b435-133">Shows the arrival date of an inbound supply order that can cover the needed quantity on a date later than the demand date.</span><span class="sxs-lookup"><span data-stu-id="1b435-133">Shows the arrival date of an inbound supply order that can cover the needed quantity on a date later than the demand date.</span></span>|  

5.  <span data-ttu-id="1b435-134">In the **Replenishment System** field, select which type of supply order to create.</span><span class="sxs-lookup"><span data-stu-id="1b435-134">In the **Replenishment System** field, select which type of supply order to create.</span></span>  

    <span data-ttu-id="1b435-135">The default value is that of the item card, or SKU card, but you can change it to one of three options:</span><span class="sxs-lookup"><span data-stu-id="1b435-135">The default value is that of the item card, or SKU card, but you can change it to one of three options:</span></span>  

    |<span data-ttu-id="1b435-136">Option</span><span class="sxs-lookup"><span data-stu-id="1b435-136">Option</span></span>|<span data-ttu-id="1b435-137">Description</span><span class="sxs-lookup"><span data-stu-id="1b435-137">Description</span></span>|  
    |----------------------------------|---------------------------------------|  
    |<span data-ttu-id="1b435-138">**Purchase**</span><span class="sxs-lookup"><span data-stu-id="1b435-138">**Purchase**</span></span>|<span data-ttu-id="1b435-139">Creates a purchase order.</span><span class="sxs-lookup"><span data-stu-id="1b435-139">Creates a purchase order.</span></span>|  
    |<span data-ttu-id="1b435-140">**Transfer**</span><span class="sxs-lookup"><span data-stu-id="1b435-140">**Transfer**</span></span>|<span data-ttu-id="1b435-141">Creates a transfer order.</span><span class="sxs-lookup"><span data-stu-id="1b435-141">Creates a transfer order.</span></span>|  
    |<span data-ttu-id="1b435-142">**Prod. Order**</span><span class="sxs-lookup"><span data-stu-id="1b435-142">**Prod. Order**</span></span>|<span data-ttu-id="1b435-143">Creates a production order.</span><span class="sxs-lookup"><span data-stu-id="1b435-143">Creates a production order.</span></span>|  

    <span data-ttu-id="1b435-144">In the **Supply From** field you must select a value according to the selected replenishment system.</span><span class="sxs-lookup"><span data-stu-id="1b435-144">In the **Supply From** field you must select a value according to the selected replenishment system.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="1b435-145">If the field is not filled in, the system will display an error message when you use the **Make Supply Order** function, and no supply order will be created for the planning line in question.</span><span class="sxs-lookup"><span data-stu-id="1b435-145">If the field is not filled in, the system will display an error message when you use the **Make Supply Order** function, and no supply order will be created for the planning line in question.</span></span> <span data-ttu-id="1b435-146">This, however, is not the case if the replenishment system is **Prod. Order**.</span><span class="sxs-lookup"><span data-stu-id="1b435-146">This, however, is not the case if the replenishment system is **Prod. Order**.</span></span>  

6.  <span data-ttu-id="1b435-147">From the **Supply From** field, you can look up in the relevant list and select where the supply should come from:</span><span class="sxs-lookup"><span data-stu-id="1b435-147">From the **Supply From** field, you can look up in the relevant list and select where the supply should come from:</span></span>  

    - <span data-ttu-id="1b435-148">If replenishment system is **Purchase**, the look-up button in this field looks up in the **Item Vendor Catalogue** window.</span><span class="sxs-lookup"><span data-stu-id="1b435-148">If replenishment system is **Purchase**, the look-up button in this field looks up in the **Item Vendor Catalog** window.</span></span>  
    - <span data-ttu-id="1b435-149">If replenishment system is **Transfer**, the look-up button in this field looks up in the **Location List** window.</span><span class="sxs-lookup"><span data-stu-id="1b435-149">If replenishment system is **Transfer**, the look-up button in this field looks up in the **Location List** window.</span></span>  

    <span data-ttu-id="1b435-150">In case the item exists in another location, the **Qty. on Other Location** field at the bottom shows a value and you can then look up and select the location from which the item should be supplied when you make the transfer order.</span><span class="sxs-lookup"><span data-stu-id="1b435-150">In case the item exists in another location, the **Qty. on Other Location** field at the bottom shows a value and you can then look up and select the location from which the item should be supplied when you make the transfer order.</span></span>  

    <span data-ttu-id="1b435-151">If a substitute exists for the demanded item, the **Substitute Exists** field is set to **Yes**, and you can then look up to the **Item Substitution Entries** window and select the substitute.</span><span class="sxs-lookup"><span data-stu-id="1b435-151">If a substitute exists for the demanded item, the **Substitute Exists** field is set to **Yes**, and you can then look up to the **Item Substitution Entries** window and select the substitute.</span></span>  

7.  <span data-ttu-id="1b435-152">Select the **Reserve** check box if you want to make a reservation between the supply order you are creating and the demand line that it is created for.</span><span class="sxs-lookup"><span data-stu-id="1b435-152">Select the **Reserve** check box if you want to make a reservation between the supply order you are creating and the demand line that it is created for.</span></span> <span data-ttu-id="1b435-153">It is empty by default.</span><span class="sxs-lookup"><span data-stu-id="1b435-153">It is empty by default.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="1b435-154">You can only select this check box if the item has **Optional** or **Always** in the **Reserve** field on its item card.</span><span class="sxs-lookup"><span data-stu-id="1b435-154">You can only select this check box if the item has **Optional** or **Always** in the **Reserve** field on its item card.</span></span>  

8.  <span data-ttu-id="1b435-155">In the **Qty. to Order** field, you can enter the quantity that will go on the supply order you are creating.</span><span class="sxs-lookup"><span data-stu-id="1b435-155">In the **Qty. to Order** field, you can enter the quantity that will go on the supply order you are creating.</span></span>   
    <span data-ttu-id="1b435-156">The default value is the same quantity as that in the **Needed Quantity** field.</span><span class="sxs-lookup"><span data-stu-id="1b435-156">The default value is the same quantity as that in the **Needed Quantity** field.</span></span> <span data-ttu-id="1b435-157">But you may decide to order more or less than this quantity based on your knowledge of the demand situation.</span><span class="sxs-lookup"><span data-stu-id="1b435-157">But you may decide to order more or less than this quantity based on your knowledge of the demand situation.</span></span> <span data-ttu-id="1b435-158">If, for example, you see in the **Order Planning** window that several unrelated demand lines are for the same purchased item, and they are due around the same date, you can consolidate these by entering the total needed quantity in the **Qty. to Order** field of one line, and then delete the other, obsolete planning lines for that item.</span><span class="sxs-lookup"><span data-stu-id="1b435-158">If, for example, you see in the **Order Planning** window that several unrelated demand lines are for the same purchased item, and they are due around the same date, you can consolidate these by entering the total needed quantity in the **Qty. to Order** field of one line, and then delete the other, obsolete planning lines for that item.</span></span>  

9.  <span data-ttu-id="1b435-159">In the **Due Date** and **Order Date** fields, you can enter the dates that should apply to the created supply orders.</span><span class="sxs-lookup"><span data-stu-id="1b435-159">In the **Due Date** and **Order Date** fields, you can enter the dates that should apply to the created supply orders.</span></span>  

    <span data-ttu-id="1b435-160">These two fields are interrelated according to the **Default Safety Lead Time** field, which can be found in the **Manufacturing Setup** window.</span><span class="sxs-lookup"><span data-stu-id="1b435-160">These two fields are interrelated according to the **Default Safety Lead Time** field, which can be found in the **Manufacturing Setup** window.</span></span> <span data-ttu-id="1b435-161">By default, the due date is the same as the demand date, but you can change this as you like.</span><span class="sxs-lookup"><span data-stu-id="1b435-161">By default, the due date is the same as the demand date, but you can change this as you like.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="1b435-162"> If you enter a date later than the demand date, you will receive a warning message.</span><span class="sxs-lookup"><span data-stu-id="1b435-162">If you enter a date later than the demand date, you will receive a warning message.</span></span>  

## <a name="to-make-supply-orders"></a><span data-ttu-id="1b435-163">To make supply orders</span><span class="sxs-lookup"><span data-stu-id="1b435-163">To make supply orders</span></span>  
1.  <span data-ttu-id="1b435-164">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Planned Production Orders**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="1b435-164">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Planned Production Orders**, and then choose the related link.</span></span> <span data-ttu-id="1b435-165">You can perform these steps for a planned, firm planned, or released production order.</span><span class="sxs-lookup"><span data-stu-id="1b435-165">You can perform these steps for a planned, firm planned, or released production order.</span></span>  
2.  <span data-ttu-id="1b435-166">Open the production order you want to plan for, and then choose the **Planning** action.</span><span class="sxs-lookup"><span data-stu-id="1b435-166">Open the production order you want to plan for, and then choose the **Planning** action.</span></span>  
3.  <span data-ttu-id="1b435-167">Place the cursor on a relevant planning line, and then choose the **Make Orders** action.</span><span class="sxs-lookup"><span data-stu-id="1b435-167">Place the cursor on a relevant planning line, and then choose the **Make Orders** action.</span></span>  
4.  <span data-ttu-id="1b435-168">In the **Make Supply Orders** window, on the **Order Planning** FastTab, in the **Make Orders for** field, select one of the following options.</span><span class="sxs-lookup"><span data-stu-id="1b435-168">In the **Make Supply Orders** window, on the **Order Planning** FastTab, in the **Make Orders for** field, select one of the following options.</span></span>  

    |<span data-ttu-id="1b435-169">Option</span><span class="sxs-lookup"><span data-stu-id="1b435-169">Option</span></span>|<span data-ttu-id="1b435-170">Description</span><span class="sxs-lookup"><span data-stu-id="1b435-170">Description</span></span>|  
    |----------------------------------|---------------------------------------|  
    |<span data-ttu-id="1b435-171">**The Active Line**</span><span class="sxs-lookup"><span data-stu-id="1b435-171">**The Active Line**</span></span>|<span data-ttu-id="1b435-172">Make a supply order only for the line where the cursor is placed.</span><span class="sxs-lookup"><span data-stu-id="1b435-172">Make a supply order only for the line where the cursor is placed.</span></span>|  
    |<span data-ttu-id="1b435-173">**The Active Order**</span><span class="sxs-lookup"><span data-stu-id="1b435-173">**The Active Order**</span></span>|<span data-ttu-id="1b435-174">Make supply orders for all lines in the order where the cursor is placed.</span><span class="sxs-lookup"><span data-stu-id="1b435-174">Make supply orders for all lines in the order where the cursor is placed.</span></span>|  
    |<span data-ttu-id="1b435-175">**All Lines**</span><span class="sxs-lookup"><span data-stu-id="1b435-175">**All Lines**</span></span>|<span data-ttu-id="1b435-176">Make supply orders for all lines in the **Order Planning** window.</span><span class="sxs-lookup"><span data-stu-id="1b435-176">Make supply orders for all lines in the **Order Planning** window.</span></span>|  

5.  <span data-ttu-id="1b435-177">On the **Options** FastTab, define what kind of supply orders, or requisition worksheet lines, should be made.</span><span class="sxs-lookup"><span data-stu-id="1b435-177">On the **Options** FastTab, define what kind of supply orders, or requisition worksheet lines, should be made.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="1b435-178">The settings you last made in the **Make Supply Orders** window will be saved under your user ID so that they are the same the next time you use the window.</span><span class="sxs-lookup"><span data-stu-id="1b435-178">The settings you last made in the **Make Supply Orders** window will be saved under your user ID so that they are the same the next time you use the window.</span></span>  

6.  <span data-ttu-id="1b435-179">Choose the **OK** button to make the suggested supply orders or requisition worksheet lines.</span><span class="sxs-lookup"><span data-stu-id="1b435-179">Choose the **OK** button to make the suggested supply orders or requisition worksheet lines.</span></span>  

<span data-ttu-id="1b435-180">You have now planned for the unfulfilled demand by making respective supply orders.</span><span class="sxs-lookup"><span data-stu-id="1b435-180">You have now planned for the unfulfilled demand by making respective supply orders.</span></span> <span data-ttu-id="1b435-181">Details about specific work flows when using the **Order Planning** window would depend on a company’s internal policies.</span><span class="sxs-lookup"><span data-stu-id="1b435-181">Details about specific work flows when using the **Order Planning** window would depend on a company’s internal policies.</span></span>  

<span data-ttu-id="1b435-182">When you have finished your planning work in the **Order Planning** window, for example defined an alternative way to supply the quantity, you can proceed to create supply orders for one or more of the planning lines.</span><span class="sxs-lookup"><span data-stu-id="1b435-182">When you have finished your planning work in the **Order Planning** window, for example defined an alternative way to supply the quantity, you can proceed to create supply orders for one or more of the planning lines.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="1b435-183">The supply orders you create may introduce new dependent demand, for example for underlying production orders, and you should therefore choose **Calculate Plan** again to find and resolve this before moving down the list.</span><span class="sxs-lookup"><span data-stu-id="1b435-183">The supply orders you create may introduce new dependent demand, for example for underlying production orders, and you should therefore choose **Calculate Plan** again to find and resolve this before moving down the list.</span></span>  

## <a name="see-also"></a><span data-ttu-id="1b435-184">See Also</span><span class="sxs-lookup"><span data-stu-id="1b435-184">See Also</span></span>  
[<span data-ttu-id="1b435-185">Planning</span><span class="sxs-lookup"><span data-stu-id="1b435-185">Planning</span></span>](production-planning.md)  
[<span data-ttu-id="1b435-186">Setting Up Manufacturing</span><span class="sxs-lookup"><span data-stu-id="1b435-186">Setting Up Manufacturing</span></span>](production-configure-production-processes.md)  
<span data-ttu-id="1b435-187">[Manufacturing](production-manage-manufacturing.md)  </span><span class="sxs-lookup"><span data-stu-id="1b435-187">[Manufacturing](production-manage-manufacturing.md)  </span></span>  
[<span data-ttu-id="1b435-188">Inventory</span><span class="sxs-lookup"><span data-stu-id="1b435-188">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="1b435-189">Purchasing</span><span class="sxs-lookup"><span data-stu-id="1b435-189">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="1b435-190">[Design Details: Supply Planning](design-details-supply-planning.md) </span><span class="sxs-lookup"><span data-stu-id="1b435-190">[Design Details: Supply Planning](design-details-supply-planning.md) </span></span>  
[<span data-ttu-id="1b435-191">Setup Best Practices: Supply Planning</span><span class="sxs-lookup"><span data-stu-id="1b435-191">Setup Best Practices: Supply Planning</span></span>](setup-best-practices-supply-planning.md)  
<span data-ttu-id="1b435-192">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="1b435-192">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
