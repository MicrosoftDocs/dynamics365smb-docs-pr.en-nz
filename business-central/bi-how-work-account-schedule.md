---
title: Build financial reports using account schedules
description: Describes how to use account schedules to create various views and report for analysing financial performance data.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: bi, power BI, analysis, KPI
ms.date: 05/31/2018
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: e73c2dd0533aade4aa6225c9d2f385baaea3cfd1
ms.openlocfilehash: 69034b0eb97b595d0fbf5795e1fac34ecd775afe
ms.contentlocale: en-nz
ms.lasthandoff: 06/11/2018

---
# <a name="prepare-financial-reporting-with-account-schedules-and-account-categories"></a>Prepare Financial Reporting with Account Schedules and Account Categories
Use account schedules to get insight into the financial data stored in your chart of accounts. Account schedules analyse figures in G/L accounts, and compare general ledger entries with general ledger budget entries. The results display in charts on your Role Centre, such as the Cash Flow chart, and in reports, such as the Income Statement and the Balance Sheet reports.

You access these two reports, for example, with the **Financials Statements** action on the Business Manager and Accountant Role Centres.   

[!INCLUDE[d365fin](includes/d365fin_md.md)] provides a few sample account schedules that you can use right away, or you can set up your own rows and columns to specify the figures to compare. For example, you can create account schedules to calculate profit margins on dimensions like departments or customer groups. You can create as many customised financial statements as you want.  

Setting up account schedules requires an understanding of the financial data in the chart of accounts. For example, you can view general ledger entries as percentages of budget entries. This requires that budgets are created. For more information, see [Create G/L Budgets](finance-how-create-budgets.md).

## <a name="account-categories-and-account-schedules"></a>Account Categories and Account Schedules
You can use account categories to change the layout of your financial statements. After you set up your account categories in the **G/L Account Categories** window, and you choose the **Generate Account Schedules** action, the underlying account schedules for the core financial reports are updated. The next time you run one of these reports, such as the Balance Statement report, new totals and subentries are added, based on your changes. For more information, see The "Account Categories" section in [Understanding the General Ledger and the COA](finance-general-ledger.md).  

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
> If you did not assign a default column layout to the account schedule, you must set the columns up manually.

### <a name="to-copy-an-existing-account-schedule"></a>To copy an existing account schedule
The account schedules in the standard version of [!INCLUDE[d365fin](includes/d365fin_md.md)] are the basis of the standard financial reports, which may not suit the needs of your business. To quickly create your own financial reports, you can start by copying an existing account schedule.
1. In the **Account Schedules** window, select an account schedule, and then choose the **Copy Account Schedule** action.
2. In the **Copy Account Schedule** window, fill in the fields as necessary, and then choose the **OK** button.

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

## <a name="comparing-accounting-periods-using-period-formulas"></a>Comparing Accounting Periods using Period Formulas
Your account schedule can compare the results of different accounting periods, such as this month versus same month last year. To do that, you add a column with the **Comparison Period Formula** field, and then set that field to a period formula.  

An accounting period does not have to match the calendar, but each fiscal year must have the same number of accounting periods, even though each period can be different in length.   

[!INCLUDE[d365fin](includes/d365fin_md.md)] uses the period formula to calculate the amount from the comparison period in relation to the period represented by the date filter on the report request. The comparison period is based on the period of the start date of the date filter. The abbreviations for period specifications are:


<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th>Abbreviation</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>P</p></td>
<td><p>Period</p></td>
</tr>
<tr class="even">
<td><p>LP</p></td>
<td><p>Last period of a fiscal year, half-year or quarter.</p></td>
</tr>
<tr class="odd">
<td><p>CP</p></td>
<td><p>Current period of a fiscal year, half-year or quarter.</p></td>
</tr>
<tr class="even">
<td><p>FY</p></td>
<td><p>Fiscal year. For example, FY[1..3] denotes first quarter of the current fiscal year</p></td>
</tr>
</tbody>
</table>

Examples of formulas:


<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th>Formula</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>&lt;Blank&gt;</p></td>
<td><p>Current period</p></td>
</tr>
<tr class="even">
<td><p>-1P</p></td>
<td><p>Previous period</p></td>
</tr>
<tr class="odd">
<td><p>-1FY[1..LP]</p></td>
<td><p>Entire previous fiscal year</p></td>
</tr>
<tr class="even">
<td><p>-1FY</p></td>
<td><p>Current period in previous fiscal year</p></td>
</tr>
<tr class="odd">
<td><p>-1FY[1..3]</p></td>
<td><p>First quarter of previous fiscal year</p></td>
</tr>
<tr class="even">
<td><p>-1FY[1..CP]</p></td>
<td><p>From the beginning of previous fiscal year to current period in previous fiscal year, inclusive</p></td>
</tr>
<tr class="odd">
<td><p>-1FY[CP..LP]</p></td>
<td><p>From current period in previous fiscal year to last period of previous fiscal year, inclusive</p></td>
</tr>
</tbody>
</table>

If you want to calculate by regular time periods, you must enter a formula in the **Comparison Date Formula** field instead.

> [!NOTE]
> It is not always transparent which periods you are comparing because you can set a date filter on a report that spans different dates than the accounting periods that are reflected in the data in the chart of accounts. For example, you create an account schedule where you want to compare this period with the same period last year, so you set the **Comparison Date Period Filter** field to *-1FY*. Then, you run the report on February 28th and set the date filter to January and February. As a result, the account schedule compares January and February this year to January last year, which is the only completed accounting period of the two for last year.  


## <a name="see-also"></a>See Also
[Business Intelligence](bi.md)  
[Finance](finance.md)  
[Setting Up Finance](finance-setup-finance.md)  
[The General Ledger and the Chart of Accounts](finance-general-ledger.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

