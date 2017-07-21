---
title: Organise Items in Categories| Microsoft Docs
description: To help you search for and find items, you can assign item attributes and organise items in categories.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: category, search, attribute, facet
ms.date: 06/02/2017
ms.author: sgroespe
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: da87c427033d58d92a6a5222bc323c68c4bc3f4e
ms.contentlocale: en-nz
ms.lasthandoff: 07/07/2017


---
# <a name="how-to-categorize-items"></a>How to: Categorise Items
To maintain an overview of your items and to help you sort and find items, it is useful to organise your items in item categories.

To find items by characteristics, you can assign item attributes to items and also to item categories. For more information, see [How to: Work with Item Attributes](inventory-how-work-item-attributes.md).

## <a name="to-create-an-item-category"></a>To create an item category
1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Item Categories**, and then choose the related link.
2. In the **Item Categories** window, choose the **New** action.
3. In the **Item Category Card** window, on the **General** FastTab, fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4. On the **Attributes** FastTab, specify any item attributes for the item category. For more information, see the "To assign item attributes to an item category" section in [How to: Work with Item Attributes](inventory-how-work-item-attributes.md).

> [!NOTE]  
>   If the item category has a parent item category, as indicated by the **Parent Category** field, then any item attributes that are assigned to that parent item category are prefilled on the **Attributes** FastTab.

> [!NOTE]  
>   Item attributes that you assign to an item category will automatically apply to the item that the item category is assigned to.

## <a name="to-assign-an-item-category-to-an-item"></a>To assign an item category to an item
1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Items**, and then choose the related link.
2. Open the card for the item that you want to assign to an item category.
3. Choose the lookup button in the **Item Category Code** field and select an existing item category. Alternatively, choose the **New** action to first create a new item category as explained in the "To create an item category" section.

## <a name="see-also"></a>See Also
[How to: Work with Item Attributes](inventory-how-work-item-attributes.md)  
[How to: Register New Items](inventory-how-register-new-items.md)  
[Inventory](inventory-manage-inventory.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

