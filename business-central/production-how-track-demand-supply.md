---
title: How to Track Relations Between Demand and Supply | Microsoft Docs
description: From any supply or demand document in the so-called order network, you can track the order demand (tracked quantity), forecast, blanket sales order, or planning parameter (untracked quantity) that has given rise to the planning line in question.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 25eed1edd8aeb92c875e093a177e59c40d3c3a12
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 12/17/2020
ms.locfileid: "4758946"
---
# <a name="track-relations-between-demand-and-supply"></a>Track Relations Between Demand and Supply
From any supply or demand document in the so-called order network, you can track the order demand (tracked quantity), forecast, blanket sales order, or planning parameter (untracked quantity) that has given rise to the planning line in question.

The planning worksheets also offers supporting planning information about non-order entities to help the planner obtain an optimal supply plan. For more information, see [Untracked Planning Elements](production-how-track-demand-supply.md#untracked-planning-elements).

## <a name="to-track-linked-items"></a>To track linked items
Order tracking shows how sales orders, production orders, and purchase orders are related to the manufacturing order through the planning and reservation systems.

The following describes how to track linked items on a firm planned production order. The steps are similar for all other order types, and from planning worksheet lines.

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Firm Planned Prod. Order**, and then choose the related link.
2. Open the relevant firm planned production order from the list.
3. On the **Lines** FastTab, choose the **Functions** action, and then choose the **Order Tracking** action.

The lines in the **Order Tracking** display the documents that are related to the current production order line.

## <a name="untracked-planning-elements"></a>Untracked Planning Elements
The **Untracked Planning Elements** page opens when you choose the **Untracked Qty.** field on the **order Planning** page. It serves two purposes:

1. To hold information about untracked quantities displayed when the user looks up from the Order Tracking page to see untracked quantities.
2. To hold warning messages displayed when the user chooses the **Warning** icon on the **Planning Worksheet** page.

The page contains entries which account for an untracked surplus quantity in order tracking network. These entries are generated during the planning run and explain where the untracked surplus quantity in the order tracking lines came from. This untracked surplus can come from:

- Production forecast
- Blanket orders
- Safety stock quantity
- Reorder point
- Maximum inventory
- Reorder quantity
- Maximum order quantity
- Minimum order quantity
- Order multiple
- Dampener (% of lot size)

## <a name="see-also"></a>See Also  
[Planning](production-planning.md)   
[Setting Up Manufacturing](production-configure-production-processes.md)  
[Manufacturing](production-manage-manufacturing.md)    
[Inventory](inventory-manage-inventory.md)  
[Purchasing](purchasing-manage-purchasing.md)  
[Design Details: Reservation, Tracking, and Action Messaging](design-details-reservation-order-tracking-and-action-messaging.md)  
[Design Details: Supply Planning](design-details-supply-planning.md)   
[Setup Best Practices: Supply Planning](setup-best-practices-supply-planning.md)  
[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]