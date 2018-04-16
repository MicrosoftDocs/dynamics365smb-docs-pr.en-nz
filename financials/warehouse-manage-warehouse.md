---
title: Warehouse Activities | Microsoft Docs
description: After goods are received and before goods are shipped, a series of internal warehouse activities take place to ensure an effective flow through the warehouse and to organise and maintain company inventories.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/15/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b34f276a764f0e828fbc1f015429df9852242a4c
ms.openlocfilehash: c8d4ee33395c18cb7755fd1877b2af813fb9da43
ms.contentlocale: en-nz
ms.lasthandoff: 03/22/2018

---
# <a name="warehouse-management"></a>Warehouse Management
After goods are received and before goods are shipped, a series of internal warehouse activities take place to ensure an effective flow through the warehouse and to organise and maintain company inventories.

Typical warehouse activities include putting items away, moving items inside or between warehouses, and picking items for assembly, production, or shipment. Assembling items for sale or inventory may also be considered warehouse activities, but these are covered elsewhere. For more information, see [Assembly Management](assembly-assemble-items.md).  

In large warehouses, these different handling tasks can be separated by departments and the integration managed by a directed workflow. In simpler installations, the flow is less formalised and the warehouse activities are performed with so-called inventory put-aways and inventory picks. For more information about basic versus advanced warehouse configurations, see [Design Details: Warehouse Overview](design-details-warehouse-overview.md).

Before you can perform warehouse activities, you must set the system up for the relevant complexity of warehouse processing. For more information, see [Setting Up Warehouse Management](warehouse-setup-warehouse.md).

 The following table describes a sequence of tasks, with links to the topics that describe them.   

|**To**|**See**|  
|------------|-------------|  
|Record the receipt of items at warehouse locations, either with a purchase order only, in simple location setups, or with a warehouse receipt, in case of semi or fully automated warehouse processing at the location.|[Receive Items](warehouse-how-receive-items.md)|
|Bypass the put-away and pick processes to expedite an item straight from receiving or production to shipping.|[Cross-Dock Items](warehouse-how-to-cross-dock-items.md)|    
|Put away items received from purchases, sales returns, transfers, or production output according to the configured warehouse process.|[Putting Items Away](warehouse-put-away-items.md)|
|Move items between bins in the warehouse.|[Moving Items](warehouse-move-items.md)|
|Pick items to be shipped, transferred, or consumed in assembly or production, according to the configured warehouse process.|[Picking Items](warehouse-pick-items.md)|
|Record the shipment of items from warehouse locations, either with a sales order only, in simple location setups, or with a warehouse shipment, in case of semi or fully automated warehouse processes at the location.|[Ship Items](warehouse-how-ship-items.md)|  

## <a name="see-also"></a>See Also  
[Inventory](inventory-manage-inventory.md)  
[Setting Up Warehouse Management](warehouse-setup-warehouse.md)     
[Assembly Management](assembly-assemble-items.md)    
[Design Details: Warehouse Management](design-details-warehouse-management.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

## [!INCLUDE [d365fin](includes/free_trial_md.md)]  
## [!INCLUDE [d365fin](includes/training_link_md.md)]

