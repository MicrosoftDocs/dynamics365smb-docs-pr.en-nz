---
title: How to Work with Responsibility Centres
description: Responsibility centre as administrative centres help companies set up user-specific views of sales and purchase documents related exclusively to each centre.
author: brentholtorf
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: null
ms.search.forms: '5714, 5715'
ms.date: 03/09/2023
ms.author: bholtorf
---
# <a name="work-with-responsibility-centers" />Work with Responsibility Centres

Responsibility centres provide the ability to handle administrative centres. A responsibility centre can be a cost centre, a profit centre, an investment centre, or other company-defined administrative centre. Examples of responsibility centres are a sales office, a purchasing department for several locations, and a plant planning office. For example, companies can set up user-specific views of sales and purchase documents related to a particular responsibility centre.  

Using multiple locations together with responsibility centres provides the ability to manage business operations in flexible, optimal ways.

Multiple locations allows companies to manage their inventory in multiple locations using one database. Two concepts, locations and stockkeeping units, are the cornerstones of this granule. A location is defined as a place that handles physical placement and quantities of items. The concept is broad enough to include locations such as plants or production facilities as well as distribution centres, warehouses, showrooms and service vehicles. A stockkeeping unit is defined as an item at a specific location and/or as a variant. Using stockkeeping units, companies with multiple locations can add replenishment information, addresses, and some financial posting information at the location level. As a result, they can replenish variants of the same item for each location and order items on the basis of location-specific replenishment information.  

## <a name="to-set-up-a-responsibility-center" />To set up a responsibility centre

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Responsibility Centres**, and then choose the related link.  
2. Choose the **New** action.  
3. Fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

    If you're using responsibility centres to administer your company, it can be useful to have a default responsibility centre.
4. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Company Information**, and then choose the related link.
5. In the **Responsibility Centre** field, enter a responsibility centre code.

This code is used on all purchase, sales, or service documents, if the user, customer, or vendor has no default responsibility centre. On sales, purchase, or service documents, you can enter another responsibility centre than the default.

> [!NOTE]  
> When you enter a responsibility centre code on a document, it affects the address, dimensions, and prices on the document.  

## <a name="to-assign-responsibility-centers-to-users" />To assign responsibility centres to users

You can set up users so that [!INCLUDE [prod_short](includes/prod_short.md)] retrieves only the documents relevant for their particular work areas. Users are usually associated with one responsibility centre and work only with documents related to specific application areas at that particular centre.  

To set this up, you assign responsibility centres to users in three functional areas: Purchases, Sales, and Service Management.  

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **User Setup**, and then choose the related link.  
2. On the **User Setup** page, select the user you want to assign a responsibility centre to. If the user not is on the list, you must enter a user ID in the **User ID** field.  
3. In the **Sales Resp. Ctr. Filter** field, enter the responsibility centre where the user will have tasks related to sales.  
4. In the **Purchase Resp. Ctr. Filter** field, enter the responsibility centre where the user will have tasks related to purchasing.  
5. In the **Service Resp. Ctr. Filter** field, enter the responsibility centre where the user will have tasks related to service management.  

> [!NOTE]  
> Users can view only those posted documents that related to their own responsibility centre. However, they can view all ledger entries and navigate to other posted documents from the ledger entries.

## <a name="see-related-microsoft-training" />See related [Microsoft training](/training/modules/set-up-responsibility-centers/)

## <a name="see-also" />See also

[Setting Up Inventory](inventory-setup-inventory.md)  
[Setting Up Warehouse Management](warehouse-setup-warehouse.md)  
[Inventory](inventory-manage-inventory.md)  
[Warehouse Management Overview](design-details-warehouse-management.md)
[Work with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  
[Define an invoice posting policy for users](admin-setup-invoice-posting-policy.md)

[!INCLUDE[footer-include](includes/footer-banner.md)]
