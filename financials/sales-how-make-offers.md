---
title: Create a Sales Offer to a Customer | Microsoft Docs
description: Describes how to create a sales offer or a request for proposal (RFQ) document to record your offer to a customer to sell products under certain terms.
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: rfq
ms.date: 08/08/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: 552fbf283a9149c430ea1ed94bcea4bd22e43fea
ms.contentlocale: en-nz
ms.lasthandoff: 01/30/2018

---
# <a name="make-offers"></a>Make Offers
You create a sales quote to record your offer to a customer to sell certain products on certain delivery and payment terms. You can send the sales quote to the customer to communicate the offer. You can email the document as a PDF attachment. You can also have the email body prefilled with a summary of the quote. For more information, see [Send Documents by Email](ui-how-send-documents-email.md).

While you negotiate with the customer, you can change and resend the sales quote as much as needed. When the customer accepts the quote, you convert the sales quote to a sales invoice or a sales order in which you process the sale. For more information, see [Invoice Sales](sales-how-invoice-sales.md) or [Sell Products](sales-how-sell-products.md).

You can fill customer fields on the sales quote in two ways depending on whether the customer is already registered. See steps 2 and 3 in the following procedure.

## <a name="to-create-a-sales-quote"></a>To create a sales quote
On the Home page,  choose the **Sales Quote** action.  
2. In the **Customer** field, enter the name of an existing customer.

   Other fields in the **Sales Quote** window contain standard information of the selected customer. If the customer is not registered, follow these steps:
3. In the **Customer** field, enter the name of the new customer.
4. In the dialogue box about registering the new customer, choose the **Yes** button.
5. In the **Select a template for a new customer** window, choose a template to base the new customer card on, and then choose the **OK** button.
6. A new customer card displays the information on the selected customer template. Fill in the remaining fields. For more information, see [Register New Customers](sales-how-register-new-customers.md).  
7. When you have completed the customer card, choose the **OK** button to return to the **Sales Quote** window.

   Several fields on the sales quote are now filled with information that you specified on the new customer card.  
8. Fill in the remaining fields in the **Sales Quote** window as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

You are now ready to fill in the sales order lines for products that you are selling to the customer or for any transaction with the customer that you want to record in a G/L account.   

If you have set up recurring sales lines for the customer, such as a monthly replenishment order, then you can insert these lines on the order by choosing the **Get Recurring Sales Lines** action.  
9. On the **Lines** FastTab, in the **Type** field, select what type of product, charge, or transaction that you will post for the customer with the sales line.
10. In the **No.** field, select a record to post according to the value in the **Type** field.

 You leave the **No.** field empty in the following cases: -If the line is for a comment. Write the comment in the **Description** field.
 -If the line is for a nonstock item. Choose the **Select Nonstock Items** action. For more information, see [Work With Nonstock Items](inventory-how-work-nonstock-items.md).

11. In the **Quantity** field, enter how many units of the product, charge, or transaction that the line will record for the customer.

    > [!NOTE]  
>   If the item is of type **Item - Service** or **Resource**, the quantity is a time unit, such as hours, as indicated in the **Unit of Measure Code** field on the line.  

    The value in the **Line Amount** field is calculated as *Unit Price* x *Quantity*.  

    The price and line amounts are with or without sales tax, depending on what you selected in the **Prices Including Tax** field on the customer card.  
12. If you want to give a discount, enter a percentage in the **Line Discount %** field. The value in the **Line Amount** field updates accordingly.  

    If special item prices are set up on the **Sales Prices and Sales Line Discounts** FastTab on the customer or item card, the price and amount on the sales line automatically update if the price criteria is met. For more information, see [Record Sales Price, Discount, and Payment Agreements](sales-how-record-sales-price-discount-payment-agreements.md).  
13. Repeat steps 9 through 12 for every product you want to offer the customer.  

    The totals under the lines are automatically calculated as you create or modify lines.  
14. In the **Invoice Discount Amount** field, enter an amount that should be deducted from the value shown in the **Total Incl. Tax** field.

    If you have set up invoice discounts for the customer, then the specified percentage value is automatically inserted in the **Invoice Discount %** field if the criteria are met, and the related amount is inserted in the **Inv. Discount Amount Excl. Tax** field. For more information, see [Record Sales Price, Discount, and Payment Agreements](sales-how-record-sales-price-discount-payment-agreements.md).
15. When the sales quote lines are completed, choose the **Send by Email** action.
16. In the **Send Email** window, fill in any remaining fields and review the embedded sales quote. For more information, see [Send Documents by Email](ui-how-send-documents-email.md).
17. If the customer accepts the quote, choose the **Make Invoice** or the **Make Order** action.

The sales quote is removed from the database. A sales invoice or a sales order is created based on the information in the sales quote in which you can process the sale. In the **Quote No.** field on the sales invoice or sales order, you can see the number of the sales quote that it was made from. For more information, see [Invoice Sales](sales-how-invoice-sales.md) or [Sell Products](sales-how-sell-products.md).

## <a name="see-also"></a>See Also
[Sales](sales-manage-sales.md)  
[Setting Up Sales](sales-setup-sales.md)  
[Send Documents by Email](ui-how-send-documents-email.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

