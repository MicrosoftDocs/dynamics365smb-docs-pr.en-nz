---
title: Correct or Cancel a Posted Sales Invoice | Microsoft Docs
description: Describes how to correct, undo, or cancel a posted sales invoice and apply a sales credit memo.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: undo, credit memo, return
ms.date: 08/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: e8e5a4762564d036ac8c0e7bdaf9e13b448d37f4
ms.contentlocale: en-nz
ms.lasthandoff: 03/22/2018

---
# <a name="correct-or-cancel-unpaid-sales-invoices"></a><span data-ttu-id="49f0b-103">Correct or Cancel Unpaid Sales Invoices</span><span class="sxs-lookup"><span data-stu-id="49f0b-103">Correct or Cancel Unpaid Sales Invoices</span></span>
<span data-ttu-id="49f0b-104">You can correct or cancel a posted sales invoice.</span><span class="sxs-lookup"><span data-stu-id="49f0b-104">You can correct or cancel a posted sales invoice.</span></span> <span data-ttu-id="49f0b-105">This is useful if you make a mistake or if the customer requests a change.</span><span class="sxs-lookup"><span data-stu-id="49f0b-105">This is useful if you make a mistake or if the customer requests a change.</span></span>

> [!NOTE]  
>   <span data-ttu-id="49f0b-106">After a posted sales invoice has been partially or fully paid, you cannot correct or cancel it from the posted sales invoice itself.</span><span class="sxs-lookup"><span data-stu-id="49f0b-106">After a posted sales invoice has been partially or fully paid, you cannot correct or cancel it from the posted sales invoice itself.</span></span> <span data-ttu-id="49f0b-107">Instead, you must manually create a sales credit memo to void the sale and reimburse the customer, optionally managed with a sales return order.</span><span class="sxs-lookup"><span data-stu-id="49f0b-107">Instead, you must manually create a sales credit memo to void the sale and reimburse the customer, optionally managed with a sales return order.</span></span> <span data-ttu-id="49f0b-108">For more information, see [Process Sales Returns or Cancellations](sales-how-process-sales-returns-cancellations.md).</span><span class="sxs-lookup"><span data-stu-id="49f0b-108">For more information, see [Process Sales Returns or Cancellations](sales-how-process-sales-returns-cancellations.md).</span></span>

<span data-ttu-id="49f0b-109">In the **Posted Sales Invoice** window, you can choose the **Correct** action or the **Cancel** action to perform the actions that are described in the following table.</span><span class="sxs-lookup"><span data-stu-id="49f0b-109">In the **Posted Sales Invoice** window, you can choose the **Correct** action or the **Cancel** action to perform the actions that are described in the following table.</span></span>

