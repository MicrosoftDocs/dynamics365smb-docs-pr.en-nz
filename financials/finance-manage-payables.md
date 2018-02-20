---
title: Managing Accounts Payable| Microsoft Docs
description: Overview of how Financials helps you manage accounts payable (AP), including vendor payments, creditors, debt, and balance due.
services: project-madeira
documentationcenter: 
author: bholtorf
manager: edupont
editor: 
ms.service: dynamics365-financials
ms.workload: na
ms.tgt_pltfrm: na
ms.devlang: na
ms.topic: article
ms.search.keywords: vendor payment, creditor, debt, balance due, AP
ms.date: 06/02/2017
ms.author: bholtorf
ms.translationtype: HT
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: 654c34bc09967247617bda7be070a9c0ec6f635d
ms.contentlocale: en-nz
ms.lasthandoff: 01/30/2018

---
# <a name="managing-payables"></a><span data-ttu-id="ce1f2-103">Managing Payables</span><span class="sxs-lookup"><span data-stu-id="ce1f2-103">Managing Payables</span></span>
[!INCLUDE[d365fin](includes/d365fin_md.md)] <span data-ttu-id="ce1f2-104"> has what you need to effectively manage accounts payable.</span><span class="sxs-lookup"><span data-stu-id="ce1f2-104">has what you need to effectively manage accounts payable.</span></span>  

## <a name="payments"></a><span data-ttu-id="ce1f2-105">Payments</span><span class="sxs-lookup"><span data-stu-id="ce1f2-105">Payments</span></span>
<span data-ttu-id="ce1f2-106">It's easy to prioritise payments, account for penalties for overdue payments, and handle discounts for early payments.</span><span class="sxs-lookup"><span data-stu-id="ce1f2-106">It's easy to prioritize payments, account for penalties for overdue payments, and handle discounts for early payments.</span></span>

<span data-ttu-id="ce1f2-107">You can record payments in a general journal, and then print checks before posting the payment journal.</span><span class="sxs-lookup"><span data-stu-id="ce1f2-107">You can record payments in a general journal, and then print checks before posting the payment journal.</span></span>

<span data-ttu-id="ce1f2-108">You can apply payments to close invoices when you post the payment, or after you post the payment.</span><span class="sxs-lookup"><span data-stu-id="ce1f2-108">You can apply payments to close invoices when you post the payment, or after you post the payment.</span></span> <span data-ttu-id="ce1f2-109">The **Application Method** specified for the vendor (on the **Vendor Card**) determines whether you apply the payment manually, or automatically.</span><span class="sxs-lookup"><span data-stu-id="ce1f2-109">The **Application Method** specified for the vendor (on the **Vendor Card**) determines whether you apply the payment manually, or automatically.</span></span> <span data-ttu-id="ce1f2-110">You can always apply transactions manually.</span><span class="sxs-lookup"><span data-stu-id="ce1f2-110">You can always apply transactions manually.</span></span> <span data-ttu-id="ce1f2-111">However, if the application method for the vendor is **Apply to Oldest**, and you do not specify a document to apply the payment to, the payment is applied to the oldest open entry for the vendor.</span><span class="sxs-lookup"><span data-stu-id="ce1f2-111">However, if the application method for the vendor is **Apply to Oldest**, and you do not specify a document to apply the payment to, the payment is applied to the oldest open entry for the vendor.</span></span>

## <a name="suggest-vendor-payments"></a><span data-ttu-id="ce1f2-112">Suggest Vendor Payments</span><span class="sxs-lookup"><span data-stu-id="ce1f2-112">Suggest Vendor Payments</span></span>
[!INCLUDE[d365fin](includes/d365fin_md.md)] <span data-ttu-id="ce1f2-113"> can suggest various payments to vendors, such as payments that will be due soon, or payments where a discount is available.</span><span class="sxs-lookup"><span data-stu-id="ce1f2-113">can suggest various payments to vendors, such as payments that will be due soon, or payments where a discount is available.</span></span> <span data-ttu-id="ce1f2-114">The payment suggestion can consider an amount that you specify as available funds for payment, and eligibility for payment discounts.</span><span class="sxs-lookup"><span data-stu-id="ce1f2-114">The payment suggestion can consider an amount that you specify as available funds for payment, and eligibility for payment discounts.</span></span>

## <a name="issue-checks"></a><span data-ttu-id="ce1f2-115">Issue Checks</span><span class="sxs-lookup"><span data-stu-id="ce1f2-115">Issue Checks</span></span>
[!INCLUDE[d365fin](includes/d365fin_md.md)] <span data-ttu-id="ce1f2-116"> lets you issue checks to vendors manually and electronically.</span><span class="sxs-lookup"><span data-stu-id="ce1f2-116">lets you issue checks to vendors manually and electronically.</span></span> <span data-ttu-id="ce1f2-117">You do both in the **Payment Journals** window, where you can also void checks and view check ledger entries.</span><span class="sxs-lookup"><span data-stu-id="ce1f2-117">You do both in the **Payment Journals** window, where you can also void checks and view check ledger entries.</span></span>

