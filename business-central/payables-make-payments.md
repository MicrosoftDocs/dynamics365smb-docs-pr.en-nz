---
title: Overview of Tasks to Manage Payments to Vendors| Microsoft Docs
description: Outlines tasks to manage payments to vendors or creditors, including posting payment lines and getting an overview of the balance due.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: print check, vendor payment, creditor, debt, balance due, AP
ms.date: 11/17/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: fb3a95c63963c2f209dfa8d6c04711a3e5dc8339
ms.contentlocale: en-nz
ms.lasthandoff: 03/22/2018

---
# <a name="making-payments"></a><span data-ttu-id="a9845-103">Making Payments</span><span class="sxs-lookup"><span data-stu-id="a9845-103">Making Payments</span></span>
<span data-ttu-id="a9845-104">When you make payments to vendors or reimbursements to employees, you post the related payment lines in the **Payment Journal** window.</span><span class="sxs-lookup"><span data-stu-id="a9845-104">When you make payments to vendors or reimbursements to employees, you post the related payment lines in the **Payment Journal** window.</span></span> <span data-ttu-id="a9845-105">You can use the **Suggest Vendor Payments** function to find vendor payments that are due.</span><span class="sxs-lookup"><span data-stu-id="a9845-105">You can use the **Suggest Vendor Payments** function to find vendor payments that are due.</span></span> <span data-ttu-id="a9845-106">You can also use the **Vendor - Summary Ageing** report to get an overview of due vendor payments.</span><span class="sxs-lookup"><span data-stu-id="a9845-106">You can also use the **Vendor - Summary Aging** report to get an overview of due vendor payments.</span></span>

<span data-ttu-id="a9845-107">From the payment journal, you can print computer cheques or record when cheques are written.</span><span class="sxs-lookup"><span data-stu-id="a9845-107">From the payment journal, you can print computer checks or record when checks are written.</span></span> <span data-ttu-id="a9845-108">If you select **Computer Cheque** in the **Bank Payment Type** field, then any lines representing cheques must be printed before the payment journal can be posted.</span><span class="sxs-lookup"><span data-stu-id="a9845-108">If you select **Computer Check** in the **Bank Payment Type** field, then any lines representing checks must be printed before the payment journal can be posted.</span></span>

<span data-ttu-id="a9845-109">When the payments are posted, you can export them to a bank file for upload to your bank for processing.</span><span class="sxs-lookup"><span data-stu-id="a9845-109">When the payments are posted, you can export them to a bank file for upload to your bank for processing.</span></span>

<span data-ttu-id="a9845-110">After the payments are made at your bank, you must apply them to their related open vendor or employee ledger entries.</span><span class="sxs-lookup"><span data-stu-id="a9845-110">After the payments are made at your bank, you must apply them to their related open vendor or employee ledger entries.</span></span> <span data-ttu-id="a9845-111">You can do this manually or by importing a bank statement file and applying the payments automatically.</span><span class="sxs-lookup"><span data-stu-id="a9845-111">You can do this manually or by importing a bank statement file and applying the payments automatically.</span></span> <span data-ttu-id="a9845-112">For more information, see [Applying Payments Automatically and Reconciling Bank Accounts](receivables-apply-payments-auto-reconcile-bank-accounts.md).</span><span class="sxs-lookup"><span data-stu-id="a9845-112">For more information, see [Applying Payments Automatically and Reconciling Bank Accounts](receivables-apply-payments-auto-reconcile-bank-accounts.md).</span></span>

<span data-ttu-id="a9845-113">The following table describes a sequence of tasks, with links to the topics that describe them.</span><span class="sxs-lookup"><span data-stu-id="a9845-113">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>

