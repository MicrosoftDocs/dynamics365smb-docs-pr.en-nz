---
title: How to Enable Picking by FEFO | Microsoft Docs
description: First-Expired-First-Out (FEFO) is a sorting method that ensures that the oldest items, those with the earliest expiration dates, are picked first.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 1c7896988545d6f1b8269ead90dff7350bc6f320
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 12/17/2020
ms.locfileid: "4755857"
---
# <a name="enable-picking-items-by-fefo"></a>Enable Picking Items by FEFO
First-Expired-First-Out (FEFO) is a sorting method that ensures that the oldest items, those with the earliest expiration dates, are picked first.  

 This functionality only works when the following criteria are met:  

-   The item must have a serial/lot number.  
-   On the item’s item tracking code setup, the **SN Warehouse Tracking** field or the **Lot Warehouse Tracking** field must be selected.  
-   The item must be posted to inventory with an expiration date.  
-   On the location card, the **Require Pick** check box must be selected.  
-   On the location card, the **Pick According to FEFO** check box must be selected.  
-   On the location card, the **Bin Mandatory** check box must be selected.  

 When all the criteria are met, then serial/lot-numbered items to be picked are sorted with the oldest first in all picks and movements, except for items that use SN-specific or lot-specific tracking.  

> [!NOTE]  
> If some serial/lot-numbered items use specific tracking, then those are respected first and under them, the remaining, non-specific, serial/lot numbers are listed according to FEFO.
<br /><br />
If two serial/lot-numbered items have the same expiration date, then application selects the item with the lowest serial or lot number.
<br /><br />
When picking serial/lot-numbered items in locations set up for directed put-away and pick, only quantities on bins of type *Pick* are picked according to FEFO.  
<br /><br />
To enable movements according to FEFO, either on the **Inventory Movement** page or the **Movement Worksheet** page, you must leave the **From Bin** field empty.  
<br /><br />
If the **Strict Expiration Posting** field is selected, then only items that are not expired will be included in the pick. This applies even if you are not using Pick according to FEFO.

## <a name="see-also"></a>See Also  
[Picking Items](warehouse-pick-items.md)   
[Pick Items for Warehouse Shipment](warehouse-how-to-pick-items-for-warehouse-shipment.md)   
[Pick Items with Inventory Picks](warehouse-how-to-pick-items-with-inventory-picks.md)   
[Design Details: Warehouse Management](design-details-warehouse-management.md)  
[Inventory](inventory-manage-inventory.md)  
[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)
