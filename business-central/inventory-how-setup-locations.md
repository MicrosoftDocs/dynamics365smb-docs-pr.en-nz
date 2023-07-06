---
title: Set Up a Location Card and Define Transfer Routes (contains video)
description: 'If you buy, store, or sell items in more than one place, you can set up each place as a location.'
author: brentholtorf
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 'warehouse, distribution center'
ms.search.forms: '5703, 15'
ms.date: 03/25/2023
ms.author: bholtorf
---
# <a name="set-up-locations"></a><a name="set-up-locations"></a><a name="set-up-locations"></a>Set Up Locations

Locations are places such as warehouses where you buy, store, or sell items. [!INCLUDE [prod_short](includes/prod_short.md)] uses locations to help keep track of inventory in both simple and complex warehouse processes.

You can then create document lines for a specific location, view availability by location, and transfer inventory between locations. To learn more, go to [Manage Inventory](inventory-manage-inventory.md).
<br><br>  
  
> [!Video https://www.microsoft.com/videoplayer/embed/RE4aQvq?rel=0]

## <a name="location-cards"></a><a name="location-cards"></a><a name="location-cards"></a>Location cards

You specify information about a location, such as a warehouse or distribution centre, on the **Location Card** page. You give each location a name and a code that represents the location. You can then enter the location code in other parts of the program when you want to record transactions for a given location.  

You can enter information about bins and warehouse policies for each location. Based on your warehouse policies, you can use the options on the **Bins** FastTab to specify the bins to use by default for transactions. If you're using directed put-away and pick, the options on the **Bin Policies** FastTab let you define how to use advanced warehousing features.  

Some option fields depend on settings in the **Location Card** page to restrict unsupported setup combinations.  

Choose the **Zones** or **Bins** actions to view information about zones and bins that are defined for the location.

### <a name="to-set-up-a-location"></a><a name="to-set-up-a-location"></a><a name="to-set-up-a-location"></a>To set up a location

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Locations**, and then choose the related link.
2. Choose the **New** action.
3. On the **Location Card** page, fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4. Repeat steps 2 and 3 for every location where you want to keep inventory.

> [!NOTE]  
> Many fields on the Location Card page are related to the handling of items in inbound and outbound warehouse processes. These fields are not relevant for companies that do not require complex warehouse functionality. To learn more, go to [Setting Up Warehouse Management](warehouse-setup-warehouse.md).

You can change the configuration of a location as long as it doesn't have item ledger entries.  

If you have multiple locations, you can define transfer routes between locations. To learn more about transfer routes, go to [To create a transfer route](inventory-how-setup-locations.md#to-create-a-transfer-route).

### <a name="to-create-a-transfer-route"></a><a name="to-create-a-transfer-route"></a><a name="to-create-a-transfer-route"></a>To create a transfer route

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Transfer Routes**, and then choose the related link.
2. Choose the **New** action.
4. On the **Location Card** page, fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

You can now transfer inventory items between two locations. To learn more about transfers, go to [Transfer Inventory Between Locations](inventory-how-transfer-between-locations.md).

## <a name="bins"></a><a name="bins"></a><a name="bins"></a>Bins

Bins represent the basic warehouse structure and can suggest where to put items. Your bins can have contents, or be floating bins without specific contents.

To use the bin functionality at a location, on the **Location Card** page, on the **Warehouse** FastTab, turn on the **Bin Mandatory** toggle. You can design the item flow at the location by specifying bin codes in the fields for the warehouse processes on the **Bins** and **Bin Policies** FastTabs.

> [!NOTE]
> Before you can specify bin codes on a location, you must create bin codes. To learn more about bins, go to [Create Bins](warehouse-how-to-create-individual-bins.md) and [Set Up Bin Types](warehouse-how-to-set-up-bin-types.md).  

## <a name="zones"></a><a name="zones"></a><a name="zones"></a>Zones

If you want to structure your bins under zones, you can do that in the **Zones** page. When you assign a zone to bins, [!INCLUDE [prod_short](includes/prod_short.md)] copies information from the zone to the bins. You can also choose to set up one zone and use bins alone to organise your warehouse. To learn more about zones, go to [Setting Up Warehouse Management](warehouse-setup-warehouse.md).  

## <a name="default-dimensions-for-locations"></a><a name="default-dimensions-for-locations"></a><a name="default-dimensions-for-locations"></a>Default Dimensions for Locations

Dimensions are values that categorise entries so you can track and analyse them using various reporting tools. For example, dimensions can indicate the department or project an entry came from. Having default dimensions helps people avoid making mistakes and having to enter dimensions manually on the transaction level if all goods come from a single location and department.

You set default dimensions for a location on the **Location Card** page by choosing **Dimensions**. Afterward, the location's default dimensions are assigned to the following documents when you choose the location on a line.

* Transfer orders
* Physical inventory orders
* Inventory shipments
* Inventory receipts
* Item journals

If needed, you can delete or change the dimension on the line. In the **Value Posting** field, you can require people to specify dimensions for locations before they can post an entry. If you want to allow people to choose only certain dimension values, you can specify the values in the **Allowed Values Filter** field. You can also include location dimension values on the **Default Dimension Priorities** page, and for combinations of priority and dimension rules on the **Dimension Combinations** page.

Because transfer order documents and reclassification journals deal with more than one location, the order in which you enter data is important. Default dimensions are copied from the last location field (the in-transit location is ignored).

### <a name="example-of-default-dimensions-on-locations"></a><a name="example-of-default-dimensions-on-locations"></a><a name="example-of-default-dimensions-on-locations"></a>Example of default dimensions on locations

The following examples illustrate how the default dimension is used.

You have the following dimension settings:

* Location EAST. Department dimension is ADM
* Location WEST. Department dimension is PROD

You specify the location on a transfer order as follows:

1. From Location = EAST
2. To Location = WEST

The PROD dimension will be copied from location WEST.

You fill in the fields in the opposite order, as follows:

1. To Location = WEST
2. From Location = EAST

The ADM dimension will be copied from location EAST.

## <a name="see-related-training-at-microsoft-learn"></a><a name="see-related-training-at-microsoft-learn"></a><a name="see-related-training-at-microsoft-learn"></a>See related training at [Microsoft Learn](/learn/modules/trade-set-up-dynamics-365-business-central/)

## <a name="see-also"></a><a name="see-also"></a><a name="see-also"></a>See also

[Manage Inventory](inventory-manage-inventory.md)  
[Transfer Inventory Between Locations](inventory-how-transfer-between-locations.md)  
[Create Bins](warehouse-how-to-create-individual-bins.md)  
[Set Up Bin Types](warehouse-how-to-set-up-bin-types.md)  
[Setting Up Warehouse Management](warehouse-setup-warehouse.md)  
[Work with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  
[Change Which Features are Displayed](ui-experiences.md)  
[General Business Functionality](ui-across-business-areas.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
