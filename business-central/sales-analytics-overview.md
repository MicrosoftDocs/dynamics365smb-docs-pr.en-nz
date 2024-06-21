---
title: Sales analytics
description: 'Business Central contains many features to help you gather, analyse, and share valuable sales data for business intelligence and decision-making within the sales organisation.'
author: kennienp
ms.author: bholtorf
ms.reviewer: bholtorf
ms.topic: conceptual
ms.search.keywords: 'bi, power BI, analysis, KPI'
ms.search.form: '516, 9300, 5119, 9301, 9305'
ms.date: 04/28/2024
ms.service: dynamics-365-business-central
ms.custom: bap-template
---

# <a name="sales-analytics"></a>Sales analytics

Businesses capture lots of data during daily activities that supports business intelligence (BI) for sales managers:

- Opportunities
- Sales quotes
- Sales orders
- Sales invoices

[!INCLUDE[prod_short](includes/prod_short.md)] provides features to help you gather, analyse, and share your organisation's sales data:

- Ad-hoc analysis on lists
- Ad-hoc analysis of data in Excel (using Open in Excel)
- Built-in sales analytics tools
- Built-in sales reports

Each of these features has its advantages and disadvantages, depending on the type of data analysis and the role of the user. To learn more, go to [Analytics, business intelligence, and reporting overview](reports-bi-reporting.md).

This article introduces how you can use these analytical features to gain sales insights.

## <a name="analytics-needs-in-sales"></a>Analytics needs in sales

When you think about the analytics needs in sales management, it might help to use a persona-based model that describes different analytics needs at a high-level.

:::image type="content" source="/dynamics365/business-central/dev-itpro/developer/media/analytics-personas.svg" alt-text="Illustration of different personas for analytics" lightbox="/dynamics365/business-central/dev-itpro/developer/media/analytics-personas.svg":::

People in different roles have different needs when it comes to data, and they use the data in different ways. For example, people in asset management and finance interact with data differently than people in sales.

:::image type="content" source="/dynamics365/business-central/dev-itpro/developer/media/analytics-personas-scenarios.svg" alt-text="Illustration of how different personas have different analytics needs." lightbox="/dynamics365/business-central/dev-itpro/developer/media/analytics-personas-scenarios.svg":::

| Role              | Data aggregation  | Typical ways to consume data                          | 
|-------------------|-------------------| ----------------------------------------------------- |
|CCO / CFO / CEO    | Performance data  | KPIs <br> Dashboards <br> Financial reports           |
|Sales Manager      | Trends, summaries | Built-in managerial reports <br> Ad-hoc analysis      | 
|Account Manager / Sales Person | Detailed data     | Built-in operational reports <br> On-screen task data |

<!-- 
## <a name="sales-kpis"></a>Sales KPIs

A key performance indicator (KPI) is a measurable value that shows how effectively you’re meeting your goals. In sales management, people often use the following KPIs to monitor their organization's sales performance:

- TODO  
-->

## <a name="use-financial-reporting-to-produce-financial-statements-and-kpis-related-to-sales"></a>Use financial reporting to produce financial statements and KPIs related to sales

The **Financial Reporting** feature gives you insights into the financial data shown on your chart of accounts (COA). You can set up financial reports to analyse figures in general ledger (G/L) accounts, and compare general ledger entries with budget entries. Specifically for sales management, you can set up financial reports on the general ledger (G/L) accounts that you use to track sales postings.

Dimensions play an important role in business intelligence. A dimension is data that you add to an entry as a parameter. Dimensions let you group entries that have similar characteristics, such as customers, regions, products, and salesperson. Among other purposes, use dimensions when you define analysis views and create financial reports. Learn more at [Work with Dimensions](finance-dimensions.md).

To learn more about financial reports, go to [Prepare Financial Reports with Financial Data and Account Categories](bi-how-work-account-schedule.md).

## <a name="finance-reporting-across-business-units-or-legal-entities-related-to-sales"></a>Finance reporting across business units or legal entities related to sales

Some organisations use [!INCLUDE [prod_short](includes/prod_short.md)] in multiple business units or legal entities. Others use [!INCLUDE [prod_short](includes/prod_short.md)] in subsidiaries that report to parent organisations. [!INCLUDE [prod_short](includes/prod_short.md)] gives accountants tools that help them transfer general ledger entries from two or more companies (subsidiaries) into a consolidated company. Specifically for sales management, you might want to consolidate general ledger entries for your sales accounts to be able to track sales KPIs across business units or legal entities.

To learn more, go to [Company consolidation](finance-consolidated-company-reporting.md).

## <a name="ad-hoc-analysis-of-sales-data"></a>Ad-hoc analysis of sales data

Sometimes, you just need to check whether the numbers add up correctly, or quickly confirm a figure. The following features are great for ad-hoc analyses:

- Data analysis on ledger list pages
- Open in Excel

The Data Analysis feature lets you open almost any list page, such as **General Ledger Entries**, **Customer Ledger Entries**, **Item Ledger Entries**, or **Posted Invoices**, enter analysis mode, and then group, filter, and pivot data as you see fit.

