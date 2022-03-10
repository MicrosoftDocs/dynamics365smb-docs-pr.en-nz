---
title: Work with financial overviews in Excel
description: Learn about how you can open the financial statements in Microsoft Excel from Business Central for better analysis.
author: edupont04
ms.topic: overview
ms.search.keywords: accountant, accounting, financial report
ms.search.form: 9027
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: ac018d5477d42189d648936bfc7511f6214d52b5
ms.sourcegitcommit: ef80c461713fff1a75998766e7a4ed3a7c6121d0
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 02/15/2022
ms.locfileid: "8136156"
---
# <a name="analyzing-financial-statements-in-microsoft-excel"></a>Analysing Financial Statements in Microsoft Excel

In [!INCLUDE [prod_short](includes/prod_short.md)], you can see KPIs and get overviews of the company's financial state. You can also open lists in Excel and analyse the data there. But you can also export heavy financial statements such as the balance sheet or the income statement to Excel, analyse the data, and print the reports.  

In the Business Manager and Accountant Role Centres, you can choose which financial statements to view in Excel from a drop-down menu in the Reports section of the ribbon. When you choose a statement, it will be opened in Excel or Excel Online. An add-in connects the data to [!INCLUDE [prod_short](includes/prod_short.md)]. However, you have to sign in with the same account that you use with [!INCLUDE [prod_short](includes/prod_short.md)].  

## <a name="getting-the-overview-and-the-details-in-excel"></a>Getting the Overview and the Details in Excel

In the ribbon, choose the relevant Excel report, and let it open so you can get the overview that you were looking for. In this version of [!INCLUDE [prod_short](includes/prod_short.md)], we offer the following Excel reports:

- Balance Sheet  
- Income Statement  
- Cash Flow Statement  
- Retained Earnings Statement  
- Aged Accounts Payable  
- Aged Accounts Receivable  

Let's say you want to dig deeper into your cash flow. From the Business Manager or Accountant Role Centre, you can open the **Cash Flow Statement** report in Excel, but what actually happens is that we export the relevant data for you and create an Excel workbook based on a predefined template. Depending on your browser, you might be prompted to open or save the workbook.  

In Excel, you see a tab where the data is laid out for you on the first worksheet. All the data that was exported is also present in other worksheets in case you need it. You can print the report right away, or you can modify it until you have the overview and the details that you want. Use the [!INCLUDE [prod_short](includes/prod_short.md)] Excel Add-in to further filter and analyse data.  

### <a name="understanding-the-excel-templates"></a>Understanding the Excel templates

The predefined Excel reports are based on the data in the current company. For example, the demonstration company has set up the chart of accounts to list three cash accounts under *Current Assets*: 10100 **Current account**, 10200 **Saving account** and 10300 **Petty Cash**. The accounts have the **Account Subcategory** field set to *Cash*, and it's their combined amount that shows up as *Cash* in the **Balance Sheet** Excel report.  

Additional sheets in the Excel workbook show the data behind the report. But to find out what is hiding behind the groupings in the Excel reports, you might have to go back to [!INCLUDE [prod_short](includes/prod_short.md)] and apply filters to the lists, for example.  

## <a name="the-prod_short-excel-add-in"></a>The [!INCLUDE [prod_short](includes/prod_short.md)] Excel add-in

Your [!INCLUDE [prod_short](includes/prod_short.md)] experience includes an add-in for Excel. Depending on your subscription, you are logged in automatically, or you must specify the same login details that you use for [!INCLUDE [prod_short](includes/prod_short.md)]. For more information, see [Viewing and Editing in Excel From Business Central](across-work-with-excel.md).  

With the add-in, you can get fresh data from [!INCLUDE [prod_short](includes/prod_short.md)], and you can push changes back into [!INCLUDE [prod_short](includes/prod_short.md)]. However, the ability to push data back to the database is disabled for the financial Excel reports in the list above.  

## <a name="see-related-training-at-microsoft-learn"></a>See Related Training at [Microsoft Learn](/learn/modules/configure-powerbi-excel-dynamics-365-business-central/index)

## <a name="see-also"></a>See Also

[Viewing and Editing in Excel From Business Central](across-work-with-excel.md)  
[Finance](finance.md)  
[Setting Up Finance](finance-setup-finance.md)  
[The General Ledger and the Chart of Accounts](finance-general-ledger.md)  
[Working with Business Central](ui-work-product.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]