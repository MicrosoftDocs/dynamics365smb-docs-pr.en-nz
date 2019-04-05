---
title: Managing Accounts Payable| Microsoft Docs
description: Overview of how to manage accounts payable (AP), including vendor payments, creditors, debt, and balance due.
services: project-madeira
documentationcenter: ''
author: bholtorf
manager: edupont
editor: ''
ms.service: dynamics365-business-central
ms.workload: na
ms.tgt_pltfrm: na
ms.devlang: na
ms.topic: article
ms.search.keywords: vendor payment, creditor, debt, balance due, AP
ms.date: 10/01/2018
ms.author: bholtorf
redirect_url: finance-set-up-cost-accounting
ms.openlocfilehash: abf7e9cf01c8d394a022e384584e32e78c754639
ms.sourcegitcommit: 1bcfaa99ea302e6b84b8361ca02730b135557fc1
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 03/08/2019
ms.locfileid: "822009"
---
# <a name="managing-payables"></a><span data-ttu-id="5ed5d-103">Managing Payables</span><span class="sxs-lookup"><span data-stu-id="5ed5d-103">Managing Payables</span></span>
[!INCLUDE[d365fin](includes/d365fin_md.md)] <span data-ttu-id="5ed5d-104">has what you need to effectively manage accounts payable.</span><span class="sxs-lookup"><span data-stu-id="5ed5d-104">has what you need to effectively manage accounts payable.</span></span>  

## <a name="payments"></a><span data-ttu-id="5ed5d-105">Payments</span><span class="sxs-lookup"><span data-stu-id="5ed5d-105">Payments</span></span>
<span data-ttu-id="5ed5d-106">It's easy to prioritise payments, account for penalties for overdue payments, and handle discounts for early payments.</span><span class="sxs-lookup"><span data-stu-id="5ed5d-106">It's easy to prioritize payments, account for penalties for overdue payments, and handle discounts for early payments.</span></span>

<span data-ttu-id="5ed5d-107">You can record payments in a general journal, and then print checks before posting the payment journal.</span><span class="sxs-lookup"><span data-stu-id="5ed5d-107">You can record payments in a general journal, and then print checks before posting the payment journal.</span></span>

<span data-ttu-id="5ed5d-108">You can apply payments to close invoices when you post the payment, or after you post the payment.</span><span class="sxs-lookup"><span data-stu-id="5ed5d-108">You can apply payments to close invoices when you post the payment, or after you post the payment.</span></span> <span data-ttu-id="5ed5d-109">The **Application Method** specified for the vendor (on the **Vendor Card**) determines whether you apply the payment manually, or automatically.</span><span class="sxs-lookup"><span data-stu-id="5ed5d-109">The **Application Method** specified for the vendor (on the **Vendor Card**) determines whether you apply the payment manually, or automatically.</span></span> <span data-ttu-id="5ed5d-110">You can always apply transactions manually.</span><span class="sxs-lookup"><span data-stu-id="5ed5d-110">You can always apply transactions manually.</span></span> <span data-ttu-id="5ed5d-111">However, if the application method for the vendor is **Apply to Oldest**, and you do not specify a document to apply the payment to, the payment is applied to the oldest open entry for the vendor.</span><span class="sxs-lookup"><span data-stu-id="5ed5d-111">However, if the application method for the vendor is **Apply to Oldest**, and you do not specify a document to apply the payment to, the payment is applied to the oldest open entry for the vendor.</span></span>

## <a name="suggest-vendor-payments"></a><span data-ttu-id="5ed5d-112">Suggest Vendor Payments</span><span class="sxs-lookup"><span data-stu-id="5ed5d-112">Suggest Vendor Payments</span></span>
[!INCLUDE[d365fin](includes/d365fin_md.md)] <span data-ttu-id="5ed5d-113">can suggest various payments to vendors, such as payments that will be due soon, or payments where a discount is available.</span><span class="sxs-lookup"><span data-stu-id="5ed5d-113">can suggest various payments to vendors, such as payments that will be due soon, or payments where a discount is available.</span></span> <span data-ttu-id="5ed5d-114">The payment suggestion can consider an amount that you specify as available funds for payment, and eligibility for payment discounts.</span><span class="sxs-lookup"><span data-stu-id="5ed5d-114">The payment suggestion can consider an amount that you specify as available funds for payment, and eligibility for payment discounts.</span></span>

## <a name="issue-checks"></a><span data-ttu-id="5ed5d-115">Issue Checks</span><span class="sxs-lookup"><span data-stu-id="5ed5d-115">Issue Checks</span></span>
[!INCLUDE[d365fin](includes/d365fin_md.md)] <span data-ttu-id="5ed5d-116">lets you issue checks to vendors manually and electronically.</span><span class="sxs-lookup"><span data-stu-id="5ed5d-116">lets you issue checks to vendors manually and electronically.</span></span> <span data-ttu-id="5ed5d-117">You do both on the **Payment Journals** page, where you can also void cheques and view cheque ledger entries.</span><span class="sxs-lookup"><span data-stu-id="5ed5d-117">You do both on the **Payment Journals** page, where you can also void checks and view check ledger entries.</span></span>

