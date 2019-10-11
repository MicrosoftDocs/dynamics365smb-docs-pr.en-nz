---
title: Set Up a Location Card and Define Transfer Routes| Microsoft Docs
description: You create a location card for each place you store inventory items, for example, a warehouse or distribution centre, and set up routes to transfer items between locations.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: warehouse, distribution center
ms.date: 10/01/2019
ms.author: SorenGP
ms.openlocfilehash: 1ad6b8333e13c01a1ed97ebdd9553f0e7fb31297
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 10/01/2019
ms.locfileid: "2309836"
---
# <a name="set-up-locations"></a>Set Up Locations
If you buy, store, or sell items at more than one place or warehouse, you must set each location up with a location card and define transfer routes.

You can then create document lines for a specific location, view availability by location, and transfer inventory between locations. For more information, see [Manage Inventory](inventory-manage-inventory.md).

## <a name="to-create-a-location-card"></a>To create a location card
1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Locations**, and then choose the related link.
2. Choose the **New** action.
3. On the **Location Card** page, fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4. Repeat steps 2 and 3 for every location where you want to keep inventory.

> [!NOTE]  
> Many fields on the location card refer to the handling of items in inbound and outbound warehouse processes. For more information, see [Setting Up Warehouse Management](warehouse-setup-warehouse.md).

## <a name="to-create-a-transfer-route"></a>To create a transfer route
1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Transfer Routes**, and then choose the related link.
2. Alternatively, from any **Location Card** page, choose the **Transfer Routes** action.
3. Choose the **New** action.
4. On the **Location Card** page, fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

You can now transfer inventory items between two locations. For more information, see [Transfer Inventory Between Locations](inventory-how-transfer-between-locations.md).    

## <a name="see-also"></a>See Also
[Manage Inventory](inventory-manage-inventory.md)  
[Transfer Inventory Between Locations](inventory-how-transfer-between-locations.md)    
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  
[Change Which Features are Displayed](ui-experiences.md)  
[General Business Functionality](ui-across-business-areas.md)
