---
title: How to Combine Shipments on a Single Invoice | Microsoft Docs
description: If you want to invoice more than one shipment at a time, you can use the combined shipments feature.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 757f7cd38a6325df0e8dc0d283d58c42a8ab823e
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 12/17/2020
ms.locfileid: "4748284"
---
# <a name="combine-shipments-on-a-single-invoice"></a><span data-ttu-id="a5829-103">Combine Shipments on a Single Invoice</span><span class="sxs-lookup"><span data-stu-id="a5829-103">Combine Shipments on a Single Invoice</span></span>
<span data-ttu-id="a5829-104">If you want to invoice more than one shipment at a time, you can use the combined shipments feature.</span><span class="sxs-lookup"><span data-stu-id="a5829-104">If you want to invoice more than one shipment at a time, you can use the combined shipments feature.</span></span>  

<span data-ttu-id="a5829-105">Before you can create a combined shipment, more than one sales shipment for the same customer in the same currency must be posted.</span><span class="sxs-lookup"><span data-stu-id="a5829-105">Before you can create a combined shipment, more than one sales shipment for the same customer in the same currency must be posted.</span></span> <span data-ttu-id="a5829-106">In other words, you must have create two or more sales orders and post them as shipped, but not invoiced.</span><span class="sxs-lookup"><span data-stu-id="a5829-106">In other words, you must have create two or more sales orders and post them as shipped, but not invoiced.</span></span> 

## <a name="to-manually-combine-shipments-on-a-single-invoice"></a><span data-ttu-id="a5829-107">To manually combine shipments on a single invoice</span><span class="sxs-lookup"><span data-stu-id="a5829-107">To manually combine shipments on a single invoice</span></span>  
1. <span data-ttu-id="a5829-108">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Invoices**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="a5829-108">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Invoices**, and then choose the related link.</span></span>  
2. <span data-ttu-id="a5829-109">Choose the **New** action.</span><span class="sxs-lookup"><span data-stu-id="a5829-109">Choose the **New** action.</span></span> <span data-ttu-id="a5829-110">For more information, see [Invoice Sales](sales-how-invoice-sales.md).</span><span class="sxs-lookup"><span data-stu-id="a5829-110">For more information, see [Invoice Sales](sales-how-invoice-sales.md).</span></span>
3. <span data-ttu-id="a5829-111">In the **Sell-to Customer No.**</span><span class="sxs-lookup"><span data-stu-id="a5829-111">In the **Sell-to Customer No.**</span></span> <span data-ttu-id="a5829-112">field, enter the customer who will receive the invoice for the shipped items.</span><span class="sxs-lookup"><span data-stu-id="a5829-112">field, enter the customer who will receive the invoice for the shipped items.</span></span>  
4. <span data-ttu-id="a5829-113">On the **Lines** FastTab, choose the **Get Shipment Lines** action.</span><span class="sxs-lookup"><span data-stu-id="a5829-113">On the **Lines** FastTab, choose the **Get Shipment Lines** action.</span></span>  
5. <span data-ttu-id="a5829-114">Select the shipment line that you want to include in the invoice:</span><span class="sxs-lookup"><span data-stu-id="a5829-114">Select the shipment line that you want to include in the invoice:</span></span>  

    - <span data-ttu-id="a5829-115">To insert all lines, select all lines and choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="a5829-115">To insert all lines, select all lines and choose the **OK** button.</span></span>  
    - <span data-ttu-id="a5829-116">To insert specific lines, select the lines and choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="a5829-116">To insert specific lines, select the lines and choose the **OK** button.</span></span> <span data-ttu-id="a5829-117">You can use the Ctrl key to select multiple nonsequential lines.</span><span class="sxs-lookup"><span data-stu-id="a5829-117">You can use the Ctrl key to select multiple nonsequential lines.</span></span>  

    <span data-ttu-id="a5829-118">If an incorrect shipment line was selected or you want to start over, you can simply delete the lines on the invoice and re-run the **Get Shipment Lines** function.</span><span class="sxs-lookup"><span data-stu-id="a5829-118">If an incorrect shipment line was selected or you want to start over, you can simply delete the lines on the invoice and re-run the **Get Shipment Lines** function.</span></span>  
7. <span data-ttu-id="a5829-119">To post the invoice, choose the **Post** action.</span><span class="sxs-lookup"><span data-stu-id="a5829-119">To post the invoice, choose the **Post** action.</span></span>  

