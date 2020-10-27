---
title: Introduction to Business Central and Power BI| Microsoft Docs
description: Getting insight, business intelligence, and KPIs from your Business Central data is easy with the Business Central apps for Power BI.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: account schedule, analysis, reporting, financial report, business intelligence, KPI
ms.reviewer: edupont
ms.date: 10/01/2020
ms.author: jswymer
ms.openlocfilehash: e339033e8529f59f548e8bf71fd683f9a2a17eba
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 10/01/2020
ms.locfileid: "3917892"
---
# <a name="prodshort-and-power-bi"></a>[!INCLUDE[prodshort](includes/prodshort.md)] and Power BI

Getting insights into your [!INCLUDE[prodshort](includes/prodshort.md)] data is easy with [Power BI](https://powerbi.microsoft.com) - a data visualization system from Microsoft. Power BI retrieves [!INCLUDE[prodshort](includes/prodshort.md)] data allowing you to build dashboards and reports based on that data. Power BI provides a flexible alternative to reports built in [!INCLUDE[prodshort](includes/prodshort.md)], enabling you drill down and customise the visualisation, and even merge data from different companies in [!INCLUDE[prodshort](includes/prodshort.md)]. Some Power BI reports can also be embedded in Business Central and viewed without leaving the system. More complex dashboards are better experienced from the Power BI web site.

![Power BI and Business Central](media/power-bi-intro.png)


## <a name="what-you-can-do-with-power-bi-and-prodshort"></a>What you can do with Power BI and [!INCLUDE[prodshort](includes/prodshort.md)]

There are various features for working with [!INCLUDE[prodshort](includes/prodshort.md)] and Power BI. Some things you can do from Power BI, while other things are done from [!INCLUDE[prodshort](includes/prodshort.md)]. Also, some features are only available with [!INCLUDE[prodshort](includes/prodshort.md)] online, not on-premises. The following table gives you an overview.

|Feature|Description|Online|On-premises|More information|
|-------|-----------|--------------|-----------|----------------|
|View [!INCLUDE[prodshort](includes/prodshort.md)] data in Power BI|You can view your data from [!INCLUDE[prodshort](includes/prodshort.md)] in reports in Power BI. [!INCLUDE[prodshort](includes/prodshort.md)] online includes some predefined Power BI reports. Or your organisation might have made some custom reports available to you.|![Works online](media/check.png)|![Works on-premises](media/check.png)|[See...](across-working-with-powerbi.md)|
|View Power BI reports in the [!INCLUDE[prodshort](includes/prodshort.md)] client.| Power BI reports that display [!INCLUDE[prodshort](includes/prodshort.md)] data can be embedded directly in parts [!INCLUDE[prodshort](includes/prodshort.md)] pages. You can switch the part to display any report that is made available to you. |![works online](media/check.png)|![Works on-premises](media/check.png)<sup>[*](#onprem)</sup>|[See...](across-working-with-business-central-in-powerbi.md).|
|Create reports and dashboards in Power BI that display [!INCLUDE[prodshort](includes/prodshort.md)] data.|Use Power BI Desktop to create your own reports and dashboards. You can publish the reports to your own Power BI Service or share them with others within your organisation.|![Works online](media/check.png)|![works on-premises](media/check.png)|[See...](across-how-use-financials-data-source-powerbi.md)
|[!INCLUDE[prodshort](includes/prodshort.md)] apps in Power BI| [!INCLUDE[prodshort](includes/prodshort.md)] publishes three apps for Power BI on Microsoft AppSource. These apps create detailed reports and dashboards in your Power BI service for viewing [!INCLUDE[prodshort](includes/prodshort.md)] data. Available apps include: <ul><li>[!INCLUDE [prodlong](includes/prodlong.md)] - CRM </li><li>[!INCLUDE [prodlong](includes/prodlong.md)] - Finance </li><li>[!INCLUDE [prodlong](includes/prodlong.md)] - Sales </li></ul>  |![Works online](media/check.png)||[See...](across-powerbi-business-central-apps.md)

<a name="onprem"><sup>*</sup></a> This feature requires a registered application for Business Central in Microsoft Azure. For more information, see [Registering Business Central On-Premises in Azure AD for Integrating with Other Services](/dynamics365/business-central/dev-itpro/administration/register-app-azure).

## <a name="getting-ready-to-use-power-bi"></a>Getting ready to use Power BI

There are a few tasks that must be done before you can start using Power BI with [!INCLUDE[prodshort](includes/prodshort.md)]. Some of the tasks are typically only done by administrators or super users.

1. If you're using [!INCLUDE[prodshort](includes/prodshort.md)] on-premises, make sure your deployment meets the requirements outlined in [Set up [!INCLUDE[prodshort](includes/prodshort.md)] on-premises for Power BI integration](admin-powerbi-setup.md#setup). This task is typically an administrative task.

2. Publish data as web services.

    Codeunits, pages, and queries that you want to use as the data source in Power BI reports must be published as web services. There are many web services published by default. An easy way to find the web services is to search for *web services* in [!INCLUDE[prodshort](includes/prodshort.md)].
    
    For more information about publishing web services, see [Publish a Web Service](across-how-publish-web-service.md).

3. Get a Power BI account.

    To do anything with Power BI and [!INCLUDE[prodshort](includes/prodshort.md)], whether you're an administrator or just a consumer, you'll need Power BI service account. To get an account, go to [https://powerbi.microsoft.com](https://powerbi.microsoft.com). To sign up for an account, use your work email address and password. Sign-up requires that you have a licence, but in most cases you should already have a free licence. For more information, see [Power BI Licensing](admin-powerbi-setup.md#license).

4. If you want to create your own Power BI reports, get Power BI Desktop.

    You can download [Power BI Desktop](https://powerbi.microsoft.com/desktop/). For more information, see [Get Power BI Desktop](/power-bi/fundamentals/desktop-get-the-desktop).

## <a name="see-related-training-at-microsoft-learn"></a>See Related Training at [Microsoft Learn](/learn/modules/configure-powerbi-excel-dynamics-365-business-central/index)

## <a name="see-also"></a>See Also

[Power BI for consumers](/power-bi/consumer/end-user-consumer)  
[The 'new look' of the Power BI service](/power-bi/service-new-look)  
[Quickstart: Connect to data in Power BI Desktop](/power-bi/desktop-quickstart-connect-to-data)  
[Power BI documentation](/power-bi/)  
[Business Intelligence](bi.md)  
[Getting Started](product-get-started.md)  
[Importing Business Data from Other Finance Systems](across-import-data-configuration-packages.md)  
[Setting Up [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)  
[Using [!INCLUDE[d365fin](includes/d365fin_md.md)] as a Power BI Data Source](across-how-use-financials-data-source-powerbi.md)  
[Using [!INCLUDE[d365fin](includes/d365fin_md.md)] as a Power Apps Data Source](across-how-use-financials-data-source-powerapps.md)  
[Using [!INCLUDE[d365fin](includes/d365fin_md.md)] in Power Automate](across-how-use-financials-data-source-flow.md)  

## [!INCLUDE[d365fin](includes/free_trial_md.md)]  
