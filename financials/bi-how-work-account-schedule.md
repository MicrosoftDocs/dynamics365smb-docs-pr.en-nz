---
title: Work with Account Schedules| Microsoft Docs
description: Describes how to use account schedules to create various views and report for analysing financials performance data.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: bi, power BI, analysis, KPI
ms.date: 08/11/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 192efcf377f6f6d665c775b24aa715aadd50922f
ms.contentlocale: en-nz
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-work-with-account-schedules"></a>How to: Work with Account Schedules
Use account schedules to get insight into the financial data stored in your chart of accounts. Account schedules analyse figures in G/L accounts, and compare general ledger entries with general ledger budget entries. The results display in charts on your Home page, such as the Cash Flow chart.  

[!INCLUDE[d365fin](includes/d365fin_md.md)] provides a few sample account schedules that you can use right away, or you can set up your own rows and columns to specify the figures to compare. For example, you can create account schedules to calculate profit margins on dimensions like departments or customer groups. You can create as many customised financial statements as you want.  

Setting up account schedules requires an understanding of the financial data in the chart of accounts. For example, you can view general ledger entries as percentages of budget entries. This requires that budgets are created. For more information, see [How to: Create Budgets](finance-how-create-budgets.md).

> [!NOTE]  
>   This functionality requires that your experience is set to **Suite**. For more information, see [Customizing Your [!INCLUDE[d365fin](includes/d365fin_md.md)] Experience](ui-experiences.md).

## <a name="account-categories-and-account-schedules"></a>Account Categories and Account Schedules
You can use account categories to change the layout of your financial statements. After you set up your account categories in the **G/L Account Categories** window, and you choose the **Generate Account Schedules** action, the underlying account schedules for the core financial reports are updated. The next time you run one of these reports, such as the balance statement, new totals and subentries are added, based on your changes. For more information, see [The General Ledger and the Chart of Accounts](finance-general-ledger.md).  

## <a name="to-create-new-account-schedules"></a>To create new account schedules  
 You use account schedules to analyse figures in general ledger accounts or to compare general ledger entries with general ledger budget entries. For example, you can view the general ledger entries as percentages of the budget entries.

1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Account Schedules**, and then choose the related link.  
2. In the **Account Schedule Names** window, choose the **New** action to create a new account schedule name.
3. Fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4. Choose the **Edit Account Schedule** action.
5. In the **Account Schedule** window, fill in the fields as necessary.  

    When you have created a new account schedule and set up the rows, you must set up columns. You can either set them up manually or assign a predefined column layout to your account schedule.
6. Choose the **Edit Column Layout Setup** action.
7. In the **Column Layout** window, fill in the fields as necessary.

> [!NOTE]  
>   If you did not assign a default column layout to the account schedule, you must set the columns up manually.   

### <a name="to-create-a-column-that-calculates-percentages"></a>To create a column that calculates percentages  
Sometimes you may want to include a column in an account schedule to calculate percentages of a total. For example, if you have a number of rows that break down sales by dimension, you may want a column to indicate the percentage of total sales that each row represents.

1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Account Schedules**, and then choose the related link.
2. In the **Account Schedule Names** window, select an account schedule.  
3. Choose the **Edit Account Schedule** action to set up an account schedule row to calculate the total on which the percentages will be based.  
4. Insert a line immediately above the first row for which you want to display a percentage.  
5. Fill in the fields on the line as follows: In the **Totaling Type** field, enter **Set Base for Percent**. In the **Totalling** field, enter a formula for the total that the percentage will be based on. For example, if row 11 contains the total sales, enter **11**.  
6. Choose the **Edit Column Layout Setup** action to set up a column.  
7. Fill in the fields on the line as follows: In the **Column Type** field, select **Formula**. In the **Formula** field, enter a formula for the amount that you want to calculate a percentage for, followed by %. For example, if column number N contains the net change, enter **N%**.  
8. Repeat steps 4 through 7 for each group of rows that you want to break down by percentage.

## <a name="to-set-up-account-schedules-with-overviews"></a>To set up account schedules with overviews  
You can use an account schedule to create a statement comparing general ledger figures and general leger budget figures.

1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Account Schedules**, and then choose the related link.
2. In the **Account Schedule Names** window, select an account schedule.  
3. Choose the **Edit Account Schedule** action  
4. In the **Account Schedule** window, in the **Name** field, select the default account schedule name.
5. Choose the **Insert Accounts** action.  
6. Select the accounts that you want to include in your statement, and then choose the **OK** button.

    The accounts are now inserted into your account schedule. If you want you can also change the column layout.  
7. Choose the **Overview** action.  
8. On the **Dimension Filters** FastTab, set the budget filter to the desired filter name.  
9. Choose the **OK** button.  

Now you can copy and paste your budget statement into a spreadsheet.

## <a name="see-also"></a>See Also
[Business Intelligence](bi.md)  
[Finance](finance.md)  
[Setting Up Finance](finance-setup-finance.md)  
[The General Ledger and the Chart of Accounts](finance-general-ledger.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

