---
title: Walkthrough - Planning Supplies Manually | Microsoft Docs
description: This walkthrough demonstrates the process of planning supply orders to fulfill new demand. You can initiate supply planning at fixed intervals, for example, every morning or every Monday, or when you are notified by sales or production, depending on the type of demand.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2019
ms.author: sgroespe
ms.openlocfilehash: f8c20f51997ca2ec056423b9089b645e5a258235
ms.sourcegitcommit: bd78a5d990c9e83174da1409076c22df8b35eafd
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 03/31/2019
ms.locfileid: "925756"
---
# <a name="walkthrough-planning-supplies-manually"></a><span data-ttu-id="8f838-104">Walkthrough: Planning Supplies Manually</span><span class="sxs-lookup"><span data-stu-id="8f838-104">Walkthrough: Planning Supplies Manually</span></span>

<span data-ttu-id="8f838-105">**Note**: This walkthrough must be performed on a demonstration company with the **Full Evaluation - Complete Sample Data** option, which is available in the Sandbox environment.</span><span class="sxs-lookup"><span data-stu-id="8f838-105">**Note**: This walkthrough must be performed on a demonstration company with the **Full Evaluation - Complete Sample Data** option, which is available in the Sandbox environment.</span></span> <span data-ttu-id="8f838-106">For more information, see [Creating a Sandbox Environment](across-how-create-sandbox-environment.md).</span><span class="sxs-lookup"><span data-stu-id="8f838-106">For more information, see [Creating a Sandbox Environment](across-how-create-sandbox-environment.md).</span></span>

<span data-ttu-id="8f838-107">This walkthrough demonstrates the process of planning supply orders to fulfil new demand.</span><span class="sxs-lookup"><span data-stu-id="8f838-107">This walkthrough demonstrates the process of planning supply orders to fulfill new demand.</span></span> <span data-ttu-id="8f838-108">You can initiate supply planning at fixed intervals, for example, every morning or every Monday, or when you are notified by sales or production, depending on the type of demand.</span><span class="sxs-lookup"><span data-stu-id="8f838-108">You can initiate supply planning at fixed intervals, for example, every morning or every Monday, or when you are notified by sales or production, depending on the type of demand.</span></span> <span data-ttu-id="8f838-109">In this walkthrough you will use the **Order Planning** page, a simple supply planning tool that is based on manual decision-making instead of parameter-based automatic planning.</span><span class="sxs-lookup"><span data-stu-id="8f838-109">In this walkthrough you will use the **Order Planning** page, a simple supply planning tool that is based on manual decision-making instead of parameter-based automatic planning.</span></span>  

## <a name="about-this-walkthrough"></a><span data-ttu-id="8f838-110">About This Walkthrough</span><span class="sxs-lookup"><span data-stu-id="8f838-110">About This Walkthrough</span></span>  
 <span data-ttu-id="8f838-111">This walkthrough illustrates the following tasks:</span><span class="sxs-lookup"><span data-stu-id="8f838-111">This walkthrough illustrates the following tasks:</span></span>  

-   <span data-ttu-id="8f838-112">Planning a purchase order for manufacturing components.</span><span class="sxs-lookup"><span data-stu-id="8f838-112">Planning a purchase order for manufacturing components.</span></span>  
-   <span data-ttu-id="8f838-113">Planning a transfer order to fulfill sales demand.</span><span class="sxs-lookup"><span data-stu-id="8f838-113">Planning a transfer order to fulfill sales demand.</span></span>  
-   <span data-ttu-id="8f838-114">Planning a production order for a multilevel item.</span><span class="sxs-lookup"><span data-stu-id="8f838-114">Planning a production order for a multilevel item.</span></span>  

## <a name="roles"></a><span data-ttu-id="8f838-115">Roles</span><span class="sxs-lookup"><span data-stu-id="8f838-115">Roles</span></span>  
 <span data-ttu-id="8f838-116">This walkthrough demonstrates tasks performed by the following user roles:</span><span class="sxs-lookup"><span data-stu-id="8f838-116">This walkthrough demonstrates tasks performed by the following user roles:</span></span>  

-   <span data-ttu-id="8f838-117">Production Planner</span><span class="sxs-lookup"><span data-stu-id="8f838-117">Production Planner</span></span>  
-   <span data-ttu-id="8f838-118">Purchasing Agent</span><span class="sxs-lookup"><span data-stu-id="8f838-118">Purchasing Agent</span></span>  
-   <span data-ttu-id="8f838-119">Sales Order Processor</span><span class="sxs-lookup"><span data-stu-id="8f838-119">Sales Order Processor</span></span>  

