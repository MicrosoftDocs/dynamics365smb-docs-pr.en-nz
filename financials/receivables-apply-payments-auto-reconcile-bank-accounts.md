---
title: Tasks to Reconcile Bank Accounts and Apply Payments to Related Entries | Microsoft Docs
description: Outlines tasks to reconcile your bank, receivables, and payables accounts, post cash receipts or expenses, and apply payments automatically.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: payment process, direct payment posting, reconcile payment, expenses, cash receipts
ms.date: 03/29/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: daa014eaa78caa7a317b05ca92ff27c1d1530c06
ms.openlocfilehash: b12a298fd9dc8d03d04790debb7a66715cc96458
ms.contentlocale: en-nz
ms.lasthandoff: 10/17/2017

---
# <a name="applying-payments-automatically-and-reconciling-bank-accounts"></a>Applying Payments Automatically and Reconciling Bank Accounts
You must regularly reconcile your bank, receivables, and payables accounts by applying payments recorded in the bank to their related unpaid invoices and credit memos or other open entries in [!INCLUDE[d365fin](includes/d365fin_long_md.md)].  

You can perform this task in the **Payment Reconciliation Journal** window by importing a bank statement file or feed to quickly register the payments. Payments are applied to open customer or vendor ledger entries based on matches between payment text and entry information. You can review and change automatic applications before you post the journal. You can choose to close any open bank account ledger entries related to the applied ledger entries when you post the journal. The bank account is automatically reconciled when all payments are applied.  

To import bank statements as a bank feed, you must first set up and enable the Envestnet Yodlee Bank Feed service, and then link your bank accounts to the related online bank accounts. For more information, see [How to: Set Up the Envestnet Yodlee Bank Feeds Service](bank-how-setup-bank-statement-service.md).  

Alternatively, you can use the bank data conversion service to convert a bank statement file, from any format, to a data stream that you can import into [!INCLUDE[d365fin](includes/d365fin_long_md.md)]. For more information, see [How to: Set Up the Bank Data Conversion Service](bank-how-setup-bank-data-conversion-service.md).  

The following table describes a sequence of tasks, with links to the topics that describe them.  

| To | See |
| --- | --- |
| Apply payments to open customer or vendor ledger entries by importing a bank statement, and reconcile the bank account when all payments are applied. |[How to: Reconcile Payments Using Automatic Application](receivables-how-reconcile-payments-auto-application.md) |
| Manually apply payments by viewing detailed information about matched data and suggestions for candidate open entries to apply payments to. |[How to: Review or Apply Payments After Automatic Application](receivables-how-review-apply-payments-auto-application.md) |
| Resolve payments that cannot be applied automatically to their related open ledger entries. For example because the amounts differ, or because a related ledger entry does not exist. |[How to: Reconcile Payments That Cannot be Applied Automatically](receivables-how-reconcile-payments-cannot-apply-auto.md) |
| Link text on payments to specific customer, vendor, or general ledger accounts to always post recurring cash receipts or expenses to those accounts when no documents exist to apply to. |[How to: Map Text on Recurring Payments to Accounts for Automatic Reconciliation](receivables-how-map-text-recurring-payments-accounts-auto-reconcilliation.md) |

## <a name="see-also"></a>See Also
[Managing Receivables](receivables-manage-receivables.md)  
[Sales](sales-manage-sales.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

