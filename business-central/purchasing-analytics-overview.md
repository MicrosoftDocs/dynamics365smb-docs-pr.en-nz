---
title: Analytics in purchasing
description: 'Business Central contains many features to help you gather, analyse, and share valuable sales data for business intelligence and decision-making within the purchasing organisation.'
author: kennienp
ms.author: kepontop
ms.reviewer: bholtorf
ms.topic: conceptual
ms.search.keywords: 'bi, power BI, analysis, KPI'
ms.search.form: '9306, 9307, 518, 29'
ms.date: 04/29/2024
ms.service: dynamics-365-business-central
ms.custom: bap-template
---

# <a name="analytics-in-purchasing"></a>Analytics in purchasing

Businesses capture lots of data during daily activities that supports business intelligence (BI) for purchasing managers:

- Purchase quotes
- Purchase orders
- Purchase invoices

[!INCLUDE[prod_short](includes/prod_short.md)] provides features to help you gather, analyse, and share your organisation's purchasing data:

- Ad-hoc analysis on lists
- Ad-hoc analysis of data in Excel (using open in Excel)
- Built-in sales reports

Each of these features has advantages and disadvantages, depending on the type of data analysis and the role of the user. To learn more, go to [Analytics, business intelligence, and reporting overview](reports-bi-reporting.md).

This article introduces how you can use these analytical features to gain purchasing insights.

## <a name="analytics-needs-in-purchasing"></a>Analytics needs in purchasing

When you think about the analytics needs in purchasing, it might help to use a persona-based model that describes different analytics needs at a high-level.

:::image type="content" source="/dynamics365/business-central/dev-itpro/developer/media/analytics-personas.svg" alt-text="Illustration of different personas for analytics" lightbox="/dynamics365/business-central/dev-itpro/developer/media/analytics-personas.svg":::

People in different roles have different needs when it comes to data, and they use the data in different ways. For example, people in asset management and finance interact with data differently than people in sales.

:::image type="content" source="/dynamics365/business-central/dev-itpro/developer/media/analytics-personas-scenarios.svg" alt-text="Illustration of how different personas have different analytics needs." lightbox="/dynamics365/business-central/dev-itpro/developer/media/analytics-personas-scenarios.svg":::

| Role              | Data aggregation  | Typical ways to consume data                          | 
|-------------------|-------------------| ----------------------------------------------------- |
|COO / CSO / CFO / CEO    | Performance data  | KPIs <br> Dashboards <br> Financial reports           |
|Purchasing Manager      | Trends, summaries | Built-in managerial reports <br> Ad-hoc analysis      | 
|Purchasing Officer / Purchasing Agent | Detailed data     | Built-in operational reports <br> On-screen task data |

<!-- 
## <a name="purchasing-kpis"></a>Purchasing KPIs

A key performance indicator (KPI) is a measurable value that shows how effectively you’re meeting your goals. In purchasing management, people often use the following KPIs to monitor their organization's purchasing performance:

- TODO  
-->

## <a name="use-financial-reporting-to-produce-financial-statements-and-kpis-related-to-purchasing"></a>Use financial reporting to produce financial statements and KPIs (related to purchasing)

The **Financial Reporting** feature gives you insights into the financial data shown on your chart of accounts (COA). You can set up financial reports to analyse figures in general ledger (G/L) accounts, and compare general ledger entries with budget entries. Specifically for purchasing, you can set up financial reports on the general ledger (G/L) accounts that you use to track purchase postings.

Dimensions play an important role in business intelligence. A dimension is data that you can add to an entry as a parameter. Dimensions let you group entries that have similar characteristics, such as customers, regions, and products, and easily retrieve these groups for analysis. Among other purposes, use dimensions when you define analysis views and create financial reports. Learn more at [Work with Dimensions](finance-dimensions.md).

To learn more about financial reports, go to [Prepare Financial Reports with Financial Data and Account Categories](bi-how-work-account-schedule.md).

## <a name="finance-reporting-across-business-units-or-legal-entities-related-to-purchasing"></a>Finance reporting across business units or legal entities (related to purchasing)

Some organisations use [!INCLUDE [prod_short](includes/prod_short.md)] in multiple business units or legal entities. Others use [!INCLUDE [prod_short](includes/prod_short.md)] in subsidiaries that report to parent organisations. [!INCLUDE [prod_short](includes/prod_short.md)] gives accountants tools that help them transfer general ledger entries from two or more companies (subsidiaries) into a consolidated company. Specifically for purchasing management, you might want to consolidate general ledger entries for your purchasing accounts to track sales KPIs across business units or legal entities.

To learn more, go to [Company consolidation](finance-consolidated-company-reporting.md).

## <a name="ad-hoc-analysis-of-purchasing-data"></a>Ad-hoc analysis of purchasing data

