---
title: Apply Customer Ledger Entries to Manually Reconcile Customer Payments | Microsoft Docs
description: Describes how to apply customer cash receipts or refunds to one or more open customer ledger entries and reconcile customer payments.
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: payment process, cash receipt
ms.date: 09/08/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: ccef6a35b1632bd94f64c5e9ad56ecd3bacbfd06
ms.contentlocale: en-nz
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-reconcile-customer-payments-manually"></a>How to: Reconcile Customer Payments Manually
When you receive a cash receipt from a customer, or you make a cash refund, you must decide whether to apply the payment or refund to close one or more open debit or credit entries. You can specify the amount you want to apply. For example, you can apply partial payments to customer ledger entries. Closing customer ledger entries makes sure that information such as customer statistics, account statements, and finance charges are correct.

> [!NOTE]  
>   In the **Customer Ledger Entries** window, red font means that the related payment is past its due date.

You can apply customer ledger entries in several ways:

* By entering information in dedicated windows, such as the **Cash Receipt Journal** and **Payment Reconciliation Journal** windows.
* From sales credit memo documents.
* From customer ledger entries after sales documents are posted but not applied.

> [!NOTE]  
>   If the **Application Method** field on the customer card contains **Apply to Oldest**, payments are applied to the oldest open credit entry, unless you manually specify an entry. If the application method is **Manual**, you always apply entries manually.

You can apply customer payments manually in the **Cash Receipt Journal** window. A cash receipt journal is a type of general journal, so you can use it to post transactions to general ledger, bank, customer, vendor, and fixed assets accounts. You can apply the payment to one or more debit entries when you post the payment, or you can apply from the posted entries later.

You can also apply customer and vendor payments in the **Payment Reconciliation Journal** window, by using functions for bank statement import, automatic application, and bank account reconciliation. For more information, see [Reconcile Payments Using Automatic Application](receivables-how-reconcile-payments-auto-application.md). Alternatively, you can reconcile customer payments based on a list of unpaid sales documents in the **Payment Registration** window. For more information, see [How to: Reconcile Customer Payments From a List of Unpaid Sales Documents](receivables-how-reconcile-customer-payments-list-unpaid-sales-documents.md)

## <a name="to-fill-and-post-a-cash-receipt-journal"></a>To fill and post a cash receipt journal
1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Cash Receipt Journal**, and then choose the related link.
2. Choose the **Edit Journal** action.
3. Select the relevant batch in the **Batch Name** field.
4. Fill in the **Posting Date** field.  
5. In the **Document Type** field, select **Payment**.

    The **Document No.** field is filled by the number series assigned to the batch.  
6. Use the **External Document No.** field to store an identifier, such as the customer's cheque number.
7. In the **Account Type** field, select **Customer**.
8. In the **Account No.** field, select the relevant G/L account.
9. If you want to post the application at the same time as you post the journal, do one of the following.
10. In the **Balancing Account Type** field, select **G/L Account** for cash payments, and **Bank Account** for other payments.
11. In the **Balancing Account No.** field, select the cash account for cash payments, or the relevant bank account for other payments.
12. Post the journal.

## <a name="to-apply-a-payment-to-a-single-customer-ledger-entry"></a>To apply a payment to a single customer ledger entry
1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Cash Receipt Journal** and choose the related link.
2. Choose the **Edit Journal** action.
3. On the first journal line, enter the relevant information about the entry to be applied.
4. In the **Document Type** field, enter **Payment**.
5. In the **Account Type** field, enter **Customer**.
6. In the **Bal. Account Type** field, enter **Bank Account**.
7. In the **Applies-to Doc. No.** field, choose the field to open the **Apply Customer Entries** window.
8. In the **Apply Customer Entries** window, select the entry to apply the payment to.
9. In the **Amount to Apply** field, enter the amount you want to apply to the entry. If you do not enter an amount, the maximum amount is applied.

    At the bottom of the **Apply Customer Entries** window, you can see the specific amount in the **Applied Amount** field and also whether the application balances.  
10. Choose the **OK** button. The **Cash Receipt Journal** window now shows the entry you have selected entered in the **Applies-to Doc. Type** and **Applies-to Doc. No.** fields.
11. Post the cash receipt journal.

## <a name="to-apply-a-payment-to-multiple-customer-ledger-entries"></a>To apply a payment to multiple customer ledger entries
1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Cash Receipt Journal**, and then choose the related link.
2. Choose the **Edit Journal** action.
3. On the first journal line, enter the relevant information about the entry to be applied.
4. In the **Document Type** field, enter **Payment**.
5. In the **Account Type** field, enter **Customer**.
6. In the **Bal. Account Type** field, enter **Bank Account**.
7. In the **Amount** field, enter the full payment as a negative amount.
8. To apply the payment to multiple customer ledger entries when posting, choose the **Apply Entries** action.  
9. Select the lines with the entries that you want the applying entry to be applied to, and then choose the **Set Applies-to ID** action.  
10. On each line, in the **Amount to Apply** field, enter the amount you want to apply to the individual entry. If you do not enter an amount, the maximum amount is applied.

    At the bottom of the **Apply Customer Entries** window, you can see the specific amount in the **Applied Amount** field and also whether the application balances.  
11. Choose the **OK** button.
12. Post the cash receipt journal.

## <a name="to-apply-a-credit-memo-to-a-single-customer-ledger-entry"></a>To apply a credit memo to a single customer ledger entry
1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sales Credit Memos**, and then choose the related link.
2. Open the relevant sales credit memo.
3. To apply the credit memo to a single customer ledger entry when posting, in the **Applies-to Doc. No.** field, select the entry to which you want to apply the payment.
4. On the line in the **Amount to Apply** field, enter the amount you want to apply to the entry.  

    If you do not enter an amount, the program automatically applies the maximum amount. At the bottom of the **Apply Customer Entries** window, you can see the specific amount in the **Applied Amount** field and also whether the application balances.    
