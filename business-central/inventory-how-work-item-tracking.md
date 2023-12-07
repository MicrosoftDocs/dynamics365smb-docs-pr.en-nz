---
title: 'Track Items with Serial, Lot, and Package Numbers'
description: 'You can add serial numbers, lot numbers, and package numbers to any outbound or inbound document, and its posted item tracking entries are displayed in the related item ledger entries.'
author: brentholtorf
ms.author: bholtorf
ms.reviewer: andreipa
ms.topic: conceptual
ms.search.forms: '6503, 6515, 6513, 6512, 6502, 6506, 6501, 6510, 6507, 6500, 6505, 6508, 9126, 6526, 6516, 6511, 6504, 6509, 163, 6550,'
ms.date: 10/02/2023
ms.custom: bap-template
---
# <a name="track-items-with-serial-lot-and-package-numbers"></a>Track Items with Serial, Lot, and Package Numbers

You can assign serial numbers, lot numbers, and package numbers to any outbound or inbound document, and its posted item tracking entries display on the related item ledger entries. You track items on the **Item Tracking Lines** page, which you can open from inbound or outbound documents.

The quantity fields at the top of the **Item Tracking Lines** page display the quantities and sums of item tracking numbers that are defined on the lines. The quantities must correspond to those on the document lines, which is indicated by 0 in the **Undefined** fields.

[!INCLUDE [prod_short](includes/prod_short.md)] updates the availability information on the **Item Tracking Lines** page when you open the page. It doesn't update the information while you have the page open, even if changes occur in inventory or on other documents during that time.

> [!NOTE]  
> In order for the features described in this article to work, you must set up item tracking. To learn more, go to [Set Up Item Tracking with Serial, Lot, and Package Numbers](inventory-how-setup-item-tracking.md).

## <a name="item-tracking-availability"></a>Item tracking availability

When you work with serial, lot, and package numbers, [!INCLUDE[prod_short](includes/prod_short.md)] calculates availability information and shows it on various item tracking pages. It shows how much of a lot, package, or serial number is used on other documents. This information helps reduce errors and uncertainty caused by double allocations.

On the **Item Tracking Lines** page, a warning icon might display in the **Availability, Lot No.** or **Availability, Serial No.** field for the following reasons:

* If some or all of the quantity you've selected is already used in other documents.
* If the lot or serial number isn't available.

The **Lot No./Serial No.-List**, **Lot No./Serial No.-Availability**, and the **Item Tracking - Select Entries** pages show the quantity of an item that's in use. The following table lists the relevant fields.

|Field|Description|
|-----|-----------|  
|**Total Quantity**|The total number of an item currently in inventory.|
|**Total Requested Quantity**|The total number of items that are requested in this and other documents.|
|**Current Pending Quantity**|The number of items that are requested on the current document but that isn't posted.|
|**Current Requested Quantity**|The number of items that are requested that will be used on the current document|
|**Total Available Quantity**|The total number of items in inventory, minus the quantity of the item that's requested on this and other documents (total requested quantity), and minus the quantity that's requested but not yet posted on this document (current pending quantity).|

If you work on the **Item Tracking Lines** page for a long time, or if there's a lot of activity with the item you're working with, you can choose the **Refresh Availability** action. Also, the availability of the item is automatically rechecked when you close the page to confirm that there aren't availability problems.

## <a name="to-assign-serial-or-lot-numbers-during-an-inbound-transaction"></a>To assign serial or lot numbers during an inbound transaction

You might want to track items from the moment they arrive. In that case, the purchase order is often the central document. However, you can do item tracking from any inbound document and its posted entries display in the related item ledger entries.

The tracking numbers automatically transfer to all outbound warehouse activities.

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchase Orders**, and then choose the related link.  
2. Either open an existing purchase order or create a new purchase order.
3. Select the document line, and on the **Lines** FastTab, choose the **Line** action, and then choose the **Item Tracking Lines** action to open the **Edit - Item Tracking Lines** page.  

   You can assign serial or lot numbers in the following ways:  
   - Automatically, by selecting **Process** then choosing **Assign Serial No.** or **Assign Lot No.** to assign serial numbers from predefined number series.  
   - Automatically, by selecting **Process** then choosing **Create Customised SN** to assign serial numbers based on number series you define specifically for the arrived items.  
   - Manually, by entering serial or lot numbers directly, for example, the vendor's numbers.  
   - Manually, by assigning a specific number to each item unit.  

4. To assign automatically, choose the **Create Customised SN** action.  
5. In the **Customised SN** field, enter the starting number of a descriptive serial number series. For example **S/N-Vend0001**.  
6. In the **Increment** field, enter 1 to define that each sequential number increases by one.  

    The **Quantity to Create** field contains the line quantity by default, but you can modify it.  

