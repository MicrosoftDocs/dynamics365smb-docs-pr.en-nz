---
title: Overview of Tasks to Manage Accounts Payable| Microsoft Docs
description: Outlines tasks to manage accounts payable, for example, paying creditors or applying outgoing payments to ledger entries to close invoices or credit memos.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: vendor payment, creditor, debt, balance due, AP
ms.date: 06/06/2017
ms.author: sgroespe
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: 9684a91268927a4f1f4d249fef019c8f6ac00325
ms.contentlocale: en-nz
ms.lasthandoff: 07/07/2017


---
# <a name="managing-payables"></a><span data-ttu-id="b5ee5-103">Managing Payables</span><span class="sxs-lookup"><span data-stu-id="b5ee5-103">Managing Payables</span></span>
<span data-ttu-id="b5ee5-104">A big part of managing accounts payable is paying your vendors.</span><span class="sxs-lookup"><span data-stu-id="b5ee5-104">A big part of managing accounts payable is paying your vendors.</span></span> <span data-ttu-id="b5ee5-105">You can use functions to add payments lines for purchase invoices that are due in the **Payment Journal** window.</span><span class="sxs-lookup"><span data-stu-id="b5ee5-105">You can use functions to add payments lines for purchase invoices that are due in the **Payment Journal** window.</span></span> <span data-ttu-id="b5ee5-106">To send transactions to your bank, you can export multiple payment journal lines to a file, and then upload the file to your bank.</span><span class="sxs-lookup"><span data-stu-id="b5ee5-106">To send transactions to your bank, you can export multiple payment journal lines to a file, and then upload the file to your bank.</span></span> <span data-ttu-id="b5ee5-107">You can also make payments by cheque, including transmitting cheques as electronic payments.</span><span class="sxs-lookup"><span data-stu-id="b5ee5-107">You can also make payments by check, including transmitting checks as electronic payments.</span></span>

<span data-ttu-id="b5ee5-108">Another typical task is to apply outgoing payments to their related vendor ledger entries in order to close purchase invoices or purchase credit memos as paid.</span><span class="sxs-lookup"><span data-stu-id="b5ee5-108">Another typical task is to apply outgoing payments to their related vendor ledger entries in order to close purchase invoices or purchase credit memos as paid.</span></span> <span data-ttu-id="b5ee5-109">You can do this in the **Payment Reconciliation Journal** window by importing a bank statement file to register the payments.</span><span class="sxs-lookup"><span data-stu-id="b5ee5-109">You can do this in the **Payment Reconciliation Journal** window by importing a bank statement file to register the payments.</span></span> <span data-ttu-id="b5ee5-110">The payments are applied to open vendor or customer ledger entries by matching payment text and entry information.</span><span class="sxs-lookup"><span data-stu-id="b5ee5-110">The payments are applied to open vendor or customer ledger entries by matching payment text and entry information.</span></span> <span data-ttu-id="b5ee5-111">There are various ways to review and change the matches before you post the journal.</span><span class="sxs-lookup"><span data-stu-id="b5ee5-111">There are various ways to review and change the matches before you post the journal.</span></span> <span data-ttu-id="b5ee5-112">You can choose to close any open bank account ledger entries related to the applied ledger entries when you post the journal.</span><span class="sxs-lookup"><span data-stu-id="b5ee5-112">You can choose to close any open bank account ledger entries related to the applied ledger entries when you post the journal.</span></span> <span data-ttu-id="b5ee5-113">The bank account is automatically reconciled when all payments are applied.</span><span class="sxs-lookup"><span data-stu-id="b5ee5-113">The bank account is automatically reconciled when all payments are applied.</span></span>

<span data-ttu-id="b5ee5-114">Alternatively, you can apply outgoing payments manually in the **Payment Journal** window or from the related vendor ledger entries.</span><span class="sxs-lookup"><span data-stu-id="b5ee5-114">Alternatively, you can apply outgoing payments manually in the **Payment Journal** window or from the related vendor ledger entries.</span></span>

<span data-ttu-id="b5ee5-115">The following table describes a sequence of tasks within accounts payable, with links to the topics that describe them.</span><span class="sxs-lookup"><span data-stu-id="b5ee5-115">The following table describes a sequence of tasks within accounts payable, with links to the topics that describe them.</span></span>

