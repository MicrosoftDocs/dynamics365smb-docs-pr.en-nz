---
title: How to Set Up Warehouse Employees | Microsoft Docs
description: Each user who performs warehouse activities must be set up as a warehouse employee assigned to one default location and potentially more non-default locations.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 7ebb81abd7e16e0c4aaa3f7cd52ab1b6f1a664c3
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 12/17/2020
ms.locfileid: "4755956"
---
# <a name="set-up-warehouse-employees"></a>Set Up Warehouse Employees
Each user who performs warehouse activities must be set up as a warehouse employee assigned to one default location and potentially more non-default locations. This user setup filters all warehouse activities across the database to the employee's location so that the employee can only perform the warehouse activities at the default location. A user can be assigned to additional non-default locations for which the employee can view activity lines but not perform the activities.

## <a name="to-set-up-warehouse-employees"></a>To set up warehouse employees  
1.  Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Warehouse Employees**, and then choose the related link.  
2. Choose the **New** action.  
3. Select the **User ID** field, and then select the user to be added as a warehouse employee. Choose the **OK** button.  
6.  In the **Location Code** field, enter the code of the location where the user will be working.  
7.  Select the **Default** check box to define the location as the only location where the employee can perform warehouse activities.  
8.  Repeat these steps to assign other employees to locations or assign non-default locations to existing warehouse employees.  

## <a name="see-also"></a>See Also  
[Warehouse Management](warehouse-manage-warehouse.md)  
[Inventory](inventory-manage-inventory.md)  
[Setting Up Warehouse Management](warehouse-setup-warehouse.md)     
[Assembly Management](assembly-assemble-items.md)    
[Design Details: Warehouse Management](design-details-warehouse-management.md)  
[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  
