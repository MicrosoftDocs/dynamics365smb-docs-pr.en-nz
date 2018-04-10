---
title: Create a Sales Invoice or Sales Order | Microsoft Docs
description: Describes how to create a bill of sale, or a sales invoice or sales order, to record your agreement with a customer to sell products under specific terms.
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: bill, sale, invoice, order
ms.date: 03/12/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: f03cc11b5d8cb349567138604857ad3a679967cf
ms.openlocfilehash: 34c5b47885e82e6dc2985fabb8a4c202ede9c0f9
ms.contentlocale: en-nz
ms.lasthandoff: 04/03/2018

---
# <a name="invoice-sales"></a>Invoice Sales
You create a sales invoice or sales order to record your agreement with a customer to sell certain products on certain delivery and payment terms.  

There are a couple of scenarios where you must use a sales order instead of a sales invoice:  

* If you need to ship only part of an order quantity, for example, because the full quantity is not on hand.  
* If you sell items that your vendor delivers directly to your customer, known as drop shipment. For more information, see [Make Drop Shipments](sales-how-drop-shipment.md).  

In all other aspects, sales orders and sales invoices work in the same way. For more information, see [Sell Products](sales-how-sell-products.md).

You can negotiate with the customer by first creating a sales quote, which you can convert to a sales invoice when you agree on the sale. For more information, see [Make Offers](sales-how-make-offers.md).

If the customer decides to buy, you post the sales invoice to create the related quantity and value entries. When you post the sales invoice, you can also email the document as a PDF attachment. You can have the email body prefilled with a summary of the invoice and payment information, such as a link to PayPal. For more information, see [Send Documents by Email](ui-how-send-documents-email.md).

In business environments where the customer must pay before products are delivered, such as in retail, you must wait for the receipt of payment before you deliver the products. In most cases, you process incoming payments some weeks after delivery by applying the payments to their related posted, unpaid sales invoices. For more information, see [Reconcile Payments Using Automatic Application](receivables-how-reconcile-payments-auto-application.md).

In business environments where the customer pays immediately, for example by cash, PayPal, or credit card, you can select the relevant method in the **Payment Method Code** field on the sales invoice. Payment is then recorded immediately on the posted invoice. For payment services, you must also fill in the **Payment Service** field. For more information, see [Enable Customer Payments Through Payment Services](sales-how-enable-payment-service-extensions.md).

You can even create directly paid invoices for non-registered customers by first setting up a "cash customer" card, which you point to on the sales invoice. For more information, see [Set Up Cash Customers](finance-how-to-set-up-cash-customers.md).  

You can easily correct or cancel a posted sales invoice before it is paid. For example, this is useful if you want to correct a typing mistake or if the customer requests a change early in the order process. For more information, see [Correct or Cancel Unpaid Sales Invoices](sales-how-correct-cancel-sales-invoice.md). If the posted sales invoice is paid, then you must create a sales credit memo to reverse the sale. For more information, see [Process Sales Returns or Cancellations](sales-how-process-sales-returns-cancellations.md).

Items can be both inventory items and services, denoted by the **Inventory** and **Service** types on the item card. The sales invoice process is the same for both item types. For more information, see [Register New Items](inventory-how-register-new-items.md).

You can fill customer fields on the sales invoice in two ways depending on whether the customer is already registered. See steps 2 and 3 in the following procedure.

## <a name="to-create-a-sales-invoice"></a>To create a sales invoice
1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sales Invoices**, and then choose the related link.  
2. In the **Customer** field, enter the name of an existing customer.

   Other fields in the **Sales Invoice** window contain standard information about the selected customer. If the customer is not registered, follow these steps:
3. In the **Customer** field, enter the name of the new customer.
4. In the dialogue box about registering the new customer, choose the **Yes** button.
5. In the **Select a template for a new customer** window, choose a template to base the new customer card on, and then choose the **OK** button.
6. A new customer card displays the information on the selected customer template. Fill in the remaining fields. For more information, see [Register New Customers](sales-how-register-new-customers.md).  
7. When you have completed the customer card, choose the **OK** button to return to the **Sales Invoice** window.

   Several fields on the sales invoice are now filled with information that you specified on the new customer card.  
8. Fill in the remaining fields in the **Sales Invoice** window as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

    You are now ready to fill in the sales invoice lines for products that you are selling to the customer or for any transaction with the customer that you want to record in a G/L account.   

    If you have set up recurring sales lines for the customer, such as a monthly replenishment order, then you can insert these lines on the order by choosing the **Get Recurring Sales Lines** action.  
9. On the **Lines** FastTab, in the **Type** field, select what type of product, charge, or transaction that you will post for the customer with the sales line.
10. In the **No.** field, select a record to post according to the value in the **Type** field.

    You leave the **No.** field empty in the following cases:

    * If the line is for a comment. Write the comment in the **Description** field.
    * If the line is for a nonstock item. Choose the **Select Nonstock Items** action. For more information, see [Work With Nonstock Items](inventory-how-work-nonstock-items.md).

11. In the **Quantity** field, enter how many units of the product, charge, or transaction that the line will record for the customer.  

    > [!NOTE]  
    >   If the item is of type **Service**, or the **Type** field contains **Resource**, then the quantity is a time unit, such as hours, as indicated in the **Unit of Measure Code** field on the line.  

    The value in the **Line Amount** field is calculated as *Unit Price* x *Quantity*.  

    The price and line amounts are with or without sales tax, depending on what you selected in the **Prices Including Tax** field on the customer card.  
12. If you want to give a discount, enter a percentage in the **Line Discount %** field. The value in the **Line Amount** field updates accordingly.  

    If special item prices are set up on the **Sales Prices and Sales Line Discounts** FastTab on the customer or item card, the price and amount on the sales line automatically update if the price criteria is met. For more information, see [Record Sales Price, Discount, and Payment Agreements](sales-how-record-sales-price-discount-payment-agreements.md).  
13. Repeat steps 9 through 12 for every product or charge you want to sell to the customer.  

    The totals under the lines are automatically calculated as you create or modify lines.  
14. In the **Invoice Discount Amount** field, enter an amount that should be deducted from the value shown in the **Total Incl. Tax** field.

    If you have set up invoice discounts for the customer, then the specified percentage value is automatically inserted in the **Invoice Discount %** field if the criteria are met, and the related amount is inserted in the **Inv. Discount Amount Excl. Tax** field. For more information, see [Record Sales Price, Discount, and Payment Agreements](sales-how-record-sales-price-discount-payment-agreements.md).  
15. When the sales invoice lines are completed, choose the **Post and Send** action.  

The **Post and Send Confirmation** dialog box displays the customer's preferred method of receiving documents. You can change the sending method by choosing the lookup button for the **Send Document to** field. For more information, see [Set Up Document Sending Profiles](sales-how-setup-document-send-profiles.md).

The related item and customer ledger entries are now created in your system, and the sales invoice is output as a PDF document. The sales invoice is removed from the list of sales invoices and replaced with a new document in the list of posted sales invoices.

## <a name="see-also"></a>See Also
[Sales](sales-manage-sales.md)  
[Setting Up Sales](sales-setup-sales.md)  
[Inventory](inventory-manage-inventory.md)  
[Send Documents by Email](ui-how-send-documents-email.md)  
[Bulk Invoicing from Microsoft Bookings in Business Central ](finance-bookings.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

