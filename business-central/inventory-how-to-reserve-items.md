---
title: How to Reserve Items
description: 'Learn about reserving items for sales orders, purchase orders, and production orders.'
author: brentholtorf
ms.author: bholtorf
ms.reviewer: andreipa
ms.topic: conceptual
ms.search.keywords: null
ms.search.forms: '498, 497'
ms.date: 09/19/2023
ms.custom: bap-template
ms.service: dynamics-365-business-central
---
# <a name="reserve-items"></a>Reserve Items

You can reserve items for sales orders, purchase orders, service orders, assembly orders, transfer orders, and production orders. You can also reserve items in inventory or inbound on open document or journal lines. You do this on the **Reservation** page.

Each line you open to reserve items on the **Reservation** page displays information about one type of line (sales, purchase, or journal) or inventory entry. The lines describe how many items are available to be reserved from each type of line or entry.

> [!TIP]
> Based on the quantities you’ve reserved in inventory, [!INCLUDE [prod_short](includes/prod_short.md)] displays a status on the documents so that you’re quickly aware of the next step. For example, to indicate that you can ship a sales order or start to work on a job, assembly, or production order. The status also helps reduce the risk of accidental partial shipments or hold-ups due to missing stock for production and assembly orders.
>
> The **Reserved from stock** field can help you understand whether you can ship or pick for a specific order or order line. For lines, the Reserved from stock field is available on FactBoxes. To access the information for the entire order, the field is on the **Statistics** page.

## <a name="reserve-items-for-sales"></a>Reserve items for sales

The following procedure describes how to reserve items from a sales order. The steps are similar for purchase, service, transfer, and assembly orders.
  
1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, then choose the related link.  
2. Choose the sales order.
3. On the **Lines** FastTab, choose the **Reserve** action. The **Reservation** page opens.  
4. Select the line you want to reserve the items from.  
5. Choose one of the following actions.  

    |**Function**|**Description**|
    |------------------|---------------------|  
    |**Auto Reserve**|To automatically reserve items on the **Reservation** page.|  
    |**Reserve from Current Line**|To reserve the items from the document on the line you have selected.|  
    |**Cancel Reservation from Current Line**|To cancel reservation of the items in the document on the line you've selected.|

