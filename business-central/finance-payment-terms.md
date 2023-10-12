---
title: Set Up Payment Terms
description: Use payment terms to manage due dates and payment discounts.
author: brentholtorf
ms.topic: conceptual
ms.search.form: '4,'
ms.date: 09/05/2023
ms.author: bholtorf
---
# Set Up Payment Terms

Payment terms determine how you manage due dates and payment discounts. You can set up any number of payment term codes and use date formulas to define the payment terms. When you first sign up for [!INCLUDE [prod_short](includes/prod_short.md)], the demonstration company provides a few payment methods that businesses often use. You can, however, add as many as you need.  

If you assign payment terms to customers and vendors, the same terms are always used on the sales and purchase documents you create for them. The document dates on sales and purchase documents, not their posting dates, are used to calculate due dates for payments. If needed, you can change the terms on the sales or purchase document, such as if you want a particular customer to pay you within 7 days rather than the default 14 days. Changing the terms on the document doesn't change the default payment term assigned to the customer. The same payment terms are available for sales and purchase documents.

When you post an invoice, [!INCLUDE [prod_short](includes/prod_short.md)] calculates the payment discounts based on the payment terms. The payment discount date is the last date that the customer can receive a discount. The date is also calculated when you post an invoice.  

Similarly, when you post a credit memo, [!INCLUDE [prod_short](includes/prod_short.md)] calculates payment discounts based on the payment terms. It calculates the discount on credit memos in the same way as discounts on invoices. When you apply a credit memo to an invoice, [!INCLUDE [prod_short](includes/prod_short.md)] reduces the discount amount for the invoice by the credit memo's discount amount.  

If you want to send your customers reminders of overdue payments, you must set up reminder levels and terms. To learn more about reminders, go to [Set Up Reminder Terms and Levels](finance-setup-reminders.md).  

## To set up payment terms

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Payment Terms**, and then choose the related link.  
2. Fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

After you set up the payment terms, you assign them to customers and vendors. Optionally, assign payment terms to your payment methods.  

> [!TIP]
> In the base version of [!INCLUDE [prod_short](includes/prod_short.md)], payment terms with partial payments are not supported. Instead, you must use the prepayments functionality. To learn more about prepayments, go to [Set Up Prepayments](finance-set-up-prepayments.md).
>
> In some countries/regions, you *can* set up payment terms with partial payments. To learn whether your country/region supports this capability, go to the **Local Functionality** section in the table of contents on the left side of a [Microsoft Learn](about-localization.md) article.

## See Also

[Set Up Payment Methods](finance-payment-methods.md)  
[Set Up Prepayments](finance-set-up-prepayments.md)  
[Setting Up Finance](finance-setup-finance.md)  
[Register New Customers](sales-how-register-new-customers.md)  
[Register New Vendors](purchasing-how-register-new-vendors.md)  
[Sales](sales-manage-sales.md)  
[Purchasing](purchasing-manage-purchasing.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]