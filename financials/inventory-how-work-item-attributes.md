---
title: Set Up Item Attributes and Assign Them to Items| Microsoft Docs
description: Describes how to set up item attribute values, for example, that can be used as search words, and assign them to items and item categories.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: categories, search words, facets
ms.date: 06/02/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: 2b29fed7bf976c896b3d663f526d9c3a96200100
ms.contentlocale: en-nz
ms.lasthandoff: 01/30/2018

---
# <a name="work-with-item-attributes"></a>Work with Item Attributes
When customers inquire about an item, either in correspondence or in an integrated web shop, they may ask or search according to characteristics, such as height and model year. To provide this customer service, you can assign item attribute values of different types to your items, which can then be used when searching for items.

You can also assign item attributes to item categories, which then apply to the items that use the item categories. For more information, see [Categorise Item](inventory-how-categorize-items.md).

> [!Tip]  
> If you attach pictures to items, the Image Analyser extension can detect attributes in the image, and suggest the attributes so you can decide whether to assign them. The extension is ready to go. You just need to enable it. For more information, see [The Image Analyser Extension for Microsoft Finance and Operations, Business edition ](ui-extensions-image-analyzer.md).

## <a name="to-create-item-attributes"></a>To create item attributes
1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Item Attributes**, and then choose the related link.
2. In the **Item Attributes** window, choose the **New** action.
3. In the **Item Attribute** window, fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

> [!NOTE]  
>   If you select **Option** in the **Type** field, then you can choose the **Item Attribute Values** action to create values for the item attribute. For more information, see the "To create values for item attributes of type Option" section.  

## <a name="to-create-values-for-item-attributes-of-type-option"></a>To create values for item attributes of type Option
1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Item Attributes**, and then choose the related link.
2. In the **Item Attributes** window, select an item attribute of type **Option** that you want to create values for, and then choose the **Item Attribute Values** action.
3. In the **Item Attribute Values** window, fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="to-assign-item-attributes-to-items"></a>To assign item attributes to items
1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Items**, and then choose the related link.
2. In the **Items** window, select the item that you want to assign item attributes to, and then choose the **Attributes** action.
3. In the **Item Attribute Values** window, choose the **New** action.
4. Choose the lookup button in the **Attribute** field and select an existing item attribute. Alternatively, choose the **New** action to first create a new item attribute as explained in the "To create item attributes" section.
5. In the **Value** field, enter the item attribute value, such as "2010" for the **Model Year** attribute.
6. For item attributes of type **Option**, choose the lookup button in the **Value** field and select an item attribute value. Alternatively, choose the **New** action to first create a new item attribute value as explained in the "To create values for item attributes of type Option" section.
7. Repeat steps 4 through 6 for all item attributes that you want to assign to the item.

## <a name="to-assign-item-attributes-to-item-categories"></a>To assign item attributes to item categories
1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Item Categories**, and then choose the related link.
2. In the **Item Categories** window, select the item category that you want to assign item attributes to, and then choose the **Edit** action.
3. In the **Item Category Card** window, on the **Attributes** FastTab, choose the **New** action.
4. Choose the lookup button in the **Attribute** field and select an existing item attribute. Alternatively, choose the **New** action to first create a new item attribute as explained in the "To create an item attribute" section.
5. In the **Default Value** field, choose the lookup button and select an item attribute value.
6. Repeat steps 4 and 5 for all item attributes that you want to assign to the item category.

> [!NOTE]  
>   Item attributes for parent item categories will be inherited to child item categories. This is indicated by the **Inherited From** field on the **Attributes** FastTab. For more information, see [Categorise Items](inventory-how-categorize-items.md).

## <a name="to-filter-by-item-attributes"></a>To filter by item attributes
1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Items**, and then choose the related link.
2. In the **Items** window, choose the **Filter by Attributes** action.
3. In the **Filter Items by Attribute** window, choose the lookup button in the **Attribute** field and select an item attribute.
4. In the **Value** field, choose the lookup button and select an attribute value to filter items by.

    > [!NOTE]  
>   You can only select values directly for item attributes that have fixed values, such as Colour. For item attributes that have variable values, such as Width, you must specify the item attribute value by first selecting a condition. See step 5.
5. In the **Value** field for a variable item attribute, choose the lookup button.
6. In the **Specify Filter Value** window, in the **Condition** field, choose the drop-down arrow and select a condition.
7. In the **Value** field, enter an attribute value to filter items by.

    **Example**: To filter on items where the material description begins with "blue", fill in the fields as follows: **Attribute** field: Material Description, **Condition** field: Begins With, **Value** field: blue.
8. Choose the **OK** button.   

The items in the **Items** window are filtered by the specified item attribute values.

## <a name="see-also"></a>See Also
[Categorise Items](inventory-how-categorize-items.md)    
[Register New Items](inventory-how-register-new-items.md)  
[Inventory](inventory-manage-inventory.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

