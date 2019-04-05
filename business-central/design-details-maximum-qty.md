---
title: Design Details - Maximum Qty. | Microsoft Docs
description: The Maximum Quantity policy is a way to maintain inventory using a reorder point.
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
ms.openlocfilehash: 21ae51ecf28458f9b09be6461243f31641a0aaef
ms.sourcegitcommit: 1bcfaa99ea302e6b84b8361ca02730b135557fc1
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 03/08/2019
ms.locfileid: "821938"
---
# <a name="design-details-maximum-qty"></a>Design Details: Maximum Qty.
The Maximum Quantity policy is a way to maintain inventory using a reorder point.  

 Everything regarding the Fixed Reorder Qty. policy also applies to this policy. The only difference is the quantity of the suggested supply. When using the maximum quantity policy, the reorder quantity will be defined dynamically based on the projected inventory level and will therefore usually differ from order to order.  

## <a name="calculated-per-time-bucket"></a>Calculated per Time Bucket  
 The reorder quantity is determined at the point of time (the end of a time bucket) when the planning system detects that the reorder point has been crossed. At this time, the system measures the gap from the current projected inventory level up to the specified maximum inventory. This constitutes the quantity that should be reordered. The system then checks if supply has already been ordered elsewhere to be received within the lead time and, if so, reduces the quantity of the new supply order by already ordered quantities.  

 The system will ensure that the projected inventory at least reaches the reorder point level – in case the user has forgotten to specify a maximum inventory quantity.  

## <a name="combines-with-order-modifiers"></a>Combines with Order Modifiers  
 Depending on the setup, it may be best to combine the Maximum Quantity policy with order modifiers to ensure a minimum order quantity or round it to an integer number of purchase units of measure, or split it into more lots as defined by the maximum order quantity.  

## <a name="combines-with-calendars"></a>Combines with Calendars  
 Before suggesting a new supply order to meet a reorder point, the planning system checks if the order is scheduled for a non-working day, according to any calendars that are defined in the **Base Calendar Code** field in the **Company Information** and **Location Card** pages.  

 If the scheduled date is a non-working day, the planning system moves the order forward to the nearest working date. This may result in an order that meets a reorder point but does not meet some specific demand. For such unbalanced demand, the planning system creates an extra supply.  

## <a name="see-also"></a>See Also  
 [Design Details: Reordering Policies](design-details-reordering-policies.md)   
 [Design Details: Planning Parameters](design-details-planning-parameters.md)   
 [Design Details: Handling Reordering Policies](design-details-handling-reordering-policies.md)   
 [Design Details: Supply Planning](design-details-supply-planning.md)
