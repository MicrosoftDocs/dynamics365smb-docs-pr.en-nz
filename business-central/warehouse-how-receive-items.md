---
title: Receive Items
description: This article is an overview of the different ways to receive items at a warehouse, for example items with a purchase order or items with a warehouse receipt.
author: SorenGP
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.form: 5768, 7330, 7332, 7333, 7342, 7363, 8510, 9008
ms.date: 09/02/2022
ms.author: edupont
ms.openlocfilehash: 8bd79a13bb7ecc806fea0dcdea33ec604bd98c41
ms.sourcegitcommit: 8b95e1700a9d1e5be16cbfe94fdf7b660f1cd5d7
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 09/09/2022
ms.locfileid: "9460903"
---
# <a name="receive-items"></a>Receive Items

When items arrive at a warehouse that is not set up for warehouse receipt processing, you simply record the receipt on the related business document, such as a purchase order, a sales return order, or an inbound transfer order.

When items arrive at a warehouse that is set up for warehouse receipt processing, you must retrieve the lines of the released source document that triggered their receipt. If you have bins, you can either accept the default bin that is filled in, or if the item has never before been received in the warehouse, fill in the bin where the item should be put away. You must then fill in the quantities of the items you've received, and post the receipt.  

## <a name="receive-items-with-a-purchase-order"></a>Receive items with a purchase order

The following describes how to receive items with a purchase order. The steps are similar to those for sales return orders and transfer orders.  

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchase Orders**, then choose the related link.
2. Open an existing purchase order, or create a new one. Learn more at [Record Purchases](purchasing-how-record-purchases.md).
3. In the **Qty. to Receive** field, enter the received quantity.

   > [!NOTE]
   > If the received quantity is higher than ordered on the purchase order, per the **Quantity** field, and the vendor has been set up to allow over-receipts, then you use the **Over-Receive** field to handle the excess quantity. Learn more in the [To receive more items than ordered](warehouse-how-receive-items.md#receive-more-items-than-ordered) section.
4. Choose the **Post** action.

  The value in the **Qty. Received** field is updated. If this is a partial receipt, then the value is lower than the value in the **Quantity** field.

> [!NOTE]
> If you use a warehouse document to post the receipt, then you cannot use the **Post** action on the purchase order. Instead, a warehouse worker has already posted the purchase order quantity as received. Learn more at [To receive items with a warehouse receipt](warehouse-how-receive-items.md#receive-items-with-a-warehouse-receipt).

## <a name="receive-items-with-a-warehouse-receipt"></a>Receive items with a warehouse receipt

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Warehouse Receipts**, then choose the related link.  
2. Choose the **New** action.  

    Fill in the fields on the **General** FastTab. When you retrieve source document lines, some of the information is copied to each line.  

    For warehouse configuration with directed put-away and pick, if the location has a default zone and bin for receipts, the **Zone Code** and **Bin Code** fields are filled in automatically, but you can change them as appropriate.  

    > [!NOTE]  
    > If you wish to receive items with warehouse class codes other than the class code of the bin in the **Bin Code** field on the document header, you must delete the contents of the **Bin Code** field on the header before you retrieve source document lines for the items.  
3. Choose the **Get Source Documents** action. The **Source Documents** page opens.

    From a new or open warehouse receipt, you can use the **Filters to Get Source Docs.** page to retrieve the released source document lines that define which items to receive or ship.

    1. Choose the **Use Filters to Get Src. Docs.** action.  
    2. To set up a new filter, enter a descriptive code in the **Code** field, then choose the **Modify** action.  
    3. Define the type of source document lines you want to retrieve by filling in the relevant filter fields.  
    4. Choose **Run**.  

    All released source document lines that fulfil the filter criteria are now inserted on the **Warehouse Receipt** page on which you activated the filter function. 

    The filter combinations you define are saved on the **Filters to Get Source Docs.** page until the next time you need it. You can make an unlimited number of filter combinations. You can change the criteria at any time by choosing the **Modify** action.

4. Select the source documents for which you want to receive items, then choose **OK**.  

    The source document lines appear on the **Warehouse Receipt** page. The **Qty. to Receive** field is filled with the quantity outstanding for each line, but you can change the quantity as necessary. If you deleted the contents of the **Bin Code** field on the **General** FastTab before getting the lines, you must fill in an appropriate bin code on each receipt line.  

    > [!NOTE]  
    >  To fill all lines in the **Qty. to Receive** field with zero, choose the **Delete Qty. to Receive** action. To fill it in once again with the quantity outstanding, choose the **Autofill Qty. to Receive** action.  
    >
    >  You cannot receive more items than the number in the **Qty. Outstanding** field on the source document line. To receive more items, retrieve another source document that contains a line for the item using the filter function.  

5. Post the warehouse receipt. The quantity fields are updated on the source documents, and the items are recorded as part of the company inventory.  

If you're using warehouse put-away, the receipt lines are sent to the warehouse put-away function. The items, although received, cannot be picked until they've been put away. The received items are identified as available inventory only when the put-away has been registered.  

If you're not using warehouse put-away but you are using bins, the put-away of the items in the bin specified on the source document line is recorded.  

> [!NOTE]  
> If you use the **Post and Print** function, you both post the receipt and print a put-away instruction that shows you where to place the items in storage.  
>
> If your location uses directed put-away and pick, then the put-away templates are used to calculate the best place to put the items away. This is then printed on the put-away instruction.

## <a name="receive-more-items-than-ordered"></a>Receive more items than ordered

When you receive more goods than you ordered, you may want to receive them instead of cancelling the receipt. For example, it may be cheaper to keep the excess on your inventory than returning them or your vendor may offer you a discount for keeping them.

### <a name="set-up-over-receipts"></a>Set up over-receipts

You must define a percentage by which you allow the ordered quantity to be exceeded when receiving. You define this with an over-receipt code, which contains the percentage in the **Over-Receipt Tolerance %** field. You then assign the code to the cards of relevant items and/or vendors.  

The following describes how to set up and assign an over-receipt code to an item. The steps are similar to set this up for a vendor.

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, then choose the related link.
2. Open the card for an item you suspect may sometimes be delivered with a higher quantity than ordered.
3. Choose **Look-up** in the **Over-Receipt Code** field.
4. Choose the **New** action.
5. On the **Over-Receipt Codes** page, create one or more new lines that define different over-receive policies. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)].
6. Select a line, then choose **OK**.

