---
title: Financial Analytics in Business Central
description: 'Business Central contains many features to help you gather, analyse, and share valuable company data for business intelligence and decision-making.'
author: brentholtorf
ms.author: bholtorf
ms.reviewer: kepontop
ms.topic: conceptual
ms.search.keywords: 'bi, power BI, analysis, KPI'
ms.search.form: '103, 108, 198, 490'
ms.date: 03/27/2024
ms.service: dynamics-365-business-central
ms.custom: bap-template
---

# <a name="financial-analytics-in-business-central"></a>Financial Analytics in Business Central

Businesses capture a tremendous amount of data during daily activities that's supports valuable business intelligence (BI) for decision makers: 

- Sales figures
- Purchases
- Operational expenses
- Employee salaries
- Budgets

[!INCLUDE[prod_short](includes/prod_short.md)] contains many features to help you gather, analyse, and share your organisation's finance data:

- Financial reporting (for financial statements and KPIs)
- Ad-hoc analysis on lists
- Ad-hoc analysis of data in Excel (using open in Excel)
- Built-in finance reports

Each of these features has its own advantages and disadvantages, depending on the type of data analysis and the role of the user. To learn more, go to [Analytics, business intelligence, and reporting overview](reports-bi-reporting.md).

This article introduces you can use these analytical features to provide financial insights.

## <a name="analytics-needs-in-finance"></a>Analytics needs in finance

When thinking of analytics needs in finance, it might help to use a mental model based on personas described on a high-level and their different analytics needs.

:::image type="content" source="/dynamics365/business-central/dev-itpro/developer/media/analytics-personas.svg" alt-text="Illustration of different personas for analytics" lightbox="/dynamics365/business-central/dev-itpro/developer/media/analytics-personas.svg":::

People in different roles have different needs when it comes to data, and they use the data in different ways. For example, people in finance interact with data differently than people in sales.

:::image type="content" source="/dynamics365/business-central/dev-itpro/developer/media/analytics-personas-scenarios.svg" alt-text="Illustration of how different personas have different analytics needs." lightbox="/dynamics365/business-central/dev-itpro/developer/media/analytics-personas-scenarios.svg":::

| Role              | Data aggregation  | Typical ways to consume data                          | 
|-------------------|-------------------| ----------------------------------------------------- |
|CFO / CEO          | Performance data  | KPIs <br> Dashboards <br> Financial reports           |
|Finance Management | Trends, summaries | Built-in managerial reports <br> Ad-hoc analysis      | 
|Bookkeeper         | Detailed data     | Built-in operational reports <br> On-screen task data |

## <a name="finance-kpis"></a>Finance KPIs

A key performance indicator (KPI) is a measurable value that shows how effectively you’re meeting your goals. In finance, people often use the following KPIs to monitor their organisation's financial health:

- Gross Profit Margin
- Net Profit Margin
- Working Capital
- Current/Quick Ratio
- Financial leverage, also known as the Equity Multiplier
- Debt-to-Equity Ratio
- Total Asset Turnover
- Return on Equity
- Return on Assets

<!-- Not ready to publish yet
For more information, see [Financial KPIs in Business Central](bi-finance-kpis.md) 
-->

## <a name="using-financial-reporting-to-produce-financial-statements-and-kpis"></a>Using financial reporting to produce financial statements and KPIs

The **Financial Reports** feature gives you insights into the financial data shown on your chart of accounts (COA). You can set up financial reports to analyse figures in general ledger (G/L) accounts, and compare general ledger entries with budget entries. The results display in charts and reports on your home page, such as the Cash Flow chart, and the Income Statement and Balance Sheet reports.

Dimensions play an important role in business intelligence. A dimension is data that you can add to an entry as a parameter. Dimensions let you group entries that have similar characteristics, such as customers, regions, products, and salesperson, and easily retrieve these groups for analysis. Among other purposes, you use dimensions when you define analysis views and create financial reports. Learn more at [Work with Dimensions](finance-dimensions.md).

> [!TIP]
> As a quick way to analyse transactional data, you can filter totals in the chart of accounts and all entries in **Entries** pages by dimensions. Look for the **Set Dimension Filter** action.  

The following table describes a sequence of tasks in financial reporting, with links to the articles that describe them.  