5. Choose the **OK** button. The **Sales Credit Memo** window now shows the entry you have selected entered in the **Applies-to Doc. Type** and **Applies-to Doc. No.** fields. And the amount of the credit memo to be posted, adjusted for any possible payment discounts.
6. Post the credit memo.

## <a name="to-apply-a-credit-memo-to-multiple-customer-ledger-entries"></a>To apply a credit memo to multiple customer ledger entries
1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sales Credit Memos**, and then choose the related link.
2. Open the relevant sales credit memo.
3. To apply the credit memo to multiple customer ledger entries when posting, choose the **Apply Entries** action.
4. Select the lines with the entries that you want the applying entry to be applied to, and then choose the **Set Applies-to ID** action.
5. On each line, in the **Amount to Apply** field, enter the amount you want to apply to the individual entry. If you do not enter an amount, the maximum amount is applied.  

    At the bottom of the **Apply Customer Entries** window, you can see the specific amount in the **Applied Amount** field and also whether the application balances.  
6. Choose the **OK** button. The **Sales Credit Memo** window now shows the amount of the credit memo to be posted, adjusted for any possible payment discounts.
7. Post the credit memo.

## <a name="to-apply-posted-customer-ledger-entries"></a>To apply posted customer ledger entries
1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Customers**, and then choose the related link.
2. Open the customer card for the customer with entries that you want to apply.
3. Choose the **Ledger Entries** action, and then select the line with the entry that will be the applying entry.
4. Choose the **Apply Entries** action. The **Apply Customer Entries** window opens showing the open entries for the customer.
5. Select the lines with the entries that you want the applying entry to be applied to, and then choose the **Set Applies-to ID.** action.
6. For each line in the **Amount to Apply** field, enter the amount you want to apply to the individual entry. If you do not enter an amount, the maximum amount is applied.  

    At the bottom of the **Apply Customer Entries** window, you can see the specific amount in the **Applied Amount** field.  
7. Choose the **Post Application** action. The **Post Application** window appears with the document number of the applying entry and the posting date of the entry with the most recent posting date.  
8. Choose the **OK** button to post the application.

    If the posted application has resulted in closed customer ledger entries, the **Open** field is cleared for these ledger entries.    
9. To see the ledger entries, choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Customers**, and then choose the related link. Browse to the card for the relevant customer to see the ledger entries.  

On the ledger entry list, on the line that contains the ledger entry that was fully applied to, you can see that the **Open** check box is not selected.  

> [!NOTE]  
>   After you select an entry in the **Apply Customer Entries** window, or several entries by setting the **Applies-to ID**, the **Applied Amount** field on the journal line will contain the sum of the remaining amounts for the posted entries you have selected, unless the field contains something already. If you select **Apply to Oldest** in the **Application Method** field on the customer card, the application occurs automatically.

## <a name="to-apply-customer-ledger-entries-in-different-currencies-to-one-another"></a>To apply customer ledger entries in different currencies to one another
If you sell to a customer in one currency and receive payment in another currency, you can still apply the invoice to the payment.  

If you apply an entry (Entry 1) in one currency to an entry (Entry 2) in a different currency, the posting date on Entry 1 is used to find the relevant exchange rate to convert amounts on Entry 2. The relevant exchange rate is found in the **Currency Exchange Rates** window.  

Applying customer ledger entries in different currencies must be enabled. For more information, see [How to: Enable Application of Ledger Entries in Different Currencies](finance-how-enable-application-ledger-entries-different-currencies.md).  

1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Cash Receipts Journal**, and then choose the related link.
2. Open the journal you want, and fill in the first empty journal line using a currency code.
3. Choose the **Apply Entries** action.
4. Select the line with the entry you want to apply to the entry in the cash receipt journal, choose the **Set Applies-to ID** action, and then select the entry you want to apply to.
5. Choose the **OK** button to return to the cash receipt journal.
6. Post the sales journal.  

> [!IMPORTANT]  
>   When you apply entries in different currencies, the entries are converted to NZD. Although the exchange rates for the two currencies are fixed, for example between NZD and EUR, there may be a small residual amount when they are converted to NZD. These small residual amounts are posted as gains and losses to the account specified in the **Realized Gains Account** or **Realized Losses Account** fields in the **Currencies** window. The **Amount (USD)** field is also adjusted on the vendor ledger entries.  

## <a name="to-correct-an-application-of-customer-entries"></a>To correct an application of customer entries
When you correct an application, correcting entries that are identical to the original entry but with opposite sign in the amount field are created and posted for all entries, including all general ledger posting derived from the application, such as payment discount and currency gains/losses. The entries that were closed by the application are reopened.  

1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Customers**, and then choose the related link.
2. Open the relevant customer card.
3. Choose the **Ledger Entries** action.
4. Select the relevant ledger entry, and then choose the **Unapply Entries** action.
5. Alternatively, choose the **Detailed Ledger Entry** action.
6. Select the application entry, and then choose the **Unapply Entries** action.
7. Fill in the fields in the header, and then choose the **Unapply** action.  

> [!IMPORTANT]  
>   If an entry has been applied by more than one application entry, you must unapply the latest application entry first.  

## <a name="see-also"></a>See Also
[Managing Receivables](receivables-manage-receivables.md)  
[Sales](sales-manage-sales.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

