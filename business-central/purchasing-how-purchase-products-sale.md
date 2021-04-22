---
title: Purchase Items for a Sale by Creating Purchase Invoices | Microsoft Docs
description: From a sales invoice, to purchase products, you can create a purchase invoice for a vendor or supplier.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: supply planning, sales demand, replenish
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 2d956b7e22e4fe079c47ca8693d717a2b451f146
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 03/31/2021
ms.locfileid: "5772745"
---
# <a name="purchase-items-for-a-sale"></a><span data-ttu-id="9a6b9-103">Purchase Items for a Sale</span><span class="sxs-lookup"><span data-stu-id="9a6b9-103">Purchase Items for a Sale</span></span>
<span data-ttu-id="9a6b9-104">From sales orders and sales invoices, you can use functions to quickly create purchase documents for missing item quantities that are required by the sale.</span><span class="sxs-lookup"><span data-stu-id="9a6b9-104">From sales orders and sales invoices, you can use functions to quickly create purchase documents for missing item quantities that are required by the sale.</span></span> <span data-ttu-id="9a6b9-105">You can use two different functions depending on the document type.</span><span class="sxs-lookup"><span data-stu-id="9a6b9-105">You can use two different functions depending on the document type.</span></span>

> [!Note]
> <span data-ttu-id="9a6b9-106">This functionality is for replenishing sales items into your own inventory.</span><span class="sxs-lookup"><span data-stu-id="9a6b9-106">This functionality is for replenishing sales items into your own inventory.</span></span> <span data-ttu-id="9a6b9-107">To purchase items for direct delivery from your vendor to your customer, you must create a drop shipment.</span><span class="sxs-lookup"><span data-stu-id="9a6b9-107">To purchase items for direct delivery from your vendor to your customer, you must create a drop shipment.</span></span> <span data-ttu-id="9a6b9-108">For more information, see [Make Drop Shipments](sales-how-drop-shipment.md).</span><span class="sxs-lookup"><span data-stu-id="9a6b9-108">For more information, see [Make Drop Shipments](sales-how-drop-shipment.md).</span></span>   

|<span data-ttu-id="9a6b9-109">Function</span><span class="sxs-lookup"><span data-stu-id="9a6b9-109">Function</span></span>|<span data-ttu-id="9a6b9-110">Description</span><span class="sxs-lookup"><span data-stu-id="9a6b9-110">Description</span></span>|
|--------|-----------|
|<span data-ttu-id="9a6b9-111">**Create Purchase Orders**</span><span class="sxs-lookup"><span data-stu-id="9a6b9-111">**Create Purchase Orders**</span></span>|<span data-ttu-id="9a6b9-112">From a sales order, this function creates a purchase order for each vendor of items on the sales order.</span><span class="sxs-lookup"><span data-stu-id="9a6b9-112">From a sales order, this function creates a purchase order for each vendor of items on the sales order.</span></span> <span data-ttu-id="9a6b9-113">You can edit the purchase quantity before you create the purchase orders.</span><span class="sxs-lookup"><span data-stu-id="9a6b9-113">You can edit the purchase quantity before you create the purchase orders.</span></span> <span data-ttu-id="9a6b9-114">Only unavailable sales quantities are suggested.</span><span class="sxs-lookup"><span data-stu-id="9a6b9-114">Only unavailable sales quantities are suggested.</span></span>
|<span data-ttu-id="9a6b9-115">**Create Purchase Invoice**</span><span class="sxs-lookup"><span data-stu-id="9a6b9-115">**Create Purchase Invoice**</span></span>|<span data-ttu-id="9a6b9-116">From a sales order and from a sales invoice, this function creates a purchase invoice for a selected vendor for all lines or selected lines on the sales document.</span><span class="sxs-lookup"><span data-stu-id="9a6b9-116">From a sales order and from a sales invoice, this function creates a purchase invoice for a selected vendor for all lines or selected lines on the sales document.</span></span> <span data-ttu-id="9a6b9-117">The full sales quantity is suggested.</span><span class="sxs-lookup"><span data-stu-id="9a6b9-117">The full sales quantity is suggested.</span></span>|

