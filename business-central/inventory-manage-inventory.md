---
title: Managing Inventory| Microsoft Docs
description: Describes how to manage the physical products that you trade in, for example, handling the stock in your warehouse.
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: warehouse, stock
ms.date: 07/23/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: c6f10f8252c00bf0a599f9fa794ee36c41ce92be
ms.openlocfilehash: 745da790218ee57e4fb44b8c0bab2bce504eda3b
ms.contentlocale: en-nz
ms.lasthandoff: 07/30/2018

---

# <a name="inventory"></a>Inventory
For each physical product that you trade in, you must create an item card of type **Inventory**. Items that you offer to customers but do not keep in inventory you can register as nonstock items, which you can convert to inventory items when necessary. You can increase or decrease the quantity of an item in inventory by posting directly to the item ledger entries, for example, after a physical count or if you do not record purchases.

Inventory increases and decreases are naturally also recorded when you post purchase and sales documents respectively. For more information, see [Record Purchases](purchasing-how-record-purchases.md), [Sell Products](sales-how-sell-products.md), and [Invoice Sales](sales-how-invoice-sales.md). Transfers between locations changes inventory quantities across your company's warehouses.   

To increase your overview of items and to help you find them, you can categorise items and give them attributes to search and sort by.

> [!NOTE]
> The physical handling of items is referred to as warehouse activities. For more information, see [Warehouse Management](warehouse-manage-warehouse.md).

## <a name="inventory-reconciliation"></a>Inventory Reconciliation
When you post inventory transactions, such as sales shipments, purchase invoices, or inventory adjustments, the changed item costs are recorded in item value entries. To reflect this change of inventory value in your financial books, the inventory costs are automatically posted to the related inventory accounts in the general ledger. For each inventory transaction that you post, the appropriate values are posted to the inventory account, adjustment account, and COGS account in the general ledger. For more information, see [Reconcile Inventory Costs with the General Ledger](finance-how-to-post-inventory-costs-to-the-general-ledger.md).

Even though inventory costs are automatically posted to the general ledger, it is still necessary to ensure that the costs of goods are forwarded to the related outbound sales transaction, especially in situations where you sell goods before you invoice the purchase of those goods. This is referred to as cost adjustment. Item costs are automatically adjusted when you post item transactions, but you can also adjust item costs manually. For more information, see [Adjust Item Costs](inventory-how-adjust-item-costs.md).

|To |See |
|---|----|
|Create item cards for inventory items that you trade in.|[Register New Items](inventory-how-register-new-items.md)|
|Structure parent items that you sell as kits consisting of the parent's components or that you assemble to order or to stock.|[Work with Bills of Material](inventory-how-work-BOMs.md)|
|Maintain an overview of items and help you find and sort items by organising them in categories.|[Categorise Items](inventory-how-categorize-items.md)|
|Assign item attributes of different value types to your items to help you sort and find items.|[Work with Item Attributes](inventory-how-work-item-attributes.md)|
|Create special item cards for items that you offer to customers but do not maintain inventory for.|[Work with Nonstock Items](inventory-how-work-nonstock-items.md)|
|Perform physical counting, make negative or positive adjustments, and change information, such as location or lot number, on item ledger entries.|[Count, Adjust, and Reclassify Inventory Inventory](inventory-how-count-adjust-reclassify.md)|
|View the availability of items per location, by period, by sales or purchase event, or by their use on assembly or production BOMs.|[View the Availability of Items](inventory-how-availability-overview.md)|
|Transfer inventory items between locations with transfer orders, to manage warehouse activities, or with the item reclassification journal.|[Transfer Inventory Between Locations](inventory-how-transfer-between-locations.md)|
|Reserve inventory or inbound items for sales orders, purchase orders, service orders, assembly orders, or production orders.|[Reserve Items](inventory-how-to-reserve-items.md)|
|Assign serial numbers or lot numbers to any outbound or inbound document or journal line, for example to track items in case of recalls.|[Work with Serial and Lot Numbers](inventory-how-work-item-tracking.md)|
|Find where any serial or lot number was used in its supply chain, for example in recall situations.|[Trace Item-Tracked Items](inventory-how-to-trace-item-tracked-items.md)|
|Block items from being entered on sales or purchase lines or from being posted in any transaction.|[Block Items](inventory-how-block-items.md)|
|Manage business operations in sales offices, a purchasing departments, or plant planning offices across multiple locations.|[Work with Responsibility Centres](inventory-responsibility-centers.md)|

## <a name="see-also"></a>See Also  
[Warehouse Management](warehouse-manage-warehouse.md)  
[Purchasing](purchasing-manage-purchasing.md)  
[Sales](sales-manage-sales.md)    
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  
[General Business Functionality](ui-across-business-areas.md)

## [!INCLUDE[d365fin](includes/free_trial_md.md)]  

