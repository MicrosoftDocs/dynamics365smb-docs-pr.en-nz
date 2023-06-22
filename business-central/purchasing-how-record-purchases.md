---
title: Record Purchases with Purchase Invoices  (contains video)
description: 'Describes how to purchase inventory, non-inventory items, or resources by creating and posting purchase invoices or orders.'
author: SorenGP
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: procurement
ms.search.form: '50 ,51, 53, 56, 146, 147, 9307, 9309, 9306, 9308, 9310'
ms.date: 09/01/2022
ms.author: edupont
---
# <a name="record-purchases-with-purchase-invoices-and-orders" />Record Purchases with Purchase Invoices and Orders

You create a purchase invoice or purchase order to record the cost of purchases and to track accounts payable. Purchase invoices and purchase orders are also used to dynamically update inventory levels, meaning you can minimise inventory costs and provide better customer service. The purchasing costs, including service expenses, and inventory values that result from posting purchase invoices or orders contribute to profit figures and other financial key performance indicators (KPIs) in your Role Centre.

## <a name="record-purchases-with-purchase-invoices" />Record Purchases with Purchase Invoices

When you receive the inventory items or the purchased service is complete, post the purchase invoice to update inventory and financial records and to activate payment to the vendor according to the payment terms. [Making Payments](payables-make-payments.md).

> [!CAUTION]  
> Do not post a purchase invoice for physical items until you receive the items and know the final cost of the purchase, including any additional charges. Otherwise, your inventory value and profit figures may be skewed.

### <a name="create-a-and-post-purchase-invoice" />Create a and post purchase invoice

The following describes how to create a purchase invoice. The steps are similar for a purchase order. The main difference is that purchase orders have additional fields and actions for physical handling of items.

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchase Invoices**,  then choose the related link.  
2. In the **Vendor** field, enter the name of an existing vendor.

    Other fields on the **Purchase Invoice** page are now filled with standard information for the selected vendor. If the vendor is not registered, follow these steps:

    1. In the **Vendor** field, enter the name of the new vendor.
    2. In the dialogue box about registering the new vendor, choose **Yes**.
    3. To learn more on how to fill in the vendor card, go to [Register New Vendors](purchasing-how-register-new-vendors.md).  
    4. When you've completed the vendor card, choose **OK** to return to the **Purchase Invoice** page.

3. Fill in the remaining fields on the **Purchase Invoice** page as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

    You are now ready to fill in the purchase invoice lines with items or resources that you've purchased from the vendor.

    > [!NOTE]  
    > If you have set up recurring purchase lines for the vendor, such as a monthly replenishment order, then you can insert these lines on the invoice by choosing the **Get Recurring Purchase Lines** action.
4. On the **Lines** FastTab, in the **Item No.** field, enter the number of an inventory item or a service.
5. In the **Quantity** field, enter the number of items to be purchased.

    The **Line Amount** field is updated to show the value in the **Direct Unit Cost** field multiplied by the value in the **Quantity** field.

    The price and line amount are shown with or without sales tax depending on what you've selected in the **Prices Including Tax** field on the vendor card.

    The totals fields under the lines are automatically updated as you create or modify lines to display the amounts that will be posted to the ledgers.

6. In the **Invoice Discount Amount** field, enter an amount that should be deducted from the value shown in the **Total Incl. Tax** field at the bottom of the invoice.

    > [!NOTE]  
    > If you have set up invoice discounts for the vendor, then the specified percentage value is automatically inserted in the **Vendor Invoice Discount %** field if the criteria are met. The related amount is inserted in the **Invoice Discount Amount** field.
7. When you receive the purchased items or services, choose **Post**.

