---
title: Introduction to Business Central and Power BI
description: 'Get an overview of using Power BI to get insight, business intelligence, and KPIs from your Business Central data.'
author: jswymer
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 'account schedule, analysis, reporting, financial report, business intelligence, KPI'
ms.search.form: '6316, 6317'
ms.reviewer: edupont
ms.date: 08/30/2022
ms.author: jswymer
---
# Introduction to [!INCLUDE[prod_short](includes/prod_short.md)] and Power BI

It's easy to get insights into your [!INCLUDE[prod_short](includes/prod_short.md)] data with [Power BI](https://powerbi.microsoft.com) - a data visualization system from Microsoft. Power BI retrieves [!INCLUDE[prod_short](includes/prod_short.md)] data so that you can build dashboards and reports based on that data. Power BI provides a flexible alternative to reports built in [!INCLUDE[prod_short](includes/prod_short.md)], enabling you drill down and customise the visualisation, and even merge data from different companies in [!INCLUDE[prod_short](includes/prod_short.md)]. Some Power BI reports can also be embedded in Business Central and viewed without leaving the system. More complex dashboards are better experienced from the Power BI web site.

![Power BI and Business Central.](media/power-bi-intro.png)

## What you can do with Power BI and [!INCLUDE[prod_short](includes/prod_short.md)]

There are various features for working with [!INCLUDE[prod_short](includes/prod_short.md)] and Power BI. Some things you can do from Power BI, while other things are done from [!INCLUDE[prod_short](includes/prod_short.md)]. Also, some features are only available with [!INCLUDE[prod_short](includes/prod_short.md)] online, not on-premises. The following table gives you an overview.