The over-receipt code is assigned to the item. Any purchase order or warehouse receipt for the item now allows receiving more than the ordered quantity according to the specified over-receipt tolerance percentage.

> [!NOTE]
> You can set up an approval workflow requiring over-receipts to be approved before they can be handled. In that case, you must select the **Approval Required** check box on the **Over-Receipt Codes** page. Learn more at [Create Workflows](across-how-to-create-workflows.md).

### <a name="perform-an-over-receipt"></a>Perform an over-receipt

On purchase lines and warehouse receipt lines, the **Over-Receipt Quantity** field is used to record over-received quantities, meaning quantities exceeding the ordered-quantity value in the **Quantity** field.

When you handle an over-receipt, you can increase the value in the **Qty. to Receive** field to the quantity actually received. The **Over-Receipt Quantity** field is then updated to show the excess quantity. Alternatively, you can enter the excess quantity in the **Over-Receipt Quantity** field. The **Qty. to Receive** field is then updated to show the ordered quantity plus the excess quantity. The following procedure described how to fill in the **Qty. to Receive** field.  

1. On a purchase order or a warehouse receipt document where the received quantity is higher than ordered, enter the quantity actually received in the **Qty. to Receive** field.

    If the increase is within the tolerance specified by an assigned over-receipt code, the **Over-Receipt Quantity** field is updated to show the quantity by which the value in the **Quantity** field is exceeded.

    If the increase is above the specified tolerance, the over-receipt is not allowed. In that case, you can investigate if another over-receipt code exists that will allow it. Otherwise, only the ordered quantity can be received, and the excess quantity must be handled another way, such as returning it to the vendor.

2. Post the receipt as you would for any other receipt.

> [!NOTE]
> [!INCLUDE[prod_short](includes/prod_short.md)] does not include functionality to automatically initiate the financial administration of over-receipts. You must manually handle this in agreement with the vendor, for example, by the vendor forwarding a new or updated invoice.

## <a name="see-related-training-at-microsoft-learn"></a>See related training at [Microsoft Learn](/learn/modules/receive-invoice-dynamics-d365-business-central/index).

## <a name="see-also"></a>See also

[Warehouse Management](warehouse-manage-warehouse.md)  
[Inventory](inventory-manage-inventory.md)  
[Setting Up Warehouse Management](warehouse-setup-warehouse.md)  
[Assembly Management](assembly-assemble-items.md)  
[Design Details: Warehouse Management](design-details-warehouse-management.md)  
[Work with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
