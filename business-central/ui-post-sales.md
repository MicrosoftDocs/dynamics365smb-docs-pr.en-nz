---
title: Posting Sales Documents
description: Learn about the different posting functions to post sales documents, and how you can update posted documents.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.reviewer: edupont
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: e59c48c31e897d235c7920f4231313a2332fdf06
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 03/31/2021
ms.locfileid: "5783275"
---
# <a name="posting-sales"></a><span data-ttu-id="a34fb-103">Posting Sales</span><span class="sxs-lookup"><span data-stu-id="a34fb-103">Posting Sales</span></span>

<span data-ttu-id="a34fb-104">Under the **Posting** menu in a sales document, you can choose between the following posting functions:</span><span class="sxs-lookup"><span data-stu-id="a34fb-104">Under the **Posting** menu in a sales document, you can choose between the following posting functions:</span></span>

* <span data-ttu-id="a34fb-105">**Post**</span><span class="sxs-lookup"><span data-stu-id="a34fb-105">**Post**</span></span>
* <span data-ttu-id="a34fb-106">**Post and New**</span><span class="sxs-lookup"><span data-stu-id="a34fb-106">**Post and New**</span></span>
* <span data-ttu-id="a34fb-107">**Post and Send**</span><span class="sxs-lookup"><span data-stu-id="a34fb-107">**Post and Send**</span></span>
* <span data-ttu-id="a34fb-108">**Preview Posting**</span><span class="sxs-lookup"><span data-stu-id="a34fb-108">**Preview Posting**</span></span>
* <span data-ttu-id="a34fb-109">**Post Batch**</span><span class="sxs-lookup"><span data-stu-id="a34fb-109">**Post Batch**</span></span>
* <span data-ttu-id="a34fb-110">**Test Report**</span><span class="sxs-lookup"><span data-stu-id="a34fb-110">**Test Report**</span></span>

> [!NOTE]
> <span data-ttu-id="a34fb-111">For sales orders, you can also see options related to the prepayments functionality.</span><span class="sxs-lookup"><span data-stu-id="a34fb-111">For sales orders, you can also see options related to the prepayments functionality.</span></span> <span data-ttu-id="a34fb-112">For more information, see [Invoicing Prepayments](finance-invoice-prepayments.md).</span><span class="sxs-lookup"><span data-stu-id="a34fb-112">For more information, see [Invoicing Prepayments](finance-invoice-prepayments.md).</span></span>

<span data-ttu-id="a34fb-113">When you have completed all the lines and entered all the information on the sales order, you can post it.</span><span class="sxs-lookup"><span data-stu-id="a34fb-113">When you have completed all the lines and entered all the information on the sales order, you can post it.</span></span> <span data-ttu-id="a34fb-114">This creates a shipment and an invoice.</span><span class="sxs-lookup"><span data-stu-id="a34fb-114">This creates a shipment and an invoice.</span></span>

<span data-ttu-id="a34fb-115">When a sales order is posted, the customer's account, the general ledger, and the item ledger entries are updated.</span><span class="sxs-lookup"><span data-stu-id="a34fb-115">When a sales order is posted, the customer's account, the general ledger, and the item ledger entries are updated.</span></span>

<span data-ttu-id="a34fb-116">For each sales order, a sales entry is created in the **G/L Entry** table.</span><span class="sxs-lookup"><span data-stu-id="a34fb-116">For each sales order, a sales entry is created in the **G/L Entry** table.</span></span> <span data-ttu-id="a34fb-117">An entry is also created in the customer's account in the **Cust. Ledger Entry** table and a general ledger entry is created in the relevant receivables account.</span><span class="sxs-lookup"><span data-stu-id="a34fb-117">An entry is also created in the customer's account in the **Cust. Ledger Entry** table and a general ledger entry is created in the relevant receivables account.</span></span> <span data-ttu-id="a34fb-118">In addition, posting the order may result in a GST entry and a general ledger entry for the discount amount.</span><span class="sxs-lookup"><span data-stu-id="a34fb-118">In addition, posting the order may result in a VAT entry and a general ledger entry for the discount amount.</span></span> <span data-ttu-id="a34fb-119">Whether an entry for the discount is posted depends on the contents of the **Discount Posting** field on the **Sales & Receivables Setup** page.</span><span class="sxs-lookup"><span data-stu-id="a34fb-119">Whether an entry for the discount is posted depends on the contents of the **Discount Posting** field on the **Sales & Receivables Setup** page.</span></span>