| <span data-ttu-id="49f0b-110">Action</span><span class="sxs-lookup"><span data-stu-id="49f0b-110">Action</span></span> | <span data-ttu-id="49f0b-111">Description</span><span class="sxs-lookup"><span data-stu-id="49f0b-111">Description</span></span> |
| --- | --- |
| <span data-ttu-id="49f0b-112">**Correct**</span><span class="sxs-lookup"><span data-stu-id="49f0b-112">**Correct**</span></span> |<span data-ttu-id="49f0b-113">The posted sales invoice is cancelled.</span><span class="sxs-lookup"><span data-stu-id="49f0b-113">The posted sales invoice is canceled.</span></span> <span data-ttu-id="49f0b-114">A new sales invoice with the same information is created.</span><span class="sxs-lookup"><span data-stu-id="49f0b-114">A new sales invoice with the same information is created.</span></span> <span data-ttu-id="49f0b-115">You can make the correction and then continue the sales process.</span><span class="sxs-lookup"><span data-stu-id="49f0b-115">You can make the correction and then continue the sales process.</span></span> <span data-ttu-id="49f0b-116">The new sales invoice has a different number than the initial sales invoice.</span><span class="sxs-lookup"><span data-stu-id="49f0b-116">The new sales invoice has a different number than the initial sales invoice.</span></span> <span data-ttu-id="49f0b-117">A corrective sales credit memo is automatically created and posted to void the initial posted sales invoice.</span><span class="sxs-lookup"><span data-stu-id="49f0b-117">A corrective sales credit memo is automatically created and posted to void the initial posted sales invoice.</span></span> <span data-ttu-id="49f0b-118">On the initial posted sales invoice, the Cancelled and Paid check boxes are selected.</span><span class="sxs-lookup"><span data-stu-id="49f0b-118">On the initial posted sales invoice, the Canceled and Paid check boxes are selected.</span></span> |
| <span data-ttu-id="49f0b-119">**Cancel**</span><span class="sxs-lookup"><span data-stu-id="49f0b-119">**Cancel**</span></span> |<span data-ttu-id="49f0b-120">The posted sales invoice is cancelled.</span><span class="sxs-lookup"><span data-stu-id="49f0b-120">The posted sales invoice is canceled.</span></span> <span data-ttu-id="49f0b-121">A corrective sales credit memo is automatically created and posted to void the initial posted sales invoice.</span><span class="sxs-lookup"><span data-stu-id="49f0b-121">A corrective sales credit memo is automatically created and posted to void the initial posted sales invoice.</span></span> <span data-ttu-id="49f0b-122">On the initial posted sales invoice, the Cancelled and Paid check boxes are selected.</span><span class="sxs-lookup"><span data-stu-id="49f0b-122">On the initial posted sales invoice, the Canceled and Paid check boxes are selected.</span></span> |

<span data-ttu-id="49f0b-123">When you correct or cancel a posted sales invoice, the corrective sales credit memo is applied to all general ledger and inventory ledger entries that were created when the initial sales invoice was posted.</span><span class="sxs-lookup"><span data-stu-id="49f0b-123">When you correct or cancel a posted sales invoice, the corrective sales credit memo is applied to all general ledger and inventory ledger entries that were created when the initial sales invoice was posted.</span></span> <span data-ttu-id="49f0b-124">This reverses the posted sales invoice in your financial records and leaves the corrective posted sales credit memo for your audit trail.</span><span class="sxs-lookup"><span data-stu-id="49f0b-124">This reverses the posted sales invoice in your financial records and leaves the corrective posted sales credit memo for your audit trail.</span></span>

## <a name="to-correct-a-posted-sales-invoice"></a><span data-ttu-id="49f0b-125">To correct a posted sales invoice</span><span class="sxs-lookup"><span data-stu-id="49f0b-125">To correct a posted sales invoice</span></span>
1. <span data-ttu-id="49f0b-126">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Posted Sales Invoices**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="49f0b-126">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Posted Sales Invoices**, and then choose the related link.</span></span>  
2. <span data-ttu-id="49f0b-127">Select the posted sales invoice that you want to correct.</span><span class="sxs-lookup"><span data-stu-id="49f0b-127">Select the posted sales invoice that you want to correct.</span></span>

    > [!NOTE]  
>   <span data-ttu-id="49f0b-128">If the **Canceled** check box is selected, then you cannot correct the posted sales invoice because it has already been corrected or canceled.</span><span class="sxs-lookup"><span data-stu-id="49f0b-128">If the **Canceled** check box is selected, then you cannot correct the posted sales invoice because it has already been corrected or canceled.</span></span>
3. <span data-ttu-id="49f0b-129">In the **Posted Sales Invoice** window, choose the **Correct** action.</span><span class="sxs-lookup"><span data-stu-id="49f0b-129">In the **Posted Sales Invoice** window, choose the **Correct** action.</span></span>  
4. <span data-ttu-id="49f0b-130">A new sales invoice with the same information is created where you can make the correction.</span><span class="sxs-lookup"><span data-stu-id="49f0b-130">A new sales invoice with the same information is created where you can make the correction.</span></span> <span data-ttu-id="49f0b-131">The **Cancelled** field on the initial posted sales invoice is changed to **Yes**.</span><span class="sxs-lookup"><span data-stu-id="49f0b-131">The **Canceled** field on the initial posted sales invoice is changed to **Yes**.</span></span>

    <span data-ttu-id="49f0b-132">A sales credit memo is automatically created and posted to void the initial posted sales invoice.</span><span class="sxs-lookup"><span data-stu-id="49f0b-132">A sales credit memo is automatically created and posted to void the initial posted sales invoice.</span></span>
