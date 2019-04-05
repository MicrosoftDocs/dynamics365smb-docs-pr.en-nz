---
title: Design Details - Staying Under the Overflow Level | Microsoft Docs
description: When using Maximum Qty. and Fixed Reorder Qty., the planning system focuses on the projected inventory in the given time-bucket only. This means that the planning system may suggest superfluous supply when negative demand or positive supply changes occur outside of the given time bucket.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2018
ms.author: sgroespe
redirect_url: design-details-handling-reordering-policies
ms.openlocfilehash: a4a35cec571f1a0c7644fe937553d87007a9567e
ms.sourcegitcommit: 1bcfaa99ea302e6b84b8361ca02730b135557fc1
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 03/08/2019
ms.locfileid: "822496"
---
# <a name="design-details-staying-under-the-overflow-level"></a>Design Details: Staying under the Overflow Level
When using the Maximum Qty. and Fixed Reorder Qty. policies, the planning system focuses on the projected inventory in the given time-bucket only. This means that the planning system may suggest superfluous supply when negative demand or positive supply changes occur outside of the given time bucket. If, for this reason, a superfluous supply is suggested, the planning system calculates which quantity the supply should be decreased to (or deleted) to avoid the superfluous supply. This quantity is called the “overflow level.” The overflow is communicated as a planning line with a **Change Qty. (Decrease)** or **Cancel** action and the following warning message:  

*Attention: The projected inventory [xx] is higher than the overflow level [xx] on the Due Date [xx].*  

![Inventory overflow level](media/supplyplanning_2_overflow1_new.png "Inventory overflow level")  

##  <a name="calculating-the-overflow-level"></a>Calculating the Overflow Level  
The overflow level is calculated in different ways depending on planning setup.  

### <a name="maximum-qty-reordering-policy"></a>Maximum Qty. reordering policy  
Overflow level = Maximum Inventory  

> [!NOTE]  
>  If a minimum order quantity exists, then it will be added as follows: Overflow level = Maximum Inventory + Minimum Order Quantity.  

### <a name="fixed-reorder-qty-reordering-policy"></a>Fixed Reorder Qty. reordering policy  
Overflow level = Reorder Quantity + Reorder Point  

> [!NOTE]  
>  If the minimum order quantity is higher than the reorder point, then it will replace as follows: Overflow Level = Reorder Quantity + Minimum Order Quantity  

### <a name="order-multiple"></a>Order Multiple  
If an order multiple exists, then it will adjust the overflow level for both Maximum Qty. and Fixed Reorder Qty. reordering policies.  

##  <a name="creating-the-planning-line-with-overflow-warning"></a>Creating the Planning Line with Overflow Warning  
When an existing supply causes the projected inventory to be higher than the overflow level at the end of a time bucket, a planning line is created. To warn about the potential superfluous supply, the planning line has a warning message, the **Accept Action Message** field is not selected, and the action message is either Cancel or Change Qty.  

### <a name="calculating-the-planning-line-quantity"></a>Calculating the Planning Line Quantity  
Planning Line Quantity = Current Supply Quantity – (Projected Inventory – Overflow Level)  

> [!NOTE]  
>  As with all warning lines, any maximum/minimum order quantity or order multiple will be ignored.  

### <a name="defining-the-action-message-type"></a>Defining the Action Message Type  

-   If the planning line quantity is higher than 0, then the action message is Change Qty.  
-   If the planning line quantity is equal to or lower than 0, then the action message is Cancel  

### <a name="composing-the-warning-message"></a>Composing the Warning Message  
In case of overflow, the **Untracked Planning Elements** page displays a warning message with the following information:  

-   The projected inventory level that triggered the warning  
-   The calculated overflow level  
-   The due date of the supply event.  

Example: “The projected inventory 120 is higher than the overflow level 60 on 28-01-11”  

## <a name="scenario"></a>Scenario  
In this scenario, a customer changes a sales order from 70 to 40 pieces between two planning runs. The overflow feature sets in to reduce the purchase that was suggested for the initial sales quantity.  

### <a name="item-setup"></a>Item setup  

|Reordering Policy|Maximum Qty.|  
|-----------------------|------------------|  
|Maximum Order Quantity|100|  
|Reorder Point|50|  
|Inventory|80|  

### <a name="situation-before-sales-decrease"></a>Situation before sales decrease  

|Event|Change Qty.|Projected Inventory|  
|-----------|-----------------|-------------------------|  
|Day one|None|80|  
|Sale|-70|10|  
|End of time bucket|None|10|  
|Suggest new purchase order|+90|100|  

### <a name="situation-after-sales-decrease"></a>Situation after sales decrease  

|Change|Change Qty.|Projected Inventory|  
|------------|-----------------|-------------------------|  
|Day one|None|80|  
|Sale|-40|40|  
|Purchase|+90|130|  
|End of time bucket|None|130|  
|Suggest to decrease purchase<br /><br /> order from 90 to 60|-30|100|  

### <a name="resulting-planning-lines"></a>Resulting Planning Lines  
 One planning line (warning) is created to reduce the purchase with 30 from 90 to 60 to keep the projected inventory on 100 according to the overflow level.  

![Plan according to overflow level](media/nav_app_supply_planning_2_overflow2.png "Plan according to overflow level")  

> [!NOTE]  
>  Without the Overflow feature, no warning is created if the projected inventory level is above maximum inventory. This could cause a superfluous supply of 30.  

## <a name="see-also"></a>See Also  
[Design Details: Reordering Policies](design-details-reordering-policies.md)   
[Design Details: Planning Parameters](design-details-planning-parameters.md)   
[Design Details: Handling Reordering Policies](design-details-handling-reordering-policies.md)   
[Design Details: Supply Planning](design-details-supply-planning.md)
