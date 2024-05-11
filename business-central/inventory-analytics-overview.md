---
title: Inventory analytics
description: 'Business Central contains many features to help you gather, analyse, and share valuable data on your inventory for business intelligence and decision-making within your organisation.'
author: kennienp
ms.author: kepontop
ms.reviewer: bholtorf
ms.topic: conceptual
ms.search.keywords: 'bi, power BI, analysis, KPI'
ms.search.form: '516, 9300, 5119, 9301, 9305'
ms.date: 05/03/2024
ms.service: dynamics-365-business-central
ms.custom: bap-template
---

# Inventory analytics

Businesses capture lots of data during daily activities that supports business intelligence (BI) for inventory managers:

- Shipping of goods when sales orders are fulfilled.
- Receipts of items when purchase orders are fulfilled.
- Movements of items between locations.

[!INCLUDE[prod_short](includes/prod_short.md)] provides features to help you gather, analyse, and share your organisation's inventory data:

- Ad-hoc analysis on lists
- Ad-hoc analysis of data in Excel (using Open in Excel)
- Built-in inventory analytics tools
- Built-in inventory reports

Each of these features has its advantages and disadvantages, depending on the type of data analysis and the role of the user. To learn more, go to [Analytics, business intelligence, and reporting overview](reports-bi-reporting.md).

This article introduces how you can use these analytical features to gain insights into your inventory.

## Analytics needs in inventory

When you think about the analytics needs in inventory management, it might help to use a persona-based model that describes different analytics needs at a high-level.

:::image type="content" source="/dynamics365/business-central/dev-itpro/developer/media/analytics-personas.svg" alt-text="Illustration of different personas for analytics" lightbox="/dynamics365/business-central/dev-itpro/developer/media/analytics-personas.svg":::

People in different roles have different needs when it comes to data, and they use the data in different ways. For example, people in asset management and finance interact with data differently than people in sales.

:::image type="content" source="/dynamics365/business-central/dev-itpro/developer/media/analytics-personas-scenarios.svg" alt-text="Illustration of how different personas have different analytics needs." lightbox="/dynamics365/business-central/dev-itpro/developer/media/analytics-personas-scenarios.svg":::

| Role              | Data aggregation  | Typical ways to consume data                          | 
|-------------------|-------------------| ----------------------------------------------------- |
|COO / CFO / CEO    | Performance data  | KPIs, dashboards, financial reports           |
|Inventory Manager  | Trends, summaries | Built-in managerial reports, ad-hoc analysis      | 
|Warehouse worker   | Detailed data     | Built-in operational reports, on-screen task data |

<!-- 
## Inventory KPIs

A key performance indicator (KPI) is a measurable value that shows how effectively you’re meeting your goals. In inventory management, people often use the following KPIs to monitor their organization's sales performance:

- TODO  
-->

## Use financial reporting to produce financial statements and KPIs related to inventory

The **Financial Reporting** feature gives you insights into the financial data shown on your chart of accounts (COA). You can set up financial reports to analyse figures in general ledger (G/L) accounts, and compare general ledger entries with budget entries. Specifically for inventory management, you can set up financial reports on the general ledger (G/L) accounts that you use to track inventory postings.

Dimensions play an important role in business intelligence. A dimension is data that you add to an entry as a parameter. Dimensions let you group entries that have similar characteristics, such as customers, regions, products, and salesperson. Among other purposes, use dimensions when you define analysis views and create financial reports. Learn more at [Work with Dimensions](finance-dimensions.md).

To learn more about financial reports, go to [Prepare Financial Reports with Financial Data and Account Categories](bi-how-work-account-schedule.md).

## Finance reporting across business units or legal entities (related to inventory)

Some organisations use [!INCLUDE [prod_short](includes/prod_short.md)] in multiple business units or legal entities. Others use [!INCLUDE [prod_short](includes/prod_short.md)] in subsidiaries that report to parent organisations. [!INCLUDE [prod_short](includes/prod_short.md)] gives accountants tools that help them transfer general ledger entries from two or more companies (subsidiaries) into a consolidated company. Specifically for inventory management, you might want to consolidate general ledger entries for your inventory accounts to be able to track sales KPIs across business units or legal entities.

To learn more, go to [Company consolidation](finance-consolidated-company-reporting.md).

## Ad-hoc analysis of inventory data

Sometimes, you just need to check whether the numbers add up correctly, or quickly confirm a figure. The following features are great for ad-hoc analyses:

- Data analysis on ledger list pages
- Open in Excel

The Data Analysis feature lets you open almost any list page, such as **Item Ledger Entries**, enter analysis mode, and then group, filter, and pivot data as you see fit.

:::image type="content" source="media/data-analysis-inventory-dead-stock.png" alt-text="Example of how to do a old stock data analysis on the Item Ledger Entries page." lightbox="media/data-analysis-inventory-dead-stock.png":::

