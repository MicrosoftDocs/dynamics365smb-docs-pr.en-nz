---
title: Viewing and Editing in Excel From Business Central
description: Learn about how you can open the pages in Microsoft Excel from Business Central for better data analysis.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: accountant, accounting, financial report
ms.date: 04/01/2021
ms.author: jswymer
ms.openlocfilehash: 6bf12f55f6bce843c4ed12f2a40db542367fffde
ms.sourcegitcommit: a7cb0be8eae6ece95f5259d7de7a48b385c9cfeb
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 07/08/2021
ms.locfileid: "6443498"
---
# <a name="viewing-and-editing-in-excel-from-business-central"></a>Viewing and Editing in Excel From Business Central

With pages that display a list of records in rows and columns, like a list of customers, sale orders, or invoices, you can also view the records using Microsoft Excel. Depending on the page, you have two options for viewing in Excel. You can either select the **Open in Excel** action or the **Edit in Excel** action on the page. This article explains the differences between the two actions.

## <a name="open-in-excel"></a>Open in Excel

With the **Open in Excel** action, you can make changes to the records in Excel, but you can't publish the changes back to [!INCLUDE[prod_short](includes/prod_short.md)]. You can only save the changes to Excel file on your computer.

- With this action, Excel respects any filters on the page that limit the records shown. The Excel workbook will contain the same rows and columns that appear on the page in [!INCLUDE[prod_short](includes/prod_short.md)].

- This action works on both on Windows and macOS.

- Starting with update 18.3, you can also view lists that are shown in page parts, like the lines in a sales order. For now, this capability is an optional feature, which requires that you enable **Export any list part to Excel** in **Feature Management**. For more information, see [Enabling Upcoming Features Ahead of Time](/dynamics365/business-central/dev-itpro/administration/feature-management). 

> [!NOTE]
> For [!INCLUDE[prod_short](includes/prod_short.md)] on-premises, the **Open in Excel** action is available by default. However, if you set up [!INCLUDE[prod_short](includes/prod_short.md)] on-premises for editing data in Excel, then the **Open in Excel** action is replaced by the **Edit in Excel** action.

[!INCLUDE [send-report-excel](includes/send-report-excel.md)]  

## <a name="edit-in-excel"></a>Edit in Excel

With the **Edit in Excel** action, you make changes to records in Excel and then publish the changes back to [!INCLUDE[prod_short](includes/prod_short.md)].

- With this action, Excel respects most filters on the page that limit the records shown, so the Excel workbook will contain almost the same records and columns.

- It only works on Windows; not macOS.

- You can switch the company that you are working with. To switch company, select the **Options** icon ![Excel add-in options.](media/cogwheel.png "Excel add-in options") in the Excel Add-in pane, then select the company from the **Company** field.  

    > [!IMPORTANT]
    > When changing the company, make sure that the **Environment** field is not empty. If it is, then set it to one of the available options; otherwise, the add-in will not work correctly.  

If you make changes to the add-in, you must reload it to update the connection. To reload, use the ![Excel add-in menu](media/excel-addin-menu.png "Excel add-in menu") menu in the top-right corner of the add-in. If you cannot load the add-in, talk to your administrator. If you are the administrator, see [Setting up the Excel Add-In for Editing Business Central Data](/dynamics365/business-central/dev-itpro/administration/configuring-excel-addin).

> [!NOTE]
> For [!INCLUDE[prod_short](includes/prod_short.md)] on-premises, the **Edit in Excel** action is only available if the Excel add-in has been configured by your administrator, and only available for the Web client. For administrators, if you want to learn how to install the Excel add-in, see [Setting up the Excel Add-In for Editing Business Central Data](/dynamics365/business-central/dev-itpro/administration/configuring-excel-addin).

### <a name="see-the-differences-between-the-options"></a>See the differences between the options
<br><br>  

> [!Video https://go.microsoft.com/fwlink/?linkid=2086039]

## <a name="see-related-training-at-microsoft-learn"></a>See Related Training at [Microsoft Learn](/learn/modules/configure-powerbi-excel-dynamics-365-business-central/index)

## <a name="see-also"></a>See Also

[Analysing Financial Statements in Microsoft Excel](finance-analyze-excel.md)  
[Working with Business Central](ui-work-product.md)  
[Enhancements to Excel integration in 2019 release wave 2](/dynamics365-release-plan/2019wave2/dynamics365-business-central/enhancements-excel-integration)  


[!INCLUDE[footer-include](includes/footer-banner.md)]