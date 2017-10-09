---
title: Defining and Allocating Costs | Microsoft Docs
description: Cost allocations move costs and revenues between cost types, cost centres, and cost objects. You can define as many allocations as you need.
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
ms.openlocfilehash: 050b0bd997629ca189cfbe035e361de7a252d079
ms.contentlocale: en-nz
ms.lasthandoff: 09/22/2017

---
# <a name="defining-and-allocating-costs"></a>Defining and Allocating Costs
Cost allocations move costs and revenues between cost types, cost centres, and cost objects. You can define as many allocations as you need. Each allocation consists of:  

-   An allocation source.  
-   One or more allocation targets.  

The allocation source establishes which costs must be allocated, and the allocation targets determine where the costs must be allocated. For example, an allocation source can be the costs for the Electricity and Heating cost type. You allocate all electricity and heating costs to three cost centres: Workshop, Production, and Sales. These cost centres are your allocation targets.  

For each allocation source, you define an allocation level, a validity period, and a variant as grouping identifier. You can use a batch job to set filters to select allocation definitions and then run cost allocations automatically.  

For each allocation target, you define an allocation base. The allocation base can be either static or dynamic.  

-   Static allocation bases are based on a definite value, such as square footage or an established allocation ratio, such as 5:2:4.  
-   Dynamic allocation bases depend on changeable values, such as the number of employees in a cost centre or sales revenue of a cost object throughout a certain time period.  

The following table describes a sequence of tasks, with links to the topics that describe them.

|To|See|  
|--------|---------|  
|Set up allocation source and its targets.|[How to: Set Up Allocation Source and Targets](finance-how-to-set-up-allocation-source-and-targets.md)|  
|Set up various filters for dynamic allocation bases.|[Setting Filters for Dynamic Allocation Bases](finance-setting-filters-for-dynamic-allocation-bases.md)|  
|See an example of how to define a static allocation.|[Scenario Example: Defining Static Allocations Based on Allocation Ratio](finance-scenario-example-defining-static-allocations-based-on-allocation-ratio.md)|  
|See an example of how to define a dynamic allocation.|[Scenario Example: Defining Dynamic Allocations Based on Items Sold](finance-scenario-example-defining-dynamic-allocations-based-on-items-sold.md)|  

## <a name="see-also"></a>See Also  
 [Setting Up Cost Accounting](finance-set-up-cost-accounting.md)   
 [Transferring and Posting Cost Entries](finance-transfer-and-post-cost-entries.md)   
 [Accounting for Costs](finance-manage-cost-accounting.md)   
 [Terminology in Cost Accounting](finance-terminology-in-cost-accounting.md)   
 [About Cost Accounting](finance-about-cost-accounting.md)

