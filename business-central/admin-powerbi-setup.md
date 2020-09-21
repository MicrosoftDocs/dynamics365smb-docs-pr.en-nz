---
title: Enabling Power BI Integration With Business Central| Microsoft Docs
description: Getting insight, business intelligence, and KPIs from your Business Central data is easy with the Business Central apps for Power BI.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: account schedule, analysis, reporting, financial report, business intelligence, KPI
ms.date: 04/01/2020
ms.author: jswymer
ms.openlocfilehash: 92b3bb1d04c58332db20c978928fe1b04ed2ab37
ms.sourcegitcommit: aeaa0dc64e54432a70c4b0e1faf325cd17d01389
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 08/17/2020
ms.locfileid: "3697845"
---
# <a name="enabling-power-bi-integration-with-prodshort"></a>Enabling Power BI Integration With [!INCLUDE[prodshort](includes/prodshort.md)]

This article describes how to get [!INCLUDE[prodshort](includes/prodshort.md)] ready for integration with Power BI. [!INCLUDE[prodshort](includes/prodshort.md)] online is already enabled for integration, although there's some information about licensing that you might want to read. For [!INCLUDE[prodshort](includes/prodshort.md)] on-premises, you'll have set up your environment to connect to Power BI before users can work with it.

## <a name="power-bi-licensing"></a><a name="license"></a>Power BI Licensing

With [!INCLUDE[prodshort](includes/prodshort.md)], users get a free Power BI licence that provides access to the most common features in [!INCLUDE[prodshort](includes/prodshort.md)] and Power BI. You can also purchase a Power BI Pro licence that provides access to additional features. The following table provides an overview of the features available with each licence.

|Power Licence|View reports|Create reports|Share reports|Refresh reports| [!INCLUDE[prodshort](includes/prodshort.md)] Apps|
|-------------|--------||
|Power BI free|![cheque](media/check.png)|![cheque](media/check.png)|(limited)|(limited)||
|Power BI Pro|![cheque](media/check.png)|![cheque](media/check.png)|![cheque](media/check.png)|(extensive)|![cheque](media/check.png)|

For more information, see [Licensing the Power BI service for users in your organisation](/power-bi/admin/service-admin-licensing-organization) or [Sign up for the Power BI service as an individual](/power-bi/fundamentals/service-self-service-signup-for-power-bi).

## <a name="set-up-prodshort-on-premises-for-power-bi-integration"></a><a name="setup"></a>Set up [!INCLUDE[prodshort](includes/prodshort.md)] on-premises for Power BI integration

This section explains the requirements for a [!INCLUDE[prodshort](includes/prodshort.md)] on-premises deployment to integrate with Power BI.

1. OData web services and the ODataV4 endpoint are enabled.

    OData web service must be enabled on the [!INCLUDE[server](includes/server.md)], and OData port opened in firewall. For more information, see [Configuring Business Central Server - OData Web Services](/dynamics365/business-central/dev-itpro/administration/configure-server-instance#ODataServices).
    
    The local server must be accessible from the Internet.

2. [!INCLUDE[prodshort](includes/prodshort.md)] user accounts have web service access key.

    A web service access key is needed to view [!INCLUDE[prodshort](includes/prodshort.md)] data in Power BI. You can assign a web service access key to each user account. Or instead, create a specific account with a web service access key for use by all users. For more information, see [Web Services Authentication](/dynamics365/business-central/dev-itpro/webservices/web-services-authentication#generate-a-web-service-access-key).

3. NavUserPassword or Azure Active Directory Authentication is configured.

4. To view Power BI reports embedded in [!INCLUDE[prodshort](includes/prodshort.md)] pages, an application must be registered for [!INCLUDE[prodshort](includes/prodshort.md)] in Microsoft Azure.

    The registered application needs permission to Power BI services. For more information, see [Registering [!INCLUDE[prodshort](includes/prodshort.md)] On-Premises in Azure AD for Integrating with Other Services](/dynamics365/business-central/dev-itpro/administration/register-app-azure).

    > [!NOTE]
    > If your deployment uses NavUserPassword authentication, [!INCLUDE[prodshort](includes/prodshort.md)] connects to the same Power BI service for all users. You'll specify this service account as part of registering the application. With Azure AD authentication, [!INCLUDE[prodshort](includes/prodshort.md)] connects to the Power BI service associated with the individual user accounts.

    <!-- Windows authentication can also be used but you can't get data from BC in Power BI -->

## <a name="publish-data-as-web-services"></a>Publish data as web services

Codeunits, pages, and queries that you want to use as the data source in Power BI reports must be published as web services. There are many web services published by default. An easy way to find the web services is to search for *web services* in [!INCLUDE[prodshort](includes/prodshort.md)]. In the **Web Services** page, make sure the **Publish** field is selected for the web services listed above. This task is typically an administrative task.

For more information about publishing web services, see [Publish a Web Service](across-how-publish-web-service.md).

> [!TIP]
> To learn about what you can do to ensure the best performance of web services, as seen from the Business Central server (the endpoint) and from the consumer (the client), read [Writing efficient Web Services](/dynamics365/business-central/dev-itpro/performance/performance-developer#writing-efficient-web-services).




## <a name="see-related-training-at-microsoft-learn"></a>See Related Training at [Microsoft Learn](/learn/modules/Configure-powerbi-excel-dynamics-365-business-central/index)

## <a name="see-also"></a>See Also

[Business Central and Power BI](admin-powerbi.md)  
[Power BI Integration Component and Architecture Overview for [!INCLUDE[prodshort](includes/prodshort.md)]](admin-powerbi-overview.md)  
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
