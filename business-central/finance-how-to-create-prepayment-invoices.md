---
title: How to Create Prepayment Invoices | Microsoft Docs
description: Learn how to handle situations where you require prepayment, or your vendor does.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2019
ms.author: sgroespe
ms.openlocfilehash: ee10367990ebb0e60879ac885ad03072dd877c2a
ms.sourcegitcommit: cfc92eefa8b06fb426482f54e393f0e6e222f712
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 12/03/2019
ms.locfileid: "2879744"
---
# <a name="create-prepayment-invoices"></a><span data-ttu-id="0bc8b-103">Create Prepayment Invoices</span><span class="sxs-lookup"><span data-stu-id="0bc8b-103">Create Prepayment Invoices</span></span>
<span data-ttu-id="0bc8b-104">If you require your customers to submit payment before you ship an order to them, or if your vendor requires you to submit payment before they ship an order to you, you can use the prepayment functionality.</span><span class="sxs-lookup"><span data-stu-id="0bc8b-104">If you require your customers to submit payment before you ship an order to them, or if your vendor requires you to submit payment before they ship an order to you, you can use the prepayment functionality.</span></span>  

<span data-ttu-id="0bc8b-105">After you create a sales or purchase order, you can create a prepayment invoice.</span><span class="sxs-lookup"><span data-stu-id="0bc8b-105">After you create a sales or purchase order, you can create a prepayment invoice.</span></span> <span data-ttu-id="0bc8b-106">You can use the default percentages for each sales or purchase line, or you can adjust the amount as necessary.</span><span class="sxs-lookup"><span data-stu-id="0bc8b-106">You can use the default percentages for each sales or purchase line, or you can adjust the amount as necessary.</span></span> <span data-ttu-id="0bc8b-107">For example, you can specify a total amount for the entire order.</span><span class="sxs-lookup"><span data-stu-id="0bc8b-107">For example, you can specify a total amount for the entire order.</span></span>  

<span data-ttu-id="0bc8b-108">The following procedure describes how to invoice a prepayment for a sales orders.</span><span class="sxs-lookup"><span data-stu-id="0bc8b-108">The following procedure describes how to invoice a prepayment for a sales orders.</span></span> <span data-ttu-id="0bc8b-109">The steps are similar for purchase orders.</span><span class="sxs-lookup"><span data-stu-id="0bc8b-109">The steps are similar for purchase orders.</span></span>  

## <a name="to-create-a-prepayment-invoice"></a><span data-ttu-id="0bc8b-110">To create a prepayment invoice</span><span class="sxs-lookup"><span data-stu-id="0bc8b-110">To create a prepayment invoice</span></span>  
1. <span data-ttu-id="0bc8b-111">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="0bc8b-111">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.</span></span>  
2. <span data-ttu-id="0bc8b-112">Create a new sales order.</span><span class="sxs-lookup"><span data-stu-id="0bc8b-112">Create a new sales order.</span></span> <span data-ttu-id="0bc8b-113">For more information, see [sell Products](sales-how-sell-products.md).</span><span class="sxs-lookup"><span data-stu-id="0bc8b-113">For more information, see [sell Products](sales-how-sell-products.md).</span></span>  

    <span data-ttu-id="0bc8b-114">On the **Prepayment** FastTab, the **Prepayment %** field will be filled in automatically if there is a default prepayment percentage on the customer card.</span><span class="sxs-lookup"><span data-stu-id="0bc8b-114">On the **Prepayment** FastTab, the **Prepayment %** field will be filled in automatically if there is a default prepayment percentage on the customer card.</span></span> <span data-ttu-id="0bc8b-115">You can change the contents of the field.</span><span class="sxs-lookup"><span data-stu-id="0bc8b-115">You can change the contents of the field.</span></span> <span data-ttu-id="0bc8b-116">The prepayment percentage is only copied from the header to lines that do not copy the default prepayment percentage from the item.</span><span class="sxs-lookup"><span data-stu-id="0bc8b-116">The prepayment percentage is only copied from the header to lines that do not copy the default prepayment percentage from the item.</span></span>  

    <span data-ttu-id="0bc8b-117">If the **Compress Prepayment** field is selected, lines will be combined on the invoice if:</span><span class="sxs-lookup"><span data-stu-id="0bc8b-117">If the **Compress Prepayment** field is selected, lines will be combined on the invoice if:</span></span>  
    - <span data-ttu-id="0bc8b-118">They have the same general ledger account for prepayments as determined by the general posting setup.</span><span class="sxs-lookup"><span data-stu-id="0bc8b-118">They have the same general ledger account for prepayments as determined by the general posting setup.</span></span>  
    - <span data-ttu-id="0bc8b-119">They have the same dimensions.</span><span class="sxs-lookup"><span data-stu-id="0bc8b-119">They have the same dimensions.</span></span>  

    <span data-ttu-id="0bc8b-120">Leave the field blank if you want to specify a prepayment invoice with one line for each sales order line that has a prepayment percentage.</span><span class="sxs-lookup"><span data-stu-id="0bc8b-120">Leave the field blank if you want to specify a prepayment invoice with one line for each sales order line that has a prepayment percentage.</span></span>  

