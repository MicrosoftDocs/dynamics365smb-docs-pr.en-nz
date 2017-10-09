---
title: Assembly Management | Microsoft Docs
description: Support companies that supply products to their customers by combining components in simple processes without the need of manufacturing functionality but with features to assemble items that integrate with existing features, such as sales, planning, reservations, and warehousing.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/08/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: d945858b3a26126a2def48d88ff1132f598c0916
ms.contentlocale: en-nz
ms.lasthandoff: 09/22/2017

---
# <a name="assembly-management"></a>Assembly Management
To support companies that supply products to their customers by combining components in simple processes without the need of manufacturing functionality, [!INCLUDE[d365fin](includes/d365fin_md.md)] includes features to assemble items that integrate with existing features, such as sales, planning, reservations, and warehousing.  

 An assembly item is defined as a sellable item that contains an assembly BOM.

 Assembly orders are internal orders, just like production orders, that are used to manage the assembly process and to connect the sales requirements with the involved warehouse activities. Assembly orders differ from other order types because they involve both output and consumption when posting. The assembly order header behaves similarly to a sales order line, and the assembly order lines behave similarly to consumption journal lines. For more information, see Assembly Order.  

 To support a just-in-time inventory strategy and the ability to customise products to customer requests, assembly orders may be automatically created and linked as soon as the sales order line is created. The link between the sales demand and the assembly supply enables sales order processors to customise the assembly item on the fly, promise delivery dates according to component availability, and to post output and shipment of the assembled item directly from their sales order interface. For more information, see [How to: Sell Items Assembled to Order](assembly-how-to-sell-items-assembled-to-order.md).  

 On one sales order line, you can sell a quantity that is available and must be picked from stock together with a quantity that must be assembled to the order. Certain rules exist to govern the distribution of such quantities to ensure that assemble-to-order quantities take priority over inventory quantities in partial shipping. For more information, see the “Combination Scenarios” section in [Understanding Assemble to Order and Assemble to Stock](assembly-assemble-to-order-or-assemble-to-stock.md).  

 Special functionality exists to govern the shipping of assemble-to-order quantities. When an assemble-to-order quantity is ready to be shipped, the warehouse worker in charge posts an inventory pick for the sales order line(s) in question. This, in turn, creates an inventory movement for the components, posts the assembly output, and the sales order shipment. For more information, see the "Handling Assemble-to-Order Items in Inventory Picks” section in [How to: Pick Items with Inventory Picks](warehouse-how-to-pick-items-with-inventory-picks.md).

The following table describes a sequence of tasks, with links to the topics that describe them.   

|**To**|**See**|  
|------------|-------------|  
|Learn about the difference between assembling items right before shipping sales orders and assembling items that are intended for storage.|[Understanding Assemble to Order and Assemble to Stock](assembly-assemble-to-order-or-assemble-to-stock.md)|
|Fill in fields on location cards and in inventory setup to define how items flow to and from the assembly department.|[How to: Set Up Basic Warehouses with Operations Areas](warehouse-how-to-set-up-basic-warehouses-with-operations-areas.md)|
|Customise an assembly item to a customer’s request during the sales process, and convert to a sale when accepted.|[How to: Quote an Assemble-to-Order Sale](assembly-how-to-quote-an-assemble-to-order-sale.md)|
|Combine components to create an item in a simple process, to order or to stock.|[How to: Assemble Items](assembly-how-to-assemble-items.md)|  
|Sell assembly items that are not currently available by creating a linked assembly order to supply the full or partial sales order quantity.|[How to: Sell Items Assembled to Order](assembly-how-to-sell-items-assembled-to-order.md)|
|When some assemble-to-order items are already in inventory, deduct that quantity from the assembly order and reserve it from inventory.|[How to: Sell Inventory Items in Assemble-to-Order Flows](assembly-how-to-sell-inventory-items-in-assemble-to-order-flows.md)|  
|When you are selling assembly items from inventory and all items are not available, initiate an assembly order to automatically supply a part or all of the sales order quantity.|[How to: Sell Assemble-to-Order Items and Inventory Items Together](assembly-how-to-sell-assemble-to-order-items-and-inventory-items-together.md)|
|Undo a posted assembly order, for example because the order was posted with mistakes that must be corrected.|[How to: Undo Assembly Posting](assembly-how-to-undo-assembly-posting.md)|
|Learn about the difference between assembly BOMs and production BOMs and the involved processing differences.|[How to: Work with Bills of Material](inventory-how-work-BOMs.md)|
|Learn how assembly consumption and output are handled when you post assembly orders and how the derived item and resource costs are processed and distributed to the general ledger.|[Design Details: Assembly Order Posting](design-details-assembly-order-posting.md)|  

## <a name="see-also"></a>See Also  
[How to: Work with Bills of Material](inventory-how-work-BOMs.md)  
[Inventory](inventory-manage-inventory.md)  
[Design Details: Warehouse Management](design-details-warehouse-management.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