## <a name="export-payments-to-a-bank-file"></a><span data-ttu-id="ce1f2-118">Export Payments to a Bank File</span><span class="sxs-lookup"><span data-stu-id="ce1f2-118">Export Payments to a Bank File</span></span>
<span data-ttu-id="ce1f2-119">When you are ready to pay a vendor, from the **Payment Journal** window you can export a file with the payment information from the journal lines.</span><span class="sxs-lookup"><span data-stu-id="ce1f2-119">When you are ready to pay a vendor, from the **Payment Journal** window you can export a file with the payment information from the journal lines.</span></span> <span data-ttu-id="ce1f2-120">You can then upload the file to your electronic bank to process the money transfers.</span><span class="sxs-lookup"><span data-stu-id="ce1f2-120">You can then upload the file to your electronic bank to process the money transfers.</span></span>

<span data-ttu-id="ce1f2-121">If you do not want to post a payment journal line for an exported payment, for example because you are waiting for the bank to confirm the transaction, just delete the journal line.</span><span class="sxs-lookup"><span data-stu-id="ce1f2-121">If you do not want to post a payment journal line for an exported payment, for example because you are waiting for the bank to confirm the transaction, just delete the journal line.</span></span> <span data-ttu-id="ce1f2-122">Later, when you create a payment journal line to pay the remaining amount on the invoice, the **Total Exported Amount** field shows how much of the payment amount has already been exported.</span><span class="sxs-lookup"><span data-stu-id="ce1f2-122">Later, when you create a payment journal line to pay the remaining amount on the invoice, the **Total Exported Amount** field shows how much of the payment amount has already been exported.</span></span> <span data-ttu-id="ce1f2-123">Also, you can find detailed information about the exported total by choosing the **Credit Transfer Reg. Entries** button.</span><span class="sxs-lookup"><span data-stu-id="ce1f2-123">Also, you can find detailed information about the exported total by choosing the **Credit Transfer Reg. Entries** button.</span></span>

<span data-ttu-id="ce1f2-124">If you wait to post payments until after your bank confirms that it has processed transactions, there are two ways to avoid accidently re-exporting payments for open documents:</span><span class="sxs-lookup"><span data-stu-id="ce1f2-124">If you wait to post payments until after your bank confirms that it has processed transactions, there are two ways to avoid accidently re-exporting payments for open documents:</span></span>  

* <span data-ttu-id="ce1f2-125">In a payment journal with suggested payment lines, sort on either the **Exported to Payment File** or **Total Exported Amount** columns, and then delete payment suggestions for open invoices for which payments have already been made and you do not want to make payments for.</span><span class="sxs-lookup"><span data-stu-id="ce1f2-125">In a payment journal with suggested payment lines, sort on either the **Exported to Payment File** or **Total Exported Amount** columns, and then delete payment suggestions for open invoices for which payments have already been made and you do not want to make payments for.</span></span>

    <span data-ttu-id="ce1f2-126">**Note** You might have to add these columns to the list.</span><span class="sxs-lookup"><span data-stu-id="ce1f2-126">**Note** You might have to add these columns to the list.</span></span> <span data-ttu-id="ce1f2-127">For more information, see [Personalising Your Workspace](ui-personalization-user.md).</span><span class="sxs-lookup"><span data-stu-id="ce1f2-127">For more information, see [Personalizing Your Workspace](ui-personalization-user.md).</span></span>  
* <span data-ttu-id="ce1f2-128">Alternatively, on the **Suggest Vendor Payments** batch job, where you specify the payments to include in the payment journal, you can specify not to insert journal lines for payments that have already been exported by choosing the **Skip Exported Payments** check box.</span><span class="sxs-lookup"><span data-stu-id="ce1f2-128">Alternatively, on the **Suggest Vendor Payments** batch job, where you specify the payments to include in the payment journal, you can specify not to insert journal lines for payments that have already been exported by choosing the **Skip Exported Payments** check box.</span></span>

## <a name="see-also"></a><span data-ttu-id="ce1f2-129">See Also</span><span class="sxs-lookup"><span data-stu-id="ce1f2-129">See Also</span></span>
[<span data-ttu-id="ce1f2-130">Payment Methods</span><span class="sxs-lookup"><span data-stu-id="ce1f2-130">Payment Methods</span></span>](finance-payment-methods.md)  
[<span data-ttu-id="ce1f2-131">Finance</span><span class="sxs-lookup"><span data-stu-id="ce1f2-131">Finance</span></span>](finance.md)  
<span data-ttu-id="ce1f2-132">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="ce1f2-132">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

