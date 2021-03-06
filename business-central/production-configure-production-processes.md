---
title: Configure Production Processes | Microsoft Docs
description: To convert material into produced end items, production resources, such as bills of material, routings, machine operators, and machinery must be set up in the system.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 29bb70d54c4e5bb1dbc366a8f566e8247f4117ef
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 12/17/2020
ms.locfileid: "4759458"
---
# <a name="setting-up-manufacturing"></a>Setting Up Manufacturing
To convert material into produced end items, production resources, such as bills of material, routings, machine operators, and machinery must be set up in the system.

Operators and machines are represented in the system as machine centres that may be organised in work centres and work centre groups. When these resources are established, they can be loaded with operations according to the item's defined material (BOM) and process (routing) structure, and according to the capacity of the machine or work centre. You can also set the production capacity of each resource. Capacity is defined by the work time available in the machine and work centres, and is governed by calendars for each level. A work centre calendar specifies the working days or hours, shifts, holidays, and absence that determine the work centre’s gross available capacity (typically measured in minutes). All of this is determined by defined efficiency and capacity values.  

When you have set up manufacturing, you can plan and execute production orders. For more information, see [Planning](production-planning.md) and [Manufacturing](production-manage-manufacturing.md).  



 The following table describes a sequence of tasks, with links to the topics that describe them.   

|**To**|**See**|  
|------------|-------------|  
|Configure the manufacturing features, such as defining shop floor work hours and selecting planning parameters.|The **Manufacturing Setup** page.|
|On the **Planning** tab on the **Manufacturing Setup** page, set global planning parameters that override parameters set on individual item cards.|[Design Details: Planning Parameters](design-details-planning-parameters.md)|
|Define a standard working week in the manufacturing department in terms of starting and ending times of each work day and related work shift.|[Create Shop Calendars](production-how-to-create-work-center-calendars.md)|  
|Organise fixed values and requirements of production resources as work centres or machine centres to govern their output of production performed.|[Set Up Work Centres and Machine Centres](production-how-to-set-up-work-and-machine-centers.md)|
|Organise production operations in the required order and assign them to work or machine centres with the required work times.|[Create Routings](production-how-to-create-routings.md)|
|Organise production components or subassemblies under a produced parent item and certify the BOM for execution at work centres.|[Create Production BOMs](production-how-to-create-production-boms.md)|
|Make sure that the right component quantity is available when produced items are stocked in one unit of measure but produced in another.|[Work With Manufacturing Batch Units of Measure](production-how-to-use-the-manufacturing-batch-unit-of-measure.md)|  
|Define families of production items with similar manufacturing processes to save consumption. For example, four pieces of the same item can be produced from one sheet and 10 pieces of another, different, item at the same time.|[Work With Production Families](production-how-work-family.md)|
|Use standard tasks to simplify the creation of routings by quickly attaching extra information to recurring operations.|[Set Up Standard Routing Lines](production-how-set-up-standard-routing-lines.md)|  
|Prepare work centres and routings to represent subcontracted production operations.|[Subcontract Manufacturing](production-how-to-subcontract-manufacturing.md)|  

## <a name="see-also"></a>See Also
[Manufacturing](production-manage-manufacturing.md)    
[Planning](production-planning.md)   
[Inventory](inventory-manage-inventory.md)  
[Purchasing](purchasing-manage-purchasing.md)  
[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]