| To | See |
| --- | --- |
| Create new financial reports to define financial statements for reporting or to display as charts.| [Prepare Financial Reports with Financial Data and Account Categories](bi-how-work-account-schedule.md)|
| Use statistical accounts to supplement information in financial reports. Statistical accounts let you add metrics that are based on non-transactional data. You can add the non-transactional data as number-based units, such as employee headcount, square footage, or number of customers with overdue accounts. | [Analyse data with statistical accounts](bi-use-statistical-accounts.md) |
| Learn how to setup a new financial report through examples. | [Walkthrough: Use financial reporting to make a cash flow forecasts](walkthrough-making-cash-flow-forecasts-by-using-account-schedules.md) |
| Analyse your financial performance by setting up key performance indicators (KPIs) based on financial reports, which you then publish as web services. The published financial reports KPIs can be viewed on a web site or imported to Microsoft Excel using OData web services. |[Set Up and Publish KPI Web Services Based on Financial Reports](bi-how-to-set-up-and-publish-kpi-web-services-based-on-account-schedules.md) |
| Set up views to analyse data using dimensions.|[Analyse Data by Dimensions](bi-how-analyze-data-dimension.md)|
| Create new analysis reports for sales, purchases, and inventory, and set up analysis templates. |[Create Analysis Reports](bi-how-create-analysis-views-reports.md)|

## <a name="finance-reporting-across-business-units-or-legal-entities"></a>Finance reporting across business units or legal entities

Some organisations use [!INCLUDE [prod_short](includes/prod_short.md)] in multiple business units or legal entities. Others use [!INCLUDE [prod_short](includes/prod_short.md)] in subsidiaries that must report into parent organisations. [!INCLUDE [prod_short](includes/prod_short.md)] gives accountants tools that help them transfer general ledger entries from two or more companies (subsidiaries) into a consolidated company.  

To learn more, go to [Company consolidation](finance-consolidated-company-reporting.md).

## <a name="ad-hoc-analysis-of-finance-data"></a>Ad-hoc analysis of finance data

Sometimes, you just need to check whether the numbers add up correctly, or quickly confirm a figure. The following features are great for ad-hoc analyses:

- Data analysis on ledger list pages
- Open in Excel

The Data analysis feature lets you open almost a list page, such as General Ledger Entries, Fixed Asset Ledger Entries, Cheque Ledger Entries, or Bank Account Ledger Entries, enter analysis mode, and then group, filter, and pivot data as you see fit.

:::image type="content" source="media/data-analysis-gl-entries.png" alt-text="Example of how to do data analysis on the G/L entries page." lightbox="media/data-analysis-gl-entries.png":::

Similarly, you can use the **Open in Excel** action to open a list page for ledger entries, optionally filter the list to a subset of the data, and then use Excel to work with the data. For example, by using features such as Analyse Data, What-If Analysis, or Forecast Sheet.

:::image type="content" source="media/open-in-excel-gl-entries.png" alt-text="Example of how to do data analysis on the G/L entries data using Excel." lightbox="media/open-in-excel-gl-entries.png":::

> [!TIP]
> If you configure OneDrive for system features, the Excel workbook opens in your browser by using Excel for the web. 

<!-- Not ready yet
For more information on how to do ad-hoc analysis on ledgers, see [Ad-hoc analysis on finance data](ad-hoc-analysis-finance.md). 
-->
## <a name="built-in-reports-for-finance"></a>Built-in reports for finance

[!INCLUDE [prod_short](includes/prod_short.md)] includes several built-in reports, tracing functions, and tools to help auditors or controllers who are responsible for reporting to the finance department.

To get an overview of available reports, you can click **All reports** on the top pane of your home page. This takes you to the Role explorer, which is filtered to the features in the **Report & Analysis** option. To learn more, go to [Finding Reports with the Role Explorer](ui-role-explorer.md).

:::image type="content" source="media/report-explorer-finance.png" alt-text="Example of reports on the finance role centre." lightbox="media/report-explorer-finance.png":::

Built-in reports come in two flavors:

- Designed for print (pdf).
- Designed for analysis in Excel.

For more information, see these overviews for reports that are relevant for finance.

- [Built-in finance Excel reports](finance-analyze-excel.md)
- [Built-in key finance reports](finance-reports.md)
- [Built-in fixed assets reports](fa-reports.md)
- [Built-in accounts receivable reports](receivables-reports.md)
- [Built-in accounts payable reports](payables-reports.md)