Sometimes, you just need to check whether the numbers add up correctly, or quickly confirm a figure. The following features are great for ad-hoc analyses:

- Data analysis on ledger list pages
- Open in Excel

The **Data Analysis** feature lets you open almost any list page, such as **Purchase Orders**, **Posted Purchase Invoices**, **Vendor Ledger Entries**, or **General Ledger Entries**, enter analysis mode, and then group, filter, and pivot data as you see fit.

:::image type="content" source="media/data-analysis-vendor-ledger-entries.png" alt-text="Example of how to do data analysis on the Customer Ledger Entries page." lightbox="media/data-analysis-vendor-ledger-entries.png":::

Similarly, you can use the **Open in Excel** action to open a list page, filter the list to a subset of the data, and then use Excel to work with the data. For example, by using features such as Analyse Data, What-If Analysis, or Forecast Sheet.

:::image type="content" source="media/open-in-excel-vendor-ledger-entries.png" alt-text="Example of how to do data analysis on the Customer Ledger Entries data using Excel." lightbox="media/open-in-excel-vendor-ledger-entries.png":::

> [!TIP]
> If you configure OneDrive for system features, the Excel workbook opens in your browser.

To learn more about how to do ad-hoc analysis on purchasing data, go to [Ad hoc analysis of purchasing data](ad-hoc-analysis-purchasing.md).

## <a name="built-in-reports-for-purchasing"></a>Built-in reports for purchasing

[!INCLUDE [prod_short](includes/prod_short.md)] includes several built-in reports, tracing functions, and tools to help purchasing organisations report on their data.

To get an overview of available reports, choose **All Reports** on the top of your Home page. This action opens the Role Explorer, which is filtered to the features in the **Report & Analysis** option. To learn more, go to [Finding Reports with the Role Explorer](ui-role-explorer.md).

:::image type="content" source="media/report-explorer-purchasing.png" alt-text="Example of reports on the XXX role centre." lightbox="media/report-explorer-purchasing.png":::

<!-- Built-in reports come in two flavors:

- Designed for print (pdf).
- Designed for analysis in Excel. -->

To learn more about reports that are relevant for purchasing, go to [Built-in purchasing reports](purchase-reports.md).

## <a name="on-screen-purchasing-analytics"></a>On-screen purchasing analytics

[!INCLUDE [prod_short](includes/prod_short.md)] has several pages that give you purchasing overviews and tasks to do. Here's an example to get you started:

- [Calculate Dates for purchases](purchasing-date-calculation-for-purchases.md)

### <a name="show-purchasing-related-general-ledger-entries-and-balances-from-the-chart-of-accounts-page"></a>Show purchasing-related general ledger entries and balances from the Chart of Accounts page

The Chart of Accounts page shows all general ledger accounts with aggregated numbers posted to the general ledger. From this page, you can do things like:  

- View reports that show general ledger entries and balances.  
- Review a list of posting groups for that account.
- View separate debit and credit balances for a single account.

Specifically for purchasing, you can create a view on the Chart of Accounts page that only shows the accounts you use to post purchasing entries.

:::image type="content" source="media/chart-of-accounts-page.png" alt-text="Example of how the Chart of Accounts page shows finance insights" lightbox="media/chart-of-accounts-page.png":::

To learn more, go to [Understand the Chart of Accounts](finance-general-ledger.md#the-chart-of-accounts).

### <a name="analyze-data-by-dimensions-related-to-purchasing"></a>Analyse data by dimensions (related to purchasing)

Dimensions are values that categorise entries so you can track and analyse them on documents, such as purchase orders. Dimensions can, for example, indicate the project or department an entry came from.  

So, instead of setting up separate general ledger accounts for each department or location, you can use dimensions as a basis for analysis and avoid having to create a complicated chart of accounts structure.

To learn more, go to [Analyse Data by Dimensions](bi-how-analyze-data-dimension.md).

## <a name="see-also"></a>See also

[Company consolidation](finance-consolidated-company-reporting.md)  
[Prepare Financial Reports with Financial Data and Account Categories](bi-how-work-account-schedule.md)  
[Handling finance reporting across business units or legal entities](finance-consolidated-company-reporting.md)  
[Ad hoc analysis of purchasing data](ad-hoc-analysis-purchasing.md)  
[Built-in purchasing reports](purchase-reports.md)  
[Understand the Chart of Accounts](finance-general-ledger.md#the-chart-of-accounts)  
[Analyse Data by Dimensions](bi-how-analyze-data-dimension.md)  
[Analytics, business intelligence, and reporting overview](reports-bi-reporting.md)  
[Work with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  

## [!INCLUDE[prod_short](includes/free_trial_md.md)]  

[!INCLUDE[footer-include](includes/footer-banner.md)]
