---
title: Reconcile Bank Accounts and Apply Payments | Microsoft Docs
description: Outlines tasks to reconcile your bank, receivables, and payables accounts, post cash receipts or expenses, and apply payments automatically.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: payment process, direct payment posting, reconcile payment, expenses, cash receipts
ms.date: 10/01/2019
ms.author: sgroespe
ms.openlocfilehash: 60a3cd3398e8a90160ab311dba1ae75fe70305b2
ms.sourcegitcommit: c6e28db8f78fa21db064c9b8a8d742f49d7db3ae
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 10/31/2019
ms.locfileid: "2692527"
---
# <a name="applying-payments-automatically-and-reconciling-bank-accounts"></a>Applying Payments Automatically and Reconciling Bank Accounts
You must regularly reconcile your bank, receivables, and payables accounts by applying payments recorded in the bank to their related unpaid invoices and credit memos or other open entries in [!INCLUDE[d365fin](includes/d365fin_md.md)].  

You can perform this task on the **Payment Reconciliation Journal** page by importing a bank statement file or feed to quickly register the payments. Payments are applied to open customer or vendor ledger entries based on matches between payment text and entry information. You can review and change automatic applications before you post the journal. You can choose to close any open bank account ledger entries related to the applied ledger entries when you post the journal. The bank account is automatically reconciled when all payments are applied.

You can also reconcile bank accounts without simultaneously applying payments. You perform this work on the **Bank Acc. Reconciliation** page. For more information, see [Reconcile Bank Account Separately](bank-how-reconcile-bank-accounts-separately.md).   

To import bank statements as a bank feed, you must first set up and enable the Envestnet Yodlee Bank Feed service, and then link your bank accounts to the related online bank accounts. For more information, see [Set Up the Envestnet Yodlee Bank Feeds Service](bank-how-setup-bank-statement-service.md).  

Alternatively, you can use the AMC Banking 365 Fundamentals extension to convert a bank statement file, from any format, to a data stream that you can import into [!INCLUDE[d365fin](includes/d365fin_md.md)]. For more information, see [Using the AMC Banking 365 Fundamentals extension](ui-extensions-amc-banking.md).  

The following table describes a sequence of tasks, with links to the topics that describe them.  

| To | See |
| --- | --- |
| Apply payments to open customer or vendor ledger entries by importing a bank statement, and reconcile the bank account when all payments are applied. |[Reconcile Payments Using Automatic Application](receivables-how-reconcile-payments-auto-application.md) |
| Manually apply payments by viewing detailed information about matched data and suggestions for candidate open entries to apply payments to. |[Review or Apply Payments After Automatic Application](receivables-how-review-apply-payments-auto-application.md) |
| Resolve payments that cannot be applied automatically to their related open ledger entries. For example because the amounts differ, or because a related ledger entry does not exist. |[Reconcile Payments that Cannot be Applied Automatically](receivables-how-reconcile-payments-cannot-apply-auto.md) |
| Link text on payments to specific customer, vendor, or general ledger accounts to always post recurring cash receipts or expenses to those accounts when no documents exist to apply to. |[Map Text on Recurring Payments to Accounts for Automatic Reconciliation](receivables-how-map-text-recurring-payments-accounts-auto-reconcilliation.md) |

## <a name="see-also"></a>See Also
[Managing Receivables](receivables-manage-receivables.md)  
[Sales](sales-manage-sales.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