## <a name="to-create-one-or-more-purchase-orders-from-a-sales-order"></a><span data-ttu-id="9a6b9-118">To create one or more purchase orders from a sales order</span><span class="sxs-lookup"><span data-stu-id="9a6b9-118">To create one or more purchase orders from a sales order</span></span>
<span data-ttu-id="9a6b9-119">To create a purchase order for each unavailable item quantity on the sales order, you use the **Create Purchase Orders** function.</span><span class="sxs-lookup"><span data-stu-id="9a6b9-119">To create a purchase order for each unavailable item quantity on the sales order, you use the **Create Purchase Orders** function.</span></span>

1. <span data-ttu-id="9a6b9-120">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="9a6b9-120">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.</span></span>
2. <span data-ttu-id="9a6b9-121">Open a sales order that you want to purchase items for.</span><span class="sxs-lookup"><span data-stu-id="9a6b9-121">Open a sales order that you want to purchase items for.</span></span>
3. <span data-ttu-id="9a6b9-122">Choose the **Create Purchase Orders** action.</span><span class="sxs-lookup"><span data-stu-id="9a6b9-122">Choose the **Create Purchase Orders** action.</span></span>

    <span data-ttu-id="9a6b9-123">The **Create Purchase Orders** page opens showing a line for each different item on the sales order.</span><span class="sxs-lookup"><span data-stu-id="9a6b9-123">The **Create Purchase Orders** page opens showing a line for each different item on the sales order.</span></span> <span data-ttu-id="9a6b9-124">Lines for both fully available sales quantities and unavailable sales quantities (greyed) are shown by default.</span><span class="sxs-lookup"><span data-stu-id="9a6b9-124">Lines for both fully available sales quantities and unavailable sales quantities (grayed) are shown by default.</span></span> <span data-ttu-id="9a6b9-125">You can choose the **Show Unavailable** action to only see lines for unavailable sales quantities.</span><span class="sxs-lookup"><span data-stu-id="9a6b9-125">You can choose the **Show Unavailable** action to only see lines for unavailable sales quantities.</span></span>

    <span data-ttu-id="9a6b9-126">The **Quantity to Purchase** field contains the unavailable sales quantity by default.</span><span class="sxs-lookup"><span data-stu-id="9a6b9-126">The **Quantity to Purchase** field contains the unavailable sales quantity by default.</span></span>
4. <span data-ttu-id="9a6b9-127">To purchase another quantity than the unavailable sales quantity, edit the value in the **Quantity to Purchase** field.</span><span class="sxs-lookup"><span data-stu-id="9a6b9-127">To purchase another quantity than the unavailable sales quantity, edit the value in the **Quantity to Purchase** field.</span></span>

    > [!NOTE]  
    >   <span data-ttu-id="9a6b9-128">You can also change the **Quantity to Purchase** field on grayed lines even though they represent fully available sales quantities.</span><span class="sxs-lookup"><span data-stu-id="9a6b9-128">You can also change the **Quantity to Purchase** field on grayed lines even though they represent fully available sales quantities.</span></span>
5. <span data-ttu-id="9a6b9-129">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="9a6b9-129">Choose the **OK** button.</span></span>

    <span data-ttu-id="9a6b9-130">A purchase order is created for each vendor of items on the sales order, including any quantity changes that you made on the **Create Purchase Orders** page.</span><span class="sxs-lookup"><span data-stu-id="9a6b9-130">A purchase order is created for each vendor of items on the sales order, including any quantity changes that you made on the **Create Purchase Orders** page.</span></span>
7. <span data-ttu-id="9a6b9-131">Proceed to process the purchase order or orders, for example, by editing or adding purchase order lines.</span><span class="sxs-lookup"><span data-stu-id="9a6b9-131">Proceed to process the purchase order or orders, for example, by editing or adding purchase order lines.</span></span> <span data-ttu-id="9a6b9-132">For more information, see [Record Purchases](purchasing-how-record-purchases.md).</span><span class="sxs-lookup"><span data-stu-id="9a6b9-132">For more information, see [Record Purchases](purchasing-how-record-purchases.md).</span></span>


## <a name="to-create-a-purchase-invoice-from-a-sales-order-or-sales-invoice"></a><span data-ttu-id="9a6b9-133">To create a purchase invoice from a sales order or sales invoice</span><span class="sxs-lookup"><span data-stu-id="9a6b9-133">To create a purchase invoice from a sales order or sales invoice</span></span>
<span data-ttu-id="9a6b9-134">To create a single purchase invoice for one or more lines on a sales document by first selecting which vendor to buy from, you use the **Create Purchase Invoice** function.</span><span class="sxs-lookup"><span data-stu-id="9a6b9-134">To create a single purchase invoice for one or more lines on a sales document by first selecting which vendor to buy from, you use the **Create Purchase Invoice** function.</span></span>

