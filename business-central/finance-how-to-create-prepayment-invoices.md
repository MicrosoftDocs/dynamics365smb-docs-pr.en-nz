---
title: How to Create Prepayment Invoices | Microsoft Docs
description: Learn how to handle situations where you require prepayment, or your vendor does.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 06/23/2020
ms.author: edupont
ms.openlocfilehash: 85a5bbd3c1920aaac3e0560737f921c7518d1d32
ms.sourcegitcommit: 63102669366eb26f9c32729848170bc2e5c4d6ae
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 06/25/2020
ms.locfileid: "3503610"
---
# <a name="create-prepayment-invoices"></a><span data-ttu-id="689d8-103">Create Prepayment Invoices</span><span class="sxs-lookup"><span data-stu-id="689d8-103">Create Prepayment Invoices</span></span>

<span data-ttu-id="689d8-104">If you require your customers to submit payment before you ship an order to them, you can use the prepayment functionality.</span><span class="sxs-lookup"><span data-stu-id="689d8-104">If you require your customers to submit payment before you ship an order to them, you can use the prepayment functionality.</span></span> <span data-ttu-id="689d8-105">The same applies if your vendor requires you to submit payment before they ship an order to you.</span><span class="sxs-lookup"><span data-stu-id="689d8-105">The same applies if your vendor requires you to submit payment before they ship an order to you.</span></span>  

<span data-ttu-id="689d8-106">You can start the prepayment process when you create a sales or purchase order.</span><span class="sxs-lookup"><span data-stu-id="689d8-106">You can start the prepayment process when you create a sales or purchase order.</span></span> <span data-ttu-id="689d8-107">If you have a default prepayment percentage for this customer or vendor, that will be included automatically in the resulting prepayment invoice.</span><span class="sxs-lookup"><span data-stu-id="689d8-107">If you have a default prepayment percentage for this customer or vendor, that will be included automatically in the resulting prepayment invoice.</span></span> <span data-ttu-id="689d8-108">You can also specify a prepayment percentage to the entire document.</span><span class="sxs-lookup"><span data-stu-id="689d8-108">You can also specify a prepayment percentage to the entire document.</span></span>

<span data-ttu-id="689d8-109">After you create a sales or purchase order, you can create a prepayment invoice.</span><span class="sxs-lookup"><span data-stu-id="689d8-109">After you create a sales or purchase order, you can create a prepayment invoice.</span></span> <span data-ttu-id="689d8-110">You can use the default percentages for each sales or purchase line, or you can adjust the amount as necessary.</span><span class="sxs-lookup"><span data-stu-id="689d8-110">You can use the default percentages for each sales or purchase line, or you can adjust the amount as necessary.</span></span> <span data-ttu-id="689d8-111">For example, you can specify a total amount for the entire order.</span><span class="sxs-lookup"><span data-stu-id="689d8-111">For example, you can specify a total amount for the entire order.</span></span>  

<span data-ttu-id="689d8-112">The following procedure describes how to invoice a prepayment for a sales order.</span><span class="sxs-lookup"><span data-stu-id="689d8-112">The following procedure describes how to invoice a prepayment for a sales order.</span></span> <span data-ttu-id="689d8-113">The steps are similar for purchase orders.</span><span class="sxs-lookup"><span data-stu-id="689d8-113">The steps are similar for purchase orders.</span></span>  

## <a name="to-create-a-prepayment-invoice"></a><span data-ttu-id="689d8-114">To create a prepayment invoice</span><span class="sxs-lookup"><span data-stu-id="689d8-114">To create a prepayment invoice</span></span>

