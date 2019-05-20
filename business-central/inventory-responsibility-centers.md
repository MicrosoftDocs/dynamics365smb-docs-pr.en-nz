---
title: How to Work with Responsibility Centres | Microsoft Docs
description: Responsibility centres providing the ability to handle administrative centres. A responsibility centre can be a cost centre, a profit centre, an investment centre, or other company-defined administrative centre.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2019
ms.author: sgroespe
ms.openlocfilehash: ee54a60705a3dff4313522500e9457243ea4907d
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 04/29/2019
ms.locfileid: "1244002"
---
# <a name="work-with-responsibility-centers"></a>Work with Responsibility Centres
Responsibility centres provide the ability to handle administrative centres. A responsibility centre can be a cost centre, a profit centre, an investment centre, or other company-defined administrative centre. Examples of responsibility centres are a sales office, a purchasing department for several locations, and a plant planning office. Using this functionality, for example, companies can set up user-specific views of sales and purchase documents related exclusively to a particular responsibility centre.  

Using multiple locations together with responsibility centres provides the ability to manage business operations in the most flexible, yet optimal way.

Multiple locations allows companies to manage their inventory in multiple locations using one database. Two concepts, locations and stockkeeping units, are the cornerstones of this granule. A location is defined as a place that handles physical placement and quantities of items. The concept is broad enough to include locations such as plants or production facilities as well as distribution centres, warehouses, showrooms and service vehicles. A stockkeeping unit is defined as an item at a specific location and/or as a variant. Using stockkeeping units, companies with multiple locations are able to add replenishment information, addresses, and some financial posting information at the location level. As a result, they have the ability to replenish variants of the same item for each location as well as to order items for each location on the basis of location-specific replenishment information.  

Responsibility centres extends the multiple locations functionality by providing users the ability to handle administrative centres. A responsibility centre can be a cost centre, a profit centre, an investment centre, or other company-defined administrative centre. Examples of responsibility centres are a sales office, a purchasing department for several locations, and a plant planning office. Using this functionality, for example, companies can set up user-specific views of sales and purchase documents related exclusively to a particular responsibility centre.

## <a name="to-set-up-a-responsibility-center"></a>To set up a responsibility centre  
1.  Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Responsibility Centres**, and then choose the related link.  
2.  Choose the **New** action.  
3.  Fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

    If you are using responsibility centres to administer your company, it can be useful to have a default responsibility centre for your company.
4. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Company Information**, and then choose the related link.
5. In the **Responsibility Centre** field, enter a responsibility centre code.

This code will be used on all purchase, sales, or service documents, if the user, customer, or vendor has no default responsibility centre. On any sales, purchase, or service document, you can enter another responsibility centre than the default.

> [!NOTE]  
>  When you enter a responsibility centre code on a document, it affects the address, dimensions, and prices on the document.  

## <a name="to-assign-responsibility-centers-to-users"></a>To assign responsibility centres to users  
You can set up users so that in their daily routines the program retrieves only the documents relevant for their particular work areas. Users are usually associated with one responsibility centre and work only with documents related to specific application areas at that particular centre.  

To set this up, you assign responsibility centres to users in three functional areas: Purchases, Sales, and Service Management.  

1.  Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **User Setup**, and then choose the related link.  
2.  On the **User Setup** page, select the user you want to assign a responsibility centre to. If the user not is on the list, you must enter a user ID in the **User ID** field.  
3.  In the **Sales Resp. Ctr. Filter** field, enter the responsibility centre where the user will have tasks related to sales.  
4.  In the **Purchase Resp. Ctr. Filter** field, enter the responsibility centre where the user will have tasks related to purchasing.  
5.  In the **Service Resp. Ctr. Filter** field, enter the responsibility centre where the user will have tasks related to service management.  

> [!NOTE]  
>  Users will still be able to view all posted documents and ledger entries, not just those related to their own responsibility centre.

## <a name="see-also"></a>See Also  
[Setting Up Inventory](inventory-setup-inventory.md)  
[Setting Up Warehouse Management](warehouse-setup-warehouse.md)
[Inventory](inventory-manage-inventory.md)[Warehouse Management](warehouse-manage-warehouse.md)  
[Warehouse Management](warehouse-manage-warehouse.md)    
[Design Details: Warehouse Management](design-details-warehouse-management.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
