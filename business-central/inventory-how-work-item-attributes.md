---
title: Set Up Item Attributes and Assign Them to Items
description: 'Describes how to set up item attribute values, for example, that can be used as search words, and assign them to items and item categories.'
author: SorenGP
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 'categories, search words, facets'
ms.search.forms: '7507, 7509, 7506, 7505, 7503, 7502, 7510, 7504, 7501, 7500, 9110, 5734, 7508'
ms.date: 04/01/2021
ms.author: edupont
---
# <a name="work-with-item-attributes"></a><a name="work-with-item-attributes"></a>Work with item attributes

When customers inquire about an item, either in correspondence or in an integrated web shop, they may ask or search according to characteristics, such as height and model year. To provide this customer service, you can assign item attribute values of different types to your items, which can then be used when searching for items.

You can also assign item attributes to item categories, which then apply to the items that use the item categories. For more information, see [Categorise Item](inventory-how-categorize-items.md).

> [!TIP]  
> If you attach pictures to items, the Image Analyser extension can detect attributes in the image, and suggest the attributes so you can decide whether to assign them. The extension is ready to go. You just need to enable it. For more information, see [The Image Analyser Extension](ui-extensions-image-analyzer.md).

## <a name="create-item-attributes"></a><a name="create-item-attributes"></a>Create item attributes

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Item Attributes**, and then choose the related link.
2. On the **Item Attributes** page, choose the **New** action.
3. On the **Item Attribute** page, fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

> [!NOTE]  
> If you select **Option** in the **Type** field you can choose the **Item Attribute Values** action to create values for the item attribute. For more information, see [To create values for item attributes of type Option](inventory-how-work-item-attributes.md#to-create-values-for-item-attributes-of-type-option).  

## <a name="create-values-for-item-attributes-of-type-option"></a><a name="create-values-for-item-attributes-of-type-option"></a>Create values for item attributes of type Option

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Item Attributes**, and then choose the related link.
2. On the **Item Attributes** page, select an item attribute of type **Option** that you want to create values for, and then choose the **Item Attribute Values** action.
3. On the **Item Attribute Values** page, fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="assign-item-attributes-to-items"></a><a name="assign-item-attributes-to-items"></a>Assign item attributes to items

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.
2. On the **Items** page, select the item that you want to assign item attributes to, and then choose the **Attributes** action.
3. On the **Item Attribute Values** page, choose the **New** action.
4. Choose the lookup button in the **Attribute** field and select an existing item attribute. Alternatively, choose the **New** action to first create a new item attribute as explained in [To create item attributes](inventory-how-work-item-attributes.md#to-create-item-attributes).
5. In the **Value** field, enter the item attribute value, such as "2010" for the **Model Year** attribute.
6. For item attributes of type **Option**, choose the lookup button in the **Value** field and select an item attribute value. Alternatively, choose the **New** action to first create a new item attribute value as explained in [To create values for item attributes of type Option](inventory-how-work-item-attributes.md#to-assign-item-attributes-to-items).
7. Repeat steps 4 through 6 for all item attributes that you want to assign to the item.

## <a name="assign-item-attributes-to-item-categories"></a><a name="assign-item-attributes-to-item-categories"></a>Assign item attributes to item categories

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Item Categories**, and then choose the related link.
2. On the **Item Categories** page, select the item category that you want to assign item attributes to, and then choose the **Edit** action.
3. On the **Item Category Card** page, on the **Attributes** FastTab, choose the **New** action.
4. Choose the lookup button in the **Attribute** field and select an existing item attribute. Alternatively, choose the **New** action to first create a new item attribute as explained in [To create item attributes](inventory-how-work-item-attributes.md#to-create-item-attributes).
5. In the **Default Value** field, choose the lookup button and select an item attribute value.
6. Repeat steps 4 and 5 for all item attributes that you want to assign to the item category.

> [!NOTE]  
> Item attributes for parent item categories will be inherited to child item categories. This is indicated by the **Inherited From** field on the **Attributes** FastTab. For more information, see [Categorise Items](inventory-how-categorize-items.md).

## <a name="filter-by-item-attributes"></a><a name="filter-by-item-attributes"></a>Filter by item attributes

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.
2. On the **Items** page, choose the **Filter by Attributes** action.
3. On the **Filter Items by Attribute** page, choose the lookup button in the **Attribute** field and select an item attribute.
4. In the **Value** field, choose the lookup button and select an attribute value to filter items by.

    > [!NOTE]  
    > You can only select values directly for item attributes that have fixed values, such as Colour. For item attributes that have variable values, such as Width, you must specify the item attribute value by first selecting a condition. See step 5.
5. In the **Value** field for a variable item attribute, choose the lookup button.
6. On the **Specify Filter Value** page, in the **Condition** field, choose the drop-down arrow and select a condition.
7. In the **Value** field, enter an attribute value to filter items by.

    **Example**: To filter on items where the material description begins with "blue", fill in the fields as follows: **Attribute** field: Material Description, **Condition** field: Begins With, **Value** field: blue.
8. Choose the **OK** button.

The items on the **Items** page are filtered by the specified item attribute values.

## <a name="see-related-microsoft-training"></a><a name="see-related-microsoft-training"></a>See related [Microsoft training](/training/modules/trade-master-data-dynamics-365-business-central/)

## <a name="see-also"></a><a name="see-also"></a>See also

[Categorise Items](inventory-how-categorize-items.md)  
[Register New Items](inventory-how-register-new-items.md)  
[Inventory](inventory-manage-inventory.md)  
[Work with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]
