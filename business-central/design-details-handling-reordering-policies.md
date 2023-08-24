---
title: Design Details - Handling Reordering Policies
description: This article gives an overview of the reordering policies you can use in supply planning.
author: brentholtorf
ms.author: bholtorf
ms.reviewer: andreipa
ms.topic: conceptual
ms.date: 02/24/2023
ms.custom: bap-template
---
# <a name="design-details-handling-reordering-policies"></a>Design Details: Handling Reordering Policies

To include an item in supply planning, you must specify a reordering policy for it on the **Item Card** page. The following reordering policies are available:  

* Fixed Reorder Qty.  
* Maximum Qty.  
* Order  
* Lot-for-Lot  

The **Fixed Reorder Qty.** and **Maximum Qty.** policies relate to inventory planning. These policies coexist with the step-by-step balancing of supply and order tracking.  

## <a name="the-role-of-the-reorder-point"></a>The role of the reorder point

A reorder point represents demand during lead time. When inventory is projected to pass below the level defined by the reorder point, it's time to order more. Inventory will decrease gradually until the replenishment arrives. It might reach zero or the safety stock level. The planning system suggests a forward-scheduled supply order at the point when the inventory passes below the reorder point.  

Inventory levels can move significantly during the time bucket. Therefore, the planning system constantly monitors available inventory.

## <a name="monitoring-the-projected-inventory-level-and-the-reorder-point"></a>Monitoring the projected inventory level and the reorder point

Inventory is a type of supply, but for inventory planning, the planning system distinguishes between two inventory levels:  

* Projected inventory  
* Projected available inventory  

### <a name="projected-inventory"></a>Projected inventory

At the start of the planning process, projected inventory is the gross quantity of inventory. The gross quantity includes posted and un-posted supply and demand in the past. This quantity becomes a projected inventory level that gross quantities from future supply and demand maintain. Future supply and demand are introduced along the time line, whether reserved or allocated in other ways.  

The planning system uses projected inventory to monitor the reorder point and determine the reorder quantity using the **Maximum Qty.** reordering policy.  

### <a name="projected-available-inventory"></a>Projected available inventory

Projected available inventory is the inventory that is available to fulfil demand at a given point in time. The planning system uses projected available inventory when monitoring the safety stock level. Safety stock must always be available for unexpected demand.  

### <a name="time-buckets"></a>Time buckets

Projected inventory is important detecting when the reorder point is reached or crossed, and to calculate the right order quantity when using the **Maximum Qty.** reordering policy.  

