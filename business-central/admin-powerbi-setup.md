---
title: Enabling Power BI Integration With Business Central
description: Learn how to set up the connection to Power Bi so you can get insights, business intelligence, and KPIs from your Business Central data with the Business Central apps for Power BI.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: account schedule, analysis, reporting, financial report, business intelligence, KPI
ms.date: 10/01/2020
ms.author: jswymer
ms.openlocfilehash: dd0974c20f8c038fcc0cac27c9ef165b2aadcd36
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 12/17/2020
ms.locfileid: "4752516"
---
# <a name="enabling-power-bi-integration-with-prod_short"></a>Enabling Power BI Integration With [!INCLUDE[prod_short](includes/prod_short.md)]

This article describes how to get [!INCLUDE[prod_short](includes/prod_short.md)] ready for integration with Power BI. [!INCLUDE[prod_short](includes/prod_short.md)] online is already enabled for integration, although there's some information about licensing that you might want to read. For [!INCLUDE[prod_short](includes/prod_short.md)] on-premises, you'll have set up your environment to connect to Power BI before users can work with it.

## <a name="power-bi-licensing"></a><a name="license"></a>Power BI Licensing

With [!INCLUDE[prod_short](includes/prod_short.md)], users get a free Power BI licence that provides access to the most common features in [!INCLUDE[prod_short](includes/prod_short.md)] and Power BI. You can also purchase a Power BI Pro licence that provides access to additional features. The following table provides an overview of the features available with each licence.

|Power Licence|View reports|Create reports|Share reports|Refresh reports| [!INCLUDE[prod_short](includes/prod_short.md)] Apps|
|-------------|--------||
|Power BI free|![a checkmark](media/check.png)|![another checkmark](media/check.png)|(limited)|(limited)||
|Power BI Pro|![yet another checkmark](media/check.png)|![it's a checkmark](media/check.png)|![again a checkmark](media/check.png)|(extensive)|![last checkmark](media/check.png)|

For more information, see [Licensing the Power BI service for users in your organisation](/power-bi/admin/service-admin-licensing-organization) or [Sign up for the Power BI service as an individual](/power-bi/fundamentals/service-self-service-signup-for-power-bi).

## <a name="set-up-prod_short-on-premises-for-power-bi-integration"></a><a name="setup"></a>Set up [!INCLUDE[prod_short](includes/prod_short.md)] on-premises for Power BI integration

This section explains the requirements for a [!INCLUDE[prod_short](includes/prod_short.md)] on-premises deployment to integrate with Power BI.

1. OData web services and the ODataV4 endpoint are enabled.

    OData web service must be enabled on the [!INCLUDE[server](includes/server.md)], and OData port opened in firewall. For more information, see [Configuring Business Central Server - OData Web Services](/dynamics365/business-central/dev-itpro/administration/configure-server-instance#ODataServices).
    
    The local server must be accessible from the Internet.

2. [!INCLUDE[prod_short](includes/prod_short.md)] user accounts have web service access key.

    A web service access key is needed to view [!INCLUDE[prod_short](includes/prod_short.md)] data in Power BI. You can assign a web service access key to each user account. Or instead, create a specific account with a web service access key for use by all users. For more information, see [Web Services Authentication](/dynamics365/business-central/dev-itpro/webservices/web-services-authentication#generate-a-web-service-access-key).

3. NavUserPassword or Azure Active Directory Authentication is configured.

4. To view Power BI reports embedded in [!INCLUDE[prod_short](includes/prod_short.md)] pages, an application must be registered for [!INCLUDE[prod_short](includes/prod_short.md)] in Microsoft Azure.

    The registered application needs permission to Power BI services. For more information, see [Registering [!INCLUDE[prod_short](includes/prod_short.md)] On-Premises in Azure AD for Integrating with Other Services](/dynamics365/business-central/dev-itpro/administration/register-app-azure).

    > [!NOTE]
    > If your deployment uses NavUserPassword authentication, [!INCLUDE[prod_short](includes/prod_short.md)] connects to the same Power BI service for all users. You'll specify this service account as part of registering the application. With Azure AD authentication, [!INCLUDE[prod_short](includes/prod_short.md)] connects to the Power BI service associated with the individual user accounts.

    <!-- Windows authentication can also be used but you can't get data from BC in Power BI -->

## <a name="publish-data-as-web-services"></a>Publish data as web services

Codeunits, pages, and queries that you want to use as the data source in Power BI reports must be published as web services. There are many web services published by default. An easy way to find the web services is to search for *web services* in [!INCLUDE[prod_short](includes/prod_short.md)]. In the **Web Services** page, make sure the **Publish** field is selected for the web services listed above. This task is typically an administrative task.

For more information about publishing web services, see [Publish a Web Service](across-how-publish-web-service.md).

> [!TIP]
> To learn about what you can do to ensure the best performance of web services, as seen from the Business Central server (the endpoint) and from the consumer (the client), read [Writing efficient Web Services](/dynamics365/business-central/dev-itpro/performance/performance-developer#writing-efficient-web-services).




## <a name="see-related-training-at-microsoft-learn"></a>See Related Training at [Microsoft Learn](/learn/modules/Configure-powerbi-excel-dynamics-365-business-central/index)

## <a name="see-also"></a>See Also

[Business Central and Power BI](admin-powerbi.md)  
[Power BI Integration Component and Architecture Overview for [!INCLUDE[prod_short](includes/prod_short.md)]](admin-powerbi-overview.md)  
[Power BI for consumers](/power-bi/consumer/end-user-consumer)  
[The 'new look' of the Power BI service](/power-bi/service-new-look)  
[Quickstart: Connect to data in Power BI Desktop](/power-bi/desktop-quickstart-connect-to-data)  
[Power BI documentation](/power-bi/)  
[Business Intelligence](bi.md)  
[Getting Started](product-get-started.md)  
[Importing Business Data from Other Finance Systems](across-import-data-configuration-packages.md)  
[Setting Up [!INCLUDE[prod_short](includes/prod_short.md)]](setup.md)  
[Using [!INCLUDE[prod_short](includes/prod_short.md)] as a Power BI Data Source](across-how-use-financials-data-source-powerbi.md)  
[Using [!INCLUDE[prod_short](includes/prod_short.md)] as a Power Apps Data Source](across-how-use-financials-data-source-powerapps.md)  
[Using [!INCLUDE[prod_short](includes/prod_short.md)] in Power Automate](across-how-use-financials-data-source-flow.md)  

## [!INCLUDE[prod_short](includes/free_trial_md.md)]  


[!INCLUDE[footer-include](includes/footer-banner.md)]