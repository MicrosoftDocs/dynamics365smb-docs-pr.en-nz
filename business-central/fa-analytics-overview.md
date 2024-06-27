---
title: Fixed assets analytics
description: 'Learn how to gather, analyse, and share data about fixed assets for business intelligence.'
author: brentholtorf
ms.author: kepontop
ms.reviewer: bholtorf
ms.topic: conceptual
ms.search.keywords: 'bi, power BI, analysis, KPI'
ms.search.form: '5601, 5600, 5615, 5616, 5617'
ms.date: 05/22/2024
ms.service: dynamics-365-business-central
ms.custom: bap-template
---

# Fixed assets analytics

Businesses with fixed assets capture a lot of data about them during daily activities. That data supports valuable business intelligence (BI) for fixed assets managers:

- Asset acquisitions
- Asset deprecation
- Insurance and maintenance
- Asset budgets

[!INCLUDE[prod_short](includes/prod_short.md)] provides features to help you gather, analyse, and share data about your organisation's fixed assets:

- Financial reporting (for financial statements and KPIs on fixed assets accounts)
- Ad-hoc analysis on lists
- Ad-hoc analysis of data in Excel (using open in Excel)
- Built-in fixed assets analytics tools
- Built-in fixed assets reports

> [!NOTE]
> Analytics for fixed assets is a little different than other areas. You need to analyse data that's already present, such as asset acquisitions, deprecation, and insurance, but also data about future (projected) data, such as depreciation and asset retirements. For the latter type of analysis, [!INCLUDE[prod_short](includes/prod_short.md)] has built-in reports that can calculate these numbers.

Each feature has its advantages and disadvantages, depending on the type of data analysis and the role of the user. To learn more, go to [Analytics, business intelligence, and reporting overview](reports-bi-reporting.md).

This article describes ways use these analytical features to get insights into your fixed assets.

## Analytics needs in asset management

When thinking of analytics needs in asset management, it might help to use a persona-based model that describes their analytics needs at a high-level.

:::image type="content" source="/dynamics365/business-central/dev-itpro/developer/media/analytics-personas.svg" alt-text="Illustration of different personas for analytics" lightbox="/dynamics365/business-central/dev-itpro/developer/media/analytics-personas.svg":::

When it comes to data, people in different roles have different needs, and they use the data in different ways. For example, people in asset management and finance interact with data differently than people in sales.

:::image type="content" source="/dynamics365/business-central/dev-itpro/developer/media/analytics-personas-scenarios.svg" alt-text="Illustration of how different personas have different analytics needs." lightbox="/dynamics365/business-central/dev-itpro/developer/media/analytics-personas-scenarios.svg":::

| Role              | Data aggregation  | Typical ways to consume data                          | 
|-------------------|-------------------| ----------------------------------------------------- |
|CFO / COO / CEO                 | Performance data  | KPIs <br> Dashboards <br> Financial reports           |
|Asset Management / Controller   | Trends, summaries | Built-in managerial reports <br> Ad-hoc analysis      | 
|Bookkeeper                      | Detailed data     | Built-in operational reports <br> On-screen task data |

## Asset Management KPIs

A key performance indicator (KPI) is a measurable value that shows how effectively you’re meeting your goals. In asset management, people often use the following KPIs to monitor their organisation's use of assets:

- Total Asset Turnover
- Return on Assets

## Use financial reporting to produce financial statements and KPIs related to fixed assets

The **Financial Reporting** feature gives you insights into the financial data shown on your chart of accounts (COA). You can set up financial reports to analyse figures in general ledger (G/L) accounts, and compare general ledger entries with budget entries. Specifically for asset management, you can set up financial reports on the general ledger (G/L) accounts that you use to track fixed assets postings.

Dimensions play an important role in business intelligence. A dimension is data that you can add to an entry as a parameter. Dimensions let you group entries that have similar characteristics, such as customers, products, and salesperson, and easily retrieve these groups for analysis. Among other purposes, you use dimensions when you define analysis views and create financial reports. Learn more at [Work with Dimensions](finance-dimensions.md).

To learn more about financial reporting, go to [Prepare Financial Reports with Financial Data and Account Categories](bi-how-work-account-schedule.md).

## Finance reporting across business units or legal entities (related to fixed assets)

Some organisations use [!INCLUDE [prod_short](includes/prod_short.md)] in multiple business units or legal entities. Others use [!INCLUDE [prod_short](includes/prod_short.md)] in subsidiaries report to parent organisations. [!INCLUDE [prod_short](includes/prod_short.md)] gives accountants tools that help them transfer general ledger entries from two or more companies (subsidiaries) into a consolidated company. Specifically for asset management, you might want to consolidate general ledger entries for your fixed assets accounts to be able to track fixed assets KPIs across business units or legal entities.

To learn more, go to [Company consolidation](finance-consolidated-company-reporting.md).

## Ad-hoc analysis of fixed assets data