1. <span data-ttu-id="689d8-115">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="689d8-115">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.</span></span>  
2. <span data-ttu-id="689d8-116">Create a new sales order for the relevant customer.</span><span class="sxs-lookup"><span data-stu-id="689d8-116">Create a new sales order for the relevant customer.</span></span> <span data-ttu-id="689d8-117">For more information, see [Sell Products](sales-how-sell-products.md).</span><span class="sxs-lookup"><span data-stu-id="689d8-117">For more information, see [Sell Products](sales-how-sell-products.md).</span></span>  

    <span data-ttu-id="689d8-118">On the **Prepayment** FastTab, the **Prepayment %** field specifies the percentage to use to calculate the prepayment amount.</span><span class="sxs-lookup"><span data-stu-id="689d8-118">On the **Prepayment** FastTab, the **Prepayment %** field specifies the percentage to use to calculate the prepayment amount.</span></span> <span data-ttu-id="689d8-119">If there is a default prepayment percentage on the customer card, the field is filled in automatically.</span><span class="sxs-lookup"><span data-stu-id="689d8-119">If there is a default prepayment percentage on the customer card, the field is filled in automatically.</span></span> <span data-ttu-id="689d8-120">You can change the percentage.</span><span class="sxs-lookup"><span data-stu-id="689d8-120">You can change the percentage.</span></span> <!--This percentage is applied to lines where the item on that line does not already specify a prepayment percentage. The prepayment percentage is only copied from the header to lines that do not copy the default prepayment percentage from the item.-->  

    <span data-ttu-id="689d8-121">Choose the **Compress Prepayment** field if you want to create lines on the prepayment invoice that combine lines from the sales order if:</span><span class="sxs-lookup"><span data-stu-id="689d8-121">Choose the **Compress Prepayment** field if you want to create lines on the prepayment invoice that combine lines from the sales order if:</span></span>  

    - <span data-ttu-id="689d8-122">They have the same general ledger account for prepayments as determined by the general posting setup.</span><span class="sxs-lookup"><span data-stu-id="689d8-122">They have the same general ledger account for prepayments as determined by the general posting setup.</span></span>  
    - <span data-ttu-id="689d8-123">They have the same dimensions.</span><span class="sxs-lookup"><span data-stu-id="689d8-123">They have the same dimensions.</span></span>  

    <span data-ttu-id="689d8-124">If you want to specify a prepayment invoice with one line for each sales order line that has a prepayment percentage, then do not choose the **Compress Prepayment** field.</span><span class="sxs-lookup"><span data-stu-id="689d8-124">If you want to specify a prepayment invoice with one line for each sales order line that has a prepayment percentage, then do not choose the **Compress Prepayment** field.</span></span>  

    <span data-ttu-id="689d8-125">The due date for the prepayment is calculated automatically based on the value of the **Prepmt. Payment Terms Code**.</span><span class="sxs-lookup"><span data-stu-id="689d8-125">The due date for the prepayment is calculated automatically based on the value of the **Prepmt. Payment Terms Code**.</span></span>

3. <span data-ttu-id="689d8-126">Fill in the sales lines.</span><span class="sxs-lookup"><span data-stu-id="689d8-126">Fill in the sales lines.</span></span>  

    <span data-ttu-id="689d8-127">If you have specified a default prepayment percentage either for the customer or on the **Prepayment** FastTab on this document, this value is copied to each line.</span><span class="sxs-lookup"><span data-stu-id="689d8-127">If you have specified a default prepayment percentage either for the customer or on the **Prepayment** FastTab on this document, this value is copied to each line.</span></span> <span data-ttu-id="689d8-128">You can change the contents of the **Prepayment %** field on the line.</span><span class="sxs-lookup"><span data-stu-id="689d8-128">You can change the contents of the **Prepayment %** field on the line.</span></span>  

4. <span data-ttu-id="689d8-129">To view the total prepayment amount, choose the **Statistics** action.</span><span class="sxs-lookup"><span data-stu-id="689d8-129">To view the total prepayment amount, choose the **Statistics** action.</span></span>

    <span data-ttu-id="689d8-130">If you want to adjust the total prepayment amount for the order, you can change the contents of the **Prepayment Amount** field on the **Sales Order Statistics** page.</span><span class="sxs-lookup"><span data-stu-id="689d8-130">If you want to adjust the total prepayment amount for the order, you can change the contents of the **Prepayment Amount** field on the **Sales Order Statistics** page.</span></span>  

    <span data-ttu-id="689d8-131">If the **Prices Including GST** field is selected, the **Prepayment Amount Incl. GST** field is editable.</span><span class="sxs-lookup"><span data-stu-id="689d8-131">If the **Prices Including VAT** field is selected, the **Prepayment Amount Incl. VAT** field is editable.</span></span>  

    <span data-ttu-id="689d8-132">If you change the contents of the **Prepayment Amount** field, the amount will be distributed proportionately between all lines, except those that have **0** in the **Prepayment %** field.</span><span class="sxs-lookup"><span data-stu-id="689d8-132">If you change the contents of the **Prepayment Amount** field, the amount will be distributed proportionately between all lines, except those that have **0** in the **Prepayment %** field.</span></span>  