## <a name="to-automatically-combine-shipments-on-a-single-invoice"></a><span data-ttu-id="a5829-120">To automatically combine shipments on a single invoice</span><span class="sxs-lookup"><span data-stu-id="a5829-120">To automatically combine shipments on a single invoice</span></span>  
[!INCLUDE[prod_short](includes/prod_short.md)] <span data-ttu-id="a5829-121">will select only sales orders where **Combine Shipments** is chosen.</span><span class="sxs-lookup"><span data-stu-id="a5829-121">will select only sales orders where **Combine Shipments** is chosen.</span></span> 

1. <span data-ttu-id="a5829-122">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Combine Shipments**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="a5829-122">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Combine Shipments**, and then choose the related link.</span></span> <span data-ttu-id="a5829-123">The batch job request page opens.</span><span class="sxs-lookup"><span data-stu-id="a5829-123">The batch job request page opens.</span></span>  
2. <span data-ttu-id="a5829-124">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="a5829-124">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. <span data-ttu-id="a5829-125">Choose the **Post Invoices** check box.</span><span class="sxs-lookup"><span data-stu-id="a5829-125">Choose the **Post Invoices** check box.</span></span>  
4. <span data-ttu-id="a5829-126">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="a5829-126">Choose the **OK** button.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="a5829-127">You will need to manually post the invoices if the **Post Invoices** check box was not selected on the batch job.</span><span class="sxs-lookup"><span data-stu-id="a5829-127">You will need to manually post the invoices if the **Post Invoices** check box was not selected on the batch job.</span></span>  

## <a name="to-remove-open-sales-orders-after-combined-shipment-posting"></a><span data-ttu-id="a5829-128">To remove open sales orders after combined shipment posting</span><span class="sxs-lookup"><span data-stu-id="a5829-128">To remove open sales orders after combined shipment posting</span></span> 
<span data-ttu-id="a5829-129">When shipments are combined on an invoice and posted, a posted sales invoice is created for the invoiced lines.</span><span class="sxs-lookup"><span data-stu-id="a5829-129">When shipments are combined on an invoice and posted, a posted sales invoice is created for the invoiced lines.</span></span> <span data-ttu-id="a5829-130">The **Quantity Invoiced** field on the originating blanket sales order or sales order is updated based on the invoiced quantity.</span><span class="sxs-lookup"><span data-stu-id="a5829-130">The **Quantity Invoiced** field on the originating blanket sales order or sales order is updated based on the invoiced quantity.</span></span>  

<span data-ttu-id="a5829-131">When you invoice shipments in this way, the orders from which the shipments were posted still exist, even if they have been fully shipped and invoiced.</span><span class="sxs-lookup"><span data-stu-id="a5829-131">When you invoice shipments in this way, the orders from which the shipments were posted still exist, even if they have been fully shipped and invoiced.</span></span>   

1. <span data-ttu-id="a5829-132">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Delete Invoiced Sales Orders**, and then select the link.</span><span class="sxs-lookup"><span data-stu-id="a5829-132">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Delete Invoiced Sales Orders**, and then select the link.</span></span>  
2. <span data-ttu-id="a5829-133">Specify in the **No.**</span><span class="sxs-lookup"><span data-stu-id="a5829-133">Specify in the **No.**</span></span> <span data-ttu-id="a5829-134">filter field which sales orders to delete.</span><span class="sxs-lookup"><span data-stu-id="a5829-134">filter field which sales orders to delete.</span></span>  
3. <span data-ttu-id="a5829-135">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="a5829-135">Choose the **OK** button.</span></span>  

<span data-ttu-id="a5829-136">Alternatively, delete individual sales orders manually.</span><span class="sxs-lookup"><span data-stu-id="a5829-136">Alternatively, delete individual sales orders manually.</span></span>  

<span data-ttu-id="a5829-137">Repeat steps 1 through 3 for any other affected documents, such as blanket sales orders.</span><span class="sxs-lookup"><span data-stu-id="a5829-137">Repeat steps 1 through 3 for any other affected documents, such as blanket sales orders.</span></span>

## <a name="see-also"></a><span data-ttu-id="a5829-138">See Also</span><span class="sxs-lookup"><span data-stu-id="a5829-138">See Also</span></span>  
[<span data-ttu-id="a5829-139">Sales</span><span class="sxs-lookup"><span data-stu-id="a5829-139">Sales</span></span>](sales-manage-sales.md)  
<span data-ttu-id="a5829-140">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="a5829-140">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>
