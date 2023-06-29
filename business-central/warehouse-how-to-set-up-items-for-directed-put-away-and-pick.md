---
title: Set Up Directed Put-away and Pick
description: Directed put-away and pick gives you functionality for running your warehouse efficiently.
author: brentholtorf
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: null
ms.search.form: null
ms.date: 11/07/2022
ms.author: bholtorf
---
# <a name="set-up-items-and-locations-for-directed-put-away-and-pick"></a><a name="set-up-items-and-locations-for-directed-put-away-and-pick"></a>Set Up Items and Locations for Directed Put-away and Pick

When you set up a warehouse location for directed put-away and pick, you have new functionality available to you to help run the warehouse in the most efficient way possible. In order to make full use of this functionality, you provide additional information about the items, which in turn helps to make the calculations necessary to suggest the most efficient and effective ways to conduct warehouse activities. 

## <a name="to-set-up-an-item-for-directed-put-away-and-pick"></a><a name="to-set-up-an-item-for-directed-put-away-and-pick"></a>To set up an item for directed put-away and pick

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.  
2. Open the card for the item that you want to set up for directed put-away and pick.
3. On the **Warehouse** FastTab of the item card, fill in the fields to define how the item should be handled in the warehouse.  
4. Choose the **Units of Measurement** action.
5. On the **Item Units of Measure** page, define the units of measure in which the item may be transacted by specifying the item's height, width, length, cubage, and weight.
6. Choose the **Bin Contents** action.
7. On the **Bin Contents** page, define the location and bin to which the item should be associated. The **Default** field is not used when the location is set up for directed put-away and pick.  

## <a name="to-start-using-directed-put-away-and-pick"></a><a name="to-start-using-directed-put-away-and-pick"></a>To start using directed put-away and pick

Directed put-away and pick gives you access to advanced warehouse configuration features that can greatly enhance your efficiency and data reliability. In order to use this functionality, you must first set up a number of parameters in your warehouse location.  

To use the directed put-away and pick functionality, you must activate the functionality on the location card.

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Locations**, and then choose the related link.  
2. Select the location where you want to use directed put-away and pick, and then choose the **Edit** action.  
3. On the **Warehouse** FastTab, select the **Directed Put-away and Pick** checkbox.  

You do not need to fill in any other fields on the location card until later in the setup process.  

> [!NOTE]  
> You can't set up the warehouse to use bins when the location has open item ledger entries.  

The next step is to define the type of bins you want to operate. For more information, see [Set Up Bin Types](warehouse-how-to-set-up-bin-types.md). The bin type defines how to use a given bin when processing the flow of items through the warehouse. You can assign a bin type to both a zone and to a bin.  

You can also define warehouse class codes, if the warehouse carries items that need specific storage conditions. Warehouse class codes are used when suggesting item placement in bins. You assign the warehouse class codes to product groups, which are then assigned to items and SKUs, or to zones and bins that can accommodate the storage conditions required by the warehouse class codes.  

You're now ready to set up zones, if you want. Using zones reduces the number of fields you need to fill in when you set up your bins, because bins created within zones inherit several properties from the zone. Zones can also make it easier for new or temporary employees to orient themselves in your warehouse. Note that flow is controlled by bins, therefore it is possible to operate with bins and only one zone.  

## <a name="to-set-up-a-zone-in-your-warehouse"></a><a name="to-set-up-a-zone-in-your-warehouse"></a>To set up a zone in your warehouse

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Locations**, and then choose the related link.  
2. Select the location where you want to set up zone and open the location card, and then choose the **Zones** action.  
3. On the **Zones** page, fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

When you change a zone parameter, all bins created thereafter in that zone will have the new characteristics, but the original bins will not be changed.  

> [!NOTE]  
> If you want to operate without zones, you must still create one zone code that is undefined except for the code.  

The next step is to define bins. Learn more at [Set Up Locations to Use Bins](warehouse-how-to-set-up-locations-to-use-bins.md).  

In addition, you must create put-away templates and counting periods. Learn more at [Set Up Put-away Templates](warehouse-how-to-set-up-put-away-templates.md).  

## <a name="see-also"></a><a name="see-also"></a>See Also

[Warehouse Management Overview](design-details-warehouse-management.md)
[Inventory](inventory-manage-inventory.md)  
[Setting Up Warehouse Management](warehouse-setup-warehouse.md)     
[Assembly Management](assembly-assemble-items.md)    
[Work with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]
