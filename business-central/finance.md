---
title: Financial Management (contains video)
description: 'Learn how Business Central supports your needs for financial management, accounting, auditing, and bookkeeping.'
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bnielse
ms.topic: conceptual
ms.search.keywords: 'accounting, auditing, bookkeeping'
ms.search.form: '1151, 1166, 9027, 9004'
ms.date: 05/01/2024
ms.service: dynamics-365-business-central
ms.custom: bap-template
---

# Financial Management

[!INCLUDE[prod_short](includes/prod_short.md)] includes a standard configuration for most financial processes, but you can change it to suit your business needs. Learn more at [Setting Up Finance](finance-setup-finance.md).

The default configuration includes a chart of accounts and standard posting groups, which make the process of assigning default general ledger posting accounts to customers, vendors, and items more efficient.  

The following sections describe a sequence of tasks, with links to the topics that describe them.  

## Take a video tour

This video introduces some of the key capabilities for managing finances. <br><br>  

> [!Video https://www.microsoft.com/videoplayer/embed/RE4Fss4?rel=0]

## Get started with finance capabilities

Before you can begin to run your business, you must specify how you want to manage your company's financial processes.

|To...| See |
|---|---|
| Change the standard configuration of [!INCLUDE[prod_short](includes/prod_short.md)] for most financial processes to suit your business needs. | [Setting Up Finance](finance-setup-finance.md) | 
| Learn about the general ledger and the chart of accounts (COA). |[Understanding the General Ledger and the COA](finance-general-ledger.md) |

## Accounting

This section describes some of the accounting tools that you use to register financial transactions so that they meet your registration, reporting, and managerial finance requirements.

| To... | See |
| --- | --- |
| Add dimensions for richer business intelligence. |[Work with Dimensions](finance-dimensions.md) |
|Learn how to use additional currencies and update currency exchange rates automatically. |[Update Currency Exchange Rates](finance-how-update-currencies.md)|
| Allocate revenues and expenses to periods other than when the transactions actually posted. |[Defer Revenues and Expenses](finance-how-defer-revenue-expenses.md)|
|Allocate an entry in a general journal to several different accounts when you post the journal. |[Allocate Costs and Income](year-allocate-costs-income.md) |
| Assign extra costs, such as freight and physical handling expenses you incur during trade, to the involved items. This way the cost is reflected in inventory valuation. |[Use Item Charges to Account for Additional Trade Costs](payables-how-assign-item-charges.md) |
| Learn about the available options to automate sending subscription invoices to customers and register recurring revenue. |[Work with Recurring Revenue](finance-recurring-invoicing.md)|
|Post employee expenses for work-related activities and make reimbursements directly to employee bank accounts.|[Record and Reimburse Employees' Expenses](finance-how-record-reimburse-employee-expenses.md)|

## Financial analytics

This section describes analytical tools you can use to get insights into your financial data.

| To... | See |
| --- | --- |
| Learn about capabilities for analysing finance data. | [Financial analytics overview](bi.md) |
| Set up financial reporting across business units or legal entities. | [Handling finance reporting across business units or legal entities](finance-consolidated-company-reporting.md) |
| Set up and use financial reporting to produce statements and overviews. | [Prepare financial reporting](bi-how-work-account-schedule.md) |
| Perform ad-hoc analysis of financial data directly on list pages and queries. | [Ad-hoc analysis on finance data](ad-hoc-analysis-finance.md) |
| Analyse financial data from your chart of accounts. | [Analyse finance data from the chart of accounts](finance-general-ledger.md) |
| Analyse actual amounts versus budgeted amounts. | [Analyse actual amounts versus budgeted amounts](bi-how-analyze-actual-versus-budget.md) |
| Analyse cash flow. | [Analyse cash flow](finance-analyze-cash-flow.md) |
| Explore built-in key financial reports. | [Built-in key finance reports](finance-reports.md) |
| Explore built-in key fixed assets reports. | [Built-in fixed assets reports](fa-reports.md) |
| Explore built-in key accounts receivable reports. | [Built-in accounts receivable reports](receivables-reports.md)
| Explore built-in accounts payable reports. | [Built-in accounts payable reports](payables-reports.md)

## GST and taxes

Working with GST in [!INCLUDE[prod_short](includes/prod_short.md)] is easy, and you can either use a manual or an automatic setup. These articles provide information about how to meet your country/region-specific regulations.

| To... | See |
| --- | --- |
|Calculate goods and services tax (GST) on sales and purchase transactions so you can report the amounts to the tax authorities.|[Work with GST on Sales and Purchases](finance-work-with-vat.md)|
|Prepare a report that lists GST from sales, and submit the report to tax authorities in the European Union (EU). | [Report GST to Tax Authorities](finance-how-report-vat.md)|
|Manually convert service contracts to change their GST rate.|[Convert Service Contracts that Include VAT Amounts](service-how-to-convert-service-contracts.md)|

## Manage receivables and payables

The core of finance is centered around managing receivables and payables, registering transactions, reconciling banks accounts, paying vendors, receiving customer payments, reimbursing employees for expenses, and so on. This section provides links to the core concepts.

| To... | See |
| --- | --- |
| Apply incoming payments, reconcile bank accounts during payment application, and collect outstanding balances. |[Managing Receivables](receivables-manage-receivables.md) |
| Make payments, apply outgoing payments, and work with checks. |[Managing Payables](payables-manage-payables.md) |
|Ask your customers to submit payment before you ship to them, or submit payment to your vendors before they ship to you.|[Invoicing Prepayments](finance-invoice-prepayments.md)|
| Reconcile and transfer funds between bank accounts. |[Reconciling Bank Accounts](bank-manage-bank-accounts.md) |

## Manage multiple companies

[!INCLUDE [prod_short](includes/prod_short.md)] gives small and mid-sized businesses a business management solution that's easy-to-use and maintain at a low cost of ownership.

| To... | See |
| --- | --- |
|Set up intercompany partners and process transactions, manually or automatically, between legal entities within the same company.|[Managing Intercompany Transactions](intercompany-manage.md)|
|Combine general ledger entries from multiple companies in one virtual consolidated company for financial analysis.|[Consolidating Financial Data from Multiple Companies](finance-consolidated-company-reporting.md)|
| Work more closely with related companies that you have access to and to get information about key point of interest (KPI) data. | [Manage Work across Multiple Companies in the Company Hub](company-hub.md)|

## Period-end reporting and related tasks

At the end of each accounting period or at the end of the fiscal year, there are a number of administrative tasks to do. For example, you'll probably want to make sure all documents and journals are posted, ensure currency data is up to date, close the books, and so on. The actual tasks will depend your company.

| To... | See |
| --- | --- |
|Manage inventory and manufacturing costs, and report and reconcile costs with the general ledger.|[Managing Inventory Costs](finance-manage-inventory-costs.md)|
| Import salary transactions from your payroll provider into the general ledger. |[Import Payroll Transactions](finance-how-import-payroll-transactions.md)|
|Learn how to use the Accountant Role Centre, engage an external accountant, and use the Company Hub to manage accounts of multiple clients.|[Accountant Experiences in Business Central](finance-accounting.md)| 

## Managerial accounting

As a business manager or controller, it's important that you can prepare and analyse the business data you need to make informed decisions. The articles in the following table help you prepare data. To learn more about analytics, go to [Business Intelligence and Reporting Overview](reports-bi-reporting.md).

| To... | See |
| --- | --- |
|Analyse the costs of running your business by allocating actual and budgeted costs of operations, departments, products, and projects to cost centres.|[Accounting for Costs](finance-manage-cost-accounting.md)|
| Monitor the flow of cash in and out of your business. |[Analysing Cash Flows in Your Company](finance-analyze-cash-flow.md) |
|Follow an end-to-end process describing how to use financial reports to make cash flow forecasts.|[Walkthrough: Making Cash Flow Forecasts by Using Financial Reports](walkthrough-making-cash-flow-forecasts-by-using-account-schedules.md)|
| Work with financial statements and overviews in Microsoft Excel. |[Analyzing Financial Statements in Excel](finance-analyze-excel.md) |

## Free e-learning modules

Want to learn more about [!INCLUDE[prod_short](includes/prod_short.md)] on your own pace? 

[!INCLUDE[footer-include](includes/footer-banner.md)]

## See also

[Setting Up Finance](finance-setup-finance.md)  
[Working with the Sales module](sales-manage-sales.md)  
[Working with the Purchasing module](purchasing-manage-purchasing.md)  
[Closing Financial Periods](year-close-years-periods.md)  
[Managing Projects](projects-manage-projects.md)  
[Importing Data from Other Finance Systems](across-import-data-configuration-packages.md)  
[Working with General Journals](ui-work-general-journals.md)  
[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  

## [!INCLUDE[prod_short](includes/free_trial_md.md)]