<span data-ttu-id="a34fb-120">For each sales order line, an item ledger entry will be created in the **Item Ledger Entry** table (if the sales lines contain item numbers) or a general ledger entry will be created in the **G/L Entry** table (if the sales lines contain a general ledger account).</span><span class="sxs-lookup"><span data-stu-id="a34fb-120">For each sales order line, an item ledger entry will be created in the **Item Ledger Entry** table (if the sales lines contain item numbers) or a general ledger entry will be created in the **G/L Entry** table (if the sales lines contain a general ledger account).</span></span> <span data-ttu-id="a34fb-121">In addition to this, sales orders are always recorded in the **Sales Shipment Header** and **Sales Invoice Header** tables.</span><span class="sxs-lookup"><span data-stu-id="a34fb-121">In addition to this, sales orders are always recorded in the **Sales Shipment Header** and **Sales Invoice Header** tables.</span></span>

> [!IMPORTANT]  
> <span data-ttu-id="a34fb-122">When you post an order, you can create both a shipment and an invoice.</span><span class="sxs-lookup"><span data-stu-id="a34fb-122">When you post an order, you can create both a shipment and an invoice.</span></span> <span data-ttu-id="a34fb-123">These can be done at the same time or independently.</span><span class="sxs-lookup"><span data-stu-id="a34fb-123">These can be done at the same time or independently.</span></span> <span data-ttu-id="a34fb-124">You can also create a partial shipment and a partial invoice by completing the **Qty. to Ship** and **Qty. to Invoice** fields on the individual sales order lines before you post.</span><span class="sxs-lookup"><span data-stu-id="a34fb-124">You can also create a partial shipment and a partial invoice by completing the **Qty. to Ship** and **Qty. to Invoice** fields on the individual sales order lines before you post.</span></span> <span data-ttu-id="a34fb-125">Note that you cannot create an invoice for something that is not shipped.</span><span class="sxs-lookup"><span data-stu-id="a34fb-125">Note that you cannot create an invoice for something that is not shipped.</span></span> <span data-ttu-id="a34fb-126">That is, before you can invoice, you must have recorded a shipment, or you must choose to ship and invoice at the same time.</span><span class="sxs-lookup"><span data-stu-id="a34fb-126">That is, before you can invoice, you must have recorded a shipment, or you must choose to ship and invoice at the same time.</span></span>

<span data-ttu-id="a34fb-127">You can either post, or post and send.</span><span class="sxs-lookup"><span data-stu-id="a34fb-127">You can either post, or post and send.</span></span> <span data-ttu-id="a34fb-128">If you choose to post and send, a PDF file is generated that you can then send.</span><span class="sxs-lookup"><span data-stu-id="a34fb-128">If you choose to post and send, a PDF file is generated that you can then send.</span></span> <span data-ttu-id="a34fb-129">You can also choose the **Post Batch** function, which lets you post several orders at the same time.</span><span class="sxs-lookup"><span data-stu-id="a34fb-129">You can also choose the **Post Batch** function, which lets you post several orders at the same time.</span></span> <span data-ttu-id="a34fb-130">For more information, see [Post Multiple Documents at the Same Time](ui-batch-posting.md).</span><span class="sxs-lookup"><span data-stu-id="a34fb-130">For more information, see [Post Multiple Documents at the Same Time](ui-batch-posting.md).</span></span>

## <a name="viewing-ledger-entries"></a><span data-ttu-id="a34fb-131">Viewing Ledger Entries</span><span class="sxs-lookup"><span data-stu-id="a34fb-131">Viewing Ledger Entries</span></span>

<span data-ttu-id="a34fb-132">When the posting is completed, the posted sales lines are removed from the order.</span><span class="sxs-lookup"><span data-stu-id="a34fb-132">When the posting is completed, the posted sales lines are removed from the order.</span></span> <span data-ttu-id="a34fb-133">A message tells you when the posting is completed.</span><span class="sxs-lookup"><span data-stu-id="a34fb-133">A message tells you when the posting is completed.</span></span> <span data-ttu-id="a34fb-134">After this, you will be able to see the posted entries in the various pages that contain posted entries, such as the **Cust. Ledger Entries**, **G/L Entries**, **Item Ledger Entries**, **Posted Sales Shipments**, and **Posted Sales Invoices** pages.</span><span class="sxs-lookup"><span data-stu-id="a34fb-134">After this, you will be able to see the posted entries in the various pages that contain posted entries, such as the **Cust. Ledger Entries**, **G/L Entries**, **Item Ledger Entries**, **Posted Sales Shipments**, and **Posted Sales Invoices** pages.</span></span>  

