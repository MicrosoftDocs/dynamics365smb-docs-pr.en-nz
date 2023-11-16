---
title: Define an Invoice Posting Policy for Users
description: Use invoice posting policies to control whether a user can post sales and purchase invoices.
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bholtorf
ms.topic: conceptual
ms.date: 03/09/2023
ms.custom: bap-template
ms.search.forms: '119, 9807,'
---

# <a name="define-an-invoice-posting-policy-for-users"></a>Define an invoice posting policy for users

Companies often have unique processes for posting sales and purchase invoices and shipments. For example, processes can vary from one person posting everything on a purchase order, to multiple employees. You can restrict users from posting invoices, or require that invoices are posted together with shipments or receipts.

## <a name="to-specify-a-posting-policy"></a>To specify a posting policy

On the **User Setup** page, in the **Sales Invoice Posting Policy** and **Purch. Invoice Posting Policy** fields, choose one of the following options:

* **Allowed** (Default) - Keep the current behaviour, where a user can choose the posting option to use, such as **Ship**, **Invoice**, and **Ship and Invoice**. 
* **Prohibited** - Prevent the user from posting invoices. Business Central will show a confirmation dialogue that provides only the **Ship** or **Receive** options.
* **Mandatory** - Allow the user to post invoices together with receipts or shipments. Business Central will show a confirmation dialogue with the **Ship and Invoice** or **Receive and Invoice** options.

## <a name="effect-on-documents"></a>Effect on documents

The following table describes how invoice posting policies affect documents.

> [!NOTE]
> When you post sales and purchase invoices and credit memos, you don't have any posting options. The documents always post the physical and financial transactions together. You can't partially post invoices and credit memos.

|Document | Option 1: Allow <br>Displays a series of options| Option 2: Prohibited <br>Confirmation dialogue | Option 3: Mandatory <br>Confirmation dialogue|
|--|--|--|--|
|Sales order |- Ship <br>- Invoice <br>- Ship and Invoice |Do you want to post the shipment? |Do you want to post the shipment and invoice?|
|Sales invoice|No options|Do you want to post the invoice?|Do you want to post the invoice?|
|Sales credit memo|No options|Do you want to post the credit memo?|Do you want to post the credit memo?|
|Sales return order |- Receive <br>- Invoice <br>- Receive and Invoice |Do you want to post the receipt? |Do you want to post the receipt and invoice?|
|Inventory pick |- Ship <br>- Ship and Invoice |Do you want to post the shipment? |Do you want to post the shipment and invoice?|
|Purchase order |- Receive <br>- Invoice <br>- Receive and Invoice |Do you want to post the receipt? |Do you want to post the receipt and invoice?|
|Purchase invoice|No options|Do you want to post the invoice?|Do you want to post the invoice?|
|Purchase credit memo|No options|Do you want to post the credit memo?|Do you want to post the credit memo?|
|Purchase Return Order |- Ship <br>- Invoice <br>- Ship and Invoice |Do you want to post the shipment? |Do you want to post the shipment and invoice?|
|Inventory Put-away |- Receive <br>- Receive and Invoice |Do you want to post the receipt? |Do you want to post the receipt and invoice?|
|Warehouse Shipment |- Ship <br>- Ship and Invoice | Do you want to post the shipment? |Do you want to post the shipment and invoice?|

   > [!Note]
   > The setting doesn't affect posting of general journal lines where you can select **Invoice** in the **Document Type** field.

## <a name="see-also"></a>See Also

[Invoice Sales](sales-how-invoice-sales.md)  
[Record Purchases with Purchase Invoices and Orders](purchasing-how-record-purchases.md)  
[Purchase Items for a Sale by Creating Purchase Invoices](purchasing-how-purchase-products-sale.md)
[Getting Ready for Doing Business](ui-get-ready-business.md)  
