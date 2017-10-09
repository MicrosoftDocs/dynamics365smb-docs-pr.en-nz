---
title: Create a Purchase Invoice and Record Purchases | Microsoft Docs
description: Describes how to purchase inventory and service items by creating and posting purchase invoices or orders.
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: procurement
ms.date: 08/08/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 5bd635465626c192d8650cbd2a999dd0fbceb15e
ms.contentlocale: en-nz
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-record-purchases"></a>How to: Record Purchases
You create a purchase invoice or purchase order to record the cost of purchases and to track accounts payable. If you need to control an inventory, purchase invoices and purchase orders are also used to dynamically update inventory levels so that you can minimise your inventory costs and provide better customer service. The purchasing costs, including service expenses, and inventory values that result from posting purchase invoices or orders contribute to profit figures and other financial KPIs on your Home page.

> [!NOTE]  
>   You must use purchase orders if your purchasing process requires that you record partial receipts of an order quantity, for example, because the full quantity was not available at the vendor. If you sell items by delivering directly from your vendor to your customer, as a drop shipment, then you must also use purchase orders. For more information, see [How to: Make Drop Shipments](sales-how-drop-shipment.md). In all other aspects, purchase orders work the same way as purchase invoices. The following procedure is based on a purchase invoice. The steps are similar for a purchase order.

When you receive the inventory items, or when the purchased service is completed, you post the purchase invoice or order to update inventory and financial records and to activate payment to the vendor according to the payment terms. For more information, see [Making Payments](payables-make-payments.md).

> [!CAUTION]  
>   Do not post a purchase invoice until you receive the items and know the final cost of the purchase, including any additional charges. Otherwise, your inventory value and profit figures may be skewed.

You can easily correct or cancel a posted purchase invoice before you pay the vendor. This is useful if you want to correct a typing mistake or if you want to change the purchase early in the order process. For more information, see [How to: Correct or Cancel Unpaid Purchase Invoices](purchasing-how-correct-cancel-unpaid-purchase-invoices.md). If you have already paid for items on the posted purchase invoice, then you must create a purchase credit memo to reverse the purchase. For more information, see [How to: Process Purchase Returns or Cancellations](purchasing-how-process-purchase-returns-cancellations.md).

Items can be type **Inventory** or **Service**. For more information, see [How to: Register New Items](inventory-how-register-new-items.md). The purchase invoice process is the same for both item types.

> [!NOTE]  
>   Purchase order functionality requires that your experience is set to **Suite**. For more information, see [Customizing Your [!INCLUDE[d365fin](includes/d365fin_md.md)] Experience](ui-experiences.md).

You can fill vendor fields on the purchase invoice in two ways depending on whether the vendor is already registered.

## <a name="to-create-a-purchase-invoice"></a>To create a purchase invoice
1. On the Home page, choose the **Purchase Invoice** action.  
2. In the **Vendor** field, enter the name of an existing vendor.

    Other fields in the **Purchase Invoice** window are now filled with the standard information of the selected vendor. If the vendor is not registered, then follow these steps:
3. In the **Vendor** field, enter the name of the new vendor.
4. In the dialogue box about registering the new vendor, choose the **Yes** button.
5. In the **Select a template for a new vendor** window, choose a template to base the new vendor card on, and then choose the **OK** button.
6. A new vendor card opens, prefilled with the information on the selected vendor template. The **Name** field is prefilled with the new vendor’s name that you entered on the purchase invoice.
7. Proceed to fill in the remaining fields on the vendor card. For more information, see [How to: Register New Vendors](purchasing-how-register-new-vendors.md).  
8. When you have completed the vendor card, choose the **OK** button to return to the **Purchase Invoice** window.

    Several fields in the **Purchase Invoice** window are filled with information that you specified on the new vendor card.
9. Fill in the remaining fields in the **Purchase Invoice** window as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

    You are now ready to fill in the purchase invoice lines with inventory items or services that you have purchased from the vendor.

    > [!NOTE]  
>   If you have set up recurring purchase lines for the vendor, such as a monthly replenishment order, then you can insert these lines on the invoice by choosing the **Get Recurring Purchase Lines** action.
10. On the **Lines** FastTab, in the **Item No.** field, enter the number of an inventory item or service.
11. In the **Quantity** field, enter the number of items to be purchased.

    > [!NOTE]  
>   For items of type **Service**, the quantity is a time unit, such as hours, as indicated in the **Unit of Measure Code** field on the line.

    The **Line Amount** field is updated to show the value in the **Direct Unit Cost** field multiplied by the value in the **Quantity** field.

    The price and line amount are shown with or without sales tax depending on what you selected in the **Prices Including Tax** field on the vendor card.
12. In the **Invoice Discount Amount** field, enter an amount that should be deducted from the value shown in the **Total Incl. Tax** field at the bottom of the invoice.

    > [!NOTE]  
>   If you have set up invoice discounts for the vendor, then the specified percentage value is automatically inserted in the **Vendor Invoice Discount %** field if the criteria are met, and the related amount is inserted in the **Invoice Discount Amount** field.
13. When you receive the purchased items or services, choose **Post**.

The purchase is now reflected in inventory and financial records, and the vendor payment is activated. The purchase invoice is removed from the list of purchase invoices and replaced with a new document in the list of posted purchase invoices.

## <a name="see-also"></a>See Also
[Purchasing](purchasing-manage-purchasing.md)  
[Setting Up Purchasing](purchasing-setup-purchasing.md)  
[How to: Request Quotes](purchasing-how-request-quotes.md)  
[How to: Purchase Items for a Sale](purchasing-how-purchase-products-sale.md)  
[How to: Register New Vendors](purchasing-how-register-new-vendors.md)  
[How to: Prepare Drop Shipments](sales-how-drop-shipment.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

