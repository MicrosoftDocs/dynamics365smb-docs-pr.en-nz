---
title: Display Custom Power BI Reports| Microsoft Docs
description: You can use Power BI reports to gain additional insight into data in lists in Financials.
services: project-madeira
documentationcenter: 
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: business intelligence, KPI, Odata, Power App, SOAP, analysis
ms.date: 06/02/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 00629240e565da65ccc7d213d0e24cfebf33fac6
ms.contentlocale: en-nz
ms.lasthandoff: 03/22/2018

---
# <a name="viewing-list-data-in-power-bi-reports-in-business-central"></a>Viewing List Data in Power BI Reports in Business Central 
[!INCLUDE[d365fin](includes/d365fin_md.md)] includes a FactBox control element on a number of key list pages that provides additional insight into the data in the list. As you move between rows in the list, the report is updated and filtered for the selected entry. You can create custom reports to display in this control, but there are a few rules to follow when creating the reports to ensure they provide the desired behaviour.  

> [!NOTE]  
>   You must have a valid account with [!INCLUDE[d365fin](includes/d365fin_md.md)] and with Power BI. Also, you must download [Power BI Desktop](https://powerbi.microsoft.com/en-us/desktop/). For more information, see [Using [!INCLUDE[d365fin](includes/d365fin_md.md)] as a Power BI Data Source](across-how-use-financials-data-source-powerbi.md).  

## <a name="report-data-set"></a>Report Data Set
When you create the report in Power BI Desktop, specify the data source or web service that contains the data related to the list that you want to associate the report with. For example, if you want to create a report for the Sales List, ensure that the data set contains information related to sales.  

To filter data on the reports based upon the record selected from the list page, the primary key must be used as a report filter. The primary keys will need to be part of your data set in order for the reports to filter correctly. In most cases, the primary key for a list is the **No.** field.  

## <a name="defining-the-report-filter"></a>Defining the Report Filter
The report is required to have a basic report filter (not a page or visual filter and not advanced filter) to filter correctly in the Power BI Fact Box Control. The filter that is passed to the Power BI report from each list page will be based on the primary key as described in the previous section.  

To define a filter for the report, select the primary key from the list of available fields, and then drag and drop that field into the **Report Filter** section.  

![Setting the report filter for the Sales Invoice Activity report](./media/across-how-use-powerbi-reports-factbox/financials-powerbi-report-filter.png)

## <a name="report-size-and-color"></a>Report Size and colour
The size of the report must be set to 325 pixels by 310 pixels. This is required for the proper scaling of the report in the available space allowed by the Power BI Fact Box control. To define the size of the report, place focus outside of the report layout area, and then choose the paint roller icon.

![Setting the report width and height for the Sales Invoice Activity report](./media/across-how-use-powerbi-reports-factbox/financials-powerbi-report-sizing.png)

You can change the width and height of the report by choosing **Custom** in the **Type** field.

Similarly, if you want to have the background of the report blend into the background color of the Power BI Fact Box control, define a custom report background color of *E5E5E5*. This is optional.  

## <a name="reports-with-multiple-pages"></a>Reports with Multiple Pages
With Power BI, you can create a single report with multiple pages. The visuals that you want to see in the [!INCLUDE[d365fin](includes/d365fin_md.md)] list pages must be on the first page of the report in Power BI.  

> [!NOTE]  
>  The Power BI Fact Box can show only the first page of your report; if you want to see other pages, you must expand the report and use tabs at the bottom of the report to navigate to other pages.  

## <a name="saving-your-report"></a>Saving Your Report

When you save your report, it's a best practice that the name of the report contains the name of the list page that you want to display the report in. For example, the word *Vendor* must be contained somewhere in the report name for reports that you want to make available on the Vendor list.  

This is not a requirement; however, it will make the process of selecting reports quicker. When the report selection page is opened from a list page, we will pass in a filter based on the page name to limit the reports that are displayed.  You may remove the filter to get a full list of reports available to you in Power BI.  

## <a name="troubleshooting"></a>Troubleshooting
This section provides a workaround for the most typical issues that can occur when you create the Power BI report.  

**User does not see a report on the Select Report page they want to select** If you cannot select a report, a possible solution is to verify the name of the report to ensure it contains the name of the list page. You can also clear the filter to get a full list of Power BI reports available.  

**Report is loaded but blank, not filtered or filtered incorrectly** Verify that the report filter contains the right primary key. In most cases, this is the **No.** field, but in the **G/L Entry** table, for example, you must use the **Entry No.** field  .

**Report is loaded, but it shows the page you have not expected** Verify that the page you want displayed is the first page in your report.  

**Report appears with unwanted gray boarders, is too small or too large**

Verify that the report size is set to 325 pixels x 310 pixels. Save the report, and then refresh the list page.  

## <a name="see-also"></a>See Also
[Using [!INCLUDE[d365fin](includes/d365fin_md.md)] as a Power BI Data Source](across-how-use-financials-data-source-powerbi.md)  
[Welcome to [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)    
[Setting Up [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)    
[Finance](finance.md)  