| <span data-ttu-id="b5ee5-116">To</span><span class="sxs-lookup"><span data-stu-id="b5ee5-116">To</span></span> | <span data-ttu-id="b5ee5-117">See</span><span class="sxs-lookup"><span data-stu-id="b5ee5-117">See</span></span> |
| --- | --- |
| <span data-ttu-id="b5ee5-118">Generate due vendor payments prioritised according to payment discounts and overdue penalties.</span><span class="sxs-lookup"><span data-stu-id="b5ee5-118">Generate due vendor payments prioritized according to payment discounts and overdue penalties.</span></span> <span data-ttu-id="b5ee5-119">Optionally, export the payments to a bank file when posting.</span><span class="sxs-lookup"><span data-stu-id="b5ee5-119">Optionally, export the payments to a bank file when posting.</span></span> |[<span data-ttu-id="b5ee5-120">Make Payments</span><span class="sxs-lookup"><span data-stu-id="b5ee5-120">Make Payments</span></span>](payables-make-payments.md) |
| <span data-ttu-id="b5ee5-121">Apply vendor payments automatically to unpaid purchase invoices by importing a bank statement file.</span><span class="sxs-lookup"><span data-stu-id="b5ee5-121">Apply vendor payments automatically to unpaid purchase invoices by importing a bank statement file.</span></span> |[<span data-ttu-id="b5ee5-122">Apply Payments Automatically and Reconcile Bank Accounts</span><span class="sxs-lookup"><span data-stu-id="b5ee5-122">Apply Payments Automatically and Reconcile Bank Accounts</span></span>](receivables-apply-payments-auto-reconcile-bank-accounts.md) |
| <span data-ttu-id="b5ee5-123">Apply vendor payments to unpaid purchase invoices manually.</span><span class="sxs-lookup"><span data-stu-id="b5ee5-123">Apply vendor payments to unpaid purchase invoices manually.</span></span> |[<span data-ttu-id="b5ee5-124">How to: Reconcile Vendor Payments Manually</span><span class="sxs-lookup"><span data-stu-id="b5ee5-124">How to: Reconcile Vendor Payments Manually</span></span>](payables-how-apply-purchase-transactions-manually.md) |
|<span data-ttu-id="b5ee5-125">Ensure correct inventory valuation by assigning added item costs, such as freight, physical handling, insurance, and transportation that you incur when purchasing.</span><span class="sxs-lookup"><span data-stu-id="b5ee5-125">Ensure correct inventory valuation by assigning added item costs, such as freight, physical handling, insurance, and transportation that you incur when purchasing.</span></span>|[<span data-ttu-id="b5ee5-126">How to: Use Item Charges to Account for Additional Trade Costs</span><span class="sxs-lookup"><span data-stu-id="b5ee5-126">How to: Use Item Charges to Account for Additional Trade Costs</span></span>](payables-how-assign-item-charges.md)|

## <a name="see-also"></a><span data-ttu-id="b5ee5-127">See Also</span><span class="sxs-lookup"><span data-stu-id="b5ee5-127">See Also</span></span>
[<span data-ttu-id="b5ee5-128">Purchasing</span><span class="sxs-lookup"><span data-stu-id="b5ee5-128">Purchasing</span></span>](purchasing-manage-purchasing.md)  
[<span data-ttu-id="b5ee5-129">Managing Receivables</span><span class="sxs-lookup"><span data-stu-id="b5ee5-129">Managing Receivables</span></span>](receivables-manage-receivables.md)  
[<span data-ttu-id="b5ee5-130">How to: Use Item Charges to Account for Additional Trade Costs</span><span class="sxs-lookup"><span data-stu-id="b5ee5-130">How to: Use Item Charges to Account for Additional Trade Costs</span></span>](payables-how-assign-item-charges.md)  
[<span data-ttu-id="b5ee5-131">General Business Functionality</span><span class="sxs-lookup"><span data-stu-id="b5ee5-131">General Business Functionality</span></span>](ui-across-business-areas.md)  
<span data-ttu-id="b5ee5-132">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="b5ee5-132">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

