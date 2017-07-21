---
title: Manage Bank Accounts| Microsoft Docs
description: You must regularly reconcile bank ledger entries in Financials with the related bank transactions in your bank accounts.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: reconcile
ms.date: 06/02/2017
ms.author: sgroespe
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: dcefa921d7e8b901d906085e6bce01d6e0aa6ac4
ms.contentlocale: en-nz
ms.lasthandoff: 07/07/2017


---
# <a name="managing-bank-accounts"></a>Managing Bank Accounts
At regular intervals, you must reconcile your bank ledger entries in [!INCLUDE[d365fin](includes/d365fin_md.md)] with the related bank transactions in bank accounts at your bank, and then post the balance to your bank account. You can perform this task either as part of processing the payments represented on a bank statement in the **Payment Reconciliation Journal**. Alternatively, you can perform the task separately from payment processing, in the **Bank Acc. Reconciliation** window, which supports cheque ledger entries. In both cases, you fill in the windows by importing the bank statement into [!INCLUDE[d365fin](includes/d365fin_md.md)].

Sometimes, you need to transfer amounts between bank account in [!INCLUDE[d365fin](includes/d365fin_md.md)] to reflect transfers at your bank. You perform this task in the **General Journal** window, in different ways depending on the currency of the funds.

Before you can manage bank accounts, you must set each bank account up as a bank account card. In addition, you must set up electronic services that you may use for bank statement import and payment file export. For more information, see [Set Up Bank Accounts](bank-setup-banking.md).

The following table describes a sequence of tasks, with links to the topics that describe them.

| To | See |
| --- | --- |
| Reconcile bank accounts in connection with payment processing in the **Payment Reconciliation Journal** window. |[Apply Payments Automatically and Reconcile Bank Accounts](receivables-apply-payments-auto-reconcile-bank-accounts.md) |
| Reconcile bank accounts, including cheque ledger entries, as a separate task in the **Bank Acc. Reconciliation** window. |[How to: Reconcile Bank Accounts Separately](bank-how-reconcile-bank-accounts-separately.md) |
| Post transfers between bank accounts in the same currency or in different currencies. |[How to: Transfer Bank Funds](bank-how-transfer-bank-funds.md) |

## <a name="see-also"></a>See Also
[Setting Up Banking](bank-setup-banking.md)  
[Managing Receivables](receivables-manage-receivables.md)  
[Managing Payables](payables-manage-payables.md)    
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  
[General Business Functionality](ui-across-business-areas.md)  

