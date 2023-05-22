---
title: Post Intercompany Documents and Journals
description: This topic explains how you use intercompany documents or journals to post transactions with your intercompany partners.
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bnielse
ms.topic: how-to
ms.date: 02/06/2023
ms.custom: bap-template
ms.search.keywords: 'IC, group, consolidation, affiliate, subsidiary, bank-to-bank'
ms.search.form: '600, 610'
---
# Work with Intercompany Documents and Journals

Use intercompany documents or journals to post transactions with your intercompany partners. You can post transactions to G/L accounts, and if you've set up intercompany bank accounts you can also post bank-to-bank transactions. To learn more about setting up intercompany bank accounts, go to [Specify the bank accounts to use for intercompany partners](intercompany-how-setup.md#specify-the-bank-accounts-to-use-for-intercompany-partners).  

When you post an intercompany document or journal line in your company, a corresponding document or journal line is created in your intercompany outbox. You transfer the line from your outbox to your partner. Your partner can then post the corresponding transaction in their company, without having to re-enter the data.

For sales and purchase documents, the intercompany partner code on the customer or vendor ensures that all orders and invoices for transactions between the partners produce corresponding documents in the partner companies. The company accounts balance correctly.

The same is true for intercompany general journal lines. You don't need to specify accounts, you just choose the the partner company. Corresponding intercompany general journal lines are then created in the partner company.

## Fill in and send an intercompany sales order

You can send sales and purchase orders and return orders before posting. Invoices and credit memos can't be sent until they're posted.

The following procedure describes how to fill in and send an intercompany sales order. The same steps apply to intercompany purchase orders and return orders, and to posted intercompany invoices and credit memos.  

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.  
2. Choose **New** to create a new sales order. For more information, see [Sell Products](sales-how-sell-products.md).  
3. Fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4. Make sure the customer is an intercompany partner.
5. To send the sales order before you post it, choose the **Send IC Sales Order** action.

> [!NOTE]
> If you do step 5, the sales order goes to your intercompany outbox, where you can send it later. To learn more about the intercompany inbox and outbox, go to [Manage the Intercompany Inbox and Outbox](intercompany-how-manage-intercompany-inbox.md).

## Fill in and post an intercompany journal

When you post an intercompany general journal line in your company, a corresponding journal line is created in your intercompany outbox that you can transfer to your partner. With 2022 release wave 1, you can also set up the company to automatically create received intercompany transactions that partners posted in intercompany general journals. Your partner can then post the corresponding transaction in their company, without having to re-enter the data.

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Intercompany General Journals**, and then choose the related link.  
2. Open the journal batch. For more information, see [Work with General Journals](ui-work-general-journals.md).
3. Fill in the fields as necessary. [!INCLUDE [tooltip-inline-tip_md](../archive/invoicing/includes/tooltip-inline-tip_md.md)]
4. In the **IC Partner G/L Acc. No.** field, enter the intercompany general ledger account that the amount will be posted to in your partner's company.

    > [!NOTE]
    > This field must be filled in on a line with a bank account or general ledger account in either the **Account No.** field or the **Bal. Account No.** field.  
5. Choose the **Post** action.

The entries are posted in your company and a journal with the corresponding entries is created in your intercompany outbox so that you can send them to your partner company.

## See Also

[Managing Intercompany Transactions](intercompany-manage.md)  
[Finance](finance.md)  
[Setting Up Finance](finance-setup-finance.md)  
[Work with General Journals](ui-work-general-journals.md)  
[Work with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]