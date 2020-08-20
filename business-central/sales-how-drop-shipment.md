---
title: Link a Sales Order to a Purchase Order for Direct Shipment | Microsoft Docs
description: Describes how to create a sales order linked to a purchase order to enable shipment directly from the vendor to the customer.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: direct shipment
ms.date: 04/01/2020
ms.author: sgroespe
ms.openlocfilehash: 7cc6101fbd63ed7bc4f92372acf651fe8868c7be
ms.sourcegitcommit: 6078bc9b2b571248d779722ce4125f250e7a3922
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 08/07/2020
ms.locfileid: "3666988"
---
# <a name="make-drop-shipments"></a><span data-ttu-id="a090b-103">Make Drop Shipments</span><span class="sxs-lookup"><span data-stu-id="a090b-103">Make Drop Shipments</span></span>
<span data-ttu-id="a090b-104">A drop shipment is the shipment of items from one of your vendors directly to one of your customers.</span><span class="sxs-lookup"><span data-stu-id="a090b-104">A drop shipment is the shipment of items from one of your vendors directly to one of your customers.</span></span>

<span data-ttu-id="a090b-105">When a sales order is marked for drop shipment, and you create a purchase order specifying the customer in the **Ship-to** field, **Customer Address**, you can link the two documents to instruct the vendor to ship directly to the customer.</span><span class="sxs-lookup"><span data-stu-id="a090b-105">When a sales order is marked for drop shipment, and you create a purchase order specifying the customer in the **Ship-to** field, **Customer Address**, you can link the two documents to instruct the vendor to ship directly to the customer.</span></span>
<br><br>  
  