:::image type="content" source="media/data-analysis-customer-ledger-entries.png" alt-text="Example of how to do data analysis on the Customer Ledger Entries page." lightbox="media/data-analysis-customer-ledger-entries.png":::

Similarly, you can use the **Open in Excel** action to open a list page, optionally filter the list to a subset of the data, and then use Excel to work with the data. For example, by using features such as Analyse Data, What-If Analysis, or Forecast Sheet.

:::image type="content" source="media/open-in-excel-customer-ledger-entries.png" alt-text="Example of how to do data analysis on the Customer Ledger Entries data using Excel." lightbox="media/open-in-excel-customer-ledger-entries.png":::

> [!TIP]
> If you configure OneDrive for system features, the Excel workbook opens in your browser.

To learn more about how to do ad-hoc analysis on sales data, go to [Ad hoc analysis of sales data](ad-hoc-analysis-sales.md). 

## <a name="built-in-reports-for-sales"></a>Built-in reports for sales

[!INCLUDE [prod_short](includes/prod_short.md)] includes several built-in reports, tracing functions, and tools to help sales organisations report on their data.

To get an overview of available reports, choose **All reports** on the top pane of your Home page. This action opens the Role Explorer, which is filtered to the features in the **Report & Analysis** option. To learn more, go to [Finding Reports with the Role Explorer](ui-role-explorer.md). 

:::image type="content" source="media/report-explorer-sales.png" alt-text="Example of reports on the sales role centre." lightbox="media/report-explorer-sales.png":::

The built-in reports come in two flavors:

- Designed for print (pdf).
- Designed for analysis in Excel.

To learn more about reports that are relevant for sales, go to [Built-in sales reports](sales-reports.md).

## <a name="on-screen-sales-analytics"></a>On-screen sales analytics

[!INCLUDE [prod_short](includes/prod_short.md)] has several pages that give you sales overviews and tasks to do. Here are some examples to get you started:

- [Open the **Sales Quotes** list](https://businesscentral.dynamics.com/?page=9300)
- [Open the **Sales Orders** list](https://businesscentral.dynamics.com/?page=9305)
- [Open the **Posted Sales Invoices** list](https://businesscentral.dynamics.com/?page=143)
- [Open the **Sales Return Orders** list](https://businesscentral.dynamics.com/?page=9304)
- [Calculate order promising dates](sales-how-to-calculate-order-promising-dates.md)
- [Calculate delivery dates for sales orders](sales-date-calculation-for-sales.md)
- [Track packages](sales-how-track-packages.md)
- [View the Availability of Items](inventory-how-availability-overview.md)
- [Blanket sales order status](sales-how-to-create-blanket-sales-orders.md#to-view-the-status-of-a-blanket-sales-order)
- [View unposted and posted blanket sales order lines](sales-how-to-create-blanket-sales-orders.md#to-view-unposted-and-posted-blanket-sales-order-lines)


### <a name="show-sales-related-general-ledger-entries-and-balances-from-the-chart-of-accounts-page"></a>Show sales-related general ledger entries and balances from the Chart of Accounts page

The Chart of Accounts page shows all general ledger accounts with aggregated numbers posted to the general ledger. From this page, you can do things like:  

- View reports that show general ledger entries and balances.  
- Review a list of posting groups for that account.
- View separate debit and credit balances for a single account.

Specifically for sales, you can create a view on the Chart of Accounts page that only shows the accounts you use for posting sales entries.

:::image type="content" source="media/chart-of-accounts-page.png" alt-text="Example of how the Chart of Accounts page shows finance insights" lightbox="media/chart-of-accounts-page.png":::

To learn more, go to [Understand the Chart of Accounts](finance-general-ledger.md#the-chart-of-accounts).

### <a name="analyze-data-by-dimensions-related-to-sales"></a>Analyse data by dimensions (related to sales)

Dimensions are values that categorise entries so you can track and analyse them on documents, such as sales orders. Dimensions can, for example, indicate the project or department an entry came from.  

So, instead of setting up separate general ledger accounts for each department or location, you can use dimensions as a basis for analysis and avoid having to create a complicated chart of accounts structure.

To learn more, go to [Analyse Data by Dimensions](bi-how-analyze-data-dimension.md).

## <a name="see-also"></a>See also

[Company consolidation](finance-consolidated-company-reporting.md)   
[Prepare Financial Reports with Financial Data and Account Categories](bi-how-work-account-schedule.md)  
[Handling finance reporting across business units or legal entities](finance-consolidated-company-reporting.md)  
[Ad hoc analysis of sales data](ad-hoc-analysis-sales.md)   
[Built-in sales reports](sales-reports.md)   
[Understand the Chart of Accounts](finance-general-ledger.md#the-chart-of-accounts)  
[Analyse Data by Dimensions](bi-how-analyze-data-dimension.md)  
[Analytics, business intelligence, and reporting overview](reports-bi-reporting.md)   
[Work with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  

## [!INCLUDE[prod_short](includes/free_trial_md.md)]  

[!INCLUDE[footer-include](includes/footer-banner.md)]
