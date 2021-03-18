---
title: Walkthrough - Planning Supplies Manually | Microsoft Docs
description: This walkthrough demonstrates the process of planning supply orders to fulfill new demand. You can initiate supply planning at fixed intervals, for example, every morning or every Monday, or when you are notified by sales or production, depending on the type of demand.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 604a783f292b04c2609b8415d6b2ec6287f5cfcb
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "5379818"
---
# <a name="walkthrough-planning-supplies-manually"></a><span data-ttu-id="aea04-104">Walkthrough: Planning Supplies Manually</span><span class="sxs-lookup"><span data-stu-id="aea04-104">Walkthrough: Planning Supplies Manually</span></span>

[!INCLUDE[complete_sample_data](includes/complete_sample_data.md)]  

<span data-ttu-id="aea04-105">This walkthrough demonstrates the process of planning supply orders to fulfill new demand.</span><span class="sxs-lookup"><span data-stu-id="aea04-105">This walkthrough demonstrates the process of planning supply orders to fulfill new demand.</span></span> <span data-ttu-id="aea04-106">You can initiate supply planning at fixed intervals, for example, every morning or every Monday, or when you are notified by sales or production, depending on the type of demand.</span><span class="sxs-lookup"><span data-stu-id="aea04-106">You can initiate supply planning at fixed intervals, for example, every morning or every Monday, or when you are notified by sales or production, depending on the type of demand.</span></span> <span data-ttu-id="aea04-107">In this walkthrough you will use the **Order Planning** page, a simple supply planning tool that is based on manual decision-making instead of parameter-based automatic planning.</span><span class="sxs-lookup"><span data-stu-id="aea04-107">In this walkthrough you will use the **Order Planning** page, a simple supply planning tool that is based on manual decision-making instead of parameter-based automatic planning.</span></span>  

## <a name="about-this-walkthrough"></a><span data-ttu-id="aea04-108">About This Walkthrough</span><span class="sxs-lookup"><span data-stu-id="aea04-108">About This Walkthrough</span></span>  
 <span data-ttu-id="aea04-109">This walkthrough illustrates the following tasks:</span><span class="sxs-lookup"><span data-stu-id="aea04-109">This walkthrough illustrates the following tasks:</span></span>  

-   <span data-ttu-id="aea04-110">Planning a purchase order for manufacturing components.</span><span class="sxs-lookup"><span data-stu-id="aea04-110">Planning a purchase order for manufacturing components.</span></span>  
-   <span data-ttu-id="aea04-111">Planning a transfer order to fulfill sales demand.</span><span class="sxs-lookup"><span data-stu-id="aea04-111">Planning a transfer order to fulfill sales demand.</span></span>  
-   <span data-ttu-id="aea04-112">Planning a production order for a multilevel item.</span><span class="sxs-lookup"><span data-stu-id="aea04-112">Planning a production order for a multilevel item.</span></span>  

## <a name="roles"></a><span data-ttu-id="aea04-113">Roles</span><span class="sxs-lookup"><span data-stu-id="aea04-113">Roles</span></span>  
 <span data-ttu-id="aea04-114">This walkthrough demonstrates tasks performed by the following user roles:</span><span class="sxs-lookup"><span data-stu-id="aea04-114">This walkthrough demonstrates tasks performed by the following user roles:</span></span>  

-   <span data-ttu-id="aea04-115">Production Planner</span><span class="sxs-lookup"><span data-stu-id="aea04-115">Production Planner</span></span>  
-   <span data-ttu-id="aea04-116">Purchasing Agent</span><span class="sxs-lookup"><span data-stu-id="aea04-116">Purchasing Agent</span></span>  
-   <span data-ttu-id="aea04-117">Sales Order Processor</span><span class="sxs-lookup"><span data-stu-id="aea04-117">Sales Order Processor</span></span>  

