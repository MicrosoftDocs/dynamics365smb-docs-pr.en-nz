---
title: Create a Customer Sales Order and Sell Products
description: Describes how to create a sales order to record your agreement with a customer to sell or trade products under specific terms.
author: SorenGP
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 'trade, partial deliveries, customer sales order, shipping advice, partial shipments,'
ms.search.form: '42, 48, 9305'
ms.date: 09/02/2022
ms.author: edupont
---
# <a name="sell-products-with-a-customer-sales-order"></a>Sell Products with a Customer Sales Order

This article provides guidance on when you should use a customer sales order in addition to an invoice. If your sales process requires you to only ship part of an order, perhaps because the full quantity is not available right away, you must process that sale by making a sales order.

You must also use sales orders if you sell items that deliver directly from your vendor to your customer, in what is called a drop shipment. Learn more at [Make Drop Shipments](sales-how-drop-shipment.md). In all other respects, sales orders work the same way as sales invoices. Learn more at [Invoice Sales](sales-how-invoice-sales.md).

When you deliver the products, either fully or partially, you post the sales order as shipped or as shipped and invoiced to create the related item and customer ledger entries in your system. When you post the sales order, you can also email it as a PDF attachment. You can prefill the email body with a summary of the order and payment information, such as a link to PayPal. Learn more at [Ship Items](warehouse-how-ship-items.md) and [Send Documents by Email](ui-how-send-documents-email.md).

In business environments where the customer pays immediately, for example by PayPal or cash, payment is recorded immediately when you post the sales order as invoiced, that is, the posted sales invoice is closed as fully applied. You select the relevant method in the **Payment Method Code** field on the sales order. See step 5 below. For electronic payments, such as PayPal, you must also fill in the **Payment Service** field. Learn more at [Enable Customer Payments Through Payment Services](sales-how-enable-payment-service-extensions.md).

You can even create directly paid orders for non-registered customers by first setting up a "cash customer" card, which you point to on the sales order. Learn more at [Set Up Cash Customers](finance-how-to-set-up-cash-customers.md).

## <a name="create-a-sales-order"></a>Create a sales order

> [!NOTE]  
> The following procedure assumes that the customer is already set up. For instructions on how to do this, please see [Register New Customers](sales-how-register-new-customers.md).

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, then choose the related link.
2. Select **New** to create a new entry.
3. In the **Customer** field, enter the name of an existing customer.

    Other fields on the **Sales Order** page are now filled with standard information about the selected customer.  

4. Fill in the remaining fields on the **Sales Order** page as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

    > [!NOTE]  
    > If you allow the customer to pay immediately, for example, by credit card or PayPal, then fill in the **Payment Method Code** field. The payment is then recorded as soon as you post the sales order as invoiced. If you select *cash*, then the payment is recorded in a specified balancing account.

    You are now ready to fill in the sales order lines with inventory items or services you want the customer to purchase.

    If you have set up recurring sales lines for the customer, such as a monthly replenishment order, you can insert these lines on the order by choosing the **Get Recurring Sales Lines** action.
5. On the **Lines** FastTab, in the **Type** field, select what type of product, charge, or transaction you will post to the customer on the sales line.

6. In the **No.** field, enter the number of an inventory item or service.

    You leave the **No.** field empty if the line is for a:

    * Comment. Write the comment in the **Description** field.
    * Catalogue item. Choose the **Select Catalogue Items** action. Learn more at [Work With Catalogue Items](inventory-how-work-nonstock-items.md).
7. In the **Quantity** field, enter the number of items to be sold.

    > [!NOTE]  
    > For items of the *Resource* or *Service* type, the quantity is a time unit, such as hours, as indicated in the **Unit of Measure Code** field on the line. Learn more at [Set Up Item Units of Measure](inventory-how-setup-units-of-measure.md).

    The **Line Amount** field is updated to show the value in the **Unit Price** field multiplied by the number in the **Quantity** field.

    The price and line amounts are shown with or without GST depending on what you selected in the **Prices Including Tax** field on the customer card.
8. In the **Line Discount %** field, enter a percentage if you want to grant the customer a discount on the product. The value in the **Line Amount** field is updated accordingly.

    If you've set up special item prices on the **Sales Prices and Sales Line Discounts** FastTab on the customer or item card, then the price and amount on the quote line are automatically updated if the agreed price criteria is met. Learn more at [Record Sales Price, Discount, and Payment Agreements](sales-how-record-sales-price-discount-payment-agreements.md).
9. To add a comment about the order line the customer can see on the printed sales order, write a comment on an empty line in the **Description** field.  
10. Repeat steps 5 through 9 for every item you want to the customer to purchase.

    The totals fields under the lines are automatically updated as you create or modify lines to display the amounts to be posted to the ledgers.

    > [!NOTE]
    > In very rare cases, the posted amounts may deviate from what is displayed in the totals fields. This is typically due to rounding calculations in relation to goods and services tax (GST) or sales tax.
    >
    > To check the amounts that will actually post, use the **Statistics** page, which takes into account the rounding calculations. Also, if you choose the **Release** action, the totals fields will be updated to include rounding calculations.  

11. Optionally, in the **Invoice Discount Amount** field, enter the amount to be deducted from the value shown in the **Total Incl. Tax** field.

    If you've set up invoice discounts for the customer, the specified percentage value is automatically inserted in the **Invoice Discount %** field if the criteria is met, and the related amount is inserted in the **Inv. Discount Amount Excl. Tax** field. Learn more at [Record Sales Price, Discount, and Payment Agreements](sales-how-record-sales-price-discount-payment-agreements.md).
12. To ship only part of the order quantity, enter that quantity in the **Qty. to Ship** field. The value automatically copies to the **Qty. to Invoice** field.

    > [!NOTE]
    > If the **Shipping Advice** field is set as **Complete** in the **Shipping and Billing** FastTab, you cannot post partial shipments. Learn more at [Process Partial Shipments](sales-how-send-partial-shipments.md).
13. To invoice only part of the shipped quantity, enter that quantity in the **Qty. to Invoice** field. The quantity must be lower than the value in the **Qty. to Ship** field.  
14. When the sales order lines are completed, choose the **Post and Send** action.

[!INCLUDE [order-ship-invoice](includes/order-ship-invoice.md)]

The **Post and Send Confirmation** dialog box displays the customer's preferred method of receiving documents. You can change the sending method by choosing the lookup button for the **Send Document to** field. Learn more at [Set Up Document Sending Profiles](sales-how-setup-document-send-profiles.md).

The related item and customer ledger entries are now created in your system, and the sales order is output as a PDF document. When the sales order is fully posted, it's removed from the list of sales orders and replaced with new documents in the list of posted sales invoices and the list of posted sales shipments.  

## <a name="external-document-number"></a>External document number

[!INCLUDE [ext-doc-no-sales](includes/ext-doc-no-sales.md)]

## <a name="see-related-microsoft-training"></a>See related [Microsoft training](/training/modules/create-sales-documents-dynamics-365-business-central/).

## <a name="see-also"></a>See also

[Invoice Sales](sales-how-invoice-sales.md)  
[Posting Sales](ui-post-sales.md)  
[Ship Items](warehouse-how-ship-items.md)  
[Make Drop Shipments](sales-how-drop-shipment.md)  
[Sales](sales-manage-sales.md)  
[Setting Up Sales](sales-setup-sales.md)  
[Print the Picking List](sales-how-print-picking-list.md)  
[Process Partial Shipments](sales-how-send-partial-shipments.md)  
[Inventory](inventory-manage-inventory.md)  
[Send Documents by Email](ui-how-send-documents-email.md)  
[Work with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