> [!NOTE]  
> If item tracking lines exist for the sales order, the reservation system will take you through special steps. Learn more in the [To reserve a specific serial or lot number](inventory-how-to-reserve-items.md#reserve-a-specific-serial-or-lot-number) section.  

## <a name="reserve-an-item-for-a-production-order-line"></a>Reserve an item for a production order line

You can reserve items for production orders. You have to distinguish between production order lines, meaning the parent item, and production order components.

In the following procedure, a firm planned production order is used.

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Firm Planned Prod. Order**, then choose the related link.  
2. Open the firm planned production order you want to reserve parent items for.  
3. Select the relevant production order line.  
4. On the **Lines** FastTab, choose the **Reserve** action.
5. On the **Reservation** page, select the **Sales Line, Order** line, then choose the **Reserve from Current Line** action.  

The quantity you entered in the firm planned production order line is now reserved.

## <a name="reserve-items-for-production-order-components"></a>Reserve items for production order components

You can reserve items for production orders. You have to distinguish between production order lines, meaning the parent item, and production order components.

In the following procedure, a firm planned production order is used.

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Firm Planned Prod. Order**, then choose the related link.  
2. Open the firm planned production order you want to reserve component items for.  
3. Select the relevant production order line.  
4. On the **Lines** FastTab, choose **Line**, then choose **Components**.  
5. Select the relevant component line.  
6. On the **Lines** FastTab, choose the **Reserve** action.  
7. On the **Reservation** page, select a line, then choose the **Reserve from Current Line** action.  

The quantity you entered in the firm planned production component line is now reserved.

## <a name="reserve-items-in-bulk"></a>Reserve items in bulk

Use the **Reservation Worksheet** page to reserve and allocate incoming goods in bulk. For example, bulk reservations can help ensure that quantities are available for your sales and production orders. You can have multiple batches for different purposes. For example, you might allocate production orders on a weekly basis but reserve daily for sales.

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Reservation Worksheet**, then choose the related link.  
2. Choose the **Get Demand** action, and then specify the kind of demand you want to reserve from available inventory.
3. In the **Reserved from stock** field, choose one of the following options:
    
   |Field  |Description  |
   |---------|---------|
   |Blank     | The outstanding quantity isn't reserved at all, or it's reserved from other source documents, such as purchase orders.        |
   |Full    |  The outstanding quantity is completely reserved from available inventory.       |
   |Partial     | The outstanding quantity is partially reserved from available inventory.        |

4. Fill in the fields as necessary. [!INCLUDE [tooltip-inline-tip_md](includes/tooltip-inline-tip_md.md)]
5. Optional: To allocate the items right away, choose the **Allocate** action.
6. On the **Allocation Policy** page, choose a policy for each step

   |Allocation policy  |Description  |
   |---------|---------|
   |Basic     | Allocates stock to a demand if there are no conflicts and the demand can be fully covered. For example, you have sales order A with a quantity of 10, and a job with a quantity of 7. If you have 20 in stock, both demands receive full quantity. If your stock is 12, no stock is allocated. You must manually allocate the quantity.        |
   |Equally    | Distributes available stock to demand equally. For example, you have a sales order with a quantity of 10, and a job with a quantity of 7. If your stock level is 20, then both demands will receive full quantity. If your stock is 12, then both demands will get 6.        |

7. To reserve all lines where **Accept** is turned on, choose the **Make reservation** action.
    
## <a name="change-a-reservation"></a>Change a reservation

You can change an item reservation.

1. From the document line you made the reservation from, on the **Lines** FastTab, choose the **Reserve** action.  
2. On the **Reservation** page, choose the **Reservation Entries** action.
3. On the **Reservation Entries** page, update the **Quantity** field on the line you want to change.
4. Confirm the subsequent message by choosing the **OK** button.

## <a name="cancel-a-reservation"></a>Cancel a reservation

You can cancel an item reservation.

1. From the document line you want to cancel a reservation from, on the **Lines** FastTab, choose the **Reserve** action.  
2. On the **Reservation** page, choose the **Reservation Entries** action.  
3. On the **Reservation Entries** page, choose the **Cancel Reservation** action.  
4. Confirm the subsequent message by choosing the **Yes** button.  

## <a name="reserve-a-specific-serial-or-lot-number"></a>Reserve a specific serial or lot number

From outbound documents for item-tracked items, such as sales orders or production component lists, you can reserve specific serial or lot numbers. For example, reserving specific serial or lot numbers can be useful in the following situations:

* If you need production components from a specific lot to ensure consistency with earlier production batches.
* Because a customer has requested a specific serial number. 

Learn more at [Work with Serial and Lot Numbers](inventory-how-work-item-tracking.md).

This practice is referred to as a specific reservation, because you reserve from the quantity of item X that belongs to lot X. In contrast, if you reserve only from quantities of item X, then it is simply a normal, non-specific, reservation. Learn more at [Design Details - Item Tracking and Reservations](design-details-item-tracking-and-reservations.md).

The following procedure is based on a sales order.

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then select the related link.  
2. Create a sales order line for an item-tracked item.  
3. Assign serial and lot numbers to the sales order line. Learn more at [Work with Serial and Lot Numbers](inventory-how-work-item-tracking.md).
4. On the sales order line, choose the **Reserve** action.  
5. Choose the **Yes** button to reserve specific serial or lot numbers.  
6. On the **Item Tracking List** page, select the serial and lot number combination you have assigned.  
7. Choose the **OK** button to open the **Reservation** page showing only supply with the specified item tracking number. If there are any non-specific reservations on any of the item tracking numbers you've specified for this line, you're informed of the quantity that has already been reserved.  
8. Choose either the **Auto Reserve** or the **Reserve from Current Line** action to create the reservation of the specific item tracking numbers.

## <a name="see-also"></a>See also

[Inventory](inventory-manage-inventory.md)  
[Design Details: Reservation, Order Tracking, and Action Messaging](design-details-reservation-order-tracking-and-action-messaging.md)  
[Design Details: Item Tracking and Reservations](design-details-item-tracking-and-reservations.md)  
[Work with Serial and Lot Numbers](inventory-how-work-item-tracking.md)  
[Work with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)

[!INCLUDE[footer-include](includes/footer-banner.md)]
