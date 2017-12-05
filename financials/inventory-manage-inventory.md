---
title: Managing Inventory| Microsoft Docs
description: Describes how to manage the physical products that you trade in, for example, handling the stock in your warehouse.
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: warehouse, stock
ms.date: 09/08/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: ba26b354d235981bd7291f9ac6402779f554ac7a
ms.openlocfilehash: c3cfae3d52cbb25882c5986ad4aedaef7939a8b6
ms.contentlocale: en-nz
ms.lasthandoff: 11/10/2017

---

# <a name="inventory"></a>Inventory
For each physical product that you trade in, you must create an item card of type **Inventory**. Items that you offer to customers but do not keep in inventory you can register as nonstock items, which you can convert to inventory items when necessary. You can increase or decrease the quantity of an item in inventory by posting directly to the item ledger entries, for example, after a physical count or if you do not record purchases.

Inventory increases and decreases are naturally also recorded when you post purchase and sales documents respectively. For more information, see [How to: Record Purchases](purchasing-how-record-purchases.md), [How to: Sell Products](sales-how-sell-products.md), and [How to: Invoice Sales](sales-how-invoice-sales.md). Transfers between locations changes inventory quantities across your company's warehouses.   

To increase your overview of items and to help you find them, you can categorise items and give them attributes to search and sort by.

> [!NOTE]
> The physical handling of items is referred to as warehouse activities. For more information, see [Warehouse Management](warehouse-manage-warehouse.md).

## <a name="inventory-reconciliation"></a>Inventory Reconciliation
When you post inventory transactions, such as sales shipments, purchase invoices, or inventory adjustments, the changed item costs are recorded in item value entries. To reflect this change of inventory value in your financial books, the inventory costs are automatically posted to the related inventory accounts in the general ledger. For each inventory transaction that you post, the appropriate values are posted to the inventory account, adjustment account, and COGS account in the general ledger. For more information, see [How to: Reconcile Inventory Costs with the General Ledger](finance-how-to-post-inventory-costs-to-the-general-ledger.md).

Even though inventory costs are automatically posted to the general ledger, it is still necessary to ensure that the costs of goods are forwarded to the related outbound sales transaction, especially in situations where you sell goods before you invoice the purchase of those goods. This is referred to as cost adjustment. Item costs are automatically adjusted when you post item transactions, but you can also adjust item costs manually. For more information, see [How to: Adjust Item Costs](inventory-how-adjust-item-costs.md).

|To |See |
|---|----|
|Create item cards for inventory items that you trade in.|[How to: Register New Items](inventory-how-register-new-items.md)|
|Structure parent items that you sell as kits consisting of the parent's components or that you assemble to order or to stock.|[How to: Work with Bills of Material](inventory-how-work-BOMs.md)|
|Maintain an overview of items and help you find and sort items by organising them in categories.|[How to: Categorize Items](inventory-how-categorize-items.md)|
|Assign item attributes of different value types to your items to help you sort and find items.|[How to: Work with Item Attributes](inventory-how-work-item-attributes.md)|
|Create special item cards for items that you offer to customers but do not maintain inventory for.|[How to: Work with Nonstock Items](inventory-how-work-nonstock-items.md)|
|Perform physical counting, make negative or positive adjustments, and change information, such as location or lot number, on item ledger entries.|[How to: Count, Adjust, and Reclassify Inventory Inventory](inventory-how-count-adjust-reclassify.md)|
|View the availability of items per location, by period, by sales or purchase event, or by their use on assembly or production BOMs.|[How to: How to: View the Availability of Items](inventory-how-availability-overview.md)|
|Transfer inventory items between locations with transfer orders, to manage warehouse activities, or with the item reclassification journal.|[How to: Transfer Inventory Between Locations](inventory-how-transfer-between-locations.md)|
|Reserve inventory or inbound items for sales orders, purchase orders, service orders, assembly orders, or production orders.|[How to: Reserve Items](inventory-how-to-reserve-items.md)|
|Assign serial numbers or lot numbers to any outbound or inbound document or journal line, for example to track items in case of recalls.|[How to: Work with Serial and Lot Numbers](inventory-how-work-item-tracking.md)|
|Find where any serial or lot number was used in its supply chain, for example in recall situations.|[How to: Trace Item-Tracked Items](inventory-how-to-trace-item-tracked-items.md)|
|Manage business operations in sales offices, a purchasing departments, or plant planning offices across multiple locations.|[How to: Work with Responsibility Centres](inventory-responsibility-centers.md)|

## <a name="see-also"></a>See Also  
[Purchasing](purchasing-manage-purchasing.md)  
[Sales](sales-manage-sales.md)    
[Working with [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](ui-work-product.md)  
[General Business Functionality](ui-across-business-areas.md)

## [!INCLUDE[d365fin](includes/free_trial_md.md)]