5. <span data-ttu-id="689d8-133">To print a test report before posting the prepayment invoice, choose the **Prepayment** action, and then choose the **Prepayment Test Report** action.</span><span class="sxs-lookup"><span data-stu-id="689d8-133">To print a test report before posting the prepayment invoice, choose the **Prepayment** action, and then choose the **Prepayment Test Report** action.</span></span>  
6. <span data-ttu-id="689d8-134">To post the prepayment invoice, choose the **Prepayment** action, and then choose the **Post Prepayment Invoice** action.</span><span class="sxs-lookup"><span data-stu-id="689d8-134">To post the prepayment invoice, choose the **Prepayment** action, and then choose the **Post Prepayment Invoice** action.</span></span>  

    <span data-ttu-id="689d8-135">To post and print the prepayment invoice, choose the **Post and Print Prepmt. Invoice** action.</span><span class="sxs-lookup"><span data-stu-id="689d8-135">To post and print the prepayment invoice, choose the **Post and Print Prepmt. Invoice** action.</span></span>  

<span data-ttu-id="689d8-136">You can issue additional prepayment invoices for the order.</span><span class="sxs-lookup"><span data-stu-id="689d8-136">You can issue additional prepayment invoices for the order.</span></span> <span data-ttu-id="689d8-137">To do this, increase the prepayment amount on one or more lines, adjust the document date if necessary, and post the prepayment invoice.</span><span class="sxs-lookup"><span data-stu-id="689d8-137">To do this, increase the prepayment amount on one or more lines, adjust the document date if necessary, and post the prepayment invoice.</span></span> <span data-ttu-id="689d8-138">A new invoice will be created for the difference between the prepayment amounts invoiced so far and the new prepayment amount.</span><span class="sxs-lookup"><span data-stu-id="689d8-138">A new invoice will be created for the difference between the prepayment amounts invoiced so far and the new prepayment amount.</span></span>  

> [!NOTE]  
> <span data-ttu-id="689d8-139">If you are located in North America, you cannot change the prepayment percentage after the prepayment invoice has been posted.</span><span class="sxs-lookup"><span data-stu-id="689d8-139">If you are located in North America, you cannot change the prepayment percentage after the prepayment invoice has been posted.</span></span> <span data-ttu-id="689d8-140">This is prevented in the North American version of [!INCLUDE[d365fin](includes/d365fin_md.md)] because the calculation of US sales tax will otherwise be incorrect.</span><span class="sxs-lookup"><span data-stu-id="689d8-140">This is prevented in the North American version of [!INCLUDE[d365fin](includes/d365fin_md.md)] because the calculation of sales tax will otherwise be incorrect.</span></span>  

 <span data-ttu-id="689d8-141">When you are ready to post the rest of the invoice, post it as you would post any invoice, and the prepayment amount will automatically be deducted from the amount due.</span><span class="sxs-lookup"><span data-stu-id="689d8-141">When you are ready to post the rest of the invoice, post it as you would post any invoice, and the prepayment amount will automatically be deducted from the amount due.</span></span>  

## <a name="see-also"></a><span data-ttu-id="689d8-142">See Also</span><span class="sxs-lookup"><span data-stu-id="689d8-142">See Also</span></span>

[<span data-ttu-id="689d8-143">Invoicing Prepayments</span><span class="sxs-lookup"><span data-stu-id="689d8-143">Invoicing Prepayments</span></span>](finance-invoice-prepayments.md)  
[<span data-ttu-id="689d8-144">Walkthrough: Setting Up and Invoicing Sales Prepayments</span><span class="sxs-lookup"><span data-stu-id="689d8-144">Walkthrough: Setting Up and Invoicing Sales Prepayments</span></span>](walkthrough-setting-up-and-invoicing-sales-prepayments.md)  
[<span data-ttu-id="689d8-145">Finance</span><span class="sxs-lookup"><span data-stu-id="689d8-145">Finance</span></span>](finance.md)  
<span data-ttu-id="689d8-146">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="689d8-146">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