The purchase is now reflected in inventory, resource ledgers, and financial records, and the vendor payment is activated. The purchase invoice is removed from the list of purchase invoices and replaced with a new document in the list of posted purchase invoices.  For more information on what happens when you post purchase documents, see [Posting Purchases](purchasing-how-record-purchases.md#posting-purchases).

> [!NOTE]
> In rare cases, the posted amounts may deviate from what is displayed in the totals fields. This is typically due to rounding calculations in relation to goods and services tax (GST) or sales tax.
>
> To check the amounts that will actually be posted, go to the **Statistics** page, which takes the rounding calculations into account. Also, if you choose the **Release** action, the totals fields will be updated to include rounding calculations.

## <a name="posted-invoices" />Posted invoices

[!INCLUDE [posted-invoices](includes/posted-invoices.md)]

You can easily correct or cancel a posted purchase invoice before you pay the vendor. This is useful if you need to correct a typing mistake or change the purchase early in the order process. Learn more at [Correct or Cancel Unpaid Purchase Invoices](purchasing-how-correct-cancel-unpaid-purchase-invoices.md). If you've already paid for items or services on the posted purchase invoice, then you must create a purchase credit memo to reverse the purchase. Learn more at [Process Purchase Returns or Cancellations](purchasing-how-process-purchase-returns-cancellations.md).

[Open the **Posted Purchase Invoices** list](https://businesscentral.dynamics.com/?page=146) in [!INCLUDE [prod_short](includes/prod_short.md)].


## <a name="purchasing-non-inventory-items" />Purchasing non-inventory items

The lines on a purchase invoice can be of the **Resource** or **Item** type. Item cards can be further classified as of the **Inventory**, **Service**, or **Non-Inventory** type, which specifies if the item is a physical inventory unit, a labour time unit (also applicable for resources), or a physical unit that is not kept in inventory. Learn more at [Register New Items](inventory-how-register-new-items.md). The purchase invoice process is the same for all mentioned types.

> [!NOTE]
> With the **Resource** purchase line type, you can also purchase external resources, for example, to invoice a vendor for work delivered. Learn more at [Set Up Resources](projects-how-setup-resources.md).
>
> To use a purchased resource, you may need to set the resource's capacity and manually assign it to a job. Purchasing a resource creates a resource ledger entry; however, resource ledger entries are not tracked for quantity and value as, for example, items are. If quantity and value tracking is required, then consider using other line item types.

## <a name="when-to-use-purchase-orders" />When to use purchase orders

You must use purchase orders if your purchasing process requires you to record partial receipts of an order quantity, for example, because the full quantity is not available at the vendor. If you deliver sold items directly from your vendor to your customer as a drop shipment, you must also use purchase orders. Learn more at [Make Drop Shipments](sales-how-drop-shipment.md).

In all other aspects, purchase orders work the same as purchase invoices. The following procedure is based on a purchase invoice. The steps are similar for a purchase order.

<br><br>

> [!Video https://www.microsoft.com/videoplayer/embed/RE4b3tt?rel=0]

## <a name="receive-items-with-a-purchase-order" />Receive items with a purchase order

The following describes how to receive items with a purchase order. 

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchase Orders**, then choose the related link.
2. Open an existing purchase order, or create a new one.
3. In the **Qty. to Receive** field, enter the received quantity.

   > [!NOTE]
   > If the received quantity is more than the quantity on the purchase order, and the vendor has been set up to allow over-receipts, use the **Over-Receive** field to handle the excess quantity. Learn more in the [To receive more items than ordered](purchasing-how-record-purchases.md#receive-more-items-than-ordered) section.
4. Choose the **Post** action.

  The value in the **Qty. Received** field is updated. If this is a partial receipt, the value is lower than the value in the **Quantity** field.

> [!NOTE]
> If you use a warehouse handling, you can't use the **Post** action on the purchase order to register receipt. That's because a warehouse employee has already posted the purchase order quantity as received. Learn more at [Design Details - Inbound Warehouse Flow](design-details-inbound-warehouse-flow.md).

## <a name="receive-more-items-than-ordered" />Receive more items than ordered

When more goods arrive than were ordered, you may want to receive them instead of cancelling the receipt. For example, it may be cheaper to keep the excess items in inventory than return them, or your vendor may offer a discount for keeping them.

<!--move the over-receipt setup info to an article about purchasing. Keep the concept info here and link to the steps-->
### <a name="set-up-over-receipts" />Set up over-receipts

Create over-receipt codes to define a percentage by which a received quantity can exceed the ordered quantity. Specify the percentage in the **Over-Receipt Tolerance %** field. You then assign the code on the Item Card or Vendor Card pages for items and vendors.  

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Over-Receipt Codes**, then choose the related link.
2. Fill in the fields as necessary. [!INCLUDE [tooltip-inline-tip_md](includes/tooltip-inline-tip_md.md)]

### <a name="assign-the-over-receipt-code-to-an-item" />Assign the over-receipt code to an item

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, then choose the related link.
2. Open the **Item Card** page for the item.
3. In the **Over-Receipt Code** field, choose the code that contains the percentage you want to allow for over-receipts.

The over-receipt code is assigned to the item. Purchase orders or warehouse receipts for the item now allow you to receive more than the ordered quantity within the over-receipt tolerance percentage.

> [!NOTE]
> You can set up an approval workflow requiring over-receipts to be approved before they can be handled. Select the **Approval Required** checkbox on the **Over-Receipt Codes** page. Learn more at [Create Workflows](across-how-to-create-workflows.md).

### <a name="over-receive-an-order" />Over-receive an order

On purchase lines and warehouse receipt lines, the **Over-Receipt Quantity** field is used to record over-received quantities, meaning quantities exceeding the ordered-quantity value in the **Quantity** field.

When you handle an over-receipt, you can increase the value in the **Qty. to Receive** field to the quantity actually received. The **Over-Receipt Quantity** field updates to show the excess quantity. Alternatively, you can enter the excess quantity in the **Over-Receipt Quantity** field. The **Qty. to Receive** field updates to show the ordered quantity plus the excess quantity. The following procedure described how to fill in the **Qty. to Receive** field.  

1. On a purchase order or a warehouse receipt document where the received quantity is higher than ordered, enter the quantity actually received in the **Qty. to Receive** field.

    If the increase is within the tolerance specified by an assigned over-receipt code, the **Over-Receipt Quantity** field updates to show the quantity by which the value in the **Quantity** field is exceeded.

    If the increase is over the tolerance, the over-receipt isn't allowed. Investigate whether another over-receipt code will allow it. Otherwise, only the ordered quantity can be received, and the excess quantity must be handled another way, such as returning it to the vendor.

2. Post the receipt as you would any other receipt.

> [!NOTE]
> [!INCLUDE[prod_short](includes/prod_short.md)] does not automatically handle financial aspects of over-receipts. You must manually handle this in agreement with the vendor, for example, by the vendor forwarding a new or updated invoice.

## <a name="external-document-number" />External document number

[!INCLUDE [ext-doc-no-purch](includes/ext-doc-no-purch.md)]

## <a name="posting-purchases" />Posting Purchases

On a purchase document, you can choose between the following posting actions:

* **Post**
* **Preview Posting**
* **Post and Print**
<!--* **Test Report**-->
* **Post Batch**

When a purchase document is posted, the vendor's account, the general ledger (G/L), the item ledger entries, and the resource ledger entries are updated.

For each purchase document, a purchase entry is created in the **G/L Entry** table. An entry is also created in the vendor's account in the **Vendor Ledger Entry** table and a G/L entry is created in the relevant payables account. In addition, posting the purchase may result in a goods and services tax (GST) entry and a G/L entry for the discount amount. Whether an entry for the discount is posted depends on the contents of the **Discount Posting** field on the **Purchases & Payables Setup** page.

For each purchase line, as applicable, entries are created in the:

* **Item Ledger Entry** table if the purchase line is of the **Item** type.
* **G/L Entry** table if the purchase line is of the **G/L Account** type.
* **Resource Ledger Entry** table if the purchase line is of the **Resource** type.

In addition, purchase documents are always recorded in the **Purch. Recpt. Header** and **Purch. Inv. Header** tables.

You can always review various ledger entries that will be created in result of postings. Choose **Preview Posting** to validate document and inspect expected ledger entries.


> [!IMPORTANT]  
> When you post a purchase order for items, you can create both a receipt and an invoice. These can be done simultaneously or independently. You can also create a partial receipt and a partial invoice by completing the **Qty. to Receive** and **Qty. to Invoice** fields on the individual purchase order lines before you post. Note that you cannot create a purchase invoice from a purchase order for products or services that have not been received. That is, before you can invoice, you must have recorded a receipt, or you must choose to receive and invoice at the same time.

You can either post or post and print. If you choose to post and print, a report is printed when the order is posted. You can also choose the **Post Batch** action to post several orders at the same time. Learn more at [Post Multiple Documents at the Same Time](ui-batch-posting.md).

## <a name="viewing-ledger-entries" />Viewing ledger entries

When the posting is completed, the posted purchase lines are removed from the order. A message tells you when the posting is completed. After this, you'll be able to see the posted entries in various pages, including the **Vendor Ledger Entries**, **G/L Entries**, **Item Ledger Entries**, **Resource Ledger Entries**, **Purchase Receipts**, and **Posted Purchase Invoices** pages.

In most cases, you can open ledger entries from the affected card or document. For example, on the **Vendor Card** page, choose the **Entries** action.

## <a name="editing-ledger-entries" />Editing ledger entries

You can edit certain fields on posted purchase documents, such as the **Payment Reference** field. Learn more at [Edit Posted Documents](across-edit-posted-document.md). For more critical fields that affect the auditing trail, you must reverse or undo posting. Learn more at [Reverse Journal Postings and Undo Receipts/Shipments](finance-how-reverse-journal-posting.md).

## <a name="see-related-microsoft-trainingtrainingmodulesreceive-invoice-dynamics-d-business-centralindex" />See related [Microsoft training](/training/modules/receive-invoice-dynamics-d365-business-central/index).

## <a name="see-related-microsoft-trainingtrainingmodulesprocessing-invoices-dynamics--business-centralindex" />See related [Microsoft training](/training/modules/processing-invoices-dynamics-365-business-central/index)

## <a name="see-also" />See also

[Request Quotes](purchasing-how-request-quotes.md)  
[Purchase Items for a Sale](purchasing-how-purchase-products-sale.md)  
[Prepare Drop Shipments](sales-how-drop-shipment.md)  
[Purchasing](purchasing-manage-purchasing.md)  
[Setting Up Purchasing](purchasing-setup-purchasing.md)  
[Set Up Resources](projects-how-setup-resources.md)  
[Register New Vendors](purchasing-how-register-new-vendors.md)  
[Edit Posted Documents](across-edit-posted-document.md)  
[Post Multiple Documents at the Same Time](ui-batch-posting.md)  
[Purchasing](purchasing-manage-purchasing.md)  
[Posting Documents and Journals](ui-post-documents-journals.md)  
[Correct or Cancel Unpaid Purchase Invoices](purchasing-how-correct-cancel-unpaid-purchase-invoices.md)  
[Finding Pages and Information with Tell Me](ui-search.md)  
[Work with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