The projected inventory level is calculated at the start of the planning period. It's a gross level that doesn't consider reservations or other allocations. To monitor this inventory level during the planning sequence, the planning system monitors the aggregated changes over a period of time. That period is called a *time bucket*. To learn more about time buckets, go to [The role of the time bucket](#the-role-of-the-time-bucket). The planning system ensures that the time bucket is at least one day. One day is the minimum unit of time for demand or supply events.  

### <a name="determining-the-projected-inventory-level"></a>Determining the projected inventory level

The following sequence describes how the planning system determines the projected inventory level:  

* When a supply event is fully planned, such as a purchase order, it increases the projected inventory on the event's due date.  
* When a demand event is fully satisfied, it won't decrease the projected inventory right away. Instead, it posts a decrease reminder, which is an internal record that holds the date and quantity of the addition to projected inventory.  
* When a later supply event is planned and added to the timeline, the system investigates posted decrease reminders one by one to the planned date of the supply. During this process, the reorder point level of the internal increase reminder might be reached or crossed.  
* If a new supply order is introduced, it checks whether it's entered before the current supply. If it is, the new supply becomes current supply and the balancing procedure restarts.  

The following image shows this principle.  

![Determining the Projected Inventory Level.](media/nav_app_supply_planning_2_projected_inventory.png "Determining the Projected Inventory Level")  

1. Supply **Sa** of 4 (fixed) closes Demand **Da** of -3.  
2. CloseDemand: Create a decrease reminder of -3 (not shown).  
3. Supply **Sa** is closed with a surplus of 1 (there isn't more demand).  

     The projected inventory level increases to +4, while the projected **available** inventory becomes -1.  

4. The next supply **Sb** of 2 (another order) has already been placed on the timeline.  
5. The planning system checks for a decrease reminder before **Sb** (in this example there isn't, so no action is taken).  
6. The planning system closes supply **Sb** (no more demand exists) by either A, reducing it to 0 (cancel) or B, by leaving it as is.  

     The projected inventory level increases (A: +0 => +4 or B: +2 = +6).  

7. The planning system makes a final check. Is there any decrease reminder? Yes, there is one on the date of **Da**.  
8. The planning system adds the decrease reminder of -3 reminder to the projected inventory level, either A: +4 -3 = 1 or B: +6 -3 = +3.  
9. For A, the planning system creates a forward-scheduled order starting on date **Da**. For B, the reorder point is reached and a new order is created.

## <a name="the-role-of-the-time-bucket"></a>The role of the time bucket

The purpose of the time bucket is to collect demand events within a time period in order to make a joint supply order.  

For reordering policies that use a reorder point, you can define a time bucket. Time buckets help ensure that demands within the same time period are accumulated. The system then check the effect on projected inventory and whether the reorder point has been passed.

If you pass the reorder point, the system forward schedules a new supply order from the end of the time bucket. Time buckets begin on the planning starting date.  

The time bucket concept reflects the manual process of checking the inventory level on a frequent basis rather than for each transaction. You define the frequency (the time bucket). For example, you might gather all item needs from a vendor to place a weekly order.  

![Example of time bucket in planning.](media/nav_app_supply_planning_2_reorder_cycle.png "Example of time bucket in planning")  

Time buckets are often used to avoid a cascade effect. For example, a balanced row of demand and supply where an early demand is cancelled, or a new one is created. The result would be that every supply order (except the last one) is rescheduled.

## <a name="stay-below-the-overflow-level"></a>Stay below the overflow level

When using the **Maximum Qty.** and **Fixed Reorder Qty.** reordering policies, the planning system focuses on the projected inventory in the given time-bucket only. It might suggest extra supply when negative demand or positive supply changes happen outside the time bucket. For extra supply, the planning system calculates the quantity by which you should decrease the supply. This quantity is called the “overflow level.” The overflow is available as a planning line with a **Change Qty. (Decrease)** or **Cancel** action and the following warning message:  

* Attention: The projected inventory [xx] is higher than the overflow level [xx] on the Due Date [xx].*  

![Inventory overflow level.](media/supplyplanning_2_overflow1_new.png "Inventory overflow level")  

### <a name="calculating-the-overflow-level"></a>Calculating the overflow level

The overflow level is calculated in different ways depending on the reordering policy.  

#### <a name="maximum-qty"></a>Maximum Qty.

Overflow level = maximum inventory  

> [!NOTE]  
> If you use a minimum order quantity, it's added as follows:
>
> overflow level = maximum inventory + minimum order quantity.  

#### <a name="fixed-reorder-qty"></a>Fixed Reorder Qty.

overflow level = reorder quantity + reorder point  

> [!NOTE]  
> If the minimum order quantity is higher than the reorder point, it's replaced as follows:
>
> overflow level = reorder quantity + minimum order quantity  

#### <a name="order-multiple"></a>Order multiple

If an order multiple exists, it adjusts the overflow level for both the Maximum Qty. and Fixed Reorder Qty. reordering policies.  

### <a name="creating-the-planning-line-with-an-overflow-warning"></a>Creating the planning line with an overflow warning

A planning line is created when a supply causes the projected inventory to be higher than the overflow level at the end of a time bucket. To warn about the extra supply, the planning line has a warning message, the **Accept Action Message** field is not selected, and the action message is either **Cancel** or **Change Qty.**  

#### <a name="calculating-the-planning-line-quantity"></a>Calculating the planning line quantity

The quantity on a planning line is calculated as follows:

planning line quantity = current supply quantity – (projected inventory – overflow level)  

> [!NOTE]  
> For sAs with all warning lines, the maximum and minimum order quantity and order multiple are ignored.  

#### <a name="defining-the-action-message-type"></a>Defining the action message type

* If the planning line quantity is higher than 0, the action message is **Change Qty.**  
* If the planning line quantity is equal to or less than 0, the action message is **Cancel**  

#### <a name="composing-the-warning-message"></a>Composing the warning message

If there's overflow, the **Untracked Planning Elements** page displays a warning message with the following information:  

* The projected inventory level that triggered the warning  
* The calculated overflow level  
* The due date of the supply event  

Example: “The projected inventory 120 is higher than the overflow level 60 on 01-28-23”  

### <a name="example-scenario"></a>Example scenario

In this scenario, a customer changes a sales order from 70 to 40 pieces between two planning runs. The overflow feature reduces the purchase that was suggested for the initial sales quantity.  

#### <a name="item-setup"></a>Item setup

|Reordering Policy|Maximum Qty.|  
|-----------------------|------------------|  
|Maximum Order Quantity|100|  
|Reorder Point|50|  
|Inventory|80|  

#### <a name="situation-before-sales-decrease"></a>Situation before sales decrease

|Event|Change Qty.|Projected Inventory|  
|-----------|-----------------|-------------------------|  
|Day one|None|80|  
|Sale|-70|10|  
|End of time bucket|None|10|  
|Suggest new purchase order|+90|100|  

#### <a name="situation-after-sales-decrease"></a>Situation after sales decrease

|Change|Change Qty.|Projected Inventory|  
|------------|-----------------|-------------------------|  
|Day one|None|80|  
|Sale|-40|40|  
|Purchase|+90|130|  
|End of time bucket|None|130|  
|Suggest to decrease purchase<br><br> order from 90 to 60|-30|100|  

#### <a name="resulting-planning-lines"></a>Resulting planning lines

The system creates a warning planning line to reduce the purchase by 30, from 90 to 60, to keep the projected inventory at 100 according to the overflow level.  

![Plan according to overflow level.](media/nav_app_supply_planning_2_overflow2.png "Plan according to overflow level")  

> [!NOTE]  
> Without the overflow feature, no warning is created if the projected inventory level is above the maximum, which could cause an extra supply of 30.

## <a name="handling-projected-negative-inventory"></a>Handling projected negative inventory

The reorder point expresses the anticipated demand during the lead time of the item. The projected inventory must be large enough to cover the demand until the new order is received. Meanwhile, the safety stock should take care of fluctuations in demand up to a targeted service level.  

The planning system considers it an emergency if a future demand can't be served from the projected inventory. Or, expressed in another way, that the projected inventory goes negative. The system suggests that you create a new supply order to cover the unmet part of the demand. The size of the new supply order won't consider the maximum inventory or the reorder quantity nor the following order modifiers:

* Maximum order quantity
* Minimum order quantity
* Order multiple 

Instead, it reflects the exact deficiency.  

The planning line for this type of supply order will display an **Emergency** warning icon provide additional information about the situation.  

In the following image, supply D represents an emergency order to adjust for negative inventory.  

![Emergency planning suggestion to avoid negative inventory.](media/nav_app_supply_planning_2_negative_inventory.png "Emergency planning suggestion to avoid negative inventory")  

1. Supply **A**, initial projected inventory, is below reorder point.  
2. A new forward-scheduled supply is created (**C**).  

     (quantity = maximum inventory – projected inventory level)  
3. Supply **A** is closed by demand **B**, which is not fully covered.  

     (Demand **B** could try to schedule Supply C in, but the time-bucket prevents that.)  
4. New supply (**D**) is created to cover the remaining quantity on Demand **B**.  
5. Demand **B** is closed (creating a reminder to the projected inventory).  
6. The new supply **D** is closed.  
7. Projected inventory is checked. The reorder point hasn't been crossed.  
8. Supply **C** is closed (there's no more demand).  
9. Final check. There are no outstanding inventory level reminders.  

The following section describes the characteristics of the four supported reordering policies.

## <a name="reordering-policies"></a>Reordering policies

Reordering policies define how much to order when the item needs to be replenished. Four different reordering policies exist.  

### <a name="fixed-reorder-quantity"></a>Fixed Reorder Quantity

The Fixed Reorder Qty. policy is typically used for inventory planning for items with the following characteristics:

* Low inventory cost
* Low risk of obsolescence
* Low number of items

Typically, use this policy with a reorder point that reflects the anticipated demand during the item's lead time.  

#### <a name="calculated-per-time-bucket"></a>Calculated per time bucket

If you reach or cross at the reorder point in a time bucket (reorder cycle), the system suggests two actions:

* Create a new supply order for the reorder quantity
* Forward schedule the order from the first date after the end of the time bucket  

The time bucketed reorder point reduces the number of supply suggestions. It reflects a process of manually checking to actual contents of bins in your warehouse.  

#### <a name="creates-only-necessary-supply"></a>Creates only necessary supply

Before it suggests a new supply order to meet a reorder point, the planning system checks for the following supply:

* Whether supply is already ordered
* Whether you expect to receive the supply within the item’s lead time

The system won't suggest a new supply order if a supply will bring the projected inventory to the reorder point within the lead time.  

Supply orders that are created specifically to meet a reorder point are excluded from supply balancing and won't be changed. If you want to phase out an item that has a reorder point, review your outstanding supply orders manually or change the reordering policy to **Lot-for-Lot**. The system will reduce or cancel extra supply.  

#### <a name="combines-with-order-modifiers"></a>Combines with order modifiers

The Minimum Order Quantity, Maximum Order Quantity, and Order Multiple order modifiers shouldn't play a significant role when you use the Fixed Reorder Qty. policy. However, the planning system takes them into account:

* Decrease the quantity to the specified maximum order quantity (and create two or more supplies in order to reach the total order quantity)
* Increase the order to the specified minimum order quantity
* Round up the order quantity to meet a specified order multiple  

#### <a name="combines-with-calendars"></a>Combines with calendars

Before suggesting a new supply order to meet a reorder point, the planning system checks whether the order is scheduled for a non-working day. It uses the calendars you specify in the **Base Calendar Code** field on the **Company Information** and **Location Card** pages.  

If the scheduled date is a non-working day, the planning system moves the order forward to the nearest work day. Moving the date might result in an order that meets a reorder point but doesn't meet a specific demand. For such unbalanced demand, the planning system creates an extra supply.  

#### <a name="shouldnt-be-used-with-forecasts"></a>Shouldn't be used with forecasts

Because the anticipated demand is already expressed in the reorder point level, it isn't necessary to include a forecast in the planning. If it's relevant to base the plan on a forecast, use the **Lot-for-Lot** policy.  

#### <a name="must-not-be-used-with-reservations"></a>Must not be used with reservations

If you have reserved a quantity, for instance a quantity in inventory, for a distant demand, you might disturb the planning foundation. Even if the projected inventory level is acceptable in relation to the reorder point, the quantities might not be available. The system might try to compensate by creating exception orders. However, we recommend that the **Reserve** field is set to **Never** on items that are planned using a reorder point.

### <a name="maximum-quantity"></a>Maximum Quantity

The Maximum Quantity policy is a way to maintain inventory using a reorder point.  

Everything regarding the Fixed Reorder Qty. policy also applies to this policy. The only difference is the quantity of the suggested supply. When using the maximum quantity policy, the reorder quantity will be defined dynamically based on the projected inventory level. Therefore, it usually differs from order to order.  

#### <a name="calculate-per-time-bucket"></a>Calculate per time bucket

When you reach or cross the reorder point, the system determines the reorder quantity at the end of a time bucket. It measures the gap between the current projected inventory level and the specified maximum inventory to determine the quantity to order. The system then checks:

* Whether supply is already ordered
* Whether you expect to receive the supply within the item’s lead time

If so, the system reduces the quantity of the new supply order by the quantities already ordered.  

If you don't specify a maximum inventory quantity, the planning system ensures that the projected inventory reaches the reorder quantity.

#### <a name="combine-with-order-modifiers"></a>Combine with order modifiers

Depending on your setup, it might be best to combine the Maximum Quantity policy with order modifiers: 

* To ensure a minimum order quantity
* Round the quantity to an integer number of purchase units of measure
* Split the quantity into lots as defined by the maximum order quantity  

### <a name="combine-with-calendars"></a>Combine with calendars

Before suggesting a new supply order to meet a reorder point, the planning system checks whether the order is scheduled for a non-working day. It uses the calendars you specify in the **Base Calendar Code** field in the **Company Information** and **Location Card** pages.  

If the scheduled date is a non-working day, the planning system moves the order forward to the nearest work day. Moving the date might result in an order that meets a reorder point but doesn't meet a specific demand. For such unbalanced demand, the planning system creates an extra supply.

### <a name="order"></a>Order

In a make-to-order environment, an item is purchased or produced to cover a specific demand. Typically, the Order reordering policy is used for items with the following characteristics

* Demand is infrequent
* The lead-time is insignificant
* Required attributes vary  

[!INCLUDE [prod_short](includes/prod_short.md)] creates an order-to-order link, which acts as a preliminary connection between the supply (a supply order or inventory) and the demand. You can apply the order-to-order link during planning in the following ways:  

* When you use the Make-to-Order manufacturing policy to create multi-level or project type production orders (producing needed components on the same production order)  
* When you use sales order planning to create a production order from a sales order  

> [!TIP]
> If item attributes don't vary, it might be best to use a Lot-for-Lot reordering policy. As a result, the system uses unplanned inventory and only accumulates sales orders with the same shipment date or within a defined time bucket.  

#### <a name="order-to-order-links-and-past-due-dates"></a>Order-to-order links and past due dates

Unlike most supply-demand sets, linked orders with due dates before the planning starting date are fully planned for by the system. The reason for this exception is that specific demand-supply sets must be synchronised. To learn more about the frozen zone that applies to most demand-supply types, go to [Process orders before the planning start date](design-details-balancing-demand-and-supply.md#process-orders-before-the-planning-start-date).

### <a name="lot-for-lot"></a>Lot-for-Lot

The Lot-for-Lot policy is the most flexible because the system only reacts to actual demand. It acts on anticipated demand from forecast and blanket orders and then settles the order quantity based on the demand. The policy is intended for items where inventory can be accepted but should be avoided.  

In some ways, the Lot-for-Lot policy is similar to the Order policy. It can accept quantities in inventory, and it bundles demand and supply in the time buckets you define.

You specify the time bucket in the **Time Bucket** field on the **Item Card** page. The minimum size of time bucket is one day, because that's the smallest time unit of measure on demand and supply events in [!INCLUDE [prod_short](includes/prod_short.md)].  

The time bucket also limits when you should reschedule a supply order to meet a given demand. Supply within the time bucket is rescheduled in or out to meet the demand. Earlier supply will cause extra inventory, and you should cancel it. For supply that's later, create a new supply order.  

With this policy, you can specify a safety stock to compensate for changes in supply or to meet a sudden demand. The lot-for-lot policy can also include a dampener period and dampener quantity to reduce order scheduling.  

Together with the **Rescheduling Period** field, the **Lot Accumulation Period** field contributes to defining the reorder cycle. From the date of the first demand, all demands are accumulated in the next lot accumulation period into one supply order on the date of the first demand. Demand that is outside the lot accumulation period is not covered by the supply order.

Because the supply order quantity is based on the actual demand, it can make sense to use order modifiers:

* Round up the order quantity to meet an order multiple (or purchase unit of measure)
* Increase the order to a specified minimum order quantity
* Decrease the quantity to the specified maximum quantity (and thus create two or more supplies to reach the total needed quantity)

## <a name="see-also"></a>See Also

[Design Details: Planning Parameters](design-details-planning-parameters.md)  
[Design Details: Planning Assignment Table](design-details-planning-assignment-table.md)  
[Design Details: Central Concepts of the Planning System](design-details-central-concepts-of-the-planning-system.md)  
[Design Details: Balancing Demand and Supply](design-details-balancing-demand-and-supply.md)  
[Design Details: Supply Planning](design-details-supply-planning.md)

[!INCLUDE[footer-include](includes/footer-banner.md)]
