---
title: Manage Employee Absence| Microsoft Docs
description: Describes how to record employees' absence and analyse absence statistics.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 10/01/2018
ms.author: SorenGP
ms.translationtype: HT
ms.sourcegitcommit: 7c346455a9e27d7274b116754f1d594484b95d67
ms.openlocfilehash: 09866f6774af5b2d9644015e986772052146d901
ms.contentlocale: en-nz
ms.lasthandoff: 04/18/2018

---
# <a name="manage-employee-absence"></a>Manage Employee Absence
To manage an employee's absence, you must record the absence in the **Absence Registration** window. It can then be viewed in different ways for analysis and reporting needs.

You can view employee absence in two different windows:

* The **Absence Registration** window, where you register all employee absences with a line for each absence.
* The **Employee Absences** window, where the absences for one employee only is shown. This is the information that you entered in the **Absence Registration** window, filtered by the particular employee.

To obtain meaningful statistics, you should always use the same unit of measure (hour or day) when registering employee absences.

## <a name="to-register-employee-absence"></a>To register employee absence
You can register employee absences on a daily basis or at some other interval that meets your organisational needs.

1. In the top right corner, choose the **Search for Page or Report** icon, enter **Absence Registration**, and then choose the related link.
2. Choose the **New** action.
3. Fill in a line for each employee absence you want to register.
4. Close the window.

    > [!Tip]
    > To obtain meaningful statistics, always use the same unit of measure, hour or day, when registering employee absences.

## <a name="to-view-an-individual-employees-absence"></a>To view an individual employee's absence
1. In the top right corner, choose the **Search for Page or Report** icon, enter **Employees**, and then choose the related link.
2. Select the relevant employee, and then choose the **Absences** action.

    The **Employee Absences** window opens showing all the absences and the date on which they started and ended.

## <a name="to-view-an-employees-absence-by-categories"></a>To view an employee's absence by categories
1. In the top right corner, choose the **Search for Page or Report** icon, enter **Employees**, and then choose the related link.
2. Select the relevant employee, and then choose the **Absences by Categories** action.
3. In the **Empl. Absences by categories** window, fill in the filter fields as necessary, and then choose the **Show Matrix** action.

    The **Empl. Absences by Cat. Matrix** window opens showing all absences, broken down by causes of absence.

## <a name="to-view-all-employee-absences-by-category"></a>To view all employee absences by category
1. In the top right corner, choose the **Search for Page or Report** icon, enter **Absence Registration**, and then choose the related link.
2. In the **Absence Registration** window, choose the **Overview by Categories** action.
3. In the **Absence Overview by Categories** window, set a filter in the **Employee No. Filter** field to view employee absences for individual or a defined group of employees.
4. Choose the **Show Matrix** action.

    The **Absence Overview by Categories Matrix** window opens showing all employees’ absences broken down by the various causes of absence.

## <a name="to-view-all-employee-absences-by-period"></a>To view all employee absences by period
1. In the top right corner, choose the **Search for Page or Report** icon, enter **Absence Registration**, and then choose the related link.
   In the **Absence Registration** window, choose the **Overview by Periods** action.
2. In the **Absence Overview by Periods** window, set a filter in the **Cause of Absence Filter** field to view employee absences for specified causes of absence.
3. Choose the **Show Matrix** action.

    The **Abs. Overview by Periods Matrix** window opens showing employee absences broken down by periods.

## <a name="see-also"></a>See Also
[Manage Human Resources](hr-manage-human-resources.md)  
[Finance](finance.md)  
[Working With [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  
[Changing Which Features are Displayed](ui-experiences.md)

