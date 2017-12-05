---
title: Setting Up Text-to-Account Mapping for Recurring Payments | Microsoft Docs
description: Link text on payments with specific accounts, so that payments are posted to the accounts when you post the payment reconciliation journal.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: account linking, direct payment posting, automatic payment processing, reconcile payment, recurring expense, recurring cash receipt
ms.date: 03/29/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: ba26b354d235981bd7291f9ac6402779f554ac7a
ms.openlocfilehash: 53c65f7f47c189905e277eff1ea86af241aa1b0b
ms.contentlocale: en-nz
ms.lasthandoff: 11/10/2017

---
# <a name="how-to-map-text-on-recurring-payments-to-accounts-for-automatic-reconciliation"></a>How to: Map Text on Recurring Payments to Accounts for Automatic Reconciliation
In the **Text-to-Account Mapping** window, which you open from the **Payment Reconciliation Journal** window, you can set up mappings between text on payments and specific debit, credit, and balancing accounts so that such payments are posted to the specified accounts when you post the payment reconciliation journal.

Similar functionality exists to reconcile excess amounts on payment reconciliation journal lines on an ad-hoc basis. For more information, see [How to: Reconcile Payments That Cannot be Applied Automatically](receivables-how-reconcile-payments-cannot-apply-auto.md).

Payments posted based on text-to-account mapping are not applied to open entries, but are merely posted to the specified accounts in addition to creating bank account ledger entries. Accordingly, text-to-account mapping is suited for recurring cash receipts or expenses, such as frequent purchases of car fuel or bank fees and interest, that regularly occur on the bank statement and do not need a related business document. For more information, see the “Example - Text-to-Account Mapping for Fuel Expense” section in this topic.

> [!NOTE]  
>   Payments on reconciliation journal lines are only set to posting according to text-to-account mapping if the automatic application function can only provide a match confidence of **Low** or **Medium**. If the automatic application function provides a match confidence of High, then the payment is automatically applied to one or more open entries, and the payment is not posted to the accounts specified in the **Text-to-Account Mapping** window. In other words, a match confidence of **High** overrules a text-to-account mapping.

On a payment reconciliation journal line where the payment has been set to posting according to text-to-account mapping, the **Match Confidence** field contains **High - Text-to-Account Mapping**, and the **Account Type** and **Account No.** fields contain the mapped accounts.

## <a name="to-map-text-on-recurring-payments-to-accounts-for-automatic-reconciliation"></a>To map text on recurring payments to accounts for automatic reconciliation
1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Payment Reconciliation Journals**, and then choose the related link.
2. Open a payment reconciliation journal. For more information, see [How to: Reconcile Payments Using Automatic Application](receivables-how-reconcile-payments-auto-application.md).
3. Choose the **Map Text to Account** action. The **Text-to-Account Mapping** window opens.
4. In the **Mapping Text** field, enter any text that occurs on payments that you want to post to specified accounts without applying to an open entry. You can enter up to 50 characters.

    > [!NOTE]  
>   If no other payments exist with the mapping text in question, then the text-to-account mapping will occur even when only a part of the text on the payment exists as a mapping text.
5. In the **Vendor No.** field, enter the vendor that the payments will be posted to.
6. In the **Bal. Source Type** field, specify if the payment will be posted to a general ledger account or to a customer or vendor account.
7. In the **Bal. Source No.** field, specify the account that the payment will be posted to, depending on your selection in the **Bal. Source Type** field.

    > [!NOTE]
    > Do not use the **Debit Acc. No.** and **Credit Acc. No.** fields in connection with payment reconciliation. They are used for incoming documents only. For more information, see [How to: Use OCR to Turn PDF and Image Files into Electronic Documents](across-how-use-ocr-pdf-images-files.md).

8. Repeat steps 3 through 7 for all text on payments that you want to map to accounts for direct posting without application.

Next time you import a bank statement file or choose the **Apply Automatically** action in the **Payment Reconciliation Journal** window, journal lines for the payments that contain the specified mapping text will contain the mapped accounts in the **Account Type** and **Account No.** fields. The **Match Confidence** field will contain **High - Text-to-Account Mapping**. This is on the condition that the automatic application function can only provide a match confidence of **Low** or **Medium**.

## <a name="example-text-to-account-mapping-for-fuel-expense"></a>Example: Text-to-Account Mapping for Fuel Expense
To always post fuel expenses incurred at Shell gas stations to the general ledger account for gasoline (account 8510), fill a line in the **Text-to-Account Mapping** window as follows.

| Mapping Text | Debit Acc. No. | Credit Acc. No. | Bal. Source Type | Bal. Source No. |
| --- | --- | --- | --- | --- |
| Shell |BLANK |8510 |G/L Account |BLANK |

> [!TIP]  
>   For more information about how to work with fields and columns, see [Working with [!INCLUDE[d365fin](includes/d365fin_long_md.md)]](ui-work-product.md). For more information about how to find specific pages, see [Search](ui-search.md).

## <a name="see-also"></a>See Also
[Managing Receivables](receivables-manage-receivables.md)  
[Sales](sales-manage-sales.md)  
[How to: Set Up the Envestnet Yodlee Bank Feeds Service](bank-how-setup-bank-statement-service.md)  
[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions](ui-extensions.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

