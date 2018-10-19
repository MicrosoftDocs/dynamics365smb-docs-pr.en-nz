---
title: Set Up Inventory Valuation and Costing | Microsoft Docs
description: The following table describes a sequence of tasks, with links to the topics that describe them.
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
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: 296f660f2ca4dfe7a605d2990e18567c5062a482
ms.contentlocale: en-nz
ms.lasthandoff: 09/28/2018

---
# <a name="setting-up-inventory-valuation-and-costing"></a>Setting Up Inventory Valuation and Costing
To make sure that inventory costs are recorded correctly, you must set up various fields and windows before you begin to make item transactions.

The following table describes a sequence of tasks, with links to the topics that describe them.

|**To**|**See**|  
|------------|-------------|  
|Set a costing method for each item to govern how its incoming cost is used to assess inventory value and the cost of goods sold.|[Register New Items](inventory-how-register-new-items.md)|  
|Ensure that the cost is automatically posted to the general ledger whenever an inventory transaction is posted.|**Automatic Cost Posting** field in the **Inventory Setup** window|  
|Ensure that expected costs are posted to the general ledger to see from the interim G/L accounts an estimate of the amounts due and the cost of the traded items before they are actually invoiced.|**Expected Cost Posting to G/L** field in the **Inventory Setup** window|  
|Set the system up to adjust for any cost changes automatically every time you post inventory transactions.|[Adjust Item Costs](inventory-how-adjust-item-costs.md)|  
|Define if the average cost is to be calculated per item only or per item for each stockkeping unit and for each variant of the item.|**Average Cost Calc. Type** field in the **Inventory Setup** window|  
|Select the period of time you would like the program to use for calculating the weighted average cost of items that use the average costing method.|**Average Cost Period** field in the **Inventory Setup** window|  
|Define inventory periods to control inventory value over time by disallowing transaction posting in closed inventory periods.|[Work with Inventory Periods](finance-how-to-work-with-inventory-periods.md)|  
|Ensure that sales returns are applied to the original outbound transaction to preserve inventory value.|**Exact Cost Reversing Mandatory** field in the **Sales & Receivables** window|  
|Ensure that purchase returns are applied to the original inbound transaction to preserve inventory value.|**Exact Cost Reversing Mandatory** field in the **´Purchases & Payables** window|
|Set up the rounding rules to apply when adjusting or suggesting item prices and when adjusting or suggesting standard costs.|**Rounding Method** window|  

## <a name="see-also"></a>See Also  
[Managing Inventory Costs](finance-manage-inventory-costs.md)  
[Working with Business Central](ui-work-product.md)  
[Finance](finance.md)  

