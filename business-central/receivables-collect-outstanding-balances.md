---
title: Collect outstanding balances
description: 'Learn how to remind your customers of outstanding payments. Send a customer statement, issue a reminder, or send a finance charge memo.'
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bholtorf
ms.topic: how-to
ms.search.keywords: 'payment due, debt, overdue, fee, charge, reminder'
ms.search.form: '6, 25, 440, 443, 448, 452'
ms.date: 07/01/2024
ms.service: dynamics-365-business-central
ms.custom: bap-template
---
# <a name="collect-outstanding-balances"></a>Collect outstanding balances

Managing receivables includes checking whether amounts due are paid on time. If customers have overdue payments, you can begin by sending the **Customer Statement** report as a reminder. Alternatively, you can issue reminders.

Use reminders to alert customers to overdue amounts. You can also use reminders to calculate finance charges, such as interest or fees and include them on the reminder. Use finance charge memos if you want to debit customers for interest or fees without reminding them of overdue amounts.

## <a name="statements"></a>Statements

From the customer card, you can create a statement for customer's transactions with you. Then, you can generate a PDF file and send it to the customer. Alternatively, use the **Customer Statement** report to send your customers an overview of their business with you. 

> [!TIP]
> If needed, you can send the statement to Excel to make changes.  

### <a name="to-send-the-customer-statement-report"></a>To send the Customer Statement report

1. Choose the ![Lightbulb that opens the Tell Me feature 10.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Customer Statement**, and then choose the related link.
2. Fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. Under **Output Options**, select how to send the report to the customer.

> [!NOTE]
> If you are using multiple currencies, the Customer Statement report is always printed in the customer's currency. The last date in a statement period is also used as the statement date and the ageing date, if ageing is included.

## <a name="reminders"></a>Reminders

[!INCLUDE [receivables-reminders](includes/receivables-reminders.md)]

## <a name="finance-charges"></a>Finance charges

When a customer doesn't pay by the due date, you can have finance charges calculated automatically and add them to the overdue amounts on the customer's account. You can inform customers of the added charges by sending finance charge memos.  

> [!NOTE]  
> You use finance charge memos to calculate interest and finance charges and to inform your customers about interest and finance charges without reminding them of overdue payments. Alternatively, you can calculate interest on overdue payments when you create reminders.  

Before you can create finance charge memos, you must set up terms. For more information, see [Set Up Finance Charge Terms](finance-setup-finance-charges.md).  

You can manually create a finance charge memo for an individual customer, and fill in the lines automatically. Alternatively, you can use the **Create Finance Charge Memos** function to create finance charge memos for all or selected customers with overdue balances.  

After you create the finance charge memos, you can modify them. The text that appears at the beginning and end of the finance charge memo is determined by the finance charge terms, and can be seen in the **Description** column on the lines. If a calculated amount has been inserted automatically in the beginning or ending text, the text won't be adjusted if you delete lines. Then you must use the **Update Finance Charge Text** function.  

After you have created finance charge memos and made any needed modifications, you can either print test reports or issue the finance charge memos, typically as email.

### <a name="to-create-a-finance-charge-memo-manually"></a>To create a finance charge memo manually

A finance charge memo is similar to an invoice. You can fill in a header manually and have the lines filled in for you, or you can create finance charge memos for all customers automatically.

1. Choose the ![Lightbulb that opens the Tell Me feature 2.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Finance Charge Memos**, and then choose the related link.  
2. Choose the **New** action, and then fill in the fields as necessary.  
3. Choose **Suggest Fin. Charge Memo Lines** action.
4. On the **Suggest Finance Charge Memo Lines** page, set a filter on the **Cust. Ledger Entry** FastTab if you want to create finance charge memos only for specific entries.

    > [!NOTE]
    > Although they are listed, selecting **Payment** and **Credit Memo** as **Document Type** filters will not have any effect because the **Suggest Finance Charge Memo Lines** function only handles positive amounts.
5. Choose the **OK** button to start the batch job.  

### <a name="to-update-finance-charge-memo-texts"></a>To update finance charge memo texts

In some cases, you might want to modify the beginning and ending text that you have set up for the finance charge terms. If you do this at a time when you have created, but not yet issued, finance charge memos, you can update the memos with the modified text.

1. Choose the ![Lightbulb that opens the Tell Me feature 3.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Finance Charge Memo**, and then choose the related link.  
2. open the finance charge memo that you want to change text for, and then choose the **Update Finance Charge Text** action.
3. On the **Update Finance Charge Text** page, you can set a filter if you want to update several memos.
4. Choose the **OK** button to update the beginning and ending texts.  

### <a name="to-issue-finance-charge-memos"></a>To issue finance charge memos

After you create finance charge memos and make any needed modifications, you can either print test reports or issue the finance charge memos.

When you issue a reminder, the entries post according to your specifications on the **Finance Charge Terms** page. This specification determines whether interest and/or additional fees post to the customer's account and the general ledger. Settings on the **Customer Posting Groups** page determine the accounts that interest or fees post to.

For each customer ledger entry on the finance charge memo, an entry is created on the **Reminder/Fin. Charge Entries** page.

If the **Post Interest** or the **Post Additional Fee** checkboxes are selected on the **Finance Charge Terms** page, the following entries are also created:

- One entry on the **Cust. Ledger Entries** page
- One receivables entry in the relevant G/L account
- One interest and/or one additional fee entry in the relevant G/L account

Also, issuing the finance charge memo might result in GST entries.

1. Choose the ![Lightbulb that opens the Tell Me feature 4.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Finance Charge Memos**, and then choose the related link.
2. Select the relevant memo, and then choose the **Issue** action.
3. On the **Issue Finance Charge Memos** page, fill in the fields as necessary.
4. Choose the **OK** button

The finance charge memo is either printed for sent to a specified email as a PDF attachment.

### <a name="to-cancel-an-issued-finance-charge-memo"></a>To cancel an issued finance charge memo

If finance charge memos were issued in error, you can cancel them before they're sent out. You can do this either one by one or as a batch.

1. On the **Issued Finance Charge Memos** page, select one or more lines for issued finance charge memos that you want to cancel, and then choose the **Cancel** action.
2. On the **Cancel Issued Fin. Charge Memos** page, fill in the fields as necessary, and then choose the **OK** button.

### <a name="to-view-reminder-and-finance-charge-entries"></a>To view reminder and finance charge entries

When you issue a reminder, a reminder entry is created on the **Reminder/Fin. Charge Entries** page for each reminder line that contains a customer ledger entry. You can then get an overview of the created reminder entries for a specific customer.

1. Choose the ![Lightbulb that opens the Tell Me feature 5.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Customers**, and then choose the related link.  
2. Open the relevant customer card, and then choose the **Ledger Entries** action.
3. On the **Customer Ledger Entries** page, select the line with the ledger entry you want to see the reminder entries for, and then choose the **Reminder/Fin. Charge Entries** action.

## <a name="multiple-interest-rates"></a>Multiple interest rates

[!INCLUDE [multiple-interest-rates-def](includes/multiple-interest-rates-def.md)] For more information, see [Set Up Multiple Interest Rates](finance-how-to-set-up-multiple-interest-rates.md).  

## <a name="see-also"></a>See also

[Set Up Reminder Terms and Levels](finance-setup-reminders.md)  
[Set Up Finance Charge Terms](finance-setup-finance-charges.md)  
[Managing Receivables](receivables-manage-receivables.md)  
[Sales](sales-manage-sales.md)  
[Work with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)

[!INCLUDE[footer-include](includes/footer-banner.md)]
