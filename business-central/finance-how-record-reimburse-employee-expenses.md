---
title: Record and Reimburse Employees' Business-Related Expenses
description: Post employees' expenses with the general journal to the employee's account and later post a payment to the employee's bank account to reimburse for the business-related expense.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: reimbursement
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: dd4ce755e3414f19ae501c1d437f3e1d78d565a1
ms.sourcegitcommit: 1aab52477956bf1aa7376fc7fb984644bc398c61
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 06/04/2021
ms.locfileid: "6184415"
---
# <a name="record-and-reimburse-employees-expenses"></a><span data-ttu-id="1f8f9-103">Record and Reimburse Employees' Expenses</span><span class="sxs-lookup"><span data-stu-id="1f8f9-103">Record and Reimburse Employees' Expenses</span></span>

[!INCLUDE[prod_short](includes/prod_short.md)] <span data-ttu-id="1f8f9-104">supports transactions for employees in a similar way as for vendors.</span><span class="sxs-lookup"><span data-stu-id="1f8f9-104">supports transactions for employees in a similar way as for vendors.</span></span> <span data-ttu-id="1f8f9-105">Accordingly, employee posting groups exist to make sure that employee ledger entries are posted to the relevant accounts in the general ledger.</span><span class="sxs-lookup"><span data-stu-id="1f8f9-105">Accordingly, employee posting groups exist to make sure that employee ledger entries are posted to the relevant accounts in the general ledger.</span></span>

> [!NOTE]  
> <span data-ttu-id="1f8f9-106">Employee transactions can be posted in the local currency only.</span><span class="sxs-lookup"><span data-stu-id="1f8f9-106">Employee transactions can be posted in the local currency only.</span></span> <span data-ttu-id="1f8f9-107">Reimbursement payments to employees do not support discounts and payment tolerances.</span><span class="sxs-lookup"><span data-stu-id="1f8f9-107">Reimbursement payments to employees do not support discounts and payment tolerances.</span></span>

<span data-ttu-id="1f8f9-108">If employees spend their own money during business activities, you can post the expense to the employee's account.</span><span class="sxs-lookup"><span data-stu-id="1f8f9-108">If employees spend their own money during business activities, you can post the expense to the employee's account.</span></span> <span data-ttu-id="1f8f9-109">Then you can reimburse the employee by making a payment to the employee's bank account, similarly to how you pay vendors.</span><span class="sxs-lookup"><span data-stu-id="1f8f9-109">Then you can reimburse the employee by making a payment to the employee's bank account, similarly to how you pay vendors.</span></span>  

> [!TIP]
> <span data-ttu-id="1f8f9-110">This article explains how to record the expense in the books and how to reimburse the employee.</span><span class="sxs-lookup"><span data-stu-id="1f8f9-110">This article explains how to record the expense in the books and how to reimburse the employee.</span></span> <span data-ttu-id="1f8f9-111">Your organisation may have a portal or app where employees can submit their expense reports.</span><span class="sxs-lookup"><span data-stu-id="1f8f9-111">Your organization may have a portal or app where employees can submit their expense reports.</span></span>

<span data-ttu-id="1f8f9-112">[!INCLUDE [prod_short](includes/prod_short.md)] is flexible enough to suit many different practices.</span><span class="sxs-lookup"><span data-stu-id="1f8f9-112">[!INCLUDE [prod_short](includes/prod_short.md)] is flexible enough to suit many different practices.</span></span> <span data-ttu-id="1f8f9-113">The exact account numbers to use depends on your organisation's configuration and processes.</span><span class="sxs-lookup"><span data-stu-id="1f8f9-113">The exact account numbers to use depends on your organization's configuration and processes.</span></span>  

## <a name="to-record-an-employees-expense"></a><span data-ttu-id="1f8f9-114">To record an employee's expense</span><span class="sxs-lookup"><span data-stu-id="1f8f9-114">To record an employee's expense</span></span>

