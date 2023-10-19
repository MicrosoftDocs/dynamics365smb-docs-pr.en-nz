---
author: brentholtorf
ms.topic: include
ms.date: 09/11/2023
ms.author: bholtorf
---

Increase efficiency in your warehouse with accurate, real-time information about factors that can affect available quantities. For example: 

* Inventory levels
* Locations
* Processing stages
* Quarantined items
* Reservations

You can access information about item availability from the following source documents:

* Sales orders
* Production orders
* Assembly orders
* Jobs

The information also respects other factors that affect availability. For example, dedicated bins, locked bins, and items that aren't available for picking. For example, items might be reserved, or pending put-away or shipment operations. The **Pick Summary** page lets you review the items that [!INCLUDE [prod_short](prod_short.md)] didn’t include in pick documents and take the necessary actions.

> [!NOTE]
> This capability requires that you turn on the **Directed Put-away and Pick** toggle for the locations you use in your picking process.

### <a name="set-up-previews"></a>Set up previews

To get details on what's being picked and what isn't, turn on the **Show Summary (Directed Put-away and Pick)** toggle on the **Whse.-Source - Create Document** or **Whse.-Shipment - Create Pick** request pages.

### <a name="determine-the-quantity-you-can-pick"></a>Determine the quantity you can pick

On lines on the **Create Warehouse Pick Summary** page, the **Qty. to Handle (Base)** field shows which, and how many, items [!INCLUDE [prod_short](prod_short.md)] tried to pick. The **Summary** FactBox provides more details.

For simple investigations, the **Pickable Qty.** might give you enough information. The field shows how many items are available. If the pickable quantity is less than expected, explore the bin content.

The **Pickable Qty.** is the maximum quantity that [!INCLUDE [prod_short](prod_short.md)] can consider for picking. This quantity consists of items in pickable bins. The quantity excludes quantities that are in blocked or dedicated bins, or items that are being picked in warehouse pick documents. If the item you want to pick requires item tracking, blocked lot or serial numbers stored in pickable bins are excluded from the pickable quantity.

If the pickable quantity differs from the quantity in pickable bins, there might be a problem. Explore the bin content to find blocked bins or quantities in active documents.

The **Quantity in Warehouse** field shows the total quantity you'll find in your warehouse if you do a physical count. You can drill down to the warehouse ledger entries from this field. If the field shows a quantity that's less than the quantity in the **Quantity in Pickable Bins**, there's a misalignment between warehouse and inventory quantities. In that case, use the **Calculate Warehouse Adjustment** action on the **Item Journal** page, and then create the warehouse pick again.

The following image illustrates the maximum quantity considered for picking.

:::image type="content" source="../media/pickable-qty.png" alt-text="Maximum quantity considered for picking.":::

**Legend**

|Letter  |Description  |
|---------|---------|
|P     |Bins with content of type Pick         |
|D     |Bins with content of type Pick marked as Dedicated bins        |
|A     |Bins with content of type Pick in the active documents (like another pick)       |
|T     |Bins with content of type Pick with items with blocked tracking         |
|B     |Bins with content of type Pick with blocked outbound movement         |
|O     |Other bins         |

### <a name="reservations"></a>Reservations

If there are reservations for the item being picked, then calculation continues. The idea is that reserved demand has higher priority than non-reserved, which means that picking for non-reserved demand shouldn't prevent picking for reserved demand later.

To verify that your quantity can cover a demand, compare the **Pickable Qty.** value on the **Summary** FactBox with the value in the **Qty. to Handle (Base)** field on the lines.

You can find reservations in the **Total Reserved Qty. in Warehouse** field. Reserved quantities that are already picked and are ready for shipment, usage, or consumption, don't affect availability. The **Reserved Qty. in Pick/Ship Bins** field shows this quantity.

The **Avail. Qty. Excluding Shipment Bin** field shows the quantity that's available, excluding quantities for which the following is true:

* They're already picked for shipments.
* They're in blocked item lots or serial numbers.
* They're in blocked bins.

These quantities might be available, but you might not be able to pick them yet. They could still be in the receipt, storage, or quality-assurance areas. You can move them to the picking area by processing a put-away or movement worksheet.

The difference between **Avail. Qty. Excluding Shipment Bin** and reserved quantity in warehouse is the quantity available for picking without impacting reserved stock.

### <a name="other-details"></a>Other details

If items require item tracking, you can also find the quantity in blocked lots or serial numbers, which causes the following reductions:

* The pickable quantity
* Available quantity, excluding the shipment bin
* The reserved quantity in warehouse 

If you pick the same item for multiple source documents or lines, which is also the case when you pick serial numbers, information about picks for others lines also displays because it reduces the pickable quantity.
