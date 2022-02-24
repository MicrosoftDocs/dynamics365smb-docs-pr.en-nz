---
title: Design Details - Item Tracking in the Warehouse | Microsoft Docs
description: Serial number and lot number handling is primarily a warehouse task and therefore all inbound and outbound warehouse documents have standard functionality for assigning and selecting item tracking numbers. However, because the reservation system is based on item ledger entries, warehouse activity documents that register only warehouse entries are not fully supported.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: design, item, tracking, serial number, lot number, outbound documents
ms.date: 04/01/2020
ms.author: sgroespe
ms.openlocfilehash: 02a87bc61fbadae4392800f84adbc176bfb87b23
ms.sourcegitcommit: 88e4b30eaf6fa32af0c1452ce2f85ff1111c75e2
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 04/01/2020
ms.locfileid: "3185028"
---
# <a name="design-details-item-tracking-in-the-warehouse"></a>Design Details: Item Tracking in the Warehouse
Serial number and lot number handling is primarily a warehouse task and therefore all inbound and outbound warehouse documents have standard functionality for assigning and selecting item tracking numbers.  

However, because the reservation system is based on item ledger entries, warehouse activity documents that register only warehouse entries are not fully supported. Because reservations and item tracking numbers can be handled only at the location level, not at the bin and zone level, the **Item Tracking Lines** page cannot be opened from warehouse activity documents. The same applies to the **Reservation** page.  

After a serial or lot number has been added to an item at a warehouse location, it can be moved and reclassified freely within the warehouse by using an independent item tracking structure that is unrelated to the reservation system. **Serial No.** and **Lot No.** fields are accessed directly on warehouse document lines. When the serial or lot number later partakes in outbound posting, it is synchronised with the reservation system as a part of ordinary bin adjustment. For more information, see [Design Details: Integration with Inventory](design-details-integration-with-inventory.md).  

However, the reservation system does take warehouse activities into consideration when it calculates availability. For example, items that are allocated to picks, or registered as picked, cannot be reserved. For more information, see [Design Details: Warehouse Availability](design-details-availability-in-the-warehouse.md).

## <a name="see-also"></a>See Also  
[Design Details: Item Tracking](design-details-item-tracking.md)  
[Design Details: Integration with Inventory](design-details-integration-with-inventory.md)  
[Design Details: Warehouse Availability](design-details-availability-in-the-warehouse.md)  
[Design Details: Item Tracking Design](design-details-item-tracking-design.md)