3. <span data-ttu-id="0bc8b-121">Fill in the sales lines.</span><span class="sxs-lookup"><span data-stu-id="0bc8b-121">Fill in the sales lines.</span></span>  

    <span data-ttu-id="0bc8b-122">If default prepayment percentages have been set up for your items, they are automatically copied to the **Prepayment %** field on the line.</span><span class="sxs-lookup"><span data-stu-id="0bc8b-122">If default prepayment percentages have been set up for your items, they are automatically copied to the **Prepayment %** field on the line.</span></span> <span data-ttu-id="0bc8b-123">Otherwise, the prepayment percentage is copied from the header.</span><span class="sxs-lookup"><span data-stu-id="0bc8b-123">Otherwise, the prepayment percentage is copied from the header.</span></span> <span data-ttu-id="0bc8b-124">You can change the contents of the **Prepayment %** field on the line.</span><span class="sxs-lookup"><span data-stu-id="0bc8b-124">You can change the contents of the **Prepayment %** field on the line.</span></span>  
4. <span data-ttu-id="0bc8b-125">If you want to apply one prepayment percentage to the entire order, change the **Prepayment %** field on the header after filling in the lines.</span><span class="sxs-lookup"><span data-stu-id="0bc8b-125">If you want to apply one prepayment percentage to the entire order, change the **Prepayment %** field on the header after filling in the lines.</span></span>  
5. <span data-ttu-id="0bc8b-126">To view the total prepayment amount, choose the **Statistics** action.</span><span class="sxs-lookup"><span data-stu-id="0bc8b-126">To view the total prepayment amount, choose the **Statistics** action.</span></span>

    <span data-ttu-id="0bc8b-127">If you want to adjust the total prepayment amount for the order, you can change the contents of the **Prepayment Amount** field on the **Sales Order Statistics** page.</span><span class="sxs-lookup"><span data-stu-id="0bc8b-127">If you want to adjust the total prepayment amount for the order, you can change the contents of the **Prepayment Amount** field on the **Sales Order Statistics** page.</span></span>  

    <span data-ttu-id="0bc8b-128">If the **Prices Including GST** field is selected, the **Prepayment Amount Incl. GST** field is editable.</span><span class="sxs-lookup"><span data-stu-id="0bc8b-128">If the **Prices Including VAT** field is selected, the **Prepayment Amount Incl. VAT** field is editable.</span></span>  

    <span data-ttu-id="0bc8b-129">If you change the contents of the **Prepayment Amount** field, the amount will be distributed proportionately between all lines, except those that have **0** in the **Prepayment %** field.</span><span class="sxs-lookup"><span data-stu-id="0bc8b-129">If you change the contents of the **Prepayment Amount** field, the amount will be distributed proportionately between all lines, except those that have **0** in the **Prepayment %** field.</span></span>  
