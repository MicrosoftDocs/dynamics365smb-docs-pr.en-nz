---
title: Managing Payables| Microsoft Docs
description: Managing Payables
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: vendor payment, creditor, debt, balance due, AP
ms.date: 03/28/2017
ms.author: sgroespe
ms.translationtype: Human Translation
ms.sourcegitcommit: a31be0f9d07e2abb591e26f6bae34c6f6e4dcda6
ms.openlocfilehash: 92b16c52589a07661d9ff080e9ef8a0f6be633f7
ms.contentlocale: en-nz
ms.lasthandoff: 05/04/2017


---
# <a name="managing-payables"></a>Managing Payables
A big part of managing accounts payable is paying your vendors. You can use functions to add payments lines for purchase invoices that are due in the **Payment Journal** window. To send transactions to your bank, you can export multiple payment journal lines to a file, and then upload the file to your bank. You can also make payments by cheque, including transmitting cheques as electronic payments.

Another typical task is to apply outgoing payments to their related vendor ledger entries in order to close purchase invoices or purchase credit memos as paid. You can do this in the **Payment Reconciliation Journal** window by importing a bank statement file to register the payments. The payments are applied to open vendor or customer ledger entries by matching payment text and entry information. There are various ways to review and change the matches before you post the journal. You can choose to close any open bank account ledger entries related to the applied ledger entries when you post the journal. The bank account is automatically reconciled when all payments are applied.

Alternatively, you can apply outgoing payments manually in the **Payment Journal** window or from the related vendor ledger entries.

The following table describes a sequence of tasks within accounts payable, with links to the topics that describe them.

| To | See |
| --- | --- |
| Generate due vendor payments prioritised according to payment discounts and overdue penalties. Optionally, export the payments to a bank file when posting. |[Make Payments](payables-make-payments.md) |
| Apply vendor payments automatically to unpaid purchase invoices by importing a bank statement file. |[Apply Payments Automatically and Reconcile Bank Accounts](receivables-apply-payments-auto-reconcile-bank-accounts.md) |
| Apply vendor payments to unpaid purchase invoices manually. |[How to: Reconcile Vendor Payments Manually](payables-how-apply-purchase-transactions-manually.md) |

## <a name="see-also"></a>See Also
[Purchasing](purchasing-manage-purchasing.md)  
[Managing Receivables](receivables-manage-receivables.md)  
[General Business Functionality](ui-across-business-areas.md)  
[Working With [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