## <a name="prerequisites"></a><span data-ttu-id="aea04-118">Prerequisites</span><span class="sxs-lookup"><span data-stu-id="aea04-118">Prerequisites</span></span>  
 <span data-ttu-id="aea04-119">Before you begin this walkthrough, you must install the [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="aea04-119">Before you begin this walkthrough, you must install the [!INCLUDE[prod_short](includes/prod_short.md)].</span></span> <span data-ttu-id="aea04-120">The following modifications must be made to the database:</span><span class="sxs-lookup"><span data-stu-id="aea04-120">The following modifications must be made to the database:</span></span>  

-   <span data-ttu-id="aea04-121">Delete all existing sales orders for bicycles.</span><span class="sxs-lookup"><span data-stu-id="aea04-121">Delete all existing sales orders for bicycles.</span></span>  
-   <span data-ttu-id="aea04-122">Create one sales order for 10 bicycles at EAST location.</span><span class="sxs-lookup"><span data-stu-id="aea04-122">Create one sales order for 10 bicycles at EAST location.</span></span>  
-   <span data-ttu-id="aea04-123">Delete all planned and firm planned production orders.</span><span class="sxs-lookup"><span data-stu-id="aea04-123">Delete all planned and firm planned production orders.</span></span> <span data-ttu-id="aea04-124">Do not delete started orders with entries that are already posted.</span><span class="sxs-lookup"><span data-stu-id="aea04-124">Do not delete started orders with entries that are already posted.</span></span>  

 <span data-ttu-id="aea04-125">As a rule, use the suggested data in this walkthrough because this data has the necessary records.</span><span class="sxs-lookup"><span data-stu-id="aea04-125">As a rule, use the suggested data in this walkthrough because this data has the necessary records.</span></span>  

## <a name="story"></a><span data-ttu-id="aea04-126">Story</span><span class="sxs-lookup"><span data-stu-id="aea04-126">Story</span></span>  
 <span data-ttu-id="aea04-127">Eduardo, the Production Planner of a small manufacturing company, is about to plan production and purchase orders to fulfill new sales demand.</span><span class="sxs-lookup"><span data-stu-id="aea04-127">Eduardo, the Production Planner of a small manufacturing company, is about to plan production and purchase orders to fulfill new sales demand.</span></span>  

 <span data-ttu-id="aea04-128">Because the products have few BOM levels and the flow of orders is relatively low, Eduardo uses the **Order Planning** page to manually create supply orders, one product level at a time.</span><span class="sxs-lookup"><span data-stu-id="aea04-128">Because the products have few BOM levels and the flow of orders is relatively low, Eduardo uses the **Order Planning** page to manually create supply orders, one product level at a time.</span></span>  

 <span data-ttu-id="aea04-129">In a more complex manufacturing environment, the planning worksheet is used to plan supply based on item parameters such as rescheduling period, safety lead time, reorder point, and batch calculations of consolidated demand from all product levels.</span><span class="sxs-lookup"><span data-stu-id="aea04-129">In a more complex manufacturing environment, the planning worksheet is used to plan supply based on item parameters such as rescheduling period, safety lead time, reorder point, and batch calculations of consolidated demand from all product levels.</span></span>  

## <a name="setting-up-the-sample-data"></a><span data-ttu-id="aea04-130">Setting Up the Sample Data</span><span class="sxs-lookup"><span data-stu-id="aea04-130">Setting Up the Sample Data</span></span>  
 <span data-ttu-id="aea04-131">The standard CRONUS demonstration company currently has lots of unplanned demand.</span><span class="sxs-lookup"><span data-stu-id="aea04-131">The standard CRONUS demonstration company currently has lots of unplanned demand.</span></span> <span data-ttu-id="aea04-132">During the different planning tasks in this walkthrough, you will have to deviate from the realistic business flow by ignoring demand with close due dates and instead use demand with later due dates.</span><span class="sxs-lookup"><span data-stu-id="aea04-132">During the different planning tasks in this walkthrough, you will have to deviate from the realistic business flow by ignoring demand with close due dates and instead use demand with later due dates.</span></span>  

## <a name="using-the-order-planning-page"></a><span data-ttu-id="aea04-133">Using the Order Planning Page</span><span class="sxs-lookup"><span data-stu-id="aea04-133">Using the Order Planning Page</span></span>  

<span data-ttu-id="aea04-134">The **Order Planning** page can be accessed from several different locations:</span><span class="sxs-lookup"><span data-stu-id="aea04-134">The **Order Planning** page can be accessed from several different locations:</span></span>  

-   <span data-ttu-id="aea04-135">Manufacturing, Planning</span><span class="sxs-lookup"><span data-stu-id="aea04-135">Manufacturing, Planning</span></span>  
-   <span data-ttu-id="aea04-136">Sales & Marketing, Order Processing</span><span class="sxs-lookup"><span data-stu-id="aea04-136">Sales & Marketing, Order Processing</span></span>  
-   <span data-ttu-id="aea04-137">Purchase, Planning</span><span class="sxs-lookup"><span data-stu-id="aea04-137">Purchase, Planning</span></span>  
-   <span data-ttu-id="aea04-138">In addition, you can open this page for a specific production order by choosing the **Planning** action.</span><span class="sxs-lookup"><span data-stu-id="aea04-138">In addition, you can open this page for a specific production order by choosing the **Planning** action.</span></span>

### <a name="to-use-the-order-planning-page"></a><span data-ttu-id="aea04-139">To use the Order Planning page</span><span class="sxs-lookup"><span data-stu-id="aea04-139">To use the Order Planning page</span></span>  

1.  <span data-ttu-id="aea04-140">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Order Planning**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="aea04-140">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Order Planning**, and then choose the related link.</span></span>  

     <span data-ttu-id="aea04-141">When the **Order Planning** page first opens, a plan must be calculated to show the new demand since it was last calculated.</span><span class="sxs-lookup"><span data-stu-id="aea04-141">When the **Order Planning** page first opens, a plan must be calculated to show the new demand since it was last calculated.</span></span>  

2.  <span data-ttu-id="aea04-142">Choose the **Calculate Plan** action.</span><span class="sxs-lookup"><span data-stu-id="aea04-142">Choose the **Calculate Plan** action.</span></span>  

     <span data-ttu-id="aea04-143">The planning system analyses any new demand that has been introduced, such as new sales, changed sales, or production orders.</span><span class="sxs-lookup"><span data-stu-id="aea04-143">The planning system analyzes any new demand that has been introduced, such as new sales, changed sales, or production orders.</span></span>  

     <span data-ttu-id="aea04-144">Based on total availability, the quantity needed for each demand line is calculated.</span><span class="sxs-lookup"><span data-stu-id="aea04-144">Based on total availability, the quantity needed for each demand line is calculated.</span></span> <span data-ttu-id="aea04-145">This calculation is performed order-by-order.</span><span class="sxs-lookup"><span data-stu-id="aea04-145">This calculation is performed order-by-order.</span></span> <span data-ttu-id="aea04-146">This means that the order which includes the demand line with the earliest due date or shipment date will be calculated first.</span><span class="sxs-lookup"><span data-stu-id="aea04-146">This means that the order which includes the demand line with the earliest due date or shipment date will be calculated first.</span></span> <span data-ttu-id="aea04-147">After that, additional demand lines will be calculated in the same order, regardless of the due date or shipment date.</span><span class="sxs-lookup"><span data-stu-id="aea04-147">After that, additional demand lines will be calculated in the same order, regardless of the due date or shipment date.</span></span>  

3.  <span data-ttu-id="aea04-148">Be sure that the **Order Planning** page is maximised and that column fields are resized to show all the default field names.</span><span class="sxs-lookup"><span data-stu-id="aea04-148">Be sure that the **Order Planning** page is maximized and that column fields are resized to show all the default field names.</span></span>  

     <span data-ttu-id="aea04-149">When the calculation is completed, the page displays all unfulfilled demand as collapsed order header lines sorted by earliest demand date.</span><span class="sxs-lookup"><span data-stu-id="aea04-149">When the calculation is completed, the page displays all unfulfilled demand as collapsed order header lines sorted by earliest demand date.</span></span>  

     <span data-ttu-id="aea04-150">Notice that CRONUS has several orders with unfulfilled demand.</span><span class="sxs-lookup"><span data-stu-id="aea04-150">Notice that CRONUS has several orders with unfulfilled demand.</span></span> <span data-ttu-id="aea04-151">Each bold planning line represents an order, sales order, or production order, including at least one order line with insufficient availability.</span><span class="sxs-lookup"><span data-stu-id="aea04-151">Each bold planning line represents an order, sales order, or production order, including at least one order line with insufficient availability.</span></span>  

4.  <span data-ttu-id="aea04-152">In the **Show Demand As** field, select the **All Demand** filter.</span><span class="sxs-lookup"><span data-stu-id="aea04-152">In the **Show Demand As** field, select the **All Demand** filter.</span></span>  

     <span data-ttu-id="aea04-153">With the **Demand Type** field, you can choose which order types that you want to display.</span><span class="sxs-lookup"><span data-stu-id="aea04-153">With the **Demand Type** field, you can choose which order types that you want to display.</span></span>  

     <span data-ttu-id="aea04-154">Orders that do not have availability problems are not shown.</span><span class="sxs-lookup"><span data-stu-id="aea04-154">Orders that do not have availability problems are not shown.</span></span> <span data-ttu-id="aea04-155">If no orders exist when a plan is calculated, a message will display and no planning lines will appear.</span><span class="sxs-lookup"><span data-stu-id="aea04-155">If no orders exist when a plan is calculated, a message will display and no planning lines will appear.</span></span>  

## <a name="planning-a-purchase-order-to-fulfill-component-demand"></a><span data-ttu-id="aea04-156">Planning a Purchase Order to Fulfill Component Demand</span><span class="sxs-lookup"><span data-stu-id="aea04-156">Planning a Purchase Order to Fulfill Component Demand</span></span>  
 <span data-ttu-id="aea04-157">In this procedure, you create a purchase order for needed manufacturing components.</span><span class="sxs-lookup"><span data-stu-id="aea04-157">In this procedure, you create a purchase order for needed manufacturing components.</span></span>  

### <a name="to-plan-a-purchase-order-to-fulfill-component-need-in-production"></a><span data-ttu-id="aea04-158">To plan a purchase order to fulfill component need in production</span><span class="sxs-lookup"><span data-stu-id="aea04-158">To plan a purchase order to fulfill component need in production</span></span>  

1.  <span data-ttu-id="aea04-159">Expand the first line (choose the + symbol).</span><span class="sxs-lookup"><span data-stu-id="aea04-159">Expand the first line (choose the + symbol).</span></span>  
2.  <span data-ttu-id="aea04-160">Choose the first demand line, with item **LSU-15**, and then choose the **Show Document** action.</span><span class="sxs-lookup"><span data-stu-id="aea04-160">Choose the first demand line, with item **LSU-15**, and then choose the **Show Document** action.</span></span>  
3.  <span data-ttu-id="aea04-161">Close the opened production order to return to the **Order Planning** page.</span><span class="sxs-lookup"><span data-stu-id="aea04-161">Close the opened production order to return to the **Order Planning** page.</span></span>  
4.  <span data-ttu-id="aea04-162">In the **Replenishment System** field, select **Purchase**.</span><span class="sxs-lookup"><span data-stu-id="aea04-162">In the **Replenishment System** field, select **Purchase**.</span></span>  

     <span data-ttu-id="aea04-163">The default value is from the item card, or SKU card, but you can change it to one of the following options:</span><span class="sxs-lookup"><span data-stu-id="aea04-163">The default value is from the item card, or SKU card, but you can change it to one of the following options:</span></span>  

    -   <span data-ttu-id="aea04-164">**Purchase** – To create a purchase order.</span><span class="sxs-lookup"><span data-stu-id="aea04-164">**Purchase** – To create a purchase order.</span></span>  
    -   <span data-ttu-id="aea04-165">**Transfer** – To create a transfer order.</span><span class="sxs-lookup"><span data-stu-id="aea04-165">**Transfer** – To create a transfer order.</span></span>  
    -   <span data-ttu-id="aea04-166">**Prod. Order** – To create a production order.</span><span class="sxs-lookup"><span data-stu-id="aea04-166">**Prod. Order** – To create a production order.</span></span>  

5.  <span data-ttu-id="aea04-167">In the **Supply From** field, select one of the following options according to the selected replenishment system:</span><span class="sxs-lookup"><span data-stu-id="aea04-167">In the **Supply From** field, select one of the following options according to the selected replenishment system:</span></span>  

    -   <span data-ttu-id="aea04-168">**Vendor** – For purchases</span><span class="sxs-lookup"><span data-stu-id="aea04-168">**Vendor** – For purchases</span></span>  
    -   <span data-ttu-id="aea04-169">**Location** – For transfers</span><span class="sxs-lookup"><span data-stu-id="aea04-169">**Location** – For transfers</span></span>  

     <span data-ttu-id="aea04-170">If the field is not filled in, an error message will display when you try to create the supply orders.</span><span class="sxs-lookup"><span data-stu-id="aea04-170">If the field is not filled in, an error message will display when you try to create the supply orders.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="aea04-171">If the components have a default vendor number set up on the item cards, the lines will be preset.</span><span class="sxs-lookup"><span data-stu-id="aea04-171">If the components have a default vendor number set up on the item cards, the lines will be preset.</span></span>  

6.  <span data-ttu-id="aea04-172">Choose the **Supply From**  field.</span><span class="sxs-lookup"><span data-stu-id="aea04-172">Choose the **Supply From**  field.</span></span>  
7.  <span data-ttu-id="aea04-173">On the **Item Vendor Catalogue** page, choose the **New** action, and then select vendor **30000**.</span><span class="sxs-lookup"><span data-stu-id="aea04-173">On the **Item Vendor Catalogue** page, choose the **New** action, and then select vendor **30000**.</span></span>  
8.  <span data-ttu-id="aea04-174">Choose the **OK** button to return to the **Order Planning** page.</span><span class="sxs-lookup"><span data-stu-id="aea04-174">Choose the **OK** button to return to the **Order Planning** page.</span></span>  
9. <span data-ttu-id="aea04-175">Copy vendor **30000** to the other lines for loudspeaker components on this production order.</span><span class="sxs-lookup"><span data-stu-id="aea04-175">Copy vendor **30000** to the other lines for loudspeaker components on this production order.</span></span>  

     <span data-ttu-id="aea04-176">You are now ready to create a purchase order.</span><span class="sxs-lookup"><span data-stu-id="aea04-176">You are now ready to create a purchase order.</span></span>  

10. <span data-ttu-id="aea04-177">Choose the **Make Orders** action.</span><span class="sxs-lookup"><span data-stu-id="aea04-177">Choose the **Make Orders** action.</span></span> <span data-ttu-id="aea04-178">The **Make Supply Orders** page opens.</span><span class="sxs-lookup"><span data-stu-id="aea04-178">The **Make Supply Orders** page opens.</span></span>  
11. <span data-ttu-id="aea04-179">On the **Order Planning** FastTab, in the **Make Orders for** field, choose the **Active Order** option.</span><span class="sxs-lookup"><span data-stu-id="aea04-179">On the **Order Planning** FastTab, in the **Make Orders for** field, choose the **Active Order** option.</span></span>  
12. <span data-ttu-id="aea04-180">On the **Options** FastTab, in the **Create Purchase Order** field, choose the **Make Purch. Order** option.</span><span class="sxs-lookup"><span data-stu-id="aea04-180">On the **Options** FastTab, in the **Create Purchase Order** field, choose the **Make Purch. Order** option.</span></span>  
13. <span data-ttu-id="aea04-181">Choose the **OK** button to create purchase orders for all the components of the order.</span><span class="sxs-lookup"><span data-stu-id="aea04-181">Choose the **OK** button to create purchase orders for all the components of the order.</span></span>  

     <span data-ttu-id="aea04-182">The purchase orders are now created and saved as the last orders in the list of purchase orders.</span><span class="sxs-lookup"><span data-stu-id="aea04-182">The purchase orders are now created and saved as the last orders in the list of purchase orders.</span></span>  

## <a name="planning-a-transfer-order-to-fulfill-sales-demand"></a><span data-ttu-id="aea04-183">Planning a Transfer Order to Fulfill Sales Demand</span><span class="sxs-lookup"><span data-stu-id="aea04-183">Planning a Transfer Order to Fulfill Sales Demand</span></span>  
 <span data-ttu-id="aea04-184">In this procedure, you will plan for demand from a sales order.</span><span class="sxs-lookup"><span data-stu-id="aea04-184">In this procedure, you will plan for demand from a sales order.</span></span> <span data-ttu-id="aea04-185">Demand lines represent sales lines and not component lines, as in production demand.</span><span class="sxs-lookup"><span data-stu-id="aea04-185">Demand lines represent sales lines and not component lines, as in production demand.</span></span>  

### <a name="to-plan-a-transfer-order-to-fulfill-sales-demand"></a><span data-ttu-id="aea04-186">To plan a transfer order to fulfill sales demand</span><span class="sxs-lookup"><span data-stu-id="aea04-186">To plan a transfer order to fulfill sales demand</span></span>  

1.  <span data-ttu-id="aea04-187">Move the pointer to the planning line for order **2008**.</span><span class="sxs-lookup"><span data-stu-id="aea04-187">Move the pointer to the planning line for order **2008**.</span></span>  
2.  <span data-ttu-id="aea04-188">Expand the line and move the pointer to the demand line.</span><span class="sxs-lookup"><span data-stu-id="aea04-188">Expand the line and move the pointer to the demand line.</span></span>  

     <span data-ttu-id="aea04-189">Sales order **2008** is for ten loudspeakers, item **LS-120**, ordered by John Haddock Insurance Co.</span><span class="sxs-lookup"><span data-stu-id="aea04-189">Sales order **2008** is for ten loudspeakers, item **LS-120**, ordered by John Haddock Insurance Co.</span></span>  

     <span data-ttu-id="aea04-190">The item's defined replenishment system and default vendor will display.</span><span class="sxs-lookup"><span data-stu-id="aea04-190">The item's defined replenishment system and default vendor will display.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="aea04-191">At the bottom of the page, there are four information fields.</span><span class="sxs-lookup"><span data-stu-id="aea04-191">At the bottom of the page, there are four information fields.</span></span> <span data-ttu-id="aea04-192">In the **Earliest Date Available** field, the ten pieces that are needed will be available, on an inbound supply order, nine days later than the current due date.</span><span class="sxs-lookup"><span data-stu-id="aea04-192">In the **Earliest Date Available** field, the ten pieces that are needed will be available, on an inbound supply order, nine days later than the current due date.</span></span> <span data-ttu-id="aea04-193">If this is too late for the customer, the **Available for Transfer** field shows 13 pieces of the item at another location.</span><span class="sxs-lookup"><span data-stu-id="aea04-193">If this is too late for the customer, the **Available for Transfer** field shows 13 pieces of the item at another location.</span></span> <span data-ttu-id="aea04-194">You will want to plan for this stock.</span><span class="sxs-lookup"><span data-stu-id="aea04-194">You will want to plan for this stock.</span></span>  

3.  <span data-ttu-id="aea04-195">Choose the **Available for Transfer** field to open the **Get Alternative Supply** page.</span><span class="sxs-lookup"><span data-stu-id="aea04-195">Choose the **Available for Transfer** field to open the **Get Alternative Supply** page.</span></span>  
4.  <span data-ttu-id="aea04-196">Choose the **OK** button to book the ten items that are available.</span><span class="sxs-lookup"><span data-stu-id="aea04-196">Choose the **OK** button to book the ten items that are available.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="aea04-197">In the demand line, the suggested purchase has been exchanged with a transfer from MAIN location.</span><span class="sxs-lookup"><span data-stu-id="aea04-197">In the demand line, the suggested purchase has been exchanged with a transfer from MAIN location.</span></span> <span data-ttu-id="aea04-198">The **Make Orders** function creates a transfer order from MAIN to the demanded location.</span><span class="sxs-lookup"><span data-stu-id="aea04-198">The **Make Orders** function creates a transfer order from MAIN to the demanded location.</span></span> <span data-ttu-id="aea04-199">The **Substitutes Exists** field works in the same way.</span><span class="sxs-lookup"><span data-stu-id="aea04-199">The **Substitutes Exists** field works in the same way.</span></span>  

5.  <span data-ttu-id="aea04-200">Choose the **Make Orders** action.</span><span class="sxs-lookup"><span data-stu-id="aea04-200">Choose the **Make Orders** action.</span></span> <span data-ttu-id="aea04-201">The **Make Supply Orders** page opens.</span><span class="sxs-lookup"><span data-stu-id="aea04-201">The **Make Supply Orders** page opens.</span></span>  
6.  <span data-ttu-id="aea04-202">On the **Order Planning** FastTab, in the **Make Orders for** field, choose the **The Active Order** option.</span><span class="sxs-lookup"><span data-stu-id="aea04-202">On the **Order Planning** FastTab, in the **Make Orders for** field, choose the **The Active Order** option.</span></span>  
7.  <span data-ttu-id="aea04-203">On the **Options** FastTab, in the **Create Transfer Order** field, select the **Make Trans. Orders** option.</span><span class="sxs-lookup"><span data-stu-id="aea04-203">On the **Options** FastTab, in the **Create Transfer Order** field, select the **Make Trans. Orders** option.</span></span>  
8.  <span data-ttu-id="aea04-204">Choose the **OK** button to create the transfer order to supply the sales order.</span><span class="sxs-lookup"><span data-stu-id="aea04-204">Choose the **OK** button to create the transfer order to supply the sales order.</span></span>  

     <span data-ttu-id="aea04-205">The transfer order is now created and saved in the list as the last order in the list of open transfer orders.</span><span class="sxs-lookup"><span data-stu-id="aea04-205">The transfer order is now created and saved in the list as the last order in the list of open transfer orders.</span></span>  

## <a name="planning-a-multilevel-production-order-to-fulfill-sales-demand"></a><span data-ttu-id="aea04-206">Planning a Multilevel Production Order to Fulfill Sales Demand</span><span class="sxs-lookup"><span data-stu-id="aea04-206">Planning a Multilevel Production Order to Fulfill Sales Demand</span></span>  
 <span data-ttu-id="aea04-207">In this procedure, you will plan to fulfill sales demand for a produced item with multiple product levels, each creating dependent production demand.</span><span class="sxs-lookup"><span data-stu-id="aea04-207">In this procedure, you will plan to fulfill sales demand for a produced item with multiple product levels, each creating dependent production demand.</span></span>  

### <a name="to-plan-multilevel-production-to-fulfill-sales-demand"></a><span data-ttu-id="aea04-208">To plan multilevel production to fulfill sales demand</span><span class="sxs-lookup"><span data-stu-id="aea04-208">To plan multilevel production to fulfill sales demand</span></span>  

1.  <span data-ttu-id="aea04-209">Select the planning line with sales demand for order **1001**, created earlier as prerequisite data.</span><span class="sxs-lookup"><span data-stu-id="aea04-209">Select the planning line with sales demand for order **1001**, created earlier as prerequisite data.</span></span>  

     <span data-ttu-id="aea04-210">This demand is a sales line, but the item has a defined replenishment system of **Prod. Order**.</span><span class="sxs-lookup"><span data-stu-id="aea04-210">This demand is a sales line, but the item has a defined replenishment system of **Prod. Order**.</span></span> <span data-ttu-id="aea04-211">Proceed to add an extra bell to the component need of each bicycle.</span><span class="sxs-lookup"><span data-stu-id="aea04-211">Proceed to add an extra bell to the component need of each bicycle.</span></span>  

2.  <span data-ttu-id="aea04-212">Choose the **Components** action to open the **Planning Components** page.</span><span class="sxs-lookup"><span data-stu-id="aea04-212">Choose the **Components** action to open the **Planning Components** page.</span></span>  
3.  <span data-ttu-id="aea04-213">On the line with the Bell item, change the **Quantity per** field from **1** to **2**.</span><span class="sxs-lookup"><span data-stu-id="aea04-213">On the line with the Bell item, change the **Quantity per** field from **1** to **2**.</span></span>  
4.  <span data-ttu-id="aea04-214">On the **Order Planning** page, consider your planning alternatives.</span><span class="sxs-lookup"><span data-stu-id="aea04-214">On the **Order Planning** page, consider your planning alternatives.</span></span> <span data-ttu-id="aea04-215">In this case, you have no alternative means of supply, no transfer, substitute, or later delivery.</span><span class="sxs-lookup"><span data-stu-id="aea04-215">In this case, you have no alternative means of supply, no transfer, substitute, or later delivery.</span></span> <span data-ttu-id="aea04-216">You must create the suggested supply order, a production order.</span><span class="sxs-lookup"><span data-stu-id="aea04-216">You must create the suggested supply order, a production order.</span></span>  
5.  <span data-ttu-id="aea04-217">Choose the **Make Orders** action to create the production order.</span><span class="sxs-lookup"><span data-stu-id="aea04-217">Choose the **Make Orders** action to create the production order.</span></span>  

     <span data-ttu-id="aea04-218">On the **Order Planning** page, notice that the planning line for sales order **1001** no longer exists and that the initial sales demand has been covered.</span><span class="sxs-lookup"><span data-stu-id="aea04-218">On the **Order Planning** page, notice that the planning line for sales order **1001** no longer exists and that the initial sales demand has been covered.</span></span>  

6.  <span data-ttu-id="aea04-219">Close the **Order Planning** page.</span><span class="sxs-lookup"><span data-stu-id="aea04-219">Close the **Order Planning** page.</span></span>  

     <span data-ttu-id="aea04-220">Now, you could choose to stay in this view and complete all the planning tasks.</span><span class="sxs-lookup"><span data-stu-id="aea04-220">Now, you could choose to stay in this view and complete all the planning tasks.</span></span> <span data-ttu-id="aea04-221">Instead, you will now take on the Production Planner role by going to the production order that you just created and access the **Order Planning** page.</span><span class="sxs-lookup"><span data-stu-id="aea04-221">Instead, you will now take on the Production Planner role by going to the production order that you just created and access the **Order Planning** page.</span></span>  

 <span data-ttu-id="aea04-222">As a production planner you now must plan a specific production order.</span><span class="sxs-lookup"><span data-stu-id="aea04-222">As a production planner you now must plan a specific production order.</span></span>  

### <a name="to-plan-a-specific-production-order"></a><span data-ttu-id="aea04-223">To plan a specific production order</span><span class="sxs-lookup"><span data-stu-id="aea04-223">To plan a specific production order</span></span>  

1.  <span data-ttu-id="aea04-224">Open the production order **101001**, for ten bicycles, that you just created by using the **Make Orders** function.</span><span class="sxs-lookup"><span data-stu-id="aea04-224">Open the production order **101001**, for ten bicycles, that you just created by using the **Make Orders** function.</span></span>  
2.  <span data-ttu-id="aea04-225">Open the **Prod. Order Components** page to check that the extra bell is reflected on the production order.</span><span class="sxs-lookup"><span data-stu-id="aea04-225">Open the **Prod. Order Components** page to check that the extra bell is reflected on the production order.</span></span>  
3.  <span data-ttu-id="aea04-226">Choose the **Planning** action.</span><span class="sxs-lookup"><span data-stu-id="aea04-226">Choose the **Planning** action.</span></span>  

     <span data-ttu-id="aea04-227">The **Order Planning** page opens in a view that is always filtered on the specific production demand.</span><span class="sxs-lookup"><span data-stu-id="aea04-227">The **Order Planning** page opens in a view that is always filtered on the specific production demand.</span></span> <span data-ttu-id="aea04-228">Sales demand is not displayed.</span><span class="sxs-lookup"><span data-stu-id="aea04-228">Sales demand is not displayed.</span></span> <span data-ttu-id="aea04-229">You must calculate a plan before you can see any additional demand.</span><span class="sxs-lookup"><span data-stu-id="aea04-229">You must calculate a plan before you can see any additional demand.</span></span>  

4.  <span data-ttu-id="aea04-230">Choose the **Calculate Plan** action.</span><span class="sxs-lookup"><span data-stu-id="aea04-230">Choose the **Calculate Plan** action.</span></span>  

     <span data-ttu-id="aea04-231">Notice that four new production orders appear as unplanned production demand derived from order **101001**.</span><span class="sxs-lookup"><span data-stu-id="aea04-231">Notice that four new production orders appear as unplanned production demand derived from order **101001**.</span></span> <span data-ttu-id="aea04-232">The new lines represent new production demand from the subassemblies that must be created to produce the order.</span><span class="sxs-lookup"><span data-stu-id="aea04-232">The new lines represent new production demand from the subassemblies that must be created to produce the order.</span></span>  

5.  <span data-ttu-id="aea04-233">Choose the **Expand All** action to get an overview of all the production demand for the production orders.</span><span class="sxs-lookup"><span data-stu-id="aea04-233">Choose the **Expand All** action to get an overview of all the production demand for the production orders.</span></span>  

     <span data-ttu-id="aea04-234">To provide additional information about the demand lines, you may want to add the **Demand Quantity** and **Demand Qty. Available** fields to your view.</span><span class="sxs-lookup"><span data-stu-id="aea04-234">To provide additional information about the demand lines, you may want to add the **Demand Quantity** and **Demand Qty. Available** fields to your view.</span></span>  

     <span data-ttu-id="aea04-235">Now you must supply ten of each component.</span><span class="sxs-lookup"><span data-stu-id="aea04-235">Now you must supply ten of each component.</span></span>  

     <span data-ttu-id="aea04-236">Note that four of the demand lines have replenishment system Prod. Order.</span><span class="sxs-lookup"><span data-stu-id="aea04-236">Note that four of the demand lines have replenishment system Prod. Order.</span></span> <span data-ttu-id="aea04-237">These four subassemblies represent the second product level of the bicycle.</span><span class="sxs-lookup"><span data-stu-id="aea04-237">These four subassemblies represent the second product level of the bicycle.</span></span>  

     <span data-ttu-id="aea04-238">The default replenishment settings are already filled in and you can proceed to make orders.</span><span class="sxs-lookup"><span data-stu-id="aea04-238">The default replenishment settings are already filled in and you can proceed to make orders.</span></span>  

6.  <span data-ttu-id="aea04-239">Choose the **Make Orders** action.</span><span class="sxs-lookup"><span data-stu-id="aea04-239">Choose the **Make Orders** action.</span></span>  

     <span data-ttu-id="aea04-240">Before you choose the **OK** button, notice the text on the **Order Planning** FastTab.</span><span class="sxs-lookup"><span data-stu-id="aea04-240">Before you choose the **OK** button, notice the text on the **Order Planning** FastTab.</span></span> <span data-ttu-id="aea04-241">This text is important because you know that the bicycle has several produced components, subassemblies, in its product structure that might be in demand when you create this production order.</span><span class="sxs-lookup"><span data-stu-id="aea04-241">This text is important because you know that the bicycle has several produced components, subassemblies, in its product structure that might be in demand when you create this production order.</span></span>  

7.  <span data-ttu-id="aea04-242">On the **Make Supply Order** page, in the **Make Orders for** field, choose the **All Lines** option, and then choose the **OK** button to create production orders for the second product level of the order.</span><span class="sxs-lookup"><span data-stu-id="aea04-242">On the **Make Supply Order** page, in the **Make Orders for** field, choose the **All Lines** option, and then choose the **OK** button to create production orders for the second product level of the order.</span></span>  

     <span data-ttu-id="aea04-243">Note that the top-level production demand for production order 101001 no longer exists.</span><span class="sxs-lookup"><span data-stu-id="aea04-243">Note that the top-level production demand for production order 101001 no longer exists.</span></span> <span data-ttu-id="aea04-244">This means that the initial production demand for subassemblies has been planned for.</span><span class="sxs-lookup"><span data-stu-id="aea04-244">This means that the initial production demand for subassemblies has been planned for.</span></span>  

     <span data-ttu-id="aea04-245">On the **Order Planning** page, you calculate a plan again in order to plan the bicycle structure.</span><span class="sxs-lookup"><span data-stu-id="aea04-245">On the **Order Planning** page, you calculate a plan again in order to plan the bicycle structure.</span></span>  

8.  <span data-ttu-id="aea04-246">Choose the **Calculate Plan** action to recalculate the plan as instructed by the embedded Help text.</span><span class="sxs-lookup"><span data-stu-id="aea04-246">Choose the **Calculate Plan** action to recalculate the plan as instructed by the embedded Help text.</span></span>  

     <span data-ttu-id="aea04-247">The two new lines represent additional production demand derived from the subassemblies planned in the previous steps.</span><span class="sxs-lookup"><span data-stu-id="aea04-247">The two new lines represent additional production demand derived from the subassemblies planned in the previous steps.</span></span> <span data-ttu-id="aea04-248">It is suggested that you make two production orders to supply the wheel hubs, one for 10 front hubs and one for 10 back hubs.</span><span class="sxs-lookup"><span data-stu-id="aea04-248">It is suggested that you make two production orders to supply the wheel hubs, one for 10 front hubs and one for 10 back hubs.</span></span>  

9. <span data-ttu-id="aea04-249">Choose the **Expand All** action to get an overview of all the demand for the two production orders.</span><span class="sxs-lookup"><span data-stu-id="aea04-249">Choose the **Expand All** action to get an overview of all the demand for the two production orders.</span></span>  

     <span data-ttu-id="aea04-250">The suggested supply plan indicates that a total of four purchase orders will be created for the components.</span><span class="sxs-lookup"><span data-stu-id="aea04-250">The suggested supply plan indicates that a total of four purchase orders will be created for the components.</span></span> <span data-ttu-id="aea04-251">You decide to make the proposed orders.</span><span class="sxs-lookup"><span data-stu-id="aea04-251">You decide to make the proposed orders.</span></span>  

10. <span data-ttu-id="aea04-252">Choose the **Make Orders** action.</span><span class="sxs-lookup"><span data-stu-id="aea04-252">Choose the **Make Orders** action.</span></span>  
11. <span data-ttu-id="aea04-253">In the **Make Orders for** field, select the **All Lines** option, and then choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="aea04-253">In the **Make Orders for** field, select the **All Lines** option, and then choose the **OK** button.</span></span> <span data-ttu-id="aea04-254">Check if additional demand exists for the production of the parent item, the bicycle, which is being sold on sales order 1001.</span><span class="sxs-lookup"><span data-stu-id="aea04-254">Check if additional demand exists for the production of the parent item, the bicycle, which is being sold on sales order 1001.</span></span>  
12. <span data-ttu-id="aea04-255">Choose the **Calculate Plan** action.</span><span class="sxs-lookup"><span data-stu-id="aea04-255">Choose the **Calculate Plan** action.</span></span>  

     <span data-ttu-id="aea04-256">The message indicates that all required items are now supplied.</span><span class="sxs-lookup"><span data-stu-id="aea04-256">The message indicates that all required items are now supplied.</span></span> <span data-ttu-id="aea04-257">Verify the firm planned production orders that are created.</span><span class="sxs-lookup"><span data-stu-id="aea04-257">Verify the firm planned production orders that are created.</span></span>  

13. <span data-ttu-id="aea04-258">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Firm Planned Prod. Orders**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="aea04-258">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Firm Planned Prod. Orders**, and then choose the related link.</span></span>  

     <span data-ttu-id="aea04-259">On the **Firm Planned Prod. Orders** page review how start times and end times of individual orders are scheduled according to the product structure.</span><span class="sxs-lookup"><span data-stu-id="aea04-259">On the **Firm Planned Prod. Orders** page review how start times and end times of individual orders are scheduled according to the product structure.</span></span> <span data-ttu-id="aea04-260">The lowest-level components are produced first.</span><span class="sxs-lookup"><span data-stu-id="aea04-260">The lowest-level components are produced first.</span></span> <span data-ttu-id="aea04-261">Therefore, you must plan multilevel orders as demonstrated in this planning workflow.</span><span class="sxs-lookup"><span data-stu-id="aea04-261">Therefore, you must plan multilevel orders as demonstrated in this planning workflow.</span></span>  

## <a name="see-also"></a><span data-ttu-id="aea04-262">See Also</span><span class="sxs-lookup"><span data-stu-id="aea04-262">See Also</span></span>  
 <span data-ttu-id="aea04-263">[Business Process Walkthroughs](walkthrough-business-process-walkthroughs.md) </span><span class="sxs-lookup"><span data-stu-id="aea04-263">[Business Process Walkthroughs](walkthrough-business-process-walkthroughs.md) </span></span>  
 [<span data-ttu-id="aea04-264">Walkthrough: Planning Supplies Automatically</span><span class="sxs-lookup"><span data-stu-id="aea04-264">Walkthrough: Planning Supplies Automatically</span></span>](walkthrough-planning-supplies-automatically.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]