<span data-ttu-id="1f8f9-115">You post employees' expenses on the **General Journal** page.</span><span class="sxs-lookup"><span data-stu-id="1f8f9-115">You post employees' expenses on the **General Journal** page.</span></span>

1. <span data-ttu-id="1f8f9-116">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **General Journals**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="1f8f9-116">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **General Journals**, and then choose the related link.</span></span>  
2. <span data-ttu-id="1f8f9-117">Open the relevant general journal batch.</span><span class="sxs-lookup"><span data-stu-id="1f8f9-117">Open the relevant general journal batch.</span></span> <span data-ttu-id="1f8f9-118">For more information, see [Working with General Journals](ui-work-general-journals.md).</span><span class="sxs-lookup"><span data-stu-id="1f8f9-118">For more information, see [Working with General Journals](ui-work-general-journals.md).</span></span>
3. <span data-ttu-id="1f8f9-119">On a new journal line, fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="1f8f9-119">On a new journal line, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

    > [!NOTE]
    > [!INCLUDE[journal-showhide-columns-inline-tip](includes/journal-showhide-columns-inline-tip.md)]
4. <span data-ttu-id="1f8f9-120">Repeat step 3 for all the expenses that the employee has incurred.</span><span class="sxs-lookup"><span data-stu-id="1f8f9-120">Repeat step 3 for all the expenses that the employee has incurred.</span></span>

    > [!TIP]  
    > <span data-ttu-id="1f8f9-121">If you want to enter multiple expense lines above one balance-account line for the employee's bank account, then select the **Suggest Balancing Amount** check box on the line for your batch on the **General Journal Batches** page.</span><span class="sxs-lookup"><span data-stu-id="1f8f9-121">If you want to enter multiple expense lines above one balance-account line for the employee's bank account, then select the **Suggest Balancing Amount** check box on the line for your batch on the **General Journal Batches** page.</span></span> <span data-ttu-id="1f8f9-122">Then the **Amount** field on the balance-account line is automatically prefilled with the value that is required to balance the expenses.</span><span class="sxs-lookup"><span data-stu-id="1f8f9-122">Then the **Amount** field on the balance-account line is automatically prefilled with the value that is required to balance the expenses.</span></span>
5. <span data-ttu-id="1f8f9-123">Choose the **Post** action to record the expenses on the employee's account.</span><span class="sxs-lookup"><span data-stu-id="1f8f9-123">Choose the **Post** action to record the expenses on the employee's account.</span></span>

## <a name="to-reimburse-an-employee"></a><span data-ttu-id="1f8f9-124">To reimburse an employee</span><span class="sxs-lookup"><span data-stu-id="1f8f9-124">To reimburse an employee</span></span>

<span data-ttu-id="1f8f9-125">You reimburse employees by posting payments to their bank account on the **Receipt Journal** page.</span><span class="sxs-lookup"><span data-stu-id="1f8f9-125">You reimburse employees by posting payments to their bank account on the **Payment Journal** page.</span></span>  

1. <span data-ttu-id="1f8f9-126">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Receipt Journals**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="1f8f9-126">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Payment Journals**, and then choose the related link.</span></span>
2. <span data-ttu-id="1f8f9-127">Open the relevant receipt journal batch.</span><span class="sxs-lookup"><span data-stu-id="1f8f9-127">Open the relevant payment journal batch.</span></span> <span data-ttu-id="1f8f9-128">For more information, see [Working with General Journals](ui-work-general-journals.md).</span><span class="sxs-lookup"><span data-stu-id="1f8f9-128">For more information, see [Working with General Journals](ui-work-general-journals.md).</span></span>
3. <span data-ttu-id="1f8f9-129">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="1f8f9-129">Fill in the fields as necessary.</span></span> <span data-ttu-id="1f8f9-130">For more information, see [Making Payments](payables-make-payments.md).</span><span class="sxs-lookup"><span data-stu-id="1f8f9-130">For more information, see [Making Payments](payables-make-payments.md).</span></span>
4. <span data-ttu-id="1f8f9-131">Alternatively, choose the **Suggest Employee Payment** action to automatically insert journal lines for pending employee reimbursements.</span><span class="sxs-lookup"><span data-stu-id="1f8f9-131">Alternatively, choose the **Suggest Employee Payment** action to automatically insert journal lines for pending employee reimbursements.</span></span>
5. <span data-ttu-id="1f8f9-132">Choose the **Post** action to register the reimbursement.</span><span class="sxs-lookup"><span data-stu-id="1f8f9-132">Choose the **Post** action to register the reimbursement.</span></span>  

