---
title: Analyse Actual Versus Budget| Microsoft Docs
description: Describes how to analyse actual amounts versus budgeted amounts.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: bi, power BI, analysis, KPI
ms.date: 06/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: 126c8da9b9ef80e954510fa8e5089906d7dd6f01
ms.contentlocale: en-nz
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-analyze-actual-amounts-versus-budgeted-amounts"></a>How to: Analyse Actual Amounts Versus Budgeted Amounts
As a part of gathering, analysing, and sharing your company data, you view actual amounts compared to budgeted amounts for all accounts and for several periods.

To analyse budgeted amounts, you must first create budgets. For more information, see [How to: Create Budgets](finance-how-create-budgets.md).

> [!NOTE]  
>   This functionality requires that your experience is set to **Suite**. For more information, see [Customizing Your [!INCLUDE[d365fin](includes/d365fin_md.md)] Experience](ui-experiences.md).

## <a name="to-view-a-budget"></a>To view a budget
In a budget with dimensions, you can filter the entries and see specific budgets.

1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **G/L Budgets**, and then choose the related link.
2. In the **G/L Budgets** window, open the budget that you want to view.  
3. At the top of the window, fill in the fields as necessary to define what is shown. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

> [!NOTE]  
>   If you have selected **Period** in either the **Show as Lines** or the **Show as Columns** field, then you must fill in the **View by** field. If you have not selected **Period** in either the **Show as Lines** or **Show as Columns** field, then enter the appropriate period in **Date Filter** field.  

> [!NOTE]  
>   Only entries from the general ledger budget with the filter codes that you enter on the **Filters** FastTab are included in the calculation. Budget entries with other filter codes or without any filter codes are not included. As long as the filter remains on the window, the budget only displays the budget entries with these filter codes.  

> [!TIP]  
>   If you want to modify the budget, you can modify the budget entries. Choose an amount to view the underlying general ledger budget entries.

## <a name="to-view-actual-and-budgeted-amounts-for-all-accounts"></a>To view actual and budgeted amounts for all accounts  
You can view general ledger budgets and compare them with actual figures in several areas of [!INCLUDE[d365fin](includes/d365fin_md.md)].

1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Chart of Accounts**, and then choose the related link.  
2. In the **Chart of Accounts** window, choose the **G/L Balance/Budget** action.
3. At the top of the window, fill in the fields as necessary to define what is shown.  
4. To see a specification that makes up the amount shown, choose the field.  

> [!NOTE]  
>   The filters you set in the window header will be applied to general ledger entries and also budget entries.

The leftmost columns contain the chart of accounts. Of the five columns on the rightmost side, the first four columns show actual and budgeted debit and credit amounts for each account. The fifth column shows the proportional relationship between the actual and the budgeted amounts on the general ledger account.  

> [!TIP]  
>   Use the **View by** field in the **G/L Balance/Budget** window to select the period length. Use the **View as** field to select the way the amounts will be calculated, **Net Change** or **Balance at Date**. Choose the **Previous Period** or **Next Period** action to change the period.  

## <a name="to-view-actual-and-budgeted-amounts-for-several-periods"></a>To view actual and budgeted amounts for several periods  
Instead of viewing the actual and budgeted amounts for all accounts within a single period, you can view a number of periods for a single account.  

1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Chart of Accounts**, and then choose the related link.  
2. In the **Chart of Accounts** window, select the relevant general ledger account, and then choose the **G/L Account Balance/Budget** action.  
3. At the top of the window, fill in the fields as necessary to define what is shown.   
4. To see a specification of an amount shown, choose the field.  

## <a name="see-also"></a>See Also
[Business Intelligence](bi.md)
[How to: Work with Account Schedules](bi-how-work-account-schedule.md)  
[Finance](finance.md)  
[Setting Up Finance](finance-setup-finance.md)  
[The General Ledger and the Chart of Accounts](finance-general-ledger.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