<!-- TODO: add when we have these articles
* [Built-in Cost Accounting reports](cost-accounting-reports.md) 
* [Built-in Cash Management reports](cost-accounting-reports.md) 
* [Built-in Tax and VAT reports](tax-and-vat-reports.md) 
-->

## <a name="on-screen-finance-task-pages"></a>On-screen finance task pages

[!INCLUDE [prod_short](includes/prod_short.md)] has a number of pages that give you financial overviews and tasks to do.

### <a name="show-general-ledger-entries-and-balances-from-the-chart-of-accounts-page"></a>Show general ledger entries and balances from the Chart of Accounts page

The Chart of Accounts page shows all general ledger accounts with aggregated numbers on what's posted to the general ledger. From this page, you can do things like:  

- View reports that show general ledger entries and balances.  
- Review a list of posting groups for that account.
- View separate debit and credit balances for a single account.

:::image type="content" source="media/chart-of-accounts-page.png" alt-text="Example of how the Chart of Accounts page shows finance insights" lightbox="media/chart-of-accounts-page.png":::

To learn more, go to [Understand the Chart of Accounts](finance-general-ledger.md#the-chart-of-accounts).

### <a name="view-actual-amounts-compared-to-budgeted-amounts-for-all-accounts-and-for-several-periods"></a>View actual amounts compared to budgeted amounts for all accounts and for several periods

As a part of gathering, analysing, and sharing your company data, you might want to view actual amounts compared to budgeted amounts for all accounts and for several periods. You can do this from the **Chart of Accounts** page, by choosing the **G/L Balance/Budget** action.

To learn more, go to [Analyse Actual Amounts Versus Budgeted Amounts](bi-how-analyze-actual-versus-budget.md).

### <a name="analyze-data-by-dimensions"></a>Analyse data by dimensions

Dimensions are values that categorise entries so you can track and analyse them on documents, such as sales orders. Dimensions can, for example, indicate the project or department an entry came from.  

So, instead of setting up separate general ledger accounts for each department and project, you can use dimensions as a basis for analysis and avoid having to create a complicated chart of accounts structure.

In financial analysis, a dimension is data you add to a G/L entry as a kind of marker. This data is used to group G/L entries with similar characteristics, such as customers, regions, products, and salesperson, and easily retrieve these groups for analysis. You can use dimensions on entries in journals, documents, and budgets. For more information, see [Analyse Data by Dimensions](bi-how-analyze-data-dimension.md)

### <a name="analyzing-cash-flow"></a>Analysing cash flow

On the Accountant home page, under **Finance Performance**, the Cash Cycle, Cash Flow, and Income & Expense charts offer ways to analyse cash flow:

- Review figures for a period by using the timeline slider.
- Filter the chart by choosing the source in the legend.
- Change the length of the period, or go to the previous or next period, by choosing options on the Finance Performance drop down.

:::image type="content" source="media/cashflow-accountant-rolecentre.png" alt-text="Example of how the cash flow visuals look on the accountant role centre" lightbox="media/cashflow-accountant-rolecentre.png":::

To examine the forecast, in addition to forecast entries, you can also look at the cash flow worksheet. For example, you can see how the forecast:

- Handles confirmed sales and purchases.
- Subtracts payables and adds receivables.
- Skips duplicate sales orders and purchase orders.

To learn more, go to [Analysing Cash Flow in Your Company](finance-analyze-cash-flow.md).

## <a name="see-also"></a>See also

[Handling finance reporting across business units or legal entities](finance-consolidated-company-reporting.md)  
<!-- [Financial KPIs in Business Central](bi-finance-kpis.md)    -->
[Prepare Financial Reports with Financial Data and Account Categories](bi-how-work-account-schedule.md)  
<!-- [Ad-hoc analysis on finance data](ad-hoc-analysis-finance.md)   -->
[Understand the Chart of Accounts](finance-general-ledger.md#the-chart-of-accounts)  
[Built-in finance Excel reports](finance-analyze-excel.md)  
[Built-in key finance reports](finance-reports.md)  
[Built-in fixed assets reports](fa-reports.md)  
[Built-in accounts receivable reports](receivables-reports.md)  
[Built-in accounts payable reports](payables-reports.md)  
[Finance overview](finance.md)  
[Analytics, business intelligence, and reporting overview](reports-bi-reporting.md)   
[Work with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  

## [!INCLUDE[prod_short](includes/free_trial_md.md)]  

[!INCLUDE[footer-include](includes/footer-banner.md)]