6. <span data-ttu-id="0bc8b-130">To print a test report before posting the prepayment invoice, choose the **Prepayment** action, and then choose the **Prepayment Test Report** action.</span><span class="sxs-lookup"><span data-stu-id="0bc8b-130">To print a test report before posting the prepayment invoice, choose the **Prepayment** action, and then choose the **Prepayment Test Report** action.</span></span>  
7. <span data-ttu-id="0bc8b-131">To post the prepayment invoice, choose the **Prepayment** action, and then choose the **Post Prepayment Invoice** action.</span><span class="sxs-lookup"><span data-stu-id="0bc8b-131">To post the prepayment invoice, choose the **Prepayment** action, and then choose the **Post Prepayment Invoice** action.</span></span>  

    <span data-ttu-id="0bc8b-132">To post and print the prepayment invoice, choose the **Post and Print Prepmt. Invoice** action.</span><span class="sxs-lookup"><span data-stu-id="0bc8b-132">To post and print the prepayment invoice, choose the **Post and Print Prepmt. Invoice** action.</span></span>  

<span data-ttu-id="0bc8b-133">You can issue additional prepayment invoices for the order.</span><span class="sxs-lookup"><span data-stu-id="0bc8b-133">You can issue additional prepayment invoices for the order.</span></span> <span data-ttu-id="0bc8b-134">To do this, increase the prepayment amount on one or more lines, adjust the document date if necessary, and post the prepayment invoice.</span><span class="sxs-lookup"><span data-stu-id="0bc8b-134">To do this, increase the prepayment amount on one or more lines, adjust the document date if necessary, and post the prepayment invoice.</span></span> <span data-ttu-id="0bc8b-135">A new invoice will be created for the difference between the prepayment amounts invoiced so far and the new prepayment amount.</span><span class="sxs-lookup"><span data-stu-id="0bc8b-135">A new invoice will be created for the difference between the prepayment amounts invoiced so far and the new prepayment amount.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="0bc8b-136">If you are located in North America, you cannot change the prepayment percentage after the prepayment invoice has been posted.</span><span class="sxs-lookup"><span data-stu-id="0bc8b-136">If you are located in North America, you cannot change the prepayment percentage after the prepayment invoice has been posted.</span></span> <span data-ttu-id="0bc8b-137">This is prevented in the North American version of [!INCLUDE[d365fin](includes/d365fin_md.md)] because the calculation of US sales tax will otherwise be incorrect.</span><span class="sxs-lookup"><span data-stu-id="0bc8b-137">This is prevented in the North American version of [!INCLUDE[d365fin](includes/d365fin_md.md)] because the calculation of sales tax will otherwise be incorrect.</span></span>  

 <span data-ttu-id="0bc8b-138">When you are ready to post the rest of the invoice, post it as you would post any invoice, and the prepayment amount will automatically be deducted from the amount due.</span><span class="sxs-lookup"><span data-stu-id="0bc8b-138">When you are ready to post the rest of the invoice, post it as you would post any invoice, and the prepayment amount will automatically be deducted from the amount due.</span></span>  

## <a name="see-also"></a><span data-ttu-id="0bc8b-139">See Also</span><span class="sxs-lookup"><span data-stu-id="0bc8b-139">See Also</span></span>  
[<span data-ttu-id="0bc8b-140">Invoicing Prepayments</span><span class="sxs-lookup"><span data-stu-id="0bc8b-140">Invoicing Prepayments</span></span>](finance-invoice-prepayments.md)  
[<span data-ttu-id="0bc8b-141">Walkthrough: Setting Up and Invoicing Sales Prepayments</span><span class="sxs-lookup"><span data-stu-id="0bc8b-141">Walkthrough: Setting Up and Invoicing Sales Prepayments</span></span>](walkthrough-setting-up-and-invoicing-sales-prepayments.md)  
[<span data-ttu-id="0bc8b-142">Finance</span><span class="sxs-lookup"><span data-stu-id="0bc8b-142">Finance</span></span>](finance.md)  
<span data-ttu-id="0bc8b-143">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="0bc8b-143">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
