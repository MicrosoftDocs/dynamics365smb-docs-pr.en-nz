---
title: Set Up Warehouse Employees
description: Each user who performs warehouse activities must be set up as a warehouse employee assigned to one default location and potentially more non-default locations.
author: SorenGP
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.form: 7328, 7348
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: a3d851ff0f44fdae3880aea841d1145fc83e7e13
ms.sourcegitcommit: 3acadf94fa34ca57fc137cb2296e644fbabc1a60
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 09/19/2022
ms.locfileid: "9530125"
---
# <a name="set-up-warehouse-employees"></a>Set Up Warehouse Employees

Each user who performs warehouse activities must be set up as a warehouse employee assigned to one default location and potentially more non-default locations. This user setup filters all warehouse activities across the database to the employee's location so that the employee can only perform the warehouse activities at the default location. A user can be assigned to additional non-default locations for which the employee can view activity lines but not perform the activities.

## <a name="to-set-up-warehouse-employees"></a>To set up warehouse employees  

1.  Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Warehouse Employees**, and then choose the related link.  
2. Choose the **New** action.  
3. Select the **User ID** field, and then select the user to be added as a warehouse employee. Choose the **OK** button.  
4. In the **Location Code** field, enter the code of the location where the user will be working.  
5. Select the **Default** check box to define the location as the only location where the employee can perform warehouse activities.  
6. Repeat these steps to assign other employees to locations or assign non-default locations to existing warehouse employees.  

## <a name="see-related-microsoft-training"></a>See related [Microsoft training](/training/modules/get-started-warehouse-management/)

## <a name="see-also"></a>See also

[Warehouse Management](warehouse-manage-warehouse.md)  
[Inventory](inventory-manage-inventory.md)  
[Setting Up Warehouse Management](warehouse-setup-warehouse.md)  
[Assembly Management](assembly-assemble-items.md)  
[Design Details: Warehouse Management](design-details-warehouse-management.md)  
[Work with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]
