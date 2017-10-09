---
title: Record and Reimburse Employees' Business-Related Expenses | Microsoft Docs
description: Post employees' expenses with the general journal to the employee's account and later post a payment to the employee's bank account to reimburse for the business-related expense.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: reimbursement
ms.date: 06/28/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 8674fcc050e11c9ecb1c423fc5048c1ef630e1ac
ms.contentlocale: en-nz
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-record-and-reimburse-employees-expenses"></a>How to: Record and Reimburse Employees' Expenses
[!INCLUDE[d365fin](includes/d365fin_md.md)] supports transactions for employee in a similar way as for vendors. Accordingly, employee posting groups exist to make sure that employee ledger entries are posted to the relevant accounts in the general ledger.

> [!NOTE]  
> Employee transactions can be posted in the local currency only. Reimbursement payments to employees do not support discounts and payment tolerances.

If employees spend their own money during business activities, you can post the expense to the employee's account. Then you can reimburse the employee by making a payment to the employee's bank account, similarly to how you pay vendors.

## <a name="to-record-an-employees-expense"></a>To record an employee's expense
You post employees' expenses in the **General Journal** window.
1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **General Journals**, and then choose the related link.
2. Open the relevant general journal batch. For more information, see [Working with General Journals](ui-work-general-journals.md).
3. On a new journal line, fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]    
4. Repeat step 3 for all the expenses that the employee has incurred.

    > [!TIP]  
    > If you want to enter multiple expense lines above one balance-account line for the employee's bank account, then select the **Suggest Balancing Amount** check box on the line for your batch in the **General Journal Batches** window. Then the **Amount** field on the balance-account line is automatically prefilled with the value that is required to balance the expenses.
5. Choose the **Post** action to record the expenses on the employee's account.

## <a name="to-reimburse-an-employee"></a>To reimburse an employee
You reimburse employees by posting payments to their bank account in the **Payment Journal** window.
1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Payment Journals**, and then choose the related link.
2. Open the relevant payment journal batch. For more information, see [Working with General Journals](ui-work-general-journals.md).
3. Fill in the fields as necessary. For more information, see [Making Payments](payables-make-payments.md).
4. Alternatively, choose the **Suggest Employee Payment** action to automatically insert journal lines for pending employee reimbursements.
5. Choose the **Post** action to register the reimbursement.  

## <a name="to-reconcile-reimbursements-with-employee-ledger-entries"></a>To reconcile reimbursements with employee ledger entries
You apply employee payments to their related open employee ledger entries in the same way as you do for vendor payments, for example in the **Payment Reconciliation Journal** window, based on the related bank statement entries. For more information, see [Apply Payments Automatically and Reconcile Bank Accounts](receivables-apply-payments-auto-reconcile-bank-accounts.md). Alternatively, you can apply manually in the **Employee Ledger Entries** window. For more information, see the related [How to: Reconcile Vendor Payments Manually](payables-how-apply-purchase-transactions-manually.md).  

## <a name="see-also"></a>See Also
[How to: Post Transactions Directly to the General Ledger](finance-how-post-transactions-directly.md)  
[Working with General Journals](ui-work-general-journals.md)  
[How to: Reverse Postings](finance-how-reverse-journal-posting.md)  
[Finance](finance.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