## <a name="prerequisites"></a><span data-ttu-id="8f838-120">Prerequisites</span><span class="sxs-lookup"><span data-stu-id="8f838-120">Prerequisites</span></span>  
 <span data-ttu-id="8f838-121">Before you begin this walkthrough, you must install the [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="8f838-121">Before you begin this walkthrough, you must install the [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="8f838-122">The following modifications must be made to the database:</span><span class="sxs-lookup"><span data-stu-id="8f838-122">The following modifications must be made to the database:</span></span>  

-   <span data-ttu-id="8f838-123">Delete all existing sales orders for bicycles.</span><span class="sxs-lookup"><span data-stu-id="8f838-123">Delete all existing sales orders for bicycles.</span></span>  
-   <span data-ttu-id="8f838-124">Create one sales order for 10 bicycles at BLUE location.</span><span class="sxs-lookup"><span data-stu-id="8f838-124">Create one sales order for 10 bicycles at BLUE location.</span></span>  
-   <span data-ttu-id="8f838-125">Delete all planned and firm planned production orders.</span><span class="sxs-lookup"><span data-stu-id="8f838-125">Delete all planned and firm planned production orders.</span></span> <span data-ttu-id="8f838-126">Do not delete started orders with entries that are already posted.</span><span class="sxs-lookup"><span data-stu-id="8f838-126">Do not delete started orders with entries that are already posted.</span></span>  

 <span data-ttu-id="8f838-127">As a rule, use the suggested data in this walkthrough because this data has the necessary records.</span><span class="sxs-lookup"><span data-stu-id="8f838-127">As a rule, use the suggested data in this walkthrough because this data has the necessary records.</span></span>  

## <a name="story"></a><span data-ttu-id="8f838-128">Story</span><span class="sxs-lookup"><span data-stu-id="8f838-128">Story</span></span>  
 <span data-ttu-id="8f838-129">Eduardo, the Production Planner of a small manufacturing company, is about to plan production and purchase orders to fulfill new sales demand.</span><span class="sxs-lookup"><span data-stu-id="8f838-129">Eduardo, the Production Planner of a small manufacturing company, is about to plan production and purchase orders to fulfill new sales demand.</span></span>  

 <span data-ttu-id="8f838-130">Because the products have few BOM levels and the flow of orders is relatively low, Eduardo uses the **Order Planning** page to manually create supply orders, one product level at a time.</span><span class="sxs-lookup"><span data-stu-id="8f838-130">Because the products have few BOM levels and the flow of orders is relatively low, Eduardo uses the **Order Planning** page to manually create supply orders, one product level at a time.</span></span>  

 <span data-ttu-id="8f838-131">In a more complex manufacturing environment, the planning worksheet is used to plan supply based on item parameters such as rescheduling period, safety lead time, reorder point, and batch calculations of consolidated demand from all product levels.</span><span class="sxs-lookup"><span data-stu-id="8f838-131">In a more complex manufacturing environment, the planning worksheet is used to plan supply based on item parameters such as rescheduling period, safety lead time, reorder point, and batch calculations of consolidated demand from all product levels.</span></span>  

## <a name="setting-up-the-sample-data"></a><span data-ttu-id="8f838-132">Setting Up the Sample Data</span><span class="sxs-lookup"><span data-stu-id="8f838-132">Setting Up the Sample Data</span></span>  
 <span data-ttu-id="8f838-133">The standard CRONUS demonstration company currently has lots of unplanned demand.</span><span class="sxs-lookup"><span data-stu-id="8f838-133">The standard CRONUS demonstration company currently has lots of unplanned demand.</span></span> <span data-ttu-id="8f838-134">During the different planning tasks in this walkthrough, you will have to deviate from the realistic business flow by ignoring demand with close due dates and instead use demand with later due dates.</span><span class="sxs-lookup"><span data-stu-id="8f838-134">During the different planning tasks in this walkthrough, you will have to deviate from the realistic business flow by ignoring demand with close due dates and instead use demand with later due dates.</span></span>  

## <a name="using-the-order-planning-page"></a><span data-ttu-id="8f838-135">Using the Order Planning Page</span><span class="sxs-lookup"><span data-stu-id="8f838-135">Using the Order Planning Page</span></span>  

<!--
The **Order Planning** page can be accessed from several different locations on the **Departments** menu in the navigation pane:  

-   Manufacturing, Planning  
-   Sales & Marketing, Order Processing  
-   Purchase, Planning  
-   In addition, you can open this page for a specific production order by choosing **Planning** on the **Navigate** tab in the **Order** group.

-->  

### <a name="to-use-the-order-planning-page"></a><span data-ttu-id="8f838-136">To use the Order Planning page</span><span class="sxs-lookup"><span data-stu-id="8f838-136">To use the Order Planning page</span></span>  

1.  <span data-ttu-id="8f838-137">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Order Planning**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="8f838-137">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Order Planning**, and then choose the related link.</span></span>  

     <span data-ttu-id="8f838-138">When the **Order Planning** page first opens, a plan must be calculated to show the new demand since it was last calculated.</span><span class="sxs-lookup"><span data-stu-id="8f838-138">When the **Order Planning** page first opens, a plan must be calculated to show the new demand since it was last calculated.</span></span>  

2.  <span data-ttu-id="8f838-139">Choose the **Calculate Plan** action.</span><span class="sxs-lookup"><span data-stu-id="8f838-139">Choose the **Calculate Plan** action.</span></span>  

     <span data-ttu-id="8f838-140">The planning system analyses any new demand that has been introduced, such as new sales, changed sales, or production orders.</span><span class="sxs-lookup"><span data-stu-id="8f838-140">The planning system analyzes any new demand that has been introduced, such as new sales, changed sales, or production orders.</span></span>  

     <span data-ttu-id="8f838-141">Based on total availability, the quantity needed for each demand line is calculated.</span><span class="sxs-lookup"><span data-stu-id="8f838-141">Based on total availability, the quantity needed for each demand line is calculated.</span></span> <span data-ttu-id="8f838-142">This calculation is performed order-by-order.</span><span class="sxs-lookup"><span data-stu-id="8f838-142">This calculation is performed order-by-order.</span></span> <span data-ttu-id="8f838-143">This means that the order which includes the demand line with the earliest due date or shipment date will be calculated first.</span><span class="sxs-lookup"><span data-stu-id="8f838-143">This means that the order which includes the demand line with the earliest due date or shipment date will be calculated first.</span></span> <span data-ttu-id="8f838-144">After that, additional demand lines will be calculated in the same order, regardless of the due date or shipment date.</span><span class="sxs-lookup"><span data-stu-id="8f838-144">After that, additional demand lines will be calculated in the same order, regardless of the due date or shipment date.</span></span>  

3.  <span data-ttu-id="8f838-145">Be sure that the **Order Planning** page is maximised and that column fields are resized to show all the default field names.</span><span class="sxs-lookup"><span data-stu-id="8f838-145">Be sure that the **Order Planning** page is maximized and that column fields are resized to show all the default field names.</span></span>  

     <span data-ttu-id="8f838-146">When the calculation is completed, the page displays all unfulfilled demand as collapsed order header lines sorted by earliest demand date.</span><span class="sxs-lookup"><span data-stu-id="8f838-146">When the calculation is completed, the page displays all unfulfilled demand as collapsed order header lines sorted by earliest demand date.</span></span>  

     <span data-ttu-id="8f838-147">Notice that CRONUS has several orders with unfulfilled demand.</span><span class="sxs-lookup"><span data-stu-id="8f838-147">Notice that CRONUS has several orders with unfulfilled demand.</span></span> <span data-ttu-id="8f838-148">Each bold planning line represents an order, sales order, or production order, including at least one order line with insufficient availability.</span><span class="sxs-lookup"><span data-stu-id="8f838-148">Each bold planning line represents an order, sales order, or production order, including at least one order line with insufficient availability.</span></span>  

4.  <span data-ttu-id="8f838-149">In the **Show Demand As** field, select the **All Demand** filter.</span><span class="sxs-lookup"><span data-stu-id="8f838-149">In the **Show Demand As** field, select the **All Demand** filter.</span></span>  

     <span data-ttu-id="8f838-150">With the **Demand Type** field, you can choose which order types that you want to display.</span><span class="sxs-lookup"><span data-stu-id="8f838-150">With the **Demand Type** field, you can choose which order types that you want to display.</span></span>  

     <span data-ttu-id="8f838-151">Orders that do not have availability problems are not shown.</span><span class="sxs-lookup"><span data-stu-id="8f838-151">Orders that do not have availability problems are not shown.</span></span> <span data-ttu-id="8f838-152">If no orders exist when a plan is calculated, a message will display and no planning lines will appear.</span><span class="sxs-lookup"><span data-stu-id="8f838-152">If no orders exist when a plan is calculated, a message will display and no planning lines will appear.</span></span>  

## <a name="planning-a-purchase-order-to-fulfill-component-demand"></a><span data-ttu-id="8f838-153">Planning a Purchase Order to Fulfill Component Demand</span><span class="sxs-lookup"><span data-stu-id="8f838-153">Planning a Purchase Order to Fulfill Component Demand</span></span>  
 <span data-ttu-id="8f838-154">In this procedure, you create a purchase order for needed manufacturing components.</span><span class="sxs-lookup"><span data-stu-id="8f838-154">In this procedure, you create a purchase order for needed manufacturing components.</span></span>  

### <a name="to-plan-a-purchase-order-to-fulfill-component-need-in-production"></a><span data-ttu-id="8f838-155">To plan a purchase order to fulfill component need in production</span><span class="sxs-lookup"><span data-stu-id="8f838-155">To plan a purchase order to fulfill component need in production</span></span>  

1.  <span data-ttu-id="8f838-156">Expand the first line (choose the + symbol).</span><span class="sxs-lookup"><span data-stu-id="8f838-156">Expand the first line (choose the + symbol).</span></span>  
2.  <span data-ttu-id="8f838-157">Choose the first demand line, with item **LSU-15**, and then choose the **Show Document** action.</span><span class="sxs-lookup"><span data-stu-id="8f838-157">Choose the first demand line, with item **LSU-15**, and then choose the **Show Document** action.</span></span>  
3.  <span data-ttu-id="8f838-158">Close the opened production order to return to the **Order Planning** page.</span><span class="sxs-lookup"><span data-stu-id="8f838-158">Close the opened production order to return to the **Order Planning** page.</span></span>  
4.  <span data-ttu-id="8f838-159">In the **Replenishment System** field, select **Purchase**.</span><span class="sxs-lookup"><span data-stu-id="8f838-159">In the **Replenishment System** field, select **Purchase**.</span></span>  

     <span data-ttu-id="8f838-160">The default value is from the item card, or SKU card, but you can change it to one of the following options:</span><span class="sxs-lookup"><span data-stu-id="8f838-160">The default value is from the item card, or SKU card, but you can change it to one of the following options:</span></span>  

    -   <span data-ttu-id="8f838-161">**Purchase** – To create a purchase order.</span><span class="sxs-lookup"><span data-stu-id="8f838-161">**Purchase** – To create a purchase order.</span></span>  
    -   <span data-ttu-id="8f838-162">**Transfer** – To create a transfer order.</span><span class="sxs-lookup"><span data-stu-id="8f838-162">**Transfer** – To create a transfer order.</span></span>  
    -   <span data-ttu-id="8f838-163">**Prod. Order** – To create a production order.</span><span class="sxs-lookup"><span data-stu-id="8f838-163">**Prod. Order** – To create a production order.</span></span>  

5.  <span data-ttu-id="8f838-164">In the **Supply From** field, select one of the following options according to the selected replenishment system:</span><span class="sxs-lookup"><span data-stu-id="8f838-164">In the **Supply From** field, select one of the following options according to the selected replenishment system:</span></span>  

    -   <span data-ttu-id="8f838-165">**Vendor** – For purchases</span><span class="sxs-lookup"><span data-stu-id="8f838-165">**Vendor** – For purchases</span></span>  
    -   <span data-ttu-id="8f838-166">**Location** – For transfers</span><span class="sxs-lookup"><span data-stu-id="8f838-166">**Location** – For transfers</span></span>  

     <span data-ttu-id="8f838-167">If the field is not filled in, an error message will display when you try to create the supply orders.</span><span class="sxs-lookup"><span data-stu-id="8f838-167">If the field is not filled in, an error message will display when you try to create the supply orders.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="8f838-168">If the components have a default vendor number set up on the item cards, the lines will be preset.</span><span class="sxs-lookup"><span data-stu-id="8f838-168">If the components have a default vendor number set up on the item cards, the lines will be preset.</span></span>  

6.  <span data-ttu-id="8f838-169">Choose the **Supply From**  field.</span><span class="sxs-lookup"><span data-stu-id="8f838-169">Choose the **Supply From**  field.</span></span>  
7.  <span data-ttu-id="8f838-170">On the **Item Vendor Catalogue** page, choose the **New** action, and then select vendor **30000**.</span><span class="sxs-lookup"><span data-stu-id="8f838-170">On the **Item Vendor Catalogue** page, choose the **New** action, and then select vendor **30000**.</span></span>  
8.  <span data-ttu-id="8f838-171">Choose the **OK** button to return to the **Order Planning** page.</span><span class="sxs-lookup"><span data-stu-id="8f838-171">Choose the **OK** button to return to the **Order Planning** page.</span></span>  
9. <span data-ttu-id="8f838-172">Copy vendor **30000** to the other lines for loudspeaker components on this production order.</span><span class="sxs-lookup"><span data-stu-id="8f838-172">Copy vendor **30000** to the other lines for loudspeaker components on this production order.</span></span>  

     <span data-ttu-id="8f838-173">You are now ready to create a purchase order.</span><span class="sxs-lookup"><span data-stu-id="8f838-173">You are now ready to create a purchase order.</span></span>  

10. <span data-ttu-id="8f838-174">Choose the **Make Orders** action.</span><span class="sxs-lookup"><span data-stu-id="8f838-174">Choose the **Make Orders** action.</span></span> <span data-ttu-id="8f838-175">The **Make Supply Orders** page opens.</span><span class="sxs-lookup"><span data-stu-id="8f838-175">The **Make Supply Orders** page opens.</span></span>  
11. <span data-ttu-id="8f838-176">On the **Order Planning** FastTab, in the **Make Orders for** field, choose the **Active Order** option.</span><span class="sxs-lookup"><span data-stu-id="8f838-176">On the **Order Planning** FastTab, in the **Make Orders for** field, choose the **Active Order** option.</span></span>  
12. <span data-ttu-id="8f838-177">On the **Options** FastTab, in the **Create Purchase Order** field, choose the **Make Purch. Order** option.</span><span class="sxs-lookup"><span data-stu-id="8f838-177">On the **Options** FastTab, in the **Create Purchase Order** field, choose the **Make Purch. Order** option.</span></span>  
13. <span data-ttu-id="8f838-178">Choose the **OK** button to create purchase orders for all the components of the order.</span><span class="sxs-lookup"><span data-stu-id="8f838-178">Choose the **OK** button to create purchase orders for all the components of the order.</span></span>  

     <span data-ttu-id="8f838-179">The purchase orders are now created and saved as the last orders in the list of purchase orders.</span><span class="sxs-lookup"><span data-stu-id="8f838-179">The purchase orders are now created and saved as the last orders in the list of purchase orders.</span></span>  

## <a name="planning-a-transfer-order-to-fulfill-sales-demand"></a><span data-ttu-id="8f838-180">Planning a Transfer Order to Fulfill Sales Demand</span><span class="sxs-lookup"><span data-stu-id="8f838-180">Planning a Transfer Order to Fulfill Sales Demand</span></span>  
 <span data-ttu-id="8f838-181">In this procedure, you will plan for demand from a sales order.</span><span class="sxs-lookup"><span data-stu-id="8f838-181">In this procedure, you will plan for demand from a sales order.</span></span> <span data-ttu-id="8f838-182">Demand lines represent sales lines and not component lines, as in production demand.</span><span class="sxs-lookup"><span data-stu-id="8f838-182">Demand lines represent sales lines and not component lines, as in production demand.</span></span>  

### <a name="to-plan-a-transfer-order-to-fulfill-sales-demand"></a><span data-ttu-id="8f838-183">To plan a transfer order to fulfill sales demand</span><span class="sxs-lookup"><span data-stu-id="8f838-183">To plan a transfer order to fulfill sales demand</span></span>  

1.  <span data-ttu-id="8f838-184">Move the pointer to the planning line for order **2008**.</span><span class="sxs-lookup"><span data-stu-id="8f838-184">Move the pointer to the planning line for order **2008**.</span></span>  
2.  <span data-ttu-id="8f838-185">Expand the line and move the pointer to the demand line.</span><span class="sxs-lookup"><span data-stu-id="8f838-185">Expand the line and move the pointer to the demand line.</span></span>  

     <span data-ttu-id="8f838-186">Sales order **2008** is for ten loudspeakers, item **LS-120**, ordered by John Haddock Insurance Co.</span><span class="sxs-lookup"><span data-stu-id="8f838-186">Sales order **2008** is for ten loudspeakers, item **LS-120**, ordered by John Haddock Insurance Co.</span></span>  

     <span data-ttu-id="8f838-187">The item’s defined replenishment system and default vendor will display.</span><span class="sxs-lookup"><span data-stu-id="8f838-187">The item’s defined replenishment system and default vendor will display.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="8f838-188">At the bottom of the page, there are four information fields.</span><span class="sxs-lookup"><span data-stu-id="8f838-188">At the bottom of the page, there are four information fields.</span></span> <span data-ttu-id="8f838-189">In the **Earliest Date Available** field, the ten pieces that are needed will be available, on an inbound supply order, nine days later than the current due date.</span><span class="sxs-lookup"><span data-stu-id="8f838-189">In the **Earliest Date Available** field, the ten pieces that are needed will be available, on an inbound supply order, nine days later than the current due date.</span></span> <span data-ttu-id="8f838-190">If this is too late for the customer, the **Available for Transfer** field shows 13 pieces of the item at another location.</span><span class="sxs-lookup"><span data-stu-id="8f838-190">If this is too late for the customer, the **Available for Transfer** field shows 13 pieces of the item at another location.</span></span> <span data-ttu-id="8f838-191">You will want to plan for this stock.</span><span class="sxs-lookup"><span data-stu-id="8f838-191">You will want to plan for this stock.</span></span>  

3.  <span data-ttu-id="8f838-192">Choose the **Available for Transfer** field to open the **Get Alternative Supply** page.</span><span class="sxs-lookup"><span data-stu-id="8f838-192">Choose the **Available for Transfer** field to open the **Get Alternative Supply** page.</span></span>  
4.  <span data-ttu-id="8f838-193">Choose the **OK** button to book the ten items that are available.</span><span class="sxs-lookup"><span data-stu-id="8f838-193">Choose the **OK** button to book the ten items that are available.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="8f838-194">In the demand line, the suggested purchase has been exchanged with a transfer from GREEN location.</span><span class="sxs-lookup"><span data-stu-id="8f838-194">In the demand line, the suggested purchase has been exchanged with a transfer from GREEN location.</span></span> <span data-ttu-id="8f838-195">The **Make Orders** function creates a transfer order from GREEN to the demanded location.</span><span class="sxs-lookup"><span data-stu-id="8f838-195">The **Make Orders** function creates a transfer order from GREEN to the demanded location.</span></span> <span data-ttu-id="8f838-196">The **Substitutes Exists** field works in the same way.</span><span class="sxs-lookup"><span data-stu-id="8f838-196">The **Substitutes Exists** field works in the same way.</span></span>  

5.  <span data-ttu-id="8f838-197">Choose the **Make Orders** action.</span><span class="sxs-lookup"><span data-stu-id="8f838-197">Choose the **Make Orders** action.</span></span> <span data-ttu-id="8f838-198">The **Make Supply Orders** page opens.</span><span class="sxs-lookup"><span data-stu-id="8f838-198">The **Make Supply Orders** page opens.</span></span>  
6.  <span data-ttu-id="8f838-199">On the **Order Planning** FastTab, in the **Make Orders for** field, choose the **The Active Order** option.</span><span class="sxs-lookup"><span data-stu-id="8f838-199">On the **Order Planning** FastTab, in the **Make Orders for** field, choose the **The Active Order** option.</span></span>  
7.  <span data-ttu-id="8f838-200">On the **Options** FastTab, in the **Create Transfer Order** field, select the **Make Trans. Orders** option.</span><span class="sxs-lookup"><span data-stu-id="8f838-200">On the **Options** FastTab, in the **Create Transfer Order** field, select the **Make Trans. Orders** option.</span></span>  
8.  <span data-ttu-id="8f838-201">Choose the **OK** button to create the transfer order to supply the sales order.</span><span class="sxs-lookup"><span data-stu-id="8f838-201">Choose the **OK** button to create the transfer order to supply the sales order.</span></span>  

     <span data-ttu-id="8f838-202">The transfer order is now created and saved in the list as the last order in the list of open transfer orders.</span><span class="sxs-lookup"><span data-stu-id="8f838-202">The transfer order is now created and saved in the list as the last order in the list of open transfer orders.</span></span>  

## <a name="planning-a-multilevel-production-order-to-fulfill-sales-demand"></a><span data-ttu-id="8f838-203">Planning a Multilevel Production Order to Fulfill Sales Demand</span><span class="sxs-lookup"><span data-stu-id="8f838-203">Planning a Multilevel Production Order to Fulfill Sales Demand</span></span>  
 <span data-ttu-id="8f838-204">In this procedure, you will plan to fulfill sales demand for a produced item with multiple product levels, each creating dependent production demand.</span><span class="sxs-lookup"><span data-stu-id="8f838-204">In this procedure, you will plan to fulfill sales demand for a produced item with multiple product levels, each creating dependent production demand.</span></span>  

### <a name="to-plan-multilevel-production-to-fulfill-sales-demand"></a><span data-ttu-id="8f838-205">To plan multilevel production to fulfill sales demand</span><span class="sxs-lookup"><span data-stu-id="8f838-205">To plan multilevel production to fulfill sales demand</span></span>  

1.  <span data-ttu-id="8f838-206">Select the planning line with sales demand for order **1001**, created earlier as prerequisite data.</span><span class="sxs-lookup"><span data-stu-id="8f838-206">Select the planning line with sales demand for order **1001**, created earlier as prerequisite data.</span></span>  

     <span data-ttu-id="8f838-207">This demand is a sales line, but the item has a defined replenishment system of **Prod. Order**.</span><span class="sxs-lookup"><span data-stu-id="8f838-207">This demand is a sales line, but the item has a defined replenishment system of **Prod. Order**.</span></span> <span data-ttu-id="8f838-208">Proceed to add an extra bell to the component need of each bicycle.</span><span class="sxs-lookup"><span data-stu-id="8f838-208">Proceed to add an extra bell to the component need of each bicycle.</span></span>  

2.  <span data-ttu-id="8f838-209">Choose the **Components** action to open the **Planning Components** page.</span><span class="sxs-lookup"><span data-stu-id="8f838-209">Choose the **Components** action to open the **Planning Components** page.</span></span>  
3.  <span data-ttu-id="8f838-210">On the line with the Bell item, change the **Quantity per** field from **1** to **2**.</span><span class="sxs-lookup"><span data-stu-id="8f838-210">On the line with the Bell item, change the **Quantity per** field from **1** to **2**.</span></span>  
4.  <span data-ttu-id="8f838-211">On the **Order Planning** page, consider your planning alternatives.</span><span class="sxs-lookup"><span data-stu-id="8f838-211">On the **Order Planning** page, consider your planning alternatives.</span></span> <span data-ttu-id="8f838-212">In this case, you have no alternative means of supply, no transfer, substitute, or later delivery.</span><span class="sxs-lookup"><span data-stu-id="8f838-212">In this case, you have no alternative means of supply, no transfer, substitute, or later delivery.</span></span> <span data-ttu-id="8f838-213">You must create the suggested supply order, a production order.</span><span class="sxs-lookup"><span data-stu-id="8f838-213">You must create the suggested supply order, a production order.</span></span>  
5.  <span data-ttu-id="8f838-214">Choose the **Make Orders** action to create the production order.</span><span class="sxs-lookup"><span data-stu-id="8f838-214">Choose the **Make Orders** action to create the production order.</span></span>  

     <span data-ttu-id="8f838-215">On the **Order Planning** page, notice that the planning line for sales order **1001** no longer exists and that the initial sales demand has been covered.</span><span class="sxs-lookup"><span data-stu-id="8f838-215">On the **Order Planning** page, notice that the planning line for sales order **1001** no longer exists and that the initial sales demand has been covered.</span></span>  

6.  <span data-ttu-id="8f838-216">Close the **Order Planning** page.</span><span class="sxs-lookup"><span data-stu-id="8f838-216">Close the **Order Planning** page.</span></span>  

     <span data-ttu-id="8f838-217">Now, you could choose to stay in this view and complete all the planning tasks.</span><span class="sxs-lookup"><span data-stu-id="8f838-217">Now, you could choose to stay in this view and complete all the planning tasks.</span></span> <span data-ttu-id="8f838-218">Instead, you will now take on the Production Planner role by going to the production order that you just created and access the **Order Planning** page.</span><span class="sxs-lookup"><span data-stu-id="8f838-218">Instead, you will now take on the Production Planner role by going to the production order that you just created and access the **Order Planning** page.</span></span>  

 <span data-ttu-id="8f838-219">As a production planner you now must plan a specific production order.</span><span class="sxs-lookup"><span data-stu-id="8f838-219">As a production planner you now must plan a specific production order.</span></span>  

### <a name="to-plan-a-specific-production-order"></a><span data-ttu-id="8f838-220">To plan a specific production order</span><span class="sxs-lookup"><span data-stu-id="8f838-220">To plan a specific production order</span></span>  

1.  <span data-ttu-id="8f838-221">Open the production order **101001**, for ten bicycles, that you just created by using the **Make Orders** function.</span><span class="sxs-lookup"><span data-stu-id="8f838-221">Open the production order **101001**, for ten bicycles, that you just created by using the **Make Orders** function.</span></span>  
2.  <span data-ttu-id="8f838-222">Open the **Prod. Order Components** page to check that the extra bell is reflected on the production order.</span><span class="sxs-lookup"><span data-stu-id="8f838-222">Open the **Prod. Order Components** page to check that the extra bell is reflected on the production order.</span></span>  
3.  <span data-ttu-id="8f838-223">Choose the **Planning** action.</span><span class="sxs-lookup"><span data-stu-id="8f838-223">Choose the **Planning** action.</span></span>  

     <span data-ttu-id="8f838-224">The **Order Planning** page opens in a view that is always filtered on the specific production demand.</span><span class="sxs-lookup"><span data-stu-id="8f838-224">The **Order Planning** page opens in a view that is always filtered on the specific production demand.</span></span> <span data-ttu-id="8f838-225">Sales demand is not displayed.</span><span class="sxs-lookup"><span data-stu-id="8f838-225">Sales demand is not displayed.</span></span> <span data-ttu-id="8f838-226">You must calculate a plan before you can see any additional demand.</span><span class="sxs-lookup"><span data-stu-id="8f838-226">You must calculate a plan before you can see any additional demand.</span></span>  

4.  <span data-ttu-id="8f838-227">Choose the **Calculate Plan** action.</span><span class="sxs-lookup"><span data-stu-id="8f838-227">Choose the **Calculate Plan** action.</span></span>  

     <span data-ttu-id="8f838-228">Notice that four new production orders appear as unplanned production demand derived from order **101001**.</span><span class="sxs-lookup"><span data-stu-id="8f838-228">Notice that four new production orders appear as unplanned production demand derived from order **101001**.</span></span> <span data-ttu-id="8f838-229">The new lines represent new production demand from the subassemblies that must be created to produce the order.</span><span class="sxs-lookup"><span data-stu-id="8f838-229">The new lines represent new production demand from the subassemblies that must be created to produce the order.</span></span>  

5.  <span data-ttu-id="8f838-230">Choose the **Expand All** action to get an overview of all the production demand for the production orders.</span><span class="sxs-lookup"><span data-stu-id="8f838-230">Choose the **Expand All** action to get an overview of all the production demand for the production orders.</span></span>  

     <span data-ttu-id="8f838-231">To provide additional information about the demand lines, you may want to add the **Demand Quantity** and **Demand Qty. Available** fields to your view.</span><span class="sxs-lookup"><span data-stu-id="8f838-231">To provide additional information about the demand lines, you may want to add the **Demand Quantity** and **Demand Qty. Available** fields to your view.</span></span>  

     <span data-ttu-id="8f838-232">Now you must supply ten of each component.</span><span class="sxs-lookup"><span data-stu-id="8f838-232">Now you must supply ten of each component.</span></span>  

     <span data-ttu-id="8f838-233">Note that four of the demand lines have replenishment system Prod. Order.</span><span class="sxs-lookup"><span data-stu-id="8f838-233">Note that four of the demand lines have replenishment system Prod. Order.</span></span> <span data-ttu-id="8f838-234">These four subassemblies represent the second product level of the bicycle.</span><span class="sxs-lookup"><span data-stu-id="8f838-234">These four subassemblies represent the second product level of the bicycle.</span></span>  

     <span data-ttu-id="8f838-235">The default replenishment settings are already filled in and you can proceed to make orders.</span><span class="sxs-lookup"><span data-stu-id="8f838-235">The default replenishment settings are already filled in and you can proceed to make orders.</span></span>  

6.  <span data-ttu-id="8f838-236">Choose the **Make Orders** action.</span><span class="sxs-lookup"><span data-stu-id="8f838-236">Choose the **Make Orders** action.</span></span>  

     <span data-ttu-id="8f838-237">Before you choose the **OK** button, notice the text on the **Order Planning** FastTab.</span><span class="sxs-lookup"><span data-stu-id="8f838-237">Before you choose the **OK** button, notice the text on the **Order Planning** FastTab.</span></span> <span data-ttu-id="8f838-238">This text is important because you know that the bicycle has several produced components, subassemblies, in its product structure that might be in demand when you create this production order.</span><span class="sxs-lookup"><span data-stu-id="8f838-238">This text is important because you know that the bicycle has several produced components, subassemblies, in its product structure that might be in demand when you create this production order.</span></span>  

7.  <span data-ttu-id="8f838-239">On the **Make Supply Order** page, in the **Make Orders for** field, choose the **All Lines** option, and then choose the **OK** button to create production orders for the second product level of the order.</span><span class="sxs-lookup"><span data-stu-id="8f838-239">On the **Make Supply Order** page, in the **Make Orders for** field, choose the **All Lines** option, and then choose the **OK** button to create production orders for the second product level of the order.</span></span>  

     <span data-ttu-id="8f838-240">Note that the top-level production demand for production order 101001 no longer exists.</span><span class="sxs-lookup"><span data-stu-id="8f838-240">Note that the top-level production demand for production order 101001 no longer exists.</span></span> <span data-ttu-id="8f838-241">This means that the initial production demand for subassemblies has been planned for.</span><span class="sxs-lookup"><span data-stu-id="8f838-241">This means that the initial production demand for subassemblies has been planned for.</span></span>  

     <span data-ttu-id="8f838-242">On the **Order Planning** page, you calculate a plan again in order to plan the bicycle structure.</span><span class="sxs-lookup"><span data-stu-id="8f838-242">On the **Order Planning** page, you calculate a plan again in order to plan the bicycle structure.</span></span>  

8.  <span data-ttu-id="8f838-243">Choose the **Calculate Plan** action to recalculate the plan as instructed by the embedded Help text.</span><span class="sxs-lookup"><span data-stu-id="8f838-243">Choose the **Calculate Plan** action to recalculate the plan as instructed by the embedded Help text.</span></span>  

     <span data-ttu-id="8f838-244">The two new lines represent additional production demand derived from the subassemblies planned in the previous steps.</span><span class="sxs-lookup"><span data-stu-id="8f838-244">The two new lines represent additional production demand derived from the subassemblies planned in the previous steps.</span></span> <span data-ttu-id="8f838-245">It is suggested that you make two production orders to supply the wheel hubs, one for 10 front hubs and one for 10 back hubs.</span><span class="sxs-lookup"><span data-stu-id="8f838-245">It is suggested that you make two production orders to supply the wheel hubs, one for 10 front hubs and one for 10 back hubs.</span></span>  

9. <span data-ttu-id="8f838-246">Choose the **Expand All** action to get an overview of all the demand for the two production orders.</span><span class="sxs-lookup"><span data-stu-id="8f838-246">Choose the **Expand All** action to get an overview of all the demand for the two production orders.</span></span>  

     <span data-ttu-id="8f838-247">The suggested supply plan indicates that a total of four purchase orders will be created for the components.</span><span class="sxs-lookup"><span data-stu-id="8f838-247">The suggested supply plan indicates that a total of four purchase orders will be created for the components.</span></span> <span data-ttu-id="8f838-248">You decide to make the proposed orders.</span><span class="sxs-lookup"><span data-stu-id="8f838-248">You decide to make the proposed orders.</span></span>  

10. <span data-ttu-id="8f838-249">Choose the **Make Orders** action.</span><span class="sxs-lookup"><span data-stu-id="8f838-249">Choose the **Make Orders** action.</span></span>  
11. <span data-ttu-id="8f838-250">In the **Make Orders for** field, select the **All Lines** option, and then choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="8f838-250">In the **Make Orders for** field, select the **All Lines** option, and then choose the **OK** button.</span></span> <span data-ttu-id="8f838-251">Check if additional demand exists for the production of the parent item, the bicycle, which is being sold on sales order 1001.</span><span class="sxs-lookup"><span data-stu-id="8f838-251">Check if additional demand exists for the production of the parent item, the bicycle, which is being sold on sales order 1001.</span></span>  
12. <span data-ttu-id="8f838-252">Choose the **Calculate Plan** action.</span><span class="sxs-lookup"><span data-stu-id="8f838-252">Choose the **Calculate Plan** action.</span></span>  

     <span data-ttu-id="8f838-253">The message indicates that all required items are now supplied.</span><span class="sxs-lookup"><span data-stu-id="8f838-253">The message indicates that all required items are now supplied.</span></span> <span data-ttu-id="8f838-254">Verify the firm planned production orders that are created.</span><span class="sxs-lookup"><span data-stu-id="8f838-254">Verify the firm planned production orders that are created.</span></span>  

13. <span data-ttu-id="8f838-255">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Firm Planned Prod. Orders**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="8f838-255">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Firm Planned Prod. Orders**, and then choose the related link.</span></span>  

     <span data-ttu-id="8f838-256">On the **Firm Planned Prod. Orders** page review how start times and end times of individual orders are scheduled according to the product structure.</span><span class="sxs-lookup"><span data-stu-id="8f838-256">On the **Firm Planned Prod. Orders** page review how start times and end times of individual orders are scheduled according to the product structure.</span></span> <span data-ttu-id="8f838-257">The lowest-level components are produced first.</span><span class="sxs-lookup"><span data-stu-id="8f838-257">The lowest-level components are produced first.</span></span> <span data-ttu-id="8f838-258">Therefore, you must plan multilevel orders as demonstrated in this planning workflow.</span><span class="sxs-lookup"><span data-stu-id="8f838-258">Therefore, you must plan multilevel orders as demonstrated in this planning workflow.</span></span>  

## <a name="see-also"></a><span data-ttu-id="8f838-259">See Also</span><span class="sxs-lookup"><span data-stu-id="8f838-259">See Also</span></span>  
 <span data-ttu-id="8f838-260">[Business Process Walkthroughs](walkthrough-business-process-walkthroughs.md) </span><span class="sxs-lookup"><span data-stu-id="8f838-260">[Business Process Walkthroughs](walkthrough-business-process-walkthroughs.md) </span></span>  
 [<span data-ttu-id="8f838-261">Walkthrough: Planning Supplies Automatically</span><span class="sxs-lookup"><span data-stu-id="8f838-261">Walkthrough: Planning Supplies Automatically</span></span>](walkthrough-planning-supplies-automatically.md)