> [!Video https://www.microsoft.com/en-us/videoplayer/embed/RE4mOyM?rel=0]

## <a name="to-create-a-sales-order-for-drop-shipment"></a><span data-ttu-id="a090b-106">To create a sales order for drop shipment</span><span class="sxs-lookup"><span data-stu-id="a090b-106">To create a sales order for drop shipment</span></span>
<span data-ttu-id="a090b-107">To prepare a drop shipment, you create a sales order for an item and indicate on the sales line that the sale requires drop shipment.</span><span class="sxs-lookup"><span data-stu-id="a090b-107">To prepare a drop shipment, you create a sales order for an item and indicate on the sales line that the sale requires drop shipment.</span></span>

1. <span data-ttu-id="a090b-108">Create a sales order for an item.</span><span class="sxs-lookup"><span data-stu-id="a090b-108">Create a sales order for an item.</span></span> <span data-ttu-id="a090b-109">For more information, see [Sell Products](sales-how-sell-products.md).</span><span class="sxs-lookup"><span data-stu-id="a090b-109">For more information, see [Sell Products](sales-how-sell-products.md).</span></span>
2. <span data-ttu-id="a090b-110">On the sales order line for the drop shipment, select the **Drop Shipment** check box.</span><span class="sxs-lookup"><span data-stu-id="a090b-110">On the sales order line for the drop shipment, select the **Drop Shipment** check box.</span></span> <span data-ttu-id="a090b-111">Use the **Choose Columns** function if the field is not visible.</span><span class="sxs-lookup"><span data-stu-id="a090b-111">Use the **Choose Columns** function if the field is not visible.</span></span> <span data-ttu-id="a090b-112">For more information, see [Personalise Your Workspace](ui-personalization-user.md).</span><span class="sxs-lookup"><span data-stu-id="a090b-112">For more information, see [Personalize Your Workspace](ui-personalization-user.md).</span></span>

## <a name="to-create-the-purchase-order-for-drop-shipment"></a><span data-ttu-id="a090b-113">To create the purchase order for drop shipment</span><span class="sxs-lookup"><span data-stu-id="a090b-113">To create the purchase order for drop shipment</span></span>
<span data-ttu-id="a090b-114">To prepare a drop shipment, you indicate on the purchase order that it must be shipped to your customer, not to yourself.</span><span class="sxs-lookup"><span data-stu-id="a090b-114">To prepare a drop shipment, you indicate on the purchase order that it must be shipped to your customer, not to yourself.</span></span>

1. <span data-ttu-id="a090b-115">Create a purchase order.</span><span class="sxs-lookup"><span data-stu-id="a090b-115">Create a purchase order.</span></span> <span data-ttu-id="a090b-116">Do not fill any fields on the lines.</span><span class="sxs-lookup"><span data-stu-id="a090b-116">Do not fill any fields on the lines.</span></span> <span data-ttu-id="a090b-117">For more information, see [Record Purchases](purchasing-how-record-purchases.md).</span><span class="sxs-lookup"><span data-stu-id="a090b-117">For more information, see [Record Purchases](purchasing-how-record-purchases.md).</span></span>
2. <span data-ttu-id="a090b-118">In the **Ship-to** field, select **Customer Address**.</span><span class="sxs-lookup"><span data-stu-id="a090b-118">In the **Ship-to** field, select **Customer Address**.</span></span>
3. <span data-ttu-id="a090b-119">In the **Customer** field, select the customer that you are selling to.</span><span class="sxs-lookup"><span data-stu-id="a090b-119">In the **Customer** field, select the customer that you are selling to.</span></span>
3. <span data-ttu-id="a090b-120">Choose the **Drop Shipments** action, and then choose the **Get Sales Order** action.</span><span class="sxs-lookup"><span data-stu-id="a090b-120">Choose the **Drop Shipments** action, and then choose the **Get Sales Order** action.</span></span>
4. <span data-ttu-id="a090b-121">On the **Sales List** page, select the sales order that you prepared in [To create a sales order for drop shipment](sales-how-drop-shipment.md#to-create-a-sales-order-for-drop-shipment).</span><span class="sxs-lookup"><span data-stu-id="a090b-121">On the **Sales List** page, select the sales order that you prepared in [To create a sales order for drop shipment](sales-how-drop-shipment.md#to-create-a-sales-order-for-drop-shipment).</span></span>
5. <span data-ttu-id="a090b-122">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="a090b-122">Choose the **OK** button.</span></span>

<span data-ttu-id="a090b-123">The line information from the sales order is inserted on the purchase order line(s).</span><span class="sxs-lookup"><span data-stu-id="a090b-123">The line information from the sales order is inserted on the purchase order line(s).</span></span>

<span data-ttu-id="a090b-124">You can now instruct the vendor to ship the items to your customer, for example, by mailing the purchase order as a PDF.</span><span class="sxs-lookup"><span data-stu-id="a090b-124">You can now instruct the vendor to ship the items to your customer, for example, by mailing the purchase order as a PDF.</span></span>     

## <a name="to-create-multiple-purchase-orders-for-drop-shipments"></a><span data-ttu-id="a090b-125">To create multiple purchase orders for drop shipments</span><span class="sxs-lookup"><span data-stu-id="a090b-125">To create multiple purchase orders for drop shipments</span></span>
<span data-ttu-id="a090b-126">You can also use the requisition worksheet to create the purchase order for the vendor.</span><span class="sxs-lookup"><span data-stu-id="a090b-126">You can also use the requisition worksheet to create the purchase order for the vendor.</span></span> <span data-ttu-id="a090b-127">The advantage of using the requisition worksheet is that it can create purchase orders for all outstanding drop shipments, so you don't have to create each one individually.</span><span class="sxs-lookup"><span data-stu-id="a090b-127">The advantage of using the requisition worksheet is that it can create purchase orders for all outstanding drop shipments, so you don't have to create each one individually.</span></span>

1. <span data-ttu-id="a090b-128">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Requistion Worksheets**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="a090b-128">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Requistion Worksheets**, and then choose the related link.</span></span>
2. <span data-ttu-id="a090b-129">Choose the **Drop Shipments** action, and then choose the **Get Sales Order** action.</span><span class="sxs-lookup"><span data-stu-id="a090b-129">Choose the **Drop Shipments** action, and then choose the **Get Sales Order** action.</span></span>
3. <span data-ttu-id="a090b-130">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="a090b-130">Choose the **OK** button.</span></span>
4. <span data-ttu-id="a090b-131">Review the purchase order lines, and in the **Vendor No.** field, select vendor that supplies required goods.</span><span class="sxs-lookup"><span data-stu-id="a090b-131">Review the purchase order lines, and in the **Vendor No.** field, select vendor that supplies required goods.</span></span> 
5. <span data-ttu-id="a090b-132">Choose the **Carry Out Action Message**\* action to convert reviewed lines to a purchase order.</span><span class="sxs-lookup"><span data-stu-id="a090b-132">Choose the **Carry Out Action Message**\* action to convert reviewed lines to a purchase order.</span></span>

## <a name="to-view-the-linked-purchase-order-from-the-sales-order"></a><span data-ttu-id="a090b-133">To view the linked purchase order from the sales order</span><span class="sxs-lookup"><span data-stu-id="a090b-133">To view the linked purchase order from the sales order</span></span>
* <span data-ttu-id="a090b-134">Select the drop-shipment sales order line, choose the **Order** action, choose the **Drop Shipment** action, and then choose the **Purchase Order** action.</span><span class="sxs-lookup"><span data-stu-id="a090b-134">Select the drop-shipment sales order line, choose the **Order** action, choose the **Drop Shipment** action, and then choose the **Purchase Order** action.</span></span>

## <a name="to-post-a-drop-shipment"></a><span data-ttu-id="a090b-135">To post a drop shipment</span><span class="sxs-lookup"><span data-stu-id="a090b-135">To post a drop shipment</span></span>
<span data-ttu-id="a090b-136">After the vendor ships the items, you can post the sales order as shipped.</span><span class="sxs-lookup"><span data-stu-id="a090b-136">After the vendor ships the items, you can post the sales order as shipped.</span></span> <span data-ttu-id="a090b-137">You can also post the purchase order, but only with the **Receive** option until the sales order has been invoiced.</span><span class="sxs-lookup"><span data-stu-id="a090b-137">You can also post the purchase order, but only with the **Receive** option until the sales order has been invoiced.</span></span>

1. <span data-ttu-id="a090b-138">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="a090b-138">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.</span></span>
2. <span data-ttu-id="a090b-139">Open the sales order that you created in [To create a sales order for drop shipment](sales-how-drop-shipment.md#to-create-a-sales-order-for-drop-shipment).</span><span class="sxs-lookup"><span data-stu-id="a090b-139">Open the sales order that you created in [To create a sales order for drop shipment]().</span></span>
3. <span data-ttu-id="a090b-140">In the **Qty. to Ship** field, specify how many of the order quantity to ship, the full or a partial order quantity.</span><span class="sxs-lookup"><span data-stu-id="a090b-140">In the **Qty. to Ship** field, specify how many of the order quantity to ship, the full or a partial order quantity.</span></span>
4. <span data-ttu-id="a090b-141">Choose the **Post** or **Post and Send** action.</span><span class="sxs-lookup"><span data-stu-id="a090b-141">Choose the **Post** or **Post and Send** action.</span></span>
5. <span data-ttu-id="a090b-142">Choose either the **Ship** option to invoice later, or the **Ship and Invoice** option to invoice immediately.</span><span class="sxs-lookup"><span data-stu-id="a090b-142">Choose either the **Ship** option to invoice later, or the **Ship and Invoice** option to invoice immediately.</span></span>

## <a name="see-also"></a><span data-ttu-id="a090b-143">See Also</span><span class="sxs-lookup"><span data-stu-id="a090b-143">See Also</span></span>
[<span data-ttu-id="a090b-144">Create Special Orders</span><span class="sxs-lookup"><span data-stu-id="a090b-144">Create Special Orders</span></span>](sales-how-to-create-special-orders.md)  
[<span data-ttu-id="a090b-145">Purchase Items for a Sale</span><span class="sxs-lookup"><span data-stu-id="a090b-145">Purchase Items for a Sale</span></span>](purchasing-how-purchase-products-sale.md)  
[<span data-ttu-id="a090b-146">Sell Products</span><span class="sxs-lookup"><span data-stu-id="a090b-146">Sell Products</span></span>](sales-how-sell-products.md)  
[<span data-ttu-id="a090b-147">Record Purchases</span><span class="sxs-lookup"><span data-stu-id="a090b-147">Record Purchases</span></span>](purchasing-how-record-purchases.md)  
[<span data-ttu-id="a090b-148">Sales</span><span class="sxs-lookup"><span data-stu-id="a090b-148">Sales</span></span>](sales-manage-sales.md)  
[<span data-ttu-id="a090b-149">Inventory</span><span class="sxs-lookup"><span data-stu-id="a090b-149">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="a090b-150">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="a090b-150">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