7. Select the **Create New Lot No.** checkbox to organise the new serial numbers in a distinct lot.  
7. Choose the **OK** button.  

[!INCLUDE [prod_short](includes/prod_short.md)] creates a lot number with individual serial numbers according to the item quantity on the document line. The number is prefixed with the value you entered in the **Customised SN** field. For example, starting from **S/N-Vend0001**.  

The quantity fields in the header dynamically display the quantities and sums of the item tracking numbers you define on the page. The quantities must correspond to those on the document lines, which is indicated by **0** in the **Undefined** field.  

When you post the document, the item tracking entries transfer to the item ledger entries.

### <a name="to-handle-serial-and-lot-numbers-when-getting-receipt-lines-from-a-purchase-invoice"></a>To handle serial and lot numbers when getting receipt lines from a purchase invoice

When you get posted receipt or shipment lines from related invoices or credit memos, item tracking lines on the warehouse documents transfer automatically. However, they're processed in a special way.

The functionality supports the following inbound processes:  

- **Get Receipt Lines** - from a purchase invoice.  
- **Get Return Shipment Lines** - from a purchase credit memo.  

The functionality supports the following outbound processes:  

- **Get Shipment Lines** - from a sales invoice or combined shipments.  
- **Get Return Receipt Lines** - from a sales credit memo.  

In these cases, the item tracking lines transfer to the invoice or credit memo, but the **Item Tracking Lines** page doesn't let you change the serial or lot numbers. You can only change the quantities.  

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchase Invoices**, and then select the related link.  
2. Open a purchase invoice for items that are purchase with serial or lot numbers.  
3. From a purchase invoice line, on the **Lines** FastTab, choose the **Get Receipt Lines** action.  
4. On the **Get Receipt Lines** page, select a receipt line that has item tracking lines, and then choose the **OK** button.  

    The source document is copied to the purchase invoice as a new line, and its item tracking lines are copied to the underlying **Item Tracking Lines** page.  

5. On the purchase invoice, select the transferred receipt line.  
6. On the **Lines** FastTab, choose the **Line** action, and then choose the **Item Tracking Lines** action to find the transferred item tracking lines.  

You can't change the **Serial No.** and **Lot No.** fields. However, you can delete complete lines or change the quantities to match changes on the source line.  

## <a name="to-assign-a-serial-or-lot-number-during-an-outbound-transaction"></a>To assign a serial or lot number during an outbound transaction

Outbound handling of serial or lot numbers is a frequent task in different warehouse processes. There are two ways to add serial and lot numbers to outbound transactions:  

- Select from existing serial or lot numbers. This applies when item tracking numbers are already assigned in an inbound transaction.
- Assign new serial or lot numbers for outbound transactions. This applies when item tracking numbers aren't assigned to items until they're sold and ready to ship.

### <a name="to-select-from-existing-serial-or-lot-numbers"></a>To select from existing serial or lot numbers

When you work with items that require item tracking, and you're creating outbound transactions, you'll typically need to select lot or serial numbers that already exist.

1. From any outbound document, select the line that you want to select serial or lot numbers for.  
2. On the **Lines** FastTab, choose the **Line** action, then **Related Information**, and then select **Item Tracking Lines**.  
3. On the **Item Tracking Lines** page, you have three options for specifying lot or serial number:  

   - Select the **Serial No.** field, and then select a number on the **Serial No. List** page.
   - Select the **Lot No.** field, and then select a number on the **Lot No. List** page. Then, select the **Serial No.** field, and select a number on the **Serial No. List** page.
   - Select the **Process** action, and then choose **Select Entries**. The **Select Entries** page shows all lot and serial numbers along with availability information.

4. In the **Selected Quantity** field, enter the quantity of each lot or serial number to use.
5. Choose the **OK** button. The item tracking information transfers to the **Item Tracking Lines** page.  

The quantity fields in the header dynamically display the quantities and sums of the item tracking numbers you define on the page. The quantities must correspond to those of the document line, which is indicated by **0** in the **Undefined** field.  

When you post the document line, the item tracking information transfers to the associated item ledger entries.

### <a name="to-assign-new-serial-or-lot-numbers"></a>To assign new serial or lot numbers

This process applies when items don't have serial or lot numbers while they're in inventory. Instead, you assign item tracking numbers when the items are sold and ready to be shipped. In this case, you'll typically assign numbers from a predefined number series.

1. Select the relevant document, for example a sales invoice or sales order, and on the **Lines** FastTab, choose the **Line** action, then **Related Information**, and then choose the **Item Tracking Lines** action.  

    You can assign item tracking numbers in the following ways:  
    - Automatically, from a predefined number series: Choose the **Assign Serial No.** or **Assign Lot No.** action.  
    - Automatically, based on parameters you define specifically for the outbound item: Choose the **Create Customised SN** action.  
    - Manually, by entering serial or lot numbers without using a number series.  