> [!NOTE]  
>   <span data-ttu-id="9a6b9-135">This function creates a purchase invoice for the exact item quantity on the selected sales document.</span><span class="sxs-lookup"><span data-stu-id="9a6b9-135">This function creates a purchase invoice for the exact item quantity on the selected sales document.</span></span> <span data-ttu-id="9a6b9-136">To change the purchase quantity, you must edit the purchase invoice after it is created.</span><span class="sxs-lookup"><span data-stu-id="9a6b9-136">To change the purchase quantity, you must edit the purchase invoice after it is created.</span></span>  

1. <span data-ttu-id="9a6b9-137">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="9a6b9-137">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.</span></span>
2. <span data-ttu-id="9a6b9-138">Open a sales invoice that you want to purchase items for.</span><span class="sxs-lookup"><span data-stu-id="9a6b9-138">Open a sales invoice that you want to purchase items for.</span></span>
3. <span data-ttu-id="9a6b9-139">Select one or more sales invoice lines that you want to use on the purchase invoice.</span><span class="sxs-lookup"><span data-stu-id="9a6b9-139">Select one or more sales invoice lines that you want to use on the purchase invoice.</span></span> <span data-ttu-id="9a6b9-140">To use all the sales invoice lines, select either all of them or do not select any lines.</span><span class="sxs-lookup"><span data-stu-id="9a6b9-140">To use all the sales invoice lines, select either all of them or do not select any lines.</span></span>
4. <span data-ttu-id="9a6b9-141">Choose the **Create Purchase Invoice** action.</span><span class="sxs-lookup"><span data-stu-id="9a6b9-141">Choose the **Create Purchase Invoice** action.</span></span>
5. <span data-ttu-id="9a6b9-142">Select either **All Lines** or **Selected Lines**, and then choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="9a6b9-142">Select either **All Lines** or **Selected Lines**, and then choose the **OK** button.</span></span>  
6. <span data-ttu-id="9a6b9-143">In the list of vendors that appears, select the vendor that you want to buy all the items from, and then choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="9a6b9-143">In the list of vendors that appears, select the vendor that you want to buy all the items from, and then choose the **OK** button.</span></span>

    <span data-ttu-id="9a6b9-144">A purchase invoice is created that contains one, more than one, or all the lines on the sales invoice.</span><span class="sxs-lookup"><span data-stu-id="9a6b9-144">A purchase invoice is created that contains one, more than one, or all the lines on the sales invoice.</span></span>
7. <span data-ttu-id="9a6b9-145">Proceed to process the purchase invoice, for example, by editing or adding purchase invoice lines.</span><span class="sxs-lookup"><span data-stu-id="9a6b9-145">Proceed to process the purchase invoice, for example, by editing or adding purchase invoice lines.</span></span> <span data-ttu-id="9a6b9-146">For more information, see [Record Purchases](purchasing-how-record-purchases.md).</span><span class="sxs-lookup"><span data-stu-id="9a6b9-146">For more information, see [Record Purchases](purchasing-how-record-purchases.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="9a6b9-147">See Also</span><span class="sxs-lookup"><span data-stu-id="9a6b9-147">See Also</span></span>
[<span data-ttu-id="9a6b9-148">Purchasing</span><span class="sxs-lookup"><span data-stu-id="9a6b9-148">Purchasing</span></span>](purchasing-manage-purchasing.md)  
[<span data-ttu-id="9a6b9-149">Record Purchases</span><span class="sxs-lookup"><span data-stu-id="9a6b9-149">Record Purchases</span></span>](purchasing-how-record-purchases.md)  
[<span data-ttu-id="9a6b9-150">Invoice Sales</span><span class="sxs-lookup"><span data-stu-id="9a6b9-150">Invoice Sales</span></span>](sales-how-invoice-sales.md)  
[<span data-ttu-id="9a6b9-151">Register New Vendors</span><span class="sxs-lookup"><span data-stu-id="9a6b9-151">Register New Vendors</span></span>](purchasing-how-register-new-vendors.md)  
<span data-ttu-id="9a6b9-152">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="9a6b9-152">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>


[!INCLUDE[footer-include](includes/footer-banner.md)]