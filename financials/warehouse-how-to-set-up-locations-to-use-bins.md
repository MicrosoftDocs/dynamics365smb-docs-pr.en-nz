---
title: How to Set Up Locations to Use Bins | Microsoft Docs
description: Bins represent the basic warehouse structure and are used to make suggestions about the placement of items. When you have created your bins, you can define very specifically the contents that you want to place in each bin, or the bin can function as a floating bin without specified contents.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/23/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: 2d84f1222dccca86f5906af1c82fc0e6192173d6
ms.contentlocale: en-nz
ms.lasthandoff: 01/30/2018

---
# <a name="set-up-locations-to-use-bins"></a>Set Up Locations to Use Bins
Bins represent the basic warehouse structure and are used to make suggestions about the placement of items. When you have created your bins, you can define very specifically the contents that you want to place in each bin, or the bin can function as a floating bin without specified contents.  

To use the bin functionality at a location, you first activate the functionality on the **Location** card. Then you design the item flow at the location by specifying bin codes in setup fields that represent the different flows.  

> [!NOTE]  
>  Before you can specify bin codes on the location card, the bin codes must be created. For more information, see [Create Bins](warehouse-how-to-create-individual-bins.md).  

## <a name="to-set-up-a-location-to-use-bins"></a>To set up a location to use bins  
1.  Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Locations**, and then choose the related link.  
2.  Select the location where you want to use bins.  
3.  Choose the **Edit** action.  
4.  On the **Warehouse** FastTab, select the **Bin Mandatory** check box.  
5.  If you are not using directed put-away and pick for the location, fill in the **Default Bin Selection** field with the method the system should use when assigning a default bin to an item.  
6.  Open the card for the location that you want to set up bins for.
7.  On the **Bins** FastTab, select the bins that you want to use as the default for receipts, shipments, inbound, outbound, and open shop floor bins.  
8.  The bin codes you fill in here will appear automatically on the headers and on the lines of various warehouse documents. The default bins define all starting or ending placements of items in the warehouse.  
9.  If you are using directed put-away and pick, select a bin for your warehouse adjustments. The bin code in the **Adjustment Bin Code** field defines the virtual bin in which to record discrepancies in inventory when you register either observed differences registered in the warehouse item journal, or differences calculated when you register a warehouse physical inventory.  
10. Fill in the fields on the **Bin Policies** FastTab if they are relevant to your warehouse. The most important fields are **Bin Capacity Policy**, **Allow Breakbulk**, and **Put-away Template Code** fields.  
11. On the **Warehouse** FastTab, fill in the **Outbound Whse. Handling Time**, **Inbound Whse. Handling Time**, and the **Base Calendar Code** fields. For more information, see [Set Up Base Calendars](across-how-to-assign-base-calendars.md).

## <a name="filling-the-consumption-bin"></a>Filling the Consumption Bin
This flow chart shows how the **Bin Code** field on production order component lines is filled according to your location setup.

![Bin flow chart](media/binflow.png "BinFlow")  

## <a name="see-also"></a>See Also
[Warehouse Management](warehouse-manage-warehouse.md)  
[Inventory](inventory-manage-inventory.md)  
[Setting Up Warehouse Management](warehouse-setup-warehouse.md)     
[Assembly Management](assembly-assemble-items.md)    
[Design Details: Warehouse Management](design-details-warehouse-management.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