5. <span data-ttu-id="49f0b-133">Choose the **Show Corrective Credit Memo** action to view the posted sales credit memo that voids the initial posted sales invoice.</span><span class="sxs-lookup"><span data-stu-id="49f0b-133">Choose the **Show Corrective Credit Memo** action to view the posted sales credit memo that voids the initial posted sales invoice.</span></span>

## <a name="to-cancel-a-posted-sales-invoice"></a><span data-ttu-id="49f0b-134">To cancel a posted sales invoice</span><span class="sxs-lookup"><span data-stu-id="49f0b-134">To cancel a posted sales invoice</span></span>
1. <span data-ttu-id="49f0b-135">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Posted Sales Invoices**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="49f0b-135">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Posted Sales Invoices**, and then choose the related link.</span></span>  
2. <span data-ttu-id="49f0b-136">Select the posted sales invoice that you want to cancel.</span><span class="sxs-lookup"><span data-stu-id="49f0b-136">Select the posted sales invoice that you want to cancel.</span></span>

    > [!NOTE]  
>   <span data-ttu-id="49f0b-137">If the **Canceled** check box is selected, then you cannot cancel the posted sales invoice because it has already been canceled or corrected.</span><span class="sxs-lookup"><span data-stu-id="49f0b-137">If the **Canceled** check box is selected, then you cannot cancel the posted sales invoice because it has already been canceled or corrected.</span></span>
3. <span data-ttu-id="49f0b-138">In the **Posted Sales Invoice** window, choose the **Cancel** action.</span><span class="sxs-lookup"><span data-stu-id="49f0b-138">In the **Posted Sales Invoice** window, choose the **Cancel** action.</span></span>

    <span data-ttu-id="49f0b-139">A sales credit memo is automatically created and posted to void the initial posted sales invoice.</span><span class="sxs-lookup"><span data-stu-id="49f0b-139">A sales credit memo is automatically created and posted to void the initial posted sales invoice.</span></span> <span data-ttu-id="49f0b-140">The **Cancelled** field on the initial posted sales invoice is changed to **Yes**.</span><span class="sxs-lookup"><span data-stu-id="49f0b-140">The **Canceled** field on the initial posted sales invoice is changed to **Yes**.</span></span>
4. <span data-ttu-id="49f0b-141">Choose **Show Corrective Credit Memo** to view the posted sales credit memo that voids the initial posted sales invoice.</span><span class="sxs-lookup"><span data-stu-id="49f0b-141">Choose **Show Corrective Credit Memo** to view the posted sales credit memo that voids the initial posted sales invoice.</span></span>

## <a name="see-also"></a><span data-ttu-id="49f0b-142">See Also</span><span class="sxs-lookup"><span data-stu-id="49f0b-142">See Also</span></span>
[<span data-ttu-id="49f0b-143">Sales</span><span class="sxs-lookup"><span data-stu-id="49f0b-143">Sales</span></span>](sales-manage-sales.md)  
[<span data-ttu-id="49f0b-144">Setting Up Sales</span><span class="sxs-lookup"><span data-stu-id="49f0b-144">Setting Up Sales</span></span>](sales-setup-sales.md)  
[<span data-ttu-id="49f0b-145">Send Documents by Email</span><span class="sxs-lookup"><span data-stu-id="49f0b-145">Send Documents by Email</span></span>](ui-how-send-documents-email.md)  
<span data-ttu-id="49f0b-146">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="49f0b-146">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