| <span data-ttu-id="a9845-114">To</span><span class="sxs-lookup"><span data-stu-id="a9845-114">To</span></span> | <span data-ttu-id="a9845-115">See</span><span class="sxs-lookup"><span data-stu-id="a9845-115">See</span></span> |
| --- | --- |
|<span data-ttu-id="a9845-116">Use the **Payment Journal** window, which is a based on the general journal, to post payments to vendors or employees.</span><span class="sxs-lookup"><span data-stu-id="a9845-116">Use the **Payment Journal** window, which is a based on the general journal, to post payments to vendors or employees.</span></span>|[<span data-ttu-id="a9845-117">Working with General Journals</span><span class="sxs-lookup"><span data-stu-id="a9845-117">Working with General Journals</span></span>](ui-work-general-journals.md)|
| <span data-ttu-id="a9845-118">Use a function to suggest vendor payments according to selected criteria, such as due date, discount eligibility, and your liquidity.</span><span class="sxs-lookup"><span data-stu-id="a9845-118">Use a function to suggest vendor payments according to selected criteria, such as due date, discount eligibility, and your liquidity.</span></span> |[<span data-ttu-id="a9845-119">Suggest Vendor Payments</span><span class="sxs-lookup"><span data-stu-id="a9845-119">Suggest Vendor Payments</span></span>](payables-how-suggest-vendor-payments.md) |
|<span data-ttu-id="a9845-120">Reimburse employees for personal expenses during business activities by making payment to their bank account.</span><span class="sxs-lookup"><span data-stu-id="a9845-120">Reimburse employees for personal expenses during business activities by making payment to their bank account.</span></span>|[<span data-ttu-id="a9845-121">Record and Reimburse Employees' Expenses</span><span class="sxs-lookup"><span data-stu-id="a9845-121">Record and Reimburse Employees' Expenses</span></span>](finance-how-record-reimburse-employee-expenses.md)|
| <span data-ttu-id="a9845-122">Issue cheques for vendor payments, either as print-outs or as computer cheques.</span><span class="sxs-lookup"><span data-stu-id="a9845-122">Issue checks for vendor payments, either as print-outs or as computer checks.</span></span> <span data-ttu-id="a9845-123">Void cheques before or after posting.</span><span class="sxs-lookup"><span data-stu-id="a9845-123">Void checks before or after posting.</span></span> |[<span data-ttu-id="a9845-124">Work With Cheques</span><span class="sxs-lookup"><span data-stu-id="a9845-124">Work With Checks</span></span>](payables-how-work-checks.md) |
| <span data-ttu-id="a9845-125">Pay the vendor by cash or cheque, and post the payment when you post the invoice.</span><span class="sxs-lookup"><span data-stu-id="a9845-125">Pay the vendor by cash or check, and post the payment when you post the invoice.</span></span> |[<span data-ttu-id="a9845-126">Settle Purchase Invoices Promptly</span><span class="sxs-lookup"><span data-stu-id="a9845-126">Settle Purchase Invoices Promptly</span></span>](finance-how-to-settle-purchase-invoices-promptly.md) |
| <span data-ttu-id="a9845-127">Make sure that your bank only clears validated cheques and amounts by sending them a file that contains vendor, cheque, and payment information.</span><span class="sxs-lookup"><span data-stu-id="a9845-127">Make sure that your bank only clears validated checks and amounts by sending them a file that contains vendor, check, and payment information.</span></span> |[<span data-ttu-id="a9845-128">Export a Positive Pay file</span><span class="sxs-lookup"><span data-stu-id="a9845-128">Export a Positive Pay file</span></span>](finance-how-positive-pay.md) |
|<span data-ttu-id="a9845-129">Export payments from the **Payment Journal** window to a bank file that you upload to your bank for processing, including EFT (electronic funds transfer) in North America.</span><span class="sxs-lookup"><span data-stu-id="a9845-129">Export payments from the **Payment Journal** window to a bank file that you upload to your bank for processing, including EFT (electronic funds transfer) in North America.</span></span> |[<span data-ttu-id="a9845-130">Export Payments to a Bank File</span><span class="sxs-lookup"><span data-stu-id="a9845-130">Export Payments to a Bank File</span></span>](payables-how-export-payments-bank-file.md)|
|<span data-ttu-id="a9845-131">Make electronic payments according to the EU SEPA Credit Transfer standard.</span><span class="sxs-lookup"><span data-stu-id="a9845-131">Make electronic payments according to the EU SEPA Credit Transfer standard.</span></span>|[<span data-ttu-id="a9845-132">Making Payments with Bank Data Conversion Service or SEPA Credit Transfer</span><span class="sxs-lookup"><span data-stu-id="a9845-132">Making Payments with Bank Data Conversion Service or SEPA Credit Transfer</span></span>](finance-make-payments-with-bank-data-conversion-service-or-sepa-credit-transfer.md)|    

## <a name="see-also"></a><span data-ttu-id="a9845-133">See Also</span><span class="sxs-lookup"><span data-stu-id="a9845-133">See Also</span></span>
[<span data-ttu-id="a9845-134">Managing Payables</span><span class="sxs-lookup"><span data-stu-id="a9845-134">Managing Payables</span></span>](payables-manage-payables.md)  
[<span data-ttu-id="a9845-135">Purchasing</span><span class="sxs-lookup"><span data-stu-id="a9845-135">Purchasing</span></span>](purchasing-manage-purchasing.md)  
[<span data-ttu-id="a9845-136">Managing Receivables</span><span class="sxs-lookup"><span data-stu-id="a9845-136">Managing Receivables</span></span>](receivables-manage-receivables.md)  
<span data-ttu-id="a9845-137">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="a9845-137">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
