---
title: Set Up Warehouse Employees
description: Each user who performs warehouse activities must be set up as a warehouse employee assigned to one default location and potentially more non-default locations.
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bholtorf
ms.topic: how-to
ms.date: 03/09/2023
ms.custom: bap-template
ms.search.form: '7328, 7348'
---
# <a name="set-up-warehouse-employees"></a>Set Up Warehouse Employees

Each user who performs warehouse activities must be set up as a warehouse employee and assigned to a default location. [!INCLUDE [prod_short](includes/prod_short.md)] filters warehouse activities to the employee's default location. They can only perform the warehouse activities at the location. You can also assign a user to other locations. They can access but not perform activities at those locations.

## <a name="to-set-up-warehouse-employees"></a>To set up warehouse employees

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Warehouse Employees**, and then choose the related link.  
2. Choose the **New** action.  
3. Select the **User ID** field, and then select the user to be added as a warehouse employee. Choose the **OK** button.  
4. In the **Location Code** field, enter the code of the location where the user will be working.  
5. Turn on the **Default** toggle to specify that this is the only location where the employee can perform warehouse activities.  
6. Repeat these steps to assign other employees to locations or assign other locations to existing warehouse employees.  

## <a name="see-also"></a>See also

[Warehouse Management Overview](design-details-warehouse-management.md)
[Inventory](inventory-manage-inventory.md)  
[Setting Up Warehouse Management](warehouse-setup-warehouse.md)  
[Assembly Management](assembly-assemble-items.md)  
[Work with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  
[Define an invoice posting policy for users](admin-setup-invoice-posting-policy.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
