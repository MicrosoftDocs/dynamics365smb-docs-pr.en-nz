---
title: Set Up a Location Card and Define Transfer Routes| Microsoft Docs
description: You create a location card for each place you store inventory items, for example, a warehouse or distribution centre, and set up routes to transfer items between locations.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: warehouse, distribution center
ms.date: 06/02/2017
ms.author: SorenGP
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 7d82b1c63bb1da367736f8dd044640b583493af8
ms.contentlocale: en-nz
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-set-up-locations"></a>How to: Set Up Locations
If you buy, store, or sell items at more than one place or warehouse, you must set each location up with a location card and define transfer routes.

You can then create document lines for a specific location, view availability by location, and transfer inventory between locations. For more information, see [Manage Inventory](inventory-manage-inventory.md).

> [!NOTE]  
>   This functionality requires that your experience is set to **Suite**. For more information, see [Customizing Your [!INCLUDE[d365fin](includes/d365fin_md.md)] Experience](ui-experiences.md).

## <a name="to-create-a-location-card"></a>To create a location card
1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Locations**, and then choose the related link.
2. Choose the **New** action.
3. In the **Location Card** window, fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4. Repeat steps 2 and 3 for every location where you want to keep inventory.

> [!NOTE]  
> Many fields on the location card refer to the handling of items in inbound and outbound warehouse processes. For more information, see [Setting Up Warehouse Management](warehouse-setup-warehouse.md). 

## <a name="to-create-a-transfer-route"></a>To create a transfer route
1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Transfer Routes**, and then choose the related link.
2. Alternatively, from any **Location Card** window, choose the **Transfer Routes** action.
3. Choose the **New** action.
4. In the **Location Card** window, fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

You can now transfer inventory items between two locations. For more information, see [How to: Transfer Inventory Between Locations](inventory-how-transfer-between-locations.md).    

## <a name="see-also"></a>See Also
[Manage Inventory](inventory-manage-inventory.md)  
[How to: Transfer Inventory Between Locations](inventory-how-transfer-between-locations.md)    
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  
[Customizing Your [!INCLUDE[d365fin](includes/d365fin_md.md)] Experience](ui-experiences.md)  
[General Business Functionality](ui-across-business-areas.md)

