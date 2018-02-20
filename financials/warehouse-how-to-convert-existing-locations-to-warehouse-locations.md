---
title: How to Convert Existing Locations to Warehouse Locations | Microsoft Docs
description: You can enable an existing inventory location to use zones and bins and to operate as a warehouse location.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: 7d4b2c86174386faa86ab6c09faa463d26d3d2ac
ms.contentlocale: en-nz
ms.lasthandoff: 01/30/2018

---
# <a name="convert-existing-locations-to-warehouse-locations"></a>Convert Existing Locations to Warehouse Locations
You can enable an existing inventory location to use zones and bins and to operate as a warehouse location.  

The batch job to enable a location for warehouse operation creates initial warehouse entries for the warehouse adjustment bin for all items that have inventory in the location. These initial entries will be balanced when warehouse physical inventory entries are entered after the batch job is run.  

You can create zones and bins either before or after the conversion. The only bin that you must create before the conversion is the one that is to be used as the future adjustment bin.  

> [!IMPORTANT]  
>  To clear all negative inventory and any open warehouse documents before you convert the location for warehouse handling, run a report to identify the items with negative inventory and open warehouse documents for the location. For more information, see Check on Negative Inventory.  

## <a name="to-enable-an-existing-location-to-operate-as-a-warehouse-location"></a>To enable an existing location to operate as a warehouse location  
1.  Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Create Warehouse Location**, and then choose the related link.  
2.  In the **Location Code** field, specify the location that you want to enable for warehouse processing.  
3.  In the **Adjustment Bin Code** field, specify the bin at the location where unsynchronised warehouse entries are stored. For more information, see the "To synchronise the adjusted warehouse entries with the related item ledger entries" section in [Count, Adjust, and Reclassify Inventory](inventory-how-count-adjust-reclassify.md).  

    Using the open item ledger entries for the specified location, warehouse journal lines are created that sum up every combination of Item No., Variant Code, Unit of Measure Code, and, if necessary, Lot No. and Serial No. in the item ledger entries. The warehouse journal lines are then posted. This posting creates warehouse entries that place the inventory in the warehouse adjustment bin. The **Adjustment Bin Code** on the location card is also set.  

4.  To see which items were added to the adjustment bin during the batch job, run the **Warehouse Adjustment Bin** report.  
5.  When the **Create Warehouse Location** batch job has completed, perform and post a warehouse physical inventory. For more information, see [Count, Adjust, and Reclassify Inventory](inventory-how-count-adjust-reclassify.md).  

> [!NOTE]  
>  It is recommended that you run the **Create Warehouse Location** batch job at a time when it will not impact the daily work in the system. This job processes each entry in the **Item Ledger Entry** table, and if there are a large number of item ledger entries, the job can last several hours.  

 For those locations that did not use warehouse management documents before the conversion, you must re-open and release any source documents that were partially received or partially shipped before the conversion.  

## <a name="see-also"></a>See Also  
[Warehouse Management](warehouse-manage-warehouse.md)  
[Inventory](inventory-manage-inventory.md)  
[Setting Up Warehouse Management](warehouse-setup-warehouse.md)     
[Assembly Management](assembly-assemble-items.md)    
[Design Details: Warehouse Management](design-details-warehouse-management.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

