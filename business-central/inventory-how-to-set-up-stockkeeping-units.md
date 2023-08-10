---
title: How to Set Up Stockkeeping Units
description: Use stockkeeping units to record information about your items for a specific location or a specific variant.
author: brentholtorf
ms.author: bholtorf
ms.reviewer: andreipa
ms.topic: how-to
ms.date: 04/19/2023
ms.custom: bap-template
ms.search.forms: '5704, 5700, 5702, 5701'
---

# <a name="set-up-stockkeeping-units"></a>Set Up Stockkeeping Units

Use stockkeeping units (SKUs) to record information about items for a specific location or a variant. They let you add different information about an item for a specific location, for example:

* A warehouse or distribution centre
* Variants, such as different shelf numbers and different replenishment information, for the same item  

## <a name="to-set-up-a-stockkeeping-unit"></a>To set up a stockkeeping unit

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Stockkeeping Units**, and then choose the related link.  
2. Choose the **New** action.  
3. Fill in the fields as necessary. The following fields are required: **Item No.**, **Location Code**, and/or **Variant Code**. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

When you have set up the first stockkeeping unit for an item, the **Stockkeeping Unit Exists** checkbox on the **Item** card is selected.  

To create several stockkeeping units for an item, use the **Create Stockkeeping Unit** batch job. To learn more about batch jobs, go to [Use Job Queues to Schedule Tasks](admin-job-queues-schedule-tasks.md).  

> [!NOTE]  
> The information on the **Stockkeeping Unit** card has priority over the **Item** card.

> [!Warning]
> If the SKU is supplied through production, the **Standard Cost** field isn't used when invoicing and adjusting the actual cost of the produced item. Instead, [!INCLUDE [prod_short](includes/prod_short.md)] uses the value in the **Standard Cost** field on the item card, and variances are calculated against the cost shares of that item.<br><br>
> Although you can assign production BOMs and routings to SKUs, the unit cost roll-up and the related calculation of cost shares aren't available on SKUs. To learn more about standard costs, go to [About Calculating Standard Cost](finance-about-calculating-standard-cost.md)

## <a name="see-related-microsoft-training"></a>See related [Microsoft training](/training/modules/control-inventory-multiple-locations/)

## <a name="see-also"></a>See also

[Register New Items](inventory-how-register-new-items.md)  
[Setting Up Warehouse Management](warehouse-setup-warehouse.md)  
[Warehouse Management Overview](design-details-warehouse-management.md)
[Inventory](inventory-manage-inventory.md)  
[Assembly Management](assembly-assemble-items.md)    
[Work with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
