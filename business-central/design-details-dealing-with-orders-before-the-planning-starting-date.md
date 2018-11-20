---
title: Design Details - Dealing with Orders Before the Planning Starting Date | Microsoft Docs
description: This topic describes the rules that planning applies to orders in the frozen zone.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: planning, frozen, design serial, lot
ms.date: 10/01/2018
ms.author: sgroespe
redirect_url: design-details-balancing-demand-and-supply
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 4fc4afa14f9f2a989fae0b1ca8ee0e61fe24fd21
ms.contentlocale: en-nz
ms.lasthandoff: 03/22/2018

---
# <a name="design-details-dealing-with-orders-before-the-planning-starting-date"></a>Design Details: Dealing with Orders Before the Planning Starting Date
To avoid that a supply plan shows impossible and therefore useless suggestions, the planning system regards the period up until the planning starting date a frozen zone where nothing is planned for. The following rule applies to the frozen zone:  

All supply and demand before the starting date of the planning period will be considered a part of inventory or shipped.  

Accordingly, the planning system will not, with a few exceptions, suggest any changes to supply orders in the frozen zone, and no order tracking links are created or maintained for that period.  

The exceptions to this rule are as follows:  

* If the projected available inventory, including the sum of supply and demand in the frozen zone, is below zero.  
* If serial/lot numbers are required on the backdated order(s).  
* If the supply-demand set is linked by an order-to-order policy.  

If the initial available inventory is below zero, the planning system suggests an emergency supply order on the day before the planning period to cover the missing quantity. Consequently, the projected and available inventory will always be at least zero when planning for the future period begins. The planning line for this supply order will display an Emergency warning icon and additional information is provided upon lookup.  

## <a name="seriallot-numbers-and-order-to-order-links-are-exempt-from-the-frozen-zone"></a>Serial/Lot Numbers and Order-to-Order Links are Exempt from the Frozen Zone  
If serial/lot numbers are required or an order-to-order link exists, the planning system will disregard the frozen zone and incorporate such quantities that are back-dated from the starting date and potentially suggest corrective actions if demand and supply is not synchronised. The business reason for this principle is that such specific demand-supply sets must match to ensure that this specific demand is fulfilled.  

## <a name="see-also"></a>See Also  
[Design Details: Balancing Demand and Supply](design-details-balancing-demand-and-supply.md)   
[Design Details: Central Concepts of the Planning System](design-details-central-concepts-of-the-planning-system.md)   
[Design Details: Supply Planning](design-details-supply-planning.md)

