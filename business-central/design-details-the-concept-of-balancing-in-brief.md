---
title: Design Details - The Concept of Balancing in Brief | Microsoft Docs
description: Demand is given by a company’s customers. Supply is what the company can create and remove to establish balance. The planning system starts with the independent demand and then tracks backwards to the supply.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2019
ms.author: sgroespe
redirect_url: design-details-balancing-demand-and-supply
ms.openlocfilehash: af63bf59def37fe873cb66366864855db52bd245
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 10/01/2019
ms.locfileid: "2302972"
---
# <a name="design-details-the-concept-of-balancing-in-brief"></a>Design Details: The Concept of Balancing in Brief
Demand is given by a company’s customers. Supply is what the company can create and remove to establish balance. The planning system starts with the independent demand and then tracks backwards to the supply.  

 The inventory profiles are used to contain information about the demands and supplies, quantities, and timing. These profiles essentially make up the two sides of the balancing scale.  

 The objective of the planning mechanism is to counterbalance the demand and supply of an item to ensure that supply will match demand in a feasible way as defined by the planning parameters and rules.  

 ![Overview of supply-demand balancing](media/nav_app_supply_planning_2_balancing.png "Overview of supply-demand balancing")  

## <a name="see-also"></a>See Also  
 [Design Details: Balancing Demand and Supply](design-details-balancing-demand-and-supply.md)   
 [Design Details: Central Concepts of the Planning System](design-details-central-concepts-of-the-planning-system.md)   
 [Design Details: Supply Planning](design-details-supply-planning.md)