Similarly, you can use the **Open in Excel** action to open a list page, optionally filter the list to a subset of the data, and then use Excel to work with the data. For example, by using features such as Analyse Data, What-If Analysis, or Forecast Sheet.

<!-- :::image type="content" source="media/open-in-excel-item-ledger-entries.png" alt-text="Example of how to do data analysis on the Item Ledger Entries data using Excel." lightbox="media/open-in-excel-item-ledger-entries.png"::: -->

> [!TIP]
> If you configure OneDrive for system features, the Excel workbook opens in your browser.

To learn more about how to do ad-hoc analysis on inventory data, go to [Ad hoc analysis of inventory data](ad-hoc-analysis-inventory.md).

## Built-in reports for inventory

[!INCLUDE [prod_short](includes/prod_short.md)] includes several built-in reports, tracing functions, and tools to help inventory organisations report on their data.

To get an overview of available reports, choose **All Reports** on your Home page. This action opens the Report Explorer, which is filtered to the features in the **Report & Analysis** option. Under the **Sales and Marketing** heading, choose **Explore**. To learn more, go to [Finding Reports with the Role Explorer](ui-role-explorer.md).

:::image type="content" source="media/report-explorer-sales.png" alt-text="Example of reports on the sales role centre." lightbox="media/report-explorer-sales.png":::

<!-- The built-in reports come in two flavors:

- Designed for print (pdf).
- Designed for analysis in Excel. -->

To learn more about reports that are relevant for inventory, go to [Built-in inventory and warehouse reports](inventory-WMS-reports.md).

## On-screen inventory analytics

[!INCLUDE [prod_short](includes/prod_short.md)] has several pages that give you inventory overviews and tasks to do. Here are some examples to get you started:

- [View the Availability of Items](inventory-how-availability-overview.md)
- [Track items with serial, lot, and package numbers](inventory-how-work-item-tracking.md)
- [Trace item-tracked items](inventory-how-to-trace-item-tracked-items.md)
- [Audit the reconciliation between the inventory ledger and the general ledger](finance-how-to-post-inventory-costs-to-the-general-ledger.md#to-audit-the-reconciliation-between-the-inventory-ledger-and-the-general-ledger)
- [View cross-docked items in a shipment or pick worksheet](warehouse-how-to-cross-dock-items.md#to-view-cross-docked-items-in-a-shipment-or-pick-worksheet)

The sales module also include analytics pages related to inventory:

- [Calculate order promising dates](sales-how-to-calculate-order-promising-dates.md)
- [Calculate delivery dates for sales orders](sales-date-calculation-for-sales.md)
- [Track packages](sales-how-track-packages.md)

### Show inventory-related general ledger entries and balances from the Chart of Accounts page

The **Chart of Accounts** page shows all general ledger accounts with aggregated numbers posted to the general ledger. From this page, you can do things like:  

- View reports that show general ledger entries and balances.  
- Review a list of posting groups for that account.
- View separate debit and credit balances for a single account.

Specifically for inventory management, you can create a view on the Chart of Accounts page that only shows the accounts you use to post inventory entries.

:::image type="content" source="media/chart-of-accounts-page.png" alt-text="Example of how the Chart of Accounts page shows finance insights" lightbox="media/chart-of-accounts-page.png":::

To learn more, go to [Understand the Chart of Accounts](finance-general-ledger.md#the-chart-of-accounts).

### Analyse inventory data by dimensions

Dimensions are values that categorise entries so you can track and analyse them on documents, such as sales orders. Dimensions can, for example, indicate the project or department an entry came from.  

So, instead of setting up separate general ledger accounts for each department or location, you can use dimensions as a basis for analysis and avoid having to create a complicated chart of accounts structure.

To learn more, go to [Analyse Data by Dimensions](bi-how-analyze-data-dimension.md).

## See also

[Company consolidation](finance-consolidated-company-reporting.md)   
[Prepare Financial Reports with Financial Data and Account Categories](bi-how-work-account-schedule.md)  
[Handling finance reporting across business units or legal entities](finance-consolidated-company-reporting.md)  
[Ad-hoc analysis of inventory data](ad-hoc-analysis-inventory.md)  
[Built-in inventory and warehouse reports](inventory-WMS-reports.md)  
[Understand the Chart of Accounts](finance-general-ledger.md#the-chart-of-accounts)  
[Analyse Data by Dimensions](bi-how-analyze-data-dimension.md)  
[Analytics, business intelligence, and reporting overview](reports-bi-reporting.md)   
[Work with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  

## [!INCLUDE[prod_short](includes/free_trial_md.md)]  

[!INCLUDE[footer-include](includes/footer-banner.md)]