<span data-ttu-id="a34fb-135">In most cases, you can open ledger entries from the affected card or document.</span><span class="sxs-lookup"><span data-stu-id="a34fb-135">In most cases, you can open ledger entries from the affected card or document.</span></span> <span data-ttu-id="a34fb-136">For example, on the **Customer Card** page, choose the **Ledger Entries** action.</span><span class="sxs-lookup"><span data-stu-id="a34fb-136">For example, on the **Customer Card** page, choose the **Ledger Entries** action.</span></span>

## <a name="editing-ledger-entries"></a><span data-ttu-id="a34fb-137">Editing Ledger Entries</span><span class="sxs-lookup"><span data-stu-id="a34fb-137">Editing Ledger Entries</span></span>

<span data-ttu-id="a34fb-138">You can edit certain fields on posted purchase documents, such as the **Package Tracking No.**</span><span class="sxs-lookup"><span data-stu-id="a34fb-138">You can edit certain fields on posted purchase documents, such as the **Package Tracking No.**</span></span> <span data-ttu-id="a34fb-139">field.</span><span class="sxs-lookup"><span data-stu-id="a34fb-139">field.</span></span> <span data-ttu-id="a34fb-140">For more information, see [Edit Posted Documents](across-edit-posted-document.md).</span><span class="sxs-lookup"><span data-stu-id="a34fb-140">For more information, see [Edit Posted Documents](across-edit-posted-document.md).</span></span> <span data-ttu-id="a34fb-141">For more critical fields that affect the auditing trail, you must reverse or undo posting.</span><span class="sxs-lookup"><span data-stu-id="a34fb-141">For more critical fields that affect the auditing trail, you must reverse or undo posting.</span></span> <span data-ttu-id="a34fb-142">For more information, see [Reverse Journal Postings and Undo Receipts/Shipments](finance-how-reverse-journal-posting.md).</span><span class="sxs-lookup"><span data-stu-id="a34fb-142">For more information, see [Reverse Journal Postings and Undo Receipts/Shipments](finance-how-reverse-journal-posting.md).</span></span>

## <a name="see-related-training-at-microsoft-learn"></a><span data-ttu-id="a34fb-143">See Related Training at [Microsoft Learn](/learn/modules/ship-invoice-items-dynamics-365-business-central/index)</span><span class="sxs-lookup"><span data-stu-id="a34fb-143">See Related Training at [Microsoft Learn](/learn/modules/ship-invoice-items-dynamics-365-business-central/index)</span></span>

## <a name="see-also"></a><span data-ttu-id="a34fb-144">See Also</span><span class="sxs-lookup"><span data-stu-id="a34fb-144">See Also</span></span>

[<span data-ttu-id="a34fb-145">Sales</span><span class="sxs-lookup"><span data-stu-id="a34fb-145">Sales</span></span>](sales-manage-sales.md)  
[<span data-ttu-id="a34fb-146">Post Multiple Documents at the Same Time</span><span class="sxs-lookup"><span data-stu-id="a34fb-146">Post Multiple Documents at the Same Time</span></span>](ui-batch-posting.md)  
[<span data-ttu-id="a34fb-147">Edit Posted Documents</span><span class="sxs-lookup"><span data-stu-id="a34fb-147">Edit Posted Documents</span></span>](across-edit-posted-document.md)  
[<span data-ttu-id="a34fb-148">Send Documents by Email</span><span class="sxs-lookup"><span data-stu-id="a34fb-148">Send Documents by Email</span></span>](ui-how-send-documents-email.md)  
[<span data-ttu-id="a34fb-149">Correct or Cancel Unpaid Sales Invoices</span><span class="sxs-lookup"><span data-stu-id="a34fb-149">Correct or Cancel Unpaid Sales Invoices</span></span>](sales-how-correct-cancel-sales-invoice.md)  
[<span data-ttu-id="a34fb-150">Finding Pages and Information with Tell Me</span><span class="sxs-lookup"><span data-stu-id="a34fb-150">Finding Pages and Information with Tell Me</span></span>](ui-search.md)  
<span data-ttu-id="a34fb-151">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="a34fb-151">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>

[!INCLUDE[footer-include](includes/footer-banner.md)]  
