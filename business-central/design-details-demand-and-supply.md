---
title: Design Details - Demand and Supply | Microsoft Docs
description: Demand is the common term used for any kind of gross demand, such as a sales order and component need from a production order. In addition, the program allows more technical types of demand, such as negative inventory and purchase returns.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: db4defc0a2bccd7c4aaa69cd06832c486178e70a
ms.contentlocale: en-nz
ms.lasthandoff: 03/22/2018

---
# <a name="design-details-demand-and-supply"></a>Design Details: Demand and Supply
Demand is the common term used for any kind of gross demand, such as a sales order and component need from a production order. In addition, the program allows more technical types of demand, such as negative inventory and purchase returns.  
  
 Supply is the common term used for any kind of positive or inbound quantity, such as inventory, purchases, assembly, production, or inbound transfers. In addition, a sales return may also represent supply.  
  
 To sort out the many sources of demand and supply, the planning system organises them on two time lines called inventory profiles. One profile holds demand events, and the other holds the corresponding supply events. Each event represents one order network entity, such as a sales order line, an item ledger entry, or a production order line.  
  
 When inventory profiles are loaded, the different demand-supply sets are balanced to output a supply plan that fulfills the listed goals.  
  
 Planning parameters and inventory levels are other types of demand and supply respectively, which undergo integrated balancing to replenish stock items. For more information, see [Design Details: Handling Reordering Policies](design-details-handling-reordering-policies.md).  
  
## <a name="see-also"></a>See Also  
 [Design Details: Balancing Demand and Supply](design-details-balancing-demand-and-supply.md)   
 [Design Details: Central Concepts of the Planning System](design-details-central-concepts-of-the-planning-system.md)   
 [Design Details: Supply Planning](design-details-supply-planning.md)
