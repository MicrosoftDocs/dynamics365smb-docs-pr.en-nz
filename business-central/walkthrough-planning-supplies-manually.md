---
title: Walkthrough - Planning Supplies Manually | Microsoft Docs
description: This walkthrough demonstrates the process of planning supply orders to fulfill new demand. You can initiate supply planning at fixed intervals, for example, every morning or every Monday, or when you are notified by sales or production, depending on the type of demand.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/07/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 2992c2a9cbd2142e69cfb59294791ec31ce4dcb1
ms.contentlocale: en-nz
ms.lasthandoff: 03/22/2018

---
# <a name="walkthrough-planning-supplies-manually"></a><span data-ttu-id="40a1e-104">Walkthrough: Planning Supplies Manually</span><span class="sxs-lookup"><span data-stu-id="40a1e-104">Walkthrough: Planning Supplies Manually</span></span>
<span data-ttu-id="40a1e-105">This walkthrough demonstrates the process of planning supply orders to fulfill new demand.</span><span class="sxs-lookup"><span data-stu-id="40a1e-105">This walkthrough demonstrates the process of planning supply orders to fulfill new demand.</span></span> <span data-ttu-id="40a1e-106">You can initiate supply planning at fixed intervals, for example, every morning or every Monday, or when you are notified by sales or production, depending on the type of demand.</span><span class="sxs-lookup"><span data-stu-id="40a1e-106">You can initiate supply planning at fixed intervals, for example, every morning or every Monday, or when you are notified by sales or production, depending on the type of demand.</span></span> <span data-ttu-id="40a1e-107">In this walkthrough you will use the **Order Planning** window, a simple supply planning tool that is based on manual decision-making instead of parameter-based automatic planning.</span><span class="sxs-lookup"><span data-stu-id="40a1e-107">In this walkthrough you will use the **Order Planning** window, a simple supply planning tool that is based on manual decision-making instead of parameter-based automatic planning.</span></span>  

## <a name="about-this-walkthrough"></a><span data-ttu-id="40a1e-108">About This Walkthrough</span><span class="sxs-lookup"><span data-stu-id="40a1e-108">About This Walkthrough</span></span>  
 <span data-ttu-id="40a1e-109">This walkthrough illustrates the following tasks:</span><span class="sxs-lookup"><span data-stu-id="40a1e-109">This walkthrough illustrates the following tasks:</span></span>  

-   <span data-ttu-id="40a1e-110">Planning a purchase order for manufacturing components.</span><span class="sxs-lookup"><span data-stu-id="40a1e-110">Planning a purchase order for manufacturing components.</span></span>  
-   <span data-ttu-id="40a1e-111">Planning a transfer order to fulfill sales demand.</span><span class="sxs-lookup"><span data-stu-id="40a1e-111">Planning a transfer order to fulfill sales demand.</span></span>  
-   <span data-ttu-id="40a1e-112">Planning a production order for a multilevel item.</span><span class="sxs-lookup"><span data-stu-id="40a1e-112">Planning a production order for a multilevel item.</span></span>  

## <a name="roles"></a><span data-ttu-id="40a1e-113">Roles</span><span class="sxs-lookup"><span data-stu-id="40a1e-113">Roles</span></span>  
 <span data-ttu-id="40a1e-114">This walkthrough demonstrates tasks performed by the following user roles:</span><span class="sxs-lookup"><span data-stu-id="40a1e-114">This walkthrough demonstrates tasks performed by the following user roles:</span></span>  

-   <span data-ttu-id="40a1e-115">Production Planner</span><span class="sxs-lookup"><span data-stu-id="40a1e-115">Production Planner</span></span>  
-   <span data-ttu-id="40a1e-116">Purchasing Agent</span><span class="sxs-lookup"><span data-stu-id="40a1e-116">Purchasing Agent</span></span>  
-   <span data-ttu-id="40a1e-117">Sales Order Processor</span><span class="sxs-lookup"><span data-stu-id="40a1e-117">Sales Order Processor</span></span>  