## <a name="export-payments-to-a-bank-file"></a><span data-ttu-id="5ed5d-118">Export Payments to a Bank File</span><span class="sxs-lookup"><span data-stu-id="5ed5d-118">Export Payments to a Bank File</span></span>
<span data-ttu-id="5ed5d-119">When you are ready to pay a vendor, from the **Payment Journal** page you can export a file with the payment information from the journal lines.</span><span class="sxs-lookup"><span data-stu-id="5ed5d-119">When you are ready to pay a vendor, from the **Payment Journal** page you can export a file with the payment information from the journal lines.</span></span> <span data-ttu-id="5ed5d-120">You can then upload the file to your electronic bank to process the money transfers.</span><span class="sxs-lookup"><span data-stu-id="5ed5d-120">You can then upload the file to your electronic bank to process the money transfers.</span></span>

<span data-ttu-id="5ed5d-121">If you do not want to post a payment journal line for an exported payment, for example because you are waiting for the bank to confirm the transaction, just delete the journal line.</span><span class="sxs-lookup"><span data-stu-id="5ed5d-121">If you do not want to post a payment journal line for an exported payment, for example because you are waiting for the bank to confirm the transaction, just delete the journal line.</span></span> <span data-ttu-id="5ed5d-122">Later, when you create a payment journal line to pay the remaining amount on the invoice, the **Total Exported Amount** field shows how much of the payment amount has already been exported.</span><span class="sxs-lookup"><span data-stu-id="5ed5d-122">Later, when you create a payment journal line to pay the remaining amount on the invoice, the **Total Exported Amount** field shows how much of the payment amount has already been exported.</span></span> <span data-ttu-id="5ed5d-123">Also, you can find detailed information about the exported total by choosing the **Credit Transfer Reg. Entries** button.</span><span class="sxs-lookup"><span data-stu-id="5ed5d-123">Also, you can find detailed information about the exported total by choosing the **Credit Transfer Reg. Entries** button.</span></span>

<span data-ttu-id="5ed5d-124">If you wait to post payments until after your bank confirms that it has processed transactions, there are two ways to avoid accidentally re-exporting payments for open documents:</span><span class="sxs-lookup"><span data-stu-id="5ed5d-124">If you wait to post payments until after your bank confirms that it has processed transactions, there are two ways to avoid accidentally re-exporting payments for open documents:</span></span>  

* <span data-ttu-id="5ed5d-125">In a payment journal with suggested payment lines, sort on either the **Exported to Payment File** or **Total Exported Amount** columns, and then delete payment suggestions for open invoices for which payments have already been made and you do not want to make payments for.</span><span class="sxs-lookup"><span data-stu-id="5ed5d-125">In a payment journal with suggested payment lines, sort on either the **Exported to Payment File** or **Total Exported Amount** columns, and then delete payment suggestions for open invoices for which payments have already been made and you do not want to make payments for.</span></span>

    <span data-ttu-id="5ed5d-126">**Note** You might have to add these columns to the list.</span><span class="sxs-lookup"><span data-stu-id="5ed5d-126">**Note** You might have to add these columns to the list.</span></span> <span data-ttu-id="5ed5d-127">For more information, see [Personalising Your Workspace](ui-personalization-user.md).</span><span class="sxs-lookup"><span data-stu-id="5ed5d-127">For more information, see [Personalizing Your Workspace](ui-personalization-user.md).</span></span>  
* <span data-ttu-id="5ed5d-128">Alternatively, on the **Suggest Vendor Payments** batch job, where you specify the payments to include in the payment journal, you can specify not to insert journal lines for payments that have already been exported by choosing the **Skip Exported Payments** check box.</span><span class="sxs-lookup"><span data-stu-id="5ed5d-128">Alternatively, on the **Suggest Vendor Payments** batch job, where you specify the payments to include in the payment journal, you can specify not to insert journal lines for payments that have already been exported by choosing the **Skip Exported Payments** check box.</span></span>

## <a name="see-also"></a><span data-ttu-id="5ed5d-129">See Also</span><span class="sxs-lookup"><span data-stu-id="5ed5d-129">See Also</span></span>
[<span data-ttu-id="5ed5d-130">Payment Methods</span><span class="sxs-lookup"><span data-stu-id="5ed5d-130">Payment Methods</span></span>](finance-payment-methods.md)  
[<span data-ttu-id="5ed5d-131">Finance</span><span class="sxs-lookup"><span data-stu-id="5ed5d-131">Finance</span></span>](finance.md)  
<span data-ttu-id="5ed5d-132">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="5ed5d-132">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
