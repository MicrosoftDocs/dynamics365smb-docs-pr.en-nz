---
title: How to Batch Post Consumption | Microsoft Docs
description: If the flushing method is **Manual**, you must post the components manually, using a consumption journal.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/06/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: 67d80735f7ea217fa62317283246f098294323da
ms.contentlocale: en-nz
ms.lasthandoff: 01/30/2018

---
# <a name="batch-post-production-consumption"></a>Batch Post Production Consumption
If the flushing method is **Manual**, you must post the components manually, using a consumption journal.

You can also set the system up to automatically post (*flush*) components when you start or finish production orders. For more information, see [Enable Flushing of Components According to Operation Output](production-how-to-flush-components-according-to-operation-output.md).

## <a name="to-post-consumption-for-one-or-more-production-order-lines"></a>To post consumption for one or more production order lines  
1.  Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Consumption Journal**, and then choose the related link.  
2.  Fill in the fields with the production order data and the consumption data. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

    If the warehouse location where the components are stored is set up to use bins but does not require pick processing, assign a bin code to the journal line to indicate where the items should be taken from in the warehouse. For more information, see [Pick for Production or Assembly](warehouse-how-to-pick-for-production.md).  
3.  Choose the **Post** action to post the consumption. The related item ledger entries are reduced.

## <a name="see-also"></a>See Also  
[Manufacturing](production-manage-manufacturing.md)    
[Setting Up Manufacturing](production-configure-production-processes.md)  
[Planning](production-planning.md)      
[Inventory](inventory-manage-inventory.md)  
[Purchasing](purchasing-manage-purchasing.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