2. For this procedure, assign a serial number automatically by choosing **Assign Serial No.**  

    The **Quantity to Create** field contains the line quantity by default, but you can change it.  
3. Select the **Create New Lot No.** field to organise the new serial numbers in a distinct lot.  
4. Choose the **OK** button to create a lot number and new individual serial numbers according to the quantity to handle on the related document line.  

The quantity fields at the top dynamically display the quantities and sums of the item tracking numbers that you define on the page. The quantities must correspond to those of the document line, which is indicated by **0** in the **Undefined** field.  

When the document is posted, the item tracking entries transfer to the item ledger entries.

### <a name="assign-tracking-numbers-on-source-documents"></a>Assign tracking numbers on source documents

Some companies define specific serial or lot numbers on source document, such as sales orders. For example, if a customer requests a specific lot. When you create the inventory pick or warehouse pick document from an outbound source document where serial or lot numbers are already defined, you can't change any fields on the **Item Tracking Lines** page under the inventory pick. The one exception is the **Qty. to Handle** field. In that case, the inventory pick lines specify the item tracking numbers on individual take and place lines. The quantity is already split into unique serial or lot number combinations because the sales order specifies the item tracking numbers to ship.

## <a name="to-handle-serial-and-lot-numbers-on-transfer-orders"></a>To handle serial and lot numbers on transfer orders

Procedures for handling serial and lot numbers that are being transferred between different locations are similar to those applied when items are sold and purchased.  

However, transfer orders are unique in that shipment and receipt are both done from the same transfer line and use the same instance of the **Item Tracking Lines** page. Item tracking numbers that shipped from one location must be received unchanged at the other location.

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Transfer Orders**, and then choose the related link.  
2. Open the transfer order you want to process. On the **Lines** FastTab, choose the **Line** action, choose the **Item Tracking Lines** action, and then choose the **Shipment** action.  
3. On the **Item Tracking Lines** page, assign or select serial or lot numbers as for any other outbound item transaction.  

    When you handle serial and lot numbers for transfer items, numbers are typically already assigned numbers. Therefore, you'll often choose from existing serial or lot numbers.  

4. Post the transfer order, first ship and then receive, to record that the items are transferred and carry their item tracking entries.  

During the transfer, you can't change values on the **Item Tracking Lines** page.  

## <a name="to-record-additional-serial-or-lot-number-information"></a>To record additional serial or lot number information

If you need to link special information to an item tracking number, for example, for quality assurance, you can do so on a serial or lot number information card.

1. Open a document that has serial or lot numbers assigned.
2. Open the **Item Tracking Lines** page for the item you want to enter information for.
3. Choose the **Line** action and then, for example, the **Serial No. Information Card** action.  
4. Choose the plus sign **(+)** sign at the top of the list to create a new entry. The **Serial No.** and **Lot No.** fields are prefilled from the item tracking line.
5. Enter a short piece of information in the **Description** field, for example about the condition of the item.  
6. Choose the **Related** action, choose the **Serial No.** action, and then choose the **Comment** action to create a separate comment record.  
7. Select the **Blocked** field to exclude the serial or lot number from any transactions.  

<!--If you create serial numbers in bulk by using the **Create Customized SN** or **Assign Serial No.** actions, you can enable **Create SN Information** and an information card will be created for each tracking line.

Alternatively, you can create an information card when you post journals or documents. On the **Item Tracking Code** page, turn on the **Create SN Info. on posting** or **Create SN Info. on posting** toggles. -->

You can modify created serial or lot information cards later.

## <a name="to-modify-existing-serial-or-lot-number-information"></a>To modify existing serial or lot number information

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.  
2. Select an item that has an item tracking code and has serial or lot number information.
3. From the **Item Card** page, choose the **Entries** action, and then choose **Ledger Entries**.
4. Choose the **Lot No.** or **Serial No.** field. If information exists for the item tracking number, then the **Lot No. Information List** or **Serial No. Information List** page opens.  
5. Select a card, and then choose the **Lot No./Serial No. Information Card** action.  
6. Modify the short description text, the comment record, or the **Blocked** field.  

You can't change the serial or lot numbers or quantities. To do that, you must reclassify the item ledger entry. To learn more about reclassification, go to [To reclassify lot or serial numbers](inventory-how-work-item-tracking.md#to-reclassify-serial-or-lot-numbers).

## <a name="to-reclassify-serial-or-lot-numbers"></a>To reclassify serial or lot numbers