## <a name="to-reconcile-reimbursements-with-employee-ledger-entries"></a><span data-ttu-id="1f8f9-133">To reconcile reimbursements with employee ledger entries</span><span class="sxs-lookup"><span data-stu-id="1f8f9-133">To reconcile reimbursements with employee ledger entries</span></span>

<span data-ttu-id="1f8f9-134">You apply employee payments to their related open employee ledger entries in the same way as you do for vendor payments, for example on the **Payment Reconciliation Journal** page, based on the related bank statement entries.</span><span class="sxs-lookup"><span data-stu-id="1f8f9-134">You apply employee payments to their related open employee ledger entries in the same way as you do for vendor payments, for example on the **Payment Reconciliation Journal** page, based on the related bank statement entries.</span></span> <span data-ttu-id="1f8f9-135">For more information, see [Applying Payments Automatically and Reconciling Bank Accounts](receivables-apply-payments-auto-reconcile-bank-accounts.md).</span><span class="sxs-lookup"><span data-stu-id="1f8f9-135">For more information, see [Applying Payments Automatically and Reconciling Bank Accounts](receivables-apply-payments-auto-reconcile-bank-accounts.md).</span></span> <span data-ttu-id="1f8f9-136">Alternatively, you can apply manually on the **Employee Ledger Entries** page.</span><span class="sxs-lookup"><span data-stu-id="1f8f9-136">Alternatively, you can apply manually on the **Employee Ledger Entries** page.</span></span> <span data-ttu-id="1f8f9-137">For more information, see the related [Reconcile Vendor Payments with the Receipt Journal or from Vendor Ledger Entries](payables-how-apply-purchase-transactions-manually.md).</span><span class="sxs-lookup"><span data-stu-id="1f8f9-137">For more information, see the related [Reconcile Vendor Payments with the Payment Journal or from Vendor Ledger Entries](payables-how-apply-purchase-transactions-manually.md).</span></span>  

## <a name="see-also"></a><span data-ttu-id="1f8f9-138">See Also</span><span class="sxs-lookup"><span data-stu-id="1f8f9-138">See Also</span></span>

[<span data-ttu-id="1f8f9-139">Post Transactions Directly to the General Ledger</span><span class="sxs-lookup"><span data-stu-id="1f8f9-139">Post Transactions Directly to the General Ledger</span></span>](finance-how-post-transactions-directly.md)  
[<span data-ttu-id="1f8f9-140">Working with General Journals</span><span class="sxs-lookup"><span data-stu-id="1f8f9-140">Working with General Journals</span></span>](ui-work-general-journals.md)  
[<span data-ttu-id="1f8f9-141">Reverse Journal Postings and Undo Receipts/Shipments</span><span class="sxs-lookup"><span data-stu-id="1f8f9-141">Reverse Journal Postings and Undo Receipts/Shipments</span></span>](finance-how-reverse-journal-posting.md)  
[<span data-ttu-id="1f8f9-142">Finance</span><span class="sxs-lookup"><span data-stu-id="1f8f9-142">Finance</span></span>](finance.md)  
<span data-ttu-id="1f8f9-143">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="1f8f9-143">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>  


[!INCLUDE[footer-include](includes/footer-banner.md)]