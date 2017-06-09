---
title: 'How to: Map Text on Recurring Payments to Accounts for Automatic Reconciliation| Microsoft Docs'
description: 'How to: Map Text on Recurring Payments to Accounts for Automatic Reconciliation'
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
ms.translationtype: Human Translation
ms.sourcegitcommit: a31be0f9d07e2abb591e26f6bae34c6f6e4dcda6
ms.openlocfilehash: 7c6f79959027625a33961d42abe26514bc94e81e
ms.contentlocale: en-nz
ms.lasthandoff: 05/04/2017


---
# <a name="how-to-map-text-on-recurring-payments-to-accounts-for-automatic-reconciliation"></a>How to: Map Text on Recurring Payments to Accounts for Automatic Reconciliation
In the **Text-to-Account Mapping** window, which you open from the **Payment Reconciliation Journal** window, you can set up mappings between text on payments and specific debit, credit, and balancing accounts so that such payments are posted to the specified accounts when you post the payment reconciliation journal.

**Note**: The topic also applies to when you use the **Map Text to Account** function from an incoming document record to assist in converting electronic documents received from external services to documents in [!INCLUDE[d365fin](includes/d365fin_md.md)]. For more information, see [How to: Use OCR to Turn PDF and Image Files into Electronic Documents](across-how-use-ocr-pdf-images-files.md).   

Similar functionality exists to reconcile excess amounts on payment reconciliation journal lines on an ad-hoc basis. For more information, see [How to: Reconcile Payments That Cannot be Applied Automatically](receivables-how-reconcile-payments-cannot-apply-auto.md).

Payments posted based on text-to-account mapping are not applied to open entries, but are merely posted to the specified accounts in addition to creating bank account ledger entries. Accordingly, text-to-account mapping is suited for recurring cash receipts or expenses, such as frequent purchases of car fuel or bank fees and interest, that regularly occur on the bank statement and do not need a related business document. For more information, see the “Example - Text-to-Account Mapping for Fuel Expense” section in this topic.

**Note**: Payments on reconciliation journal lines are only set to posting according to text-to-account mapping if the automatic application function can only provide a match confidence of **Low** or **Medium**. If the automatic application function provides a match confidence of High, then the payment is automatically applied to one or more open entries, and the payment is not posted to the accounts specified in the **Text-to-Account Mapping** window. In other words, a match confidence of **High** overrules a text-to-account mapping.

On a payment reconciliation journal line where the payment has been set to posting according to text-to-account mapping, the **Match Confidence** field contains **High - Text-to-Account Mapping**, and the **Account Type** and **Account No.** fields contain the mapped accounts.

## <a name="to-map-text-on-recurring-payments-to-accounts-for-automatic-reconciliation"></a>To map text on recurring payments to accounts for automatic reconciliation
1. In the top right corner, choose the **Search for Page or Report** icon ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon"), enter **Payment Reconciliation Journals**, and then choose the related link.
2. Open a payment reconciliation journal. For more information, see [How to: Reconcile Payments Using Automatic Application](receivables-how-reconcile-payments-auto-application.md).
3. Choose the **Map Text to Account** action. The **Text-to-Account Mapping** window opens.
4. In the **Mapping Text** field, enter any text that occurs on payments that you want to post to specified accounts without applying to an open entry. You can enter up to 50 characters.

    **Note**: If no other payments or incoming documents exist with the mapping text in question, then the text-to-account mapping will occur even when only a part of the text on the payment or incoming document exists as a mapping text.
5. In the **Vendor No.** field, enter the vendor that incoming documents containing the mapping text will be created for, or that payments will be posted to. For more information, see [How to: Use OCR to Turn PDF and Image Files into Electronic Documents](across-how-use-ocr-pdf-images-files.md).      
6. In the **Debit Acc. No.** field, enter the account that payments containing the mapping text will be posted to if they are incoming payments. For incoming payments, the sign of the value in the **Statement Amount** field is positive.
7. In the **Credit Acc. No.** field, enter the account that payments containing the mapping text will be posted to if they are outgoing payments. For outgoing payments, the sign of the value in the **Statement Amount** field is negative.
8. In the **Bal. Source Type** field, specify if the payment will be posted to a general ledger account or to a customer or vendor account.
9. In the **Bal. Source No.** field, specify the account that the payment will be posted to, depending on your selection in the **Bal. Source Type** field.
10. Repeat steps 4 through 8 for all text on payments that you want to map to accounts for direct posting without application.

Next time you import a bank statement file or choose the **Apply Automatically** action in the **Payment Reconciliation Journal** window, journal lines for the payments that contain the specified mapping text will contain the mapped accounts in the **Account Type** and **Account No.** fields. The **Match Confidence** field will contain **High - Text-to-Account Mapping**. This is on the condition that the automatic application function can only provide a match confidence of **Low** or **Medium**.

## <a name="example-text-to-account-mapping-for-fuel-expense"></a>Example: Text-to-Account Mapping for Fuel Expense
To always post fuel expenses incurred at Shell gas stations to the general ledger account for gasoline (account 8510), fill a line in the **Text-to-Account Mapping** window as follows.

| Mapping Text | Debit Acc. No. | Credit Acc. No. | Bal. Source Type | Bal. Source No. |
| --- | --- | --- | --- | --- |
| Shell |BLANK |8510 |G/L Account |BLANK |

**Tip**: For more information about how to work with fields and columns, see [Working with [!INCLUDE[d365fin](includes/d365fin_long_md.md)]](ui-work-product.md). For more information about how to find specific pages, see [Search](ui-search.md).

## <a name="see-also"></a>See Also
[Managing Receivables](receivables-manage-receivables.md)  
[Sales](sales-manage-sales.md)  
[How to: Set Up the Envestnet Yodlee Bank Feeds Service](bank-how-setup-bank-statement-service.md)  
[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions](ui-extensions.md)  
[Working With [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