Reclassifying item tracking for an item means changing a lot or serial number to a new lot or serial number, or changing the expiration date to a new expiration date. If you use lots, you can also merge multiple lots into one. Use an item reclassification journal to do these tasks.

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Item Reclass. Journal**, and then choose the related link.  
2. Fill in the line with the relevant information. For more information, see [Count Inventory Using Documents](inventory-how-count-inventory-with-documents.md) or [Count, Adjust, and Reclassify Inventory Using Journals](inventory-how-count-adjust-reclassify.md).
3. Choose the **Item Tracking Lines** action.  
4. In the **Serial No.** or **Lot No.** field, select the current serial or lot number.  
5. If you want to enter a new item tracking number, enter it in the **New Serial No.** or **New Lot No.** field. If you want, you can merge one or more lots to one new or existing lot.  

    > [!NOTE]  
    > When you reclassify expiration dates, items with the earliest expiration dates for outbound transactions are suggested first. To learn more, go to [Picking by FEFO](warehouse-picking-by-fefo.md).  

6. To specify a new expiration date for the serial or lot number, enter it in the **New Expiration Date** field.  

    > [!IMPORTANT]  
    > * If you're reclassifying a lot to the same lot number but with a different expiration date, you must reclassify the entire lot using one item reclassification journal line. 
    > * If you're reclassifying more than one lot to one new lot number, meaning that you are merging more than one lot into one new lot, you must enter the same new expiration date for all the lots. 
    > * If you're reclassifying one existing lot to a second existing lot that has a different expiration date, you must use the expiration date from the second lot. 
    > * If you leave the **New Expiration Date** field blank, the lot or serial number will be reclassified with a blank expiration date.  

7. If you have existing information on the old serial or lot number, you can copy it to the new serial or lot number.  

    1. On the **Item Tracking Lines** page, choose the **New Serial No. Information** action or the **New Lot No. Information** action.  
    2. To copy information from the old lot or serial number, choose the **Copy Info** action.  
    3. In the information list page, select the lot or serial number that you would like to copy from, and choose the **OK** button.  

8. If you want to modify the existing information for the lot or serial number, you can record lot or serial information.  
9. Post the journal to link the renewed item tracking numbers or expiration dates to the associated item ledger entry

## <a name="scan-barcodes-with-the-business-central-mobile-app"></a>Scan barcodes with the Business Central mobile app

[!INCLUDE [barcode-mobile-app](includes/barcode-mobile-app.md)]

On the **Item Tracking Lines** page, if you want to scan several serial, lot, or package barcodes, you can use the **Scan multiple** action. After you scan a barcode, its value is entered in the field on the page and the next quick-entry field becomes available. You can also use the barcode scanner icon to populate specific field.

The following tables list the pages that support barcode scanning for item tracking from the [!INCLUDE [prod_short](includes/prod_short.md)] mobile app.

|Page  |Field values you can scan  |
|---------|---------|
|Item Tracking Lines     |* Serial No.<br><br>* New Serial No.<br><br>* Lot No.<br><br>* New Lot No.<br><br>* Package No.<br><br>* New Package No.|
|Whse. Item Tracking Lines     |* Serial No.<br><br>* New Serial No.<br><br>* Lot No.<br><br>* New Lot No.<br><br>* Package No.<br><br>* New Package No.|
|Item Tracing     |* Serial No. Filter<br><br>* Lot No. Filter<br><br>* Package No. Filter |
|Item Journal     |* Serial No.<br><br>* Lot No.<br><br>* Package No.     |
|Warehouse Activity Line     |* Serial No.<br><br>* Lot No.<br><br>* Package No.<br><br>**Note**: The following pages use the Warehouse Activity Line page:<br><br>* page 5780 "Whse. Pick Subform"<br><br>* page 7378 "Invt. Pick Subform"<br><br>* page 5771 "Whse. Putaway Subform"<br><br>* page 7316 "Warehouse Movement Subform"<br><br>* page 7376 "Invt. Putaway Subform"<br><br>* page 7383 "Invt. Movement Subform"        |
|Whse. Phys. Invt. Journal     |* Serial No.<br><br>* Lot No.<br><br>* Package No.         |

## <a name="see-also"></a>See also

[Set Up Item Tracking with Serial, Lot, and Package Numbers](inventory-how-setup-item-tracking.md)  
[Trace Item-Tracked Items](inventory-how-to-trace-item-tracked-items.md)  
[Inventory](inventory-manage-inventory.md)  
[Design Details: Item Tracking](design-details-item-tracking.md)  
[Design Details - Item Tracking and Reservations](design-details-item-tracking-and-reservations.md)  
[Reserve Items](inventory-how-to-reserve-items.md)  
[Work with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