|Feature|Description|Online|On-premises|Learn more|
|-------|-----------|--------------|-----------|----------------|
|View [!INCLUDE[prod_short](includes/prod_short.md)] data in Power BI|You can view your data from [!INCLUDE[prod_short](includes/prod_short.md)] in reports in Power BI. [!INCLUDE[prod_short](includes/prod_short.md)] online includes some predefined Power BI reports. Or your organisation might have made some custom reports available to you.|![Works online.](media/check.png)|![Works on-premises](media/check.png)|[Here...](across-working-with-business-central-in-powerbi.md)|
|View Power BI reports in the [!INCLUDE[prod_short](includes/prod_short.md)] client.| Power BI reports that display [!INCLUDE[prod_short](includes/prod_short.md)] data can be embedded directly in parts [!INCLUDE[prod_short](includes/prod_short.md)] pages. You can switch the part to display any report that is made available to you. |![works online.](media/check.png)|![Works on-premises](media/check.png)<sup>[*](#onprem)</sup>|[Here...](across-working-with-powerbi.md).|
|Create reports and dashboards in Power BI that display [!INCLUDE[prod_short](includes/prod_short.md)] data.|Use Power BI Desktop to create your own reports and dashboards. You can publish the reports to your own Power BI Service or share them with others within your organisation.|![Works online.](media/check.png)|![works on-premises](media/check.png)|[Here...](across-how-use-financials-data-source-powerbi.md)|
|[!INCLUDE[prod_short](includes/prod_short.md)] apps in Power BI| [!INCLUDE[prod_short](includes/prod_short.md)] publishes three apps for Power BI on Microsoft AppSource. These apps create detailed reports and dashboards in your Power BI service for viewing [!INCLUDE[prod_short](includes/prod_short.md)] data. Available apps include: <ul><li>[!INCLUDE [prod_long](includes/prod_long.md)] - CRM </li><li>[!INCLUDE [prod_long](includes/prod_long.md)] - Finance </li><li>[!INCLUDE [prod_long](includes/prod_long.md)] - Sales </li></ul>  |![Works online.](media/check.png)||[Here...](across-powerbi-business-central-apps.md)|
|Work with [!INCLUDE [prod_short](includes/prod_short.md)] data in datamarts and dataflows|Starting in July 2022, you can use the [!INCLUDE [prod_short](includes/prod_short.md)] connector in Power Query Online to dataflows that you share across different reports and dashboards.|[Here...](across-powerbi-business-central-apps.md)|

<a name="onprem"><sup>*</sup></a> This feature requires a registered application for Business Central in Microsoft Azure. For more information, see [Registering Business Central On-Premises in Azure AD for Integrating with Other Services](/dynamics365/business-central/dev-itpro/administration/register-app-azure).

## Get ready to use Power BI

There are a few tasks that must be done before you can start using Power BI with [!INCLUDE[prod_short](includes/prod_short.md)]. <!-- Some of the tasks are typically only done by administrators or super users.--> The tasks will depend on your role in your organisation, and what you want to do with Power BI:

- As a *business user*, you want to view Power BI reports, either in the Power BI Service or in Business Central
- As an *administrator*, you're responsible for the management of the organisation-wide settings that control how Business Central and Power BI work.
- As a *report creator*, you want to build custom Power BI reports that you can share with other users.

|Task|Business user|Administrator|Report creator|More information|
|----|-------------|-------------|-----------------------|----------------|
|Get a Power BI account.|![yet another checkmark.](media/check.png)|![it's a checkmark](media/check.png)|![again a checkmark](media/check.png)|Go to [https://powerbi.microsoft.com](https://powerbi.microsoft.com). To sign up for an account, use your work email address and password. <br /><br/>Sign-up requires that you have a licence, but in most cases you should already have a free licence, For more information, see [Power BI Licensing](admin-powerbi-setup.md#license).|
|Get Power BI Desktop|||![again a checkmark.](media/check.png)|To download, go to [Power BI Desktop](https://powerbi.microsoft.com/desktop/). For more information, see [Get Power BI Desktop](/power-bi/fundamentals/desktop-get-the-desktop).
|Expose Business Central data to Power BI||![it's a checkmark.](media/check.png)|![again a checkmark](media/check.png)|[Expose data through API pages or OData web services](admin-powerbi-setup.md#exposedata)
|Enable Power BI integration<br />(on-premises only)||![it's a checkmark.](media/check.png)||[Set up Business Central on-premises for Power BI integration](admin-powerbi-setup.md#setup)|


<!--



1. If you're using [!INCLUDE[prod_short](includes/prod_short.md)] on-premises, make sure your deployment meets the requirements outlined in [Set up [!INCLUDE[prod_short](includes/prod_short.md)] on-premises for Power BI integration](admin-powerbi-setup.md#setup). This task is typically an administrative task.

2. Expose Business Central data through API pages or published web services.

    Business Central online automatically included several pages as APIs. For more information, see [Business Central API V2.0](/dynamics365/business-central/dev-itpro/api-reference/v2.0/). Application developers for Business Central online can create custom API pages that you can then consume in reports. For more information, see [Developing a Custom API](/dynamics365/business-central/dev-itpro/developer/devenv-develop-custom-api).

   Codeunit, page, and query objects can be published as OData web services. There are many web services published by default. An easy way to find the web services is to search for *web services* in [!INCLUDE[prod_short](includes/prod_short.md)]. For more information about publishing web services, see [Publish a Web Service](across-how-publish-web-service.md).

3. Get a Power BI account.

   To do anything with Power BI and [!INCLUDE[prod_short](includes/prod_short.md)], whether you're an administrator or just a consumer, you'll need Power BI service account. To get an account, go to [https://powerbi.microsoft.com](https://powerbi.microsoft.com). To sign up for an account, use your work email address and password. Sign-up requires that you have a license, but in most cases you should already have a free license. For more information, see [Power BI Licensing](admin-powerbi-setup.md#license).

4. If you want to create your own Power BI reports, get Power BI Desktop.

   You can download [Power BI Desktop](https://powerbi.microsoft.com/desktop/). For more information, see [Get Power BI Desktop](/power-bi/fundamentals/desktop-get-the-desktop).

-->

## See related [Microsoft training](/training/modules/configure-powerbi-excel-dynamics-365-business-central/index)

## See Also

[Business Intelligence](bi.md)  
[Get Ready for Doing Business](ui-get-ready-business.md)  
[Import Business Data from Other Finance Systems](across-import-data-configuration-packages.md)  
[Set Up [!INCLUDE[prod_short](includes/prod_short.md)]](setup.md)  
[Use [!INCLUDE[prod_short](includes/prod_short.md)] as a Power BI Data Source](across-how-use-financials-data-source-powerbi.md)  
[Use [!INCLUDE[prod_short](includes/prod_short.md)] as a Power Apps Data Source](across-how-use-financials-data-source-powerapps.md)  
[Use [!INCLUDE[prod_short](includes/prod_short.md)] in Power Automate](across-how-use-financials-data-source-flow.md)  
[Power BI documentation](/power-bi/)  
[What is Power BI?](/power-bi/fundamentals/power-bi-overview)  
[Quickstart: Connect to data in Power BI Desktop](/power-bi/desktop-quickstart-connect-to-data)  
[Introduction to datamarts](/power-bi/transform-model/datamarts/datamarts-overview)  
[Introduction to dataflows and self-service data prep](/power-bi/transform-model/dataflows/dataflows-introduction-self-service)  



[!INCLUDE[footer-include](includes/footer-banner.md)]