Sometimes, you just need to check whether the numbers add up correctly, or quickly confirm a figure. The following features are great for ad-hoc analyses:

- Data analysis on ledger list pages
- Open in Excel

The data analysis feature lets you open almost any list page, such as **General Ledger Entries** or **Fixed Asset Ledger Entries**, enter analysis mode, and then group, filter, and pivot data as you see fit.

:::image type="content" source="media/data-analysis-fa-ledger-entries-asset-overview-current-value.png" alt-text="Example of how to do data analysis on the FA Ledger Entries page to see asset value." lightbox="media/data-analysis-fa-ledger-entries-asset-overview-current-value.png":::

Similarly, you can use the **Open in Excel** action to open a list page for ledger entries, optionally filter the list to a subset of the data, and then use Excel to work with the data. For example, by using features such as Analyse Data, What-If Analysis, or Forecast Sheet.

<!-- :::image type="content" source="media/open-in-excel-gl-entries.png" alt-text="Example of how to do data analysis on the G/L entries data using Excel." lightbox="media/open-in-excel-gl-entries.png"::: -->

> [!TIP]
> If you configure OneDrive for system features, the Excel workbook opens in your browser by using Excel for the web. 

For more information on how to do ad-hoc analysis on Fixed Assets ledgers, see [Ad-hoc analysis of fixed assets data](ad-hoc-analysis-fa.md).


## Built-in reports for fixed assets

[!INCLUDE [prod_short](includes/prod_short.md)] includes several built-in reports, tracing functions, and tools to help auditors or controllers who report on fixed assets.

To get an overview of available reports, choose **All reports** at the top of your Home page. This action opens the Role Explorer page, which is filtered to the features in the **Report & Analysis** option. To find reports related to fixed assets, in the **Find** field, enter **fixed assets**. To learn more, go to [Finding Reports with the Role Explorer](ui-role-explorer.md).

:::image type="content" source="media/report-explorer-fixed-assets.png" alt-text="Example of reports on the finance role centre." lightbox="media/report-explorer-fixed-assets.png":::

<!-- Built-in reports come in two flavors:

- Designed for print (pdf).
- Designed for analysis in Excel. -->

For more information about reports that are relevant for fixed assets, see [Built-in fixed assets reports](fa-reports.md).

## On-screen fixed assets analytics

[!INCLUDE [prod_short](includes/prod_short.md)] has several pages that give you fixed assets overviews and tasks to do. Here are some examples to get you started:

- [Calculate depreciation, post depreciation, and analyse depreciation](fa-how-depreciate-amortize.md)
- [Monitor maintenance costs](fa-how-maintain.md#monitor-maintenance-costs)
- [Monitor insurance coverage](fa-how-insure.md#to-monitor-insurance-coverage)
- [View changed depreciation book values](fa-how-trans-split-combine.md#to-view-changed-depreciation-book-values-due-to-fixed-asset-reclassification)
- [View disposal ledger entries](fa-how-dispose-retire.md#to-view-disposal-ledger-entries)
- [View projected disposal values](fa-how-manage-budgets.md#to-view-projected-disposal-values)

### Show fixed asset general ledger entries and balances from the Chart of Accounts page

The Chart of Accounts page shows all general ledger accounts with aggregated numbers in the general ledger. From this page, you can do things like:  

- View reports that show general ledger entries and balances.  
- Review a list of posting groups for that account.
- View separate debit and credit balances for a single account.

Specifically for fixed assets, you can create a view on the Chart of Accounts page that only shows asset accounts, or maybe only the asset accounts you use for posting fixed assets entries.

:::image type="content" source="media/chart-of-accounts-page-fa.png" alt-text="Example of how the Chart of Accounts page shows finance insights" lightbox="media/chart-of-accounts-page-fa.png":::

To learn more, go to [Understand the Chart of Accounts](finance-general-ledger.md#the-chart-of-accounts).

### Analyse data by dimensions (related to fixed assets)

Dimensions are values that categorise entries so you can track and analyse them on documents, such as FA journals. Dimensions can, for example, indicate the department or location an entry came from.  

So, instead of setting up separate general ledger accounts for each department or location, you can use dimensions as a basis for analysis and avoid having to create a complicated chart of accounts structure.

To learn more, go to [Analyse Data by Dimensions](bi-how-analyze-data-dimension.md)

## See also

[Handling finance reporting across business units or legal entities](finance-consolidated-company-reporting.md)  
[Prepare Financial Reports with Financial Data and Account Categories](bi-how-work-account-schedule.md)  
[Understand the Chart of Accounts](finance-general-ledger.md#the-chart-of-accounts)  
[Ad-hoc analysis of fixed assets data](ad-hoc-analysis-fa.md)   
[Built-in fixed assets reports](fa-reports.md)  
[Analytics, business intelligence, and reporting overview](reports-bi-reporting.md)  
[Work with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  

## [!INCLUDE[prod_short](includes/free_trial_md.md)]  

[!INCLUDE[footer-include](includes/footer-banner.md)]