## <a name="prerequisites"></a><span data-ttu-id="40a1e-118">Prerequisites</span><span class="sxs-lookup"><span data-stu-id="40a1e-118">Prerequisites</span></span>  
 <span data-ttu-id="40a1e-119">Before you begin this walkthrough, you must install the [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="40a1e-119">Before you begin this walkthrough, you must install the [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="40a1e-120">The following modifications must be made to the database:</span><span class="sxs-lookup"><span data-stu-id="40a1e-120">The following modifications must be made to the database:</span></span>  

-   <span data-ttu-id="40a1e-121">Delete all existing sales orders for bicycles.</span><span class="sxs-lookup"><span data-stu-id="40a1e-121">Delete all existing sales orders for bicycles.</span></span>  
-   <span data-ttu-id="40a1e-122">Create one sales order for 10 bicycles at BLUE location.</span><span class="sxs-lookup"><span data-stu-id="40a1e-122">Create one sales order for 10 bicycles at BLUE location.</span></span>  
-   <span data-ttu-id="40a1e-123">Delete all planned and firm planned production orders.</span><span class="sxs-lookup"><span data-stu-id="40a1e-123">Delete all planned and firm planned production orders.</span></span> <span data-ttu-id="40a1e-124">Do not delete started orders with entries that are already posted.</span><span class="sxs-lookup"><span data-stu-id="40a1e-124">Do not delete started orders with entries that are already posted.</span></span>  

 <span data-ttu-id="40a1e-125">As a rule, use the suggested data in this walkthrough because this data has the necessary records.</span><span class="sxs-lookup"><span data-stu-id="40a1e-125">As a rule, use the suggested data in this walkthrough because this data has the necessary records.</span></span>  

## <a name="story"></a><span data-ttu-id="40a1e-126">Story</span><span class="sxs-lookup"><span data-stu-id="40a1e-126">Story</span></span>  
 <span data-ttu-id="40a1e-127">Eduardo, the Production Planner of a small manufacturing company, is about to plan production and purchase orders to fulfill new sales demand.</span><span class="sxs-lookup"><span data-stu-id="40a1e-127">Eduardo, the Production Planner of a small manufacturing company, is about to plan production and purchase orders to fulfill new sales demand.</span></span>  

 <span data-ttu-id="40a1e-128">Because the products have few BOM levels and the flow of orders is relatively low, Eduardo uses the **Order Planning** window to manually create supply orders, one product level at a time.</span><span class="sxs-lookup"><span data-stu-id="40a1e-128">Because the products have few BOM levels and the flow of orders is relatively low, Eduardo uses the **Order Planning** window to manually create supply orders, one product level at a time.</span></span>  

 <span data-ttu-id="40a1e-129">In a more complex manufacturing environment, the planning worksheet is used to plan supply based on item parameters such as rescheduling period, safety lead time, reorder point, and batch calculations of consolidated demand from all product levels.</span><span class="sxs-lookup"><span data-stu-id="40a1e-129">In a more complex manufacturing environment, the planning worksheet is used to plan supply based on item parameters such as rescheduling period, safety lead time, reorder point, and batch calculations of consolidated demand from all product levels.</span></span>  

## <a name="setting-up-the-sample-data"></a><span data-ttu-id="40a1e-130">Setting Up the Sample Data</span><span class="sxs-lookup"><span data-stu-id="40a1e-130">Setting Up the Sample Data</span></span>  
 <span data-ttu-id="40a1e-131">The standard CRONUS demonstration company currently has lots of unplanned demand.</span><span class="sxs-lookup"><span data-stu-id="40a1e-131">The standard CRONUS demonstration company currently has lots of unplanned demand.</span></span> <span data-ttu-id="40a1e-132">During the different planning tasks in this walkthrough, you will have to deviate from the realistic business flow by ignoring demand with close due dates and instead use demand with later due dates.</span><span class="sxs-lookup"><span data-stu-id="40a1e-132">During the different planning tasks in this walkthrough, you will have to deviate from the realistic business flow by ignoring demand with close due dates and instead use demand with later due dates.</span></span>  

## <a name="using-the-order-planning-window"></a><span data-ttu-id="40a1e-133">Using the Order Planning Window</span><span class="sxs-lookup"><span data-stu-id="40a1e-133">Using the Order Planning Window</span></span>  

<!-- 
The **Order Planning** window can be accessed from several different locations on the **Departments** menu in the navigation pane:  

-   Manufacturing, Planning  
-   Sales & Marketing, Order Processing  
-   Purchase, Planning  
-   In addition, you can open this window for a specific production order by choosing **Planning** on the **Navigate** tab in the **Order** group.

-->  

### <a name="to-use-the-order-planning-window"></a><span data-ttu-id="40a1e-134">To use the Order Planning window</span><span class="sxs-lookup"><span data-stu-id="40a1e-134">To use the Order Planning window</span></span>  

1.  <span data-ttu-id="40a1e-135">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Order Planning**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="40a1e-135">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Order Planning**, and then choose the related link.</span></span>  

     <span data-ttu-id="40a1e-136">When the **Order Planning** window first opens, a plan must be calculated to show the new demand since it was last calculated.</span><span class="sxs-lookup"><span data-stu-id="40a1e-136">When the **Order Planning** window first opens, a plan must be calculated to show the new demand since it was last calculated.</span></span>  

2.  <span data-ttu-id="40a1e-137">Choose the **Calculate Plan** action.</span><span class="sxs-lookup"><span data-stu-id="40a1e-137">Choose the **Calculate Plan** action.</span></span>  

     <span data-ttu-id="40a1e-138">The planning system analyses any new demand that has been introduced, such as new sales, changed sales, or production orders.</span><span class="sxs-lookup"><span data-stu-id="40a1e-138">The planning system analyzes any new demand that has been introduced, such as new sales, changed sales, or production orders.</span></span>  

     <span data-ttu-id="40a1e-139">Based on total availability, the quantity needed for each demand line is calculated.</span><span class="sxs-lookup"><span data-stu-id="40a1e-139">Based on total availability, the quantity needed for each demand line is calculated.</span></span> <span data-ttu-id="40a1e-140">This calculation is performed order-by-order.</span><span class="sxs-lookup"><span data-stu-id="40a1e-140">This calculation is performed order-by-order.</span></span> <span data-ttu-id="40a1e-141">This means that the order which includes the demand line with the earliest due date or shipment date will be calculated first.</span><span class="sxs-lookup"><span data-stu-id="40a1e-141">This means that the order which includes the demand line with the earliest due date or shipment date will be calculated first.</span></span> <span data-ttu-id="40a1e-142">After that, additional demand lines will be calculated in the same order, regardless of the due date or shipment date.</span><span class="sxs-lookup"><span data-stu-id="40a1e-142">After that, additional demand lines will be calculated in the same order, regardless of the due date or shipment date.</span></span>  

3.  <span data-ttu-id="40a1e-143">Be sure that the **Order Planning** window is maximised and that column fields are resized to show all the default field names.</span><span class="sxs-lookup"><span data-stu-id="40a1e-143">Be sure that the **Order Planning** window is maximized and that column fields are resized to show all the default field names.</span></span>  

     <span data-ttu-id="40a1e-144">When the calculation is completed, the window displays all unfulfilled demand as collapsed order header lines sorted by earliest demand date.</span><span class="sxs-lookup"><span data-stu-id="40a1e-144">When the calculation is completed, the window displays all unfulfilled demand as collapsed order header lines sorted by earliest demand date.</span></span>  

     <span data-ttu-id="40a1e-145">Notice that CRONUS has several orders with unfulfilled demand.</span><span class="sxs-lookup"><span data-stu-id="40a1e-145">Notice that CRONUS has several orders with unfulfilled demand.</span></span> <span data-ttu-id="40a1e-146">Each bold planning line represents an order, sales order, or production order, including at least one order line with insufficient availability.</span><span class="sxs-lookup"><span data-stu-id="40a1e-146">Each bold planning line represents an order, sales order, or production order, including at least one order line with insufficient availability.</span></span>  

4.  <span data-ttu-id="40a1e-147">In the **Show Demand As** field, select the **All Demand** filter.</span><span class="sxs-lookup"><span data-stu-id="40a1e-147">In the **Show Demand As** field, select the **All Demand** filter.</span></span>  

     <span data-ttu-id="40a1e-148">With the **Demand Type** field, you can choose which order types that you want to display.</span><span class="sxs-lookup"><span data-stu-id="40a1e-148">With the **Demand Type** field, you can choose which order types that you want to display.</span></span>  

     <span data-ttu-id="40a1e-149">Orders that do not have availability problems are not shown.</span><span class="sxs-lookup"><span data-stu-id="40a1e-149">Orders that do not have availability problems are not shown.</span></span> <span data-ttu-id="40a1e-150">If no orders exist when a plan is calculated, a message will display and no planning lines will appear.</span><span class="sxs-lookup"><span data-stu-id="40a1e-150">If no orders exist when a plan is calculated, a message will display and no planning lines will appear.</span></span>  

## <a name="planning-a-purchase-order-to-fulfill-component-demand"></a><span data-ttu-id="40a1e-151">Planning a Purchase Order to Fulfill Component Demand</span><span class="sxs-lookup"><span data-stu-id="40a1e-151">Planning a Purchase Order to Fulfill Component Demand</span></span>  
 <span data-ttu-id="40a1e-152">In this procedure, you create a purchase order for needed manufacturing components.</span><span class="sxs-lookup"><span data-stu-id="40a1e-152">In this procedure, you create a purchase order for needed manufacturing components.</span></span>  

### <a name="to-plan-a-purchase-order-to-fulfill-component-need-in-production"></a><span data-ttu-id="40a1e-153">To plan a purchase order to fulfill component need in production</span><span class="sxs-lookup"><span data-stu-id="40a1e-153">To plan a purchase order to fulfill component need in production</span></span>  

1.  <span data-ttu-id="40a1e-154">Expand the first line (choose the + symbol).</span><span class="sxs-lookup"><span data-stu-id="40a1e-154">Expand the first line (choose the + symbol).</span></span>  
2.  <span data-ttu-id="40a1e-155">Choose the first demand line, with item **LSU-15**, and then choose the **Show Document** action.</span><span class="sxs-lookup"><span data-stu-id="40a1e-155">Choose the first demand line, with item **LSU-15**, and then choose the **Show Document** action.</span></span>  
3.  <span data-ttu-id="40a1e-156">Close the opened production order to return to the **Order Planning** window.</span><span class="sxs-lookup"><span data-stu-id="40a1e-156">Close the opened production order to return to the **Order Planning** window.</span></span>  
4.  <span data-ttu-id="40a1e-157">In the **Replenishment System** field, select **Purchase**.</span><span class="sxs-lookup"><span data-stu-id="40a1e-157">In the **Replenishment System** field, select **Purchase**.</span></span>  

     <span data-ttu-id="40a1e-158">The default value is from the item card, or SKU card, but you can change it to one of the following options:</span><span class="sxs-lookup"><span data-stu-id="40a1e-158">The default value is from the item card, or SKU card, but you can change it to one of the following options:</span></span>  

    -   <span data-ttu-id="40a1e-159">**Purchase** – To create a purchase order.</span><span class="sxs-lookup"><span data-stu-id="40a1e-159">**Purchase** – To create a purchase order.</span></span>  
    -   <span data-ttu-id="40a1e-160">**Transfer** – To create a transfer order.</span><span class="sxs-lookup"><span data-stu-id="40a1e-160">**Transfer** – To create a transfer order.</span></span>  
    -   <span data-ttu-id="40a1e-161">**Prod. Order** – To create a production order.</span><span class="sxs-lookup"><span data-stu-id="40a1e-161">**Prod. Order** – To create a production order.</span></span>  

5.  <span data-ttu-id="40a1e-162">In the **Supply From** field, select one of the following options according to the selected replenishment system:</span><span class="sxs-lookup"><span data-stu-id="40a1e-162">In the **Supply From** field, select one of the following options according to the selected replenishment system:</span></span>  

    -   <span data-ttu-id="40a1e-163">**Vendor** – For purchases</span><span class="sxs-lookup"><span data-stu-id="40a1e-163">**Vendor** – For purchases</span></span>  
    -   <span data-ttu-id="40a1e-164">**Location** – For transfers</span><span class="sxs-lookup"><span data-stu-id="40a1e-164">**Location** – For transfers</span></span>  

     <span data-ttu-id="40a1e-165">If the field is not filled in, an error message will display when you try to create the supply orders.</span><span class="sxs-lookup"><span data-stu-id="40a1e-165">If the field is not filled in, an error message will display when you try to create the supply orders.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="40a1e-166">If the components have a default vendor number set up on the item cards, the lines will be preset.</span><span class="sxs-lookup"><span data-stu-id="40a1e-166">If the components have a default vendor number set up on the item cards, the lines will be preset.</span></span>  

6.  <span data-ttu-id="40a1e-167">Choose the **Supply From**  field.</span><span class="sxs-lookup"><span data-stu-id="40a1e-167">Choose the **Supply From**  field.</span></span>  
7.  <span data-ttu-id="40a1e-168">In the **Item Vendor Catalogue** window, choose the **New** action, and then select vendor **30000**.</span><span class="sxs-lookup"><span data-stu-id="40a1e-168">In the **Item Vendor Catalogue** window, choose the **New** action, and then select vendor **30000**.</span></span>  
8.  <span data-ttu-id="40a1e-169">Choose the **OK** button to return to the **Order Planning** window.</span><span class="sxs-lookup"><span data-stu-id="40a1e-169">Choose the **OK** button to return to the **Order Planning** window.</span></span>  
9. <span data-ttu-id="40a1e-170">Copy vendor **30000** to the other lines for loudspeaker components on this production order.</span><span class="sxs-lookup"><span data-stu-id="40a1e-170">Copy vendor **30000** to the other lines for loudspeaker components on this production order.</span></span>  

     <span data-ttu-id="40a1e-171">You are now ready to create a purchase order.</span><span class="sxs-lookup"><span data-stu-id="40a1e-171">You are now ready to create a purchase order.</span></span>  

10. <span data-ttu-id="40a1e-172">Choose the **Make Orders** action.</span><span class="sxs-lookup"><span data-stu-id="40a1e-172">Choose the **Make Orders** action.</span></span> <span data-ttu-id="40a1e-173">The **Make Supply Orders** window opens.</span><span class="sxs-lookup"><span data-stu-id="40a1e-173">The **Make Supply Orders** window opens.</span></span>  
11. <span data-ttu-id="40a1e-174">On the **Order Planning** FastTab, in the **Make Orders for** field, choose the **Active Order** option.</span><span class="sxs-lookup"><span data-stu-id="40a1e-174">On the **Order Planning** FastTab, in the **Make Orders for** field, choose the **Active Order** option.</span></span>  
12. <span data-ttu-id="40a1e-175">On the **Options** FastTab, in the **Create Purchase Order** field, choose the **Make Purch. Order** option.</span><span class="sxs-lookup"><span data-stu-id="40a1e-175">On the **Options** FastTab, in the **Create Purchase Order** field, choose the **Make Purch. Order** option.</span></span>  
13. <span data-ttu-id="40a1e-176">Choose the **OK** button to create purchase orders for all the components of the order.</span><span class="sxs-lookup"><span data-stu-id="40a1e-176">Choose the **OK** button to create purchase orders for all the components of the order.</span></span>  

     <span data-ttu-id="40a1e-177">The purchase orders are now created and saved as the last orders in the list of purchase orders.</span><span class="sxs-lookup"><span data-stu-id="40a1e-177">The purchase orders are now created and saved as the last orders in the list of purchase orders.</span></span>  

## <a name="planning-a-transfer-order-to-fulfill-sales-demand"></a><span data-ttu-id="40a1e-178">Planning a Transfer Order to Fulfill Sales Demand</span><span class="sxs-lookup"><span data-stu-id="40a1e-178">Planning a Transfer Order to Fulfill Sales Demand</span></span>  
 <span data-ttu-id="40a1e-179">In this procedure, you will plan for demand from a sales order.</span><span class="sxs-lookup"><span data-stu-id="40a1e-179">In this procedure, you will plan for demand from a sales order.</span></span> <span data-ttu-id="40a1e-180">Demand lines represent sales lines and not component lines, as in production demand.</span><span class="sxs-lookup"><span data-stu-id="40a1e-180">Demand lines represent sales lines and not component lines, as in production demand.</span></span>  

### <a name="to-plan-a-transfer-order-to-fulfill-sales-demand"></a><span data-ttu-id="40a1e-181">To plan a transfer order to fulfill sales demand</span><span class="sxs-lookup"><span data-stu-id="40a1e-181">To plan a transfer order to fulfill sales demand</span></span>  

1.  <span data-ttu-id="40a1e-182">Move the pointer to the planning line for order **2008**.</span><span class="sxs-lookup"><span data-stu-id="40a1e-182">Move the pointer to the planning line for order **2008**.</span></span>  
2.  <span data-ttu-id="40a1e-183">Expand the line and move the pointer to the demand line.</span><span class="sxs-lookup"><span data-stu-id="40a1e-183">Expand the line and move the pointer to the demand line.</span></span>  

     <span data-ttu-id="40a1e-184">Sales order **2008** is for ten loudspeakers, item **LS-120**, ordered by John Haddock Insurance Co.</span><span class="sxs-lookup"><span data-stu-id="40a1e-184">Sales order **2008** is for ten loudspeakers, item **LS-120**, ordered by John Haddock Insurance Co.</span></span>  

     <span data-ttu-id="40a1e-185">The item’s defined replenishment system and default vendor will display.</span><span class="sxs-lookup"><span data-stu-id="40a1e-185">The item’s defined replenishment system and default vendor will display.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="40a1e-186">At the bottom of the window, there are four information fields.</span><span class="sxs-lookup"><span data-stu-id="40a1e-186">At the bottom of the window, there are four information fields.</span></span> <span data-ttu-id="40a1e-187">In the **Earliest Date Available** field, the ten pieces that are needed will be available, on an inbound supply order, nine days later than the current due date.</span><span class="sxs-lookup"><span data-stu-id="40a1e-187">In the **Earliest Date Available** field, the ten pieces that are needed will be available, on an inbound supply order, nine days later than the current due date.</span></span> <span data-ttu-id="40a1e-188">If this is too late for the customer, the **Available for Transfer** field shows 13 pieces of the item at another location.</span><span class="sxs-lookup"><span data-stu-id="40a1e-188">If this is too late for the customer, the **Available for Transfer** field shows 13 pieces of the item at another location.</span></span> <span data-ttu-id="40a1e-189">You will want to plan for this stock.</span><span class="sxs-lookup"><span data-stu-id="40a1e-189">You will want to plan for this stock.</span></span>  

3.  <span data-ttu-id="40a1e-190">Choose the **Available for Transfer** field to open the **Get Alternative Supply** window.</span><span class="sxs-lookup"><span data-stu-id="40a1e-190">Choose the **Available for Transfer** field to open the **Get Alternative Supply** window.</span></span>  
4.  <span data-ttu-id="40a1e-191">Choose the **OK** button to book the ten items that are available.</span><span class="sxs-lookup"><span data-stu-id="40a1e-191">Choose the **OK** button to book the ten items that are available.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="40a1e-192">In the demand line, the suggested purchase has been exchanged with a transfer from GREEN location.</span><span class="sxs-lookup"><span data-stu-id="40a1e-192">In the demand line, the suggested purchase has been exchanged with a transfer from GREEN location.</span></span> <span data-ttu-id="40a1e-193">The **Make Orders** function creates a transfer order from GREEN to the demanded location.</span><span class="sxs-lookup"><span data-stu-id="40a1e-193">The **Make Orders** function creates a transfer order from GREEN to the demanded location.</span></span> <span data-ttu-id="40a1e-194">The **Substitutes Exists** field works in the same way.</span><span class="sxs-lookup"><span data-stu-id="40a1e-194">The **Substitutes Exists** field works in the same way.</span></span>  

5.  <span data-ttu-id="40a1e-195">Choose the **Make Orders** action.</span><span class="sxs-lookup"><span data-stu-id="40a1e-195">Choose the **Make Orders** action.</span></span> <span data-ttu-id="40a1e-196">The **Make Supply Orders** window opens.</span><span class="sxs-lookup"><span data-stu-id="40a1e-196">The **Make Supply Orders** window opens.</span></span>  
6.  <span data-ttu-id="40a1e-197">On the **Order Planning** FastTab, in the **Make Orders for** field, choose the **The Active Order** option.</span><span class="sxs-lookup"><span data-stu-id="40a1e-197">On the **Order Planning** FastTab, in the **Make Orders for** field, choose the **The Active Order** option.</span></span>  
7.  <span data-ttu-id="40a1e-198">On the **Options** FastTab, in the **Create Transfer Order** field, select the **Make Trans. Orders** option.</span><span class="sxs-lookup"><span data-stu-id="40a1e-198">On the **Options** FastTab, in the **Create Transfer Order** field, select the **Make Trans. Orders** option.</span></span>  
8.  <span data-ttu-id="40a1e-199">Choose the **OK** button to create the transfer order to supply the sales order.</span><span class="sxs-lookup"><span data-stu-id="40a1e-199">Choose the **OK** button to create the transfer order to supply the sales order.</span></span>  

     <span data-ttu-id="40a1e-200">The transfer order is now created and saved in the list as the last order in the list of open transfer orders.</span><span class="sxs-lookup"><span data-stu-id="40a1e-200">The transfer order is now created and saved in the list as the last order in the list of open transfer orders.</span></span>  

## <a name="planning-a-multilevel-production-order-to-fulfill-sales-demand"></a><span data-ttu-id="40a1e-201">Planning a Multilevel Production Order to Fulfill Sales Demand</span><span class="sxs-lookup"><span data-stu-id="40a1e-201">Planning a Multilevel Production Order to Fulfill Sales Demand</span></span>  
 <span data-ttu-id="40a1e-202">In this procedure, you will plan to fulfill sales demand for a produced item with multiple product levels, each creating dependent production demand.</span><span class="sxs-lookup"><span data-stu-id="40a1e-202">In this procedure, you will plan to fulfill sales demand for a produced item with multiple product levels, each creating dependent production demand.</span></span>  

### <a name="to-plan-multilevel-production-to-fulfill-sales-demand"></a><span data-ttu-id="40a1e-203">To plan multilevel production to fulfill sales demand</span><span class="sxs-lookup"><span data-stu-id="40a1e-203">To plan multilevel production to fulfill sales demand</span></span>  

1.  <span data-ttu-id="40a1e-204">Select the planning line with sales demand for order **1001**, created earlier as prerequisite data.</span><span class="sxs-lookup"><span data-stu-id="40a1e-204">Select the planning line with sales demand for order **1001**, created earlier as prerequisite data.</span></span>  

     <span data-ttu-id="40a1e-205">This demand is a sales line, but the item has a defined replenishment system of **Prod. Order**.</span><span class="sxs-lookup"><span data-stu-id="40a1e-205">This demand is a sales line, but the item has a defined replenishment system of **Prod. Order**.</span></span> <span data-ttu-id="40a1e-206">Proceed to add an extra bell to the component need of each bicycle.</span><span class="sxs-lookup"><span data-stu-id="40a1e-206">Proceed to add an extra bell to the component need of each bicycle.</span></span>  

2.  <span data-ttu-id="40a1e-207">Choose the **Components** action to open the **Planning Components** window.</span><span class="sxs-lookup"><span data-stu-id="40a1e-207">Choose the **Components** action to open the **Planning Components** window.</span></span>  
3.  <span data-ttu-id="40a1e-208">On the line with the Bell item, change the **Quantity per** field from **1** to **2**.</span><span class="sxs-lookup"><span data-stu-id="40a1e-208">On the line with the Bell item, change the **Quantity per** field from **1** to **2**.</span></span>  
4.  <span data-ttu-id="40a1e-209">In the **Order Planning** window, consider your planning alternatives.</span><span class="sxs-lookup"><span data-stu-id="40a1e-209">In the **Order Planning** window, consider your planning alternatives.</span></span> <span data-ttu-id="40a1e-210">In this case, you have no alternative means of supply, no transfer, substitute, or later delivery.</span><span class="sxs-lookup"><span data-stu-id="40a1e-210">In this case, you have no alternative means of supply, no transfer, substitute, or later delivery.</span></span> <span data-ttu-id="40a1e-211">You must create the suggested supply order, a production order.</span><span class="sxs-lookup"><span data-stu-id="40a1e-211">You must create the suggested supply order, a production order.</span></span>  
5.  <span data-ttu-id="40a1e-212">Choose the **Make Orders** action to create the production order.</span><span class="sxs-lookup"><span data-stu-id="40a1e-212">Choose the **Make Orders** action to create the production order.</span></span>  

     <span data-ttu-id="40a1e-213">In the **Order Planning** window, notice that the planning line for sales order **1001** no longer exists and that the initial sales demand has been covered.</span><span class="sxs-lookup"><span data-stu-id="40a1e-213">In the **Order Planning** window, notice that the planning line for sales order **1001** no longer exists and that the initial sales demand has been covered.</span></span>  

6.  <span data-ttu-id="40a1e-214">Close the **Order Planning** window.</span><span class="sxs-lookup"><span data-stu-id="40a1e-214">Close the **Order Planning** window.</span></span>  

     <span data-ttu-id="40a1e-215">Now, you could choose to stay in this view and complete all the planning tasks.</span><span class="sxs-lookup"><span data-stu-id="40a1e-215">Now, you could choose to stay in this view and complete all the planning tasks.</span></span> <span data-ttu-id="40a1e-216">Instead, you will now take on the Production Planner role by going to the production order that you just created and access the **Order Planning** window.</span><span class="sxs-lookup"><span data-stu-id="40a1e-216">Instead, you will now take on the Production Planner role by going to the production order that you just created and access the **Order Planning** window.</span></span>  

 <span data-ttu-id="40a1e-217">As a production planner you now must plan a specific production order.</span><span class="sxs-lookup"><span data-stu-id="40a1e-217">As a production planner you now must plan a specific production order.</span></span>  

### <a name="to-plan-a-specific-production-order"></a><span data-ttu-id="40a1e-218">To plan a specific production order</span><span class="sxs-lookup"><span data-stu-id="40a1e-218">To plan a specific production order</span></span>  

1.  <span data-ttu-id="40a1e-219">Open the production order **101001**, for ten bicycles, that you just created by using the **Make Orders** function.</span><span class="sxs-lookup"><span data-stu-id="40a1e-219">Open the production order **101001**, for ten bicycles, that you just created by using the **Make Orders** function.</span></span>  
2.  <span data-ttu-id="40a1e-220">Open the **Prod. Order Components** window to check that the extra bell is reflected on the production order.</span><span class="sxs-lookup"><span data-stu-id="40a1e-220">Open the **Prod. Order Components** window to check that the extra bell is reflected on the production order.</span></span>  
3.  <span data-ttu-id="40a1e-221">Choose the **Planning** action.</span><span class="sxs-lookup"><span data-stu-id="40a1e-221">Choose the **Planning** action.</span></span>  

     <span data-ttu-id="40a1e-222">The **Order Planning** window opens in a view that is always filtered on the specific production demand.</span><span class="sxs-lookup"><span data-stu-id="40a1e-222">The **Order Planning** window opens in a view that is always filtered on the specific production demand.</span></span> <span data-ttu-id="40a1e-223">Sales demand is not displayed.</span><span class="sxs-lookup"><span data-stu-id="40a1e-223">Sales demand is not displayed.</span></span> <span data-ttu-id="40a1e-224">You must calculate a plan before you can see any additional demand.</span><span class="sxs-lookup"><span data-stu-id="40a1e-224">You must calculate a plan before you can see any additional demand.</span></span>  

4.  <span data-ttu-id="40a1e-225">Choose the **Calculate Plan** action.</span><span class="sxs-lookup"><span data-stu-id="40a1e-225">Choose the **Calculate Plan** action.</span></span>  

     <span data-ttu-id="40a1e-226">Notice that four new production orders appear as unplanned production demand derived from order **101001**.</span><span class="sxs-lookup"><span data-stu-id="40a1e-226">Notice that four new production orders appear as unplanned production demand derived from order **101001**.</span></span> <span data-ttu-id="40a1e-227">The new lines represent new production demand from the subassemblies that must be created to produce the order.</span><span class="sxs-lookup"><span data-stu-id="40a1e-227">The new lines represent new production demand from the subassemblies that must be created to produce the order.</span></span>  

5.  <span data-ttu-id="40a1e-228">Choose the **Expand All** action to get an overview of all the production demand for the production orders.</span><span class="sxs-lookup"><span data-stu-id="40a1e-228">Choose the **Expand All** action to get an overview of all the production demand for the production orders.</span></span>  

     <span data-ttu-id="40a1e-229">To provide additional information about the demand lines, you may want to add the **Demand Quantity** and **Demand Qty. Available** fields to your view.</span><span class="sxs-lookup"><span data-stu-id="40a1e-229">To provide additional information about the demand lines, you may want to add the **Demand Quantity** and **Demand Qty. Available** fields to your view.</span></span>  

     <span data-ttu-id="40a1e-230">Now you must supply ten of each component.</span><span class="sxs-lookup"><span data-stu-id="40a1e-230">Now you must supply ten of each component.</span></span>  

     <span data-ttu-id="40a1e-231">Note that four of the demand lines have replenishment system Prod. Order.</span><span class="sxs-lookup"><span data-stu-id="40a1e-231">Note that four of the demand lines have replenishment system Prod. Order.</span></span> <span data-ttu-id="40a1e-232">These four subassemblies represent the second product level of the bicycle.</span><span class="sxs-lookup"><span data-stu-id="40a1e-232">These four subassemblies represent the second product level of the bicycle.</span></span>  

     <span data-ttu-id="40a1e-233">The default replenishment settings are already filled in and you can proceed to make orders.</span><span class="sxs-lookup"><span data-stu-id="40a1e-233">The default replenishment settings are already filled in and you can proceed to make orders.</span></span>  

6.  <span data-ttu-id="40a1e-234">Choose the **Make Orders** action.</span><span class="sxs-lookup"><span data-stu-id="40a1e-234">Choose the **Make Orders** action.</span></span>  

     <span data-ttu-id="40a1e-235">Before you choose the **OK** button, notice the text on the **Order Planning** FastTab.</span><span class="sxs-lookup"><span data-stu-id="40a1e-235">Before you choose the **OK** button, notice the text on the **Order Planning** FastTab.</span></span> <span data-ttu-id="40a1e-236">This text is important because you know that the bicycle has several produced components, subassemblies, in its product structure that might be in demand when you create this production order.</span><span class="sxs-lookup"><span data-stu-id="40a1e-236">This text is important because you know that the bicycle has several produced components, subassemblies, in its product structure that might be in demand when you create this production order.</span></span>  

7.  <span data-ttu-id="40a1e-237">In the **Make Supply Order** window, in the **Make Orders for** field, choose the **All Lines** option, and then choose the **OK** button to create production orders for the second product level of the order.</span><span class="sxs-lookup"><span data-stu-id="40a1e-237">In the **Make Supply Order** window, in the **Make Orders for** field, choose the **All Lines** option, and then choose the **OK** button to create production orders for the second product level of the order.</span></span>  

     <span data-ttu-id="40a1e-238">Note that the top-level production demand for production order 101001 no longer exists.</span><span class="sxs-lookup"><span data-stu-id="40a1e-238">Note that the top-level production demand for production order 101001 no longer exists.</span></span> <span data-ttu-id="40a1e-239">This means that the initial production demand for subassemblies has been planned for.</span><span class="sxs-lookup"><span data-stu-id="40a1e-239">This means that the initial production demand for subassemblies has been planned for.</span></span>  

     <span data-ttu-id="40a1e-240">In the **Order Planning** window, you calculate a plan again in order to plan the bicycle structure.</span><span class="sxs-lookup"><span data-stu-id="40a1e-240">In the **Order Planning** window, you calculate a plan again in order to plan the bicycle structure.</span></span>  

8.  <span data-ttu-id="40a1e-241">Choose the **Calculate Plan** action to recalculate the plan as instructed by the embedded Help text.</span><span class="sxs-lookup"><span data-stu-id="40a1e-241">Choose the **Calculate Plan** action to recalculate the plan as instructed by the embedded Help text.</span></span>  

     <span data-ttu-id="40a1e-242">The two new lines represent additional production demand derived from the subassemblies planned in the previous steps.</span><span class="sxs-lookup"><span data-stu-id="40a1e-242">The two new lines represent additional production demand derived from the subassemblies planned in the previous steps.</span></span> <span data-ttu-id="40a1e-243">It is suggested that you make two production orders to supply the wheel hubs, one for 10 front hubs and one for 10 back hubs.</span><span class="sxs-lookup"><span data-stu-id="40a1e-243">It is suggested that you make two production orders to supply the wheel hubs, one for 10 front hubs and one for 10 back hubs.</span></span>  

9. <span data-ttu-id="40a1e-244">Choose the **Expand All** action to get an overview of all the demand for the two production orders.</span><span class="sxs-lookup"><span data-stu-id="40a1e-244">Choose the **Expand All** action to get an overview of all the demand for the two production orders.</span></span>  

     <span data-ttu-id="40a1e-245">The suggested supply plan indicates that a total of four purchase orders will be created for the components.</span><span class="sxs-lookup"><span data-stu-id="40a1e-245">The suggested supply plan indicates that a total of four purchase orders will be created for the components.</span></span> <span data-ttu-id="40a1e-246">You decide to make the proposed orders.</span><span class="sxs-lookup"><span data-stu-id="40a1e-246">You decide to make the proposed orders.</span></span>  

10. <span data-ttu-id="40a1e-247">Choose the **Make Orders** action.</span><span class="sxs-lookup"><span data-stu-id="40a1e-247">Choose the **Make Orders** action.</span></span>  
11. <span data-ttu-id="40a1e-248">In the **Make Orders for** field, select the **All Lines** option, and then choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="40a1e-248">In the **Make Orders for** field, select the **All Lines** option, and then choose the **OK** button.</span></span> <span data-ttu-id="40a1e-249">Check if additional demand exists for the production of the parent item, the bicycle, which is being sold on sales order 1001.</span><span class="sxs-lookup"><span data-stu-id="40a1e-249">Check if additional demand exists for the production of the parent item, the bicycle, which is being sold on sales order 1001.</span></span>  
12. <span data-ttu-id="40a1e-250">Choose the **Calculate Plan** action.</span><span class="sxs-lookup"><span data-stu-id="40a1e-250">Choose the **Calculate Plan** action.</span></span>  

     <span data-ttu-id="40a1e-251">The message indicates that all required items are now supplied.</span><span class="sxs-lookup"><span data-stu-id="40a1e-251">The message indicates that all required items are now supplied.</span></span> <span data-ttu-id="40a1e-252">Verify the firm planned production orders that are created.</span><span class="sxs-lookup"><span data-stu-id="40a1e-252">Verify the firm planned production orders that are created.</span></span>  

13. <span data-ttu-id="40a1e-253">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Firm Planned Prod. Orders**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="40a1e-253">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Firm Planned Prod. Orders**, and then choose the related link.</span></span>  

     <span data-ttu-id="40a1e-254">In the **Firm Planned Prod. Orders** window review how start times and end times of individual orders are scheduled according to the product structure.</span><span class="sxs-lookup"><span data-stu-id="40a1e-254">In the **Firm Planned Prod. Orders** window review how start times and end times of individual orders are scheduled according to the product structure.</span></span> <span data-ttu-id="40a1e-255">The lowest-level components are produced first.</span><span class="sxs-lookup"><span data-stu-id="40a1e-255">The lowest-level components are produced first.</span></span> <span data-ttu-id="40a1e-256">Therefore, you must plan multilevel orders as demonstrated in this planning workflow.</span><span class="sxs-lookup"><span data-stu-id="40a1e-256">Therefore, you must plan multilevel orders as demonstrated in this planning workflow.</span></span>  

## <a name="see-also"></a><span data-ttu-id="40a1e-257">See Also</span><span class="sxs-lookup"><span data-stu-id="40a1e-257">See Also</span></span>  
 <span data-ttu-id="40a1e-258">[Business Process Walkthroughs](walkthrough-business-process-walkthroughs.md) </span><span class="sxs-lookup"><span data-stu-id="40a1e-258">[Business Process Walkthroughs](walkthrough-business-process-walkthroughs.md) </span></span>  
 [<span data-ttu-id="40a1e-259">Walkthrough: Planning Supplies Automatically</span><span class="sxs-lookup"><span data-stu-id="40a1e-259">Walkthrough: Planning Supplies Automatically</span></span>](walkthrough-planning-supplies-automatically.md)

