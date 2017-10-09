---
title: Design Details - Handling Reordering Policies | Microsoft Docs
description: Overview of tasks for defining a reorder policy in supply planning.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 2a6658508f8e12a11989d54da6d6c8e3a36631cc
ms.contentlocale: en-nz
ms.lasthandoff: 09/22/2017

---
# <a name="design-details-handling-reordering-policies"></a>Design Details: Handling Reordering Policies
For an item to participate in supply planning, a reorder policy must be defined. The following four reordering policies exist:  
  
* Fixed Reorder Qty.  
* Maximum Qty.  
* Order  
* Lot-for-Lot  
  
Fixed Reorder Qty. and Maximum Qty. policies relate to inventory planning. Although inventory planning is technically simpler than the balancing procedure, these policies must coexist with the step-by-step balancing of supply and order tracking. To control the integration between the two, and to provide visibility into the involved planning logic, strict principles govern how reordering policies are handled.  
  
## <a name="in-this-section"></a>In This Section  
[Design Details: The Role of the Reorder Point](design-details-the-role-of-the-reorder-point.md)  
[Design Details: Monitoring the Projected Inventory Level and the Reorder Point](design-details-monitoring-the-projected-inventory-level-and-the-reorder-point.md)  
[Design Details: The Role of the Time Bucket](design-details-the-role-of-the-time-bucket.md)  
[Design Details: Staying under the Overflow Level](design-details-staying-under-the-overflow-level.md)  
[Design Details: Handling Projected Negative Inventory](design-details-handling-projected-negative-inventory.md)  
[Design Details: Reordering Policies](design-details-reordering-policies.md)  
  
## <a name="see-also"></a>See Also  
[Design Details: Planning Parameters](design-details-planning-parameters.md)   
[Design Details: Planning Assignment Table](design-details-planning-assignment-table.md)   
[Design Details: Central Concepts of the Planning System](design-details-central-concepts-of-the-planning-system.md)   
[Design Details: Balancing Demand and Supply](design-details-balancing-demand-and-supply.md)   
[Design Details: Supply Planning](design-details-supply-planning.md)
