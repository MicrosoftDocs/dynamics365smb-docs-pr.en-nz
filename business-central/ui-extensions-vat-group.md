---
title: The GST Group Management Extension
description: You can engage with other businesses to form a GST group and act as either a member or representative of the group when reporting GST.
author: bholtorf
manager: annbe
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: 'VAT, value added tax, report'
ms.date: 04/01/2021
ms.author: bholtorf
---

# <a name="the-vat-group-management-extension"></a>The GST Group Management Extension

You can join one or more businesses in your country to consolidate GST reporting under a single registration number. This type of arrangement is known as a *GST group*. You can engage with the group as a member or the group representative.

## <a name="forming-a-vat-group"></a>Forming a GST Group
GST group members and the group representative can use the **GST Group Management Setup** assisted setup guide to define their engagement with the group and create a connection between their [!INCLUDE[prod_short](includes/prod_short.md)] tenants. The group members will use the connection to submit their GST returns to the group representative. The representative will submit GST to tax authorities on behalf of the group using a single GST return. 

## <a name="vat-group-constellations"></a>GST Group Constellations
Communication happens from group members to the representative. The group representative exposes an API that allows the members to submit their GST returns to the GST group representative. 
[!INCLUDE[prod_short](includes/prod_short.md)] supports inter-group GST return submissions for companies using [!INCLUDE[prod_short](includes/prod_short.md)] on-premises or online and in any combination. The setup of the communication depends on the constellation. The following sections describe how to set up various group constellations.

The following list shows the recommended order of the steps to set up a GST group:

1. Create the setup in Azure Active Directory. For more information, see [Requirements for Authentication](ui-extensions-vat-group.md#requirements-for-authentication).
2. Share the technical information that GST group members and the representative need to connect their [!INCLUDE[prod_short](includes/prod_short.md)] tenants. Usually, the GST group representative has this information, such as the name of the GST group representative's environment to which the GST group members will submit GST.
3. Create users in the GST group representative's [!INCLUDE[prod_short](includes/prod_short.md)] that GST group members can use to authenticate and connect.
4. Run the **Set up GST Group Management** assisted setup guide to connect the GST group members.

  The guide requires some information from the GST group representative. For more information, see the [GST Group Member Setup](#vat-group-member-setup) section. Make a note of the **Group Member ID** for each GST group member. The representative needs these IDs to add the companies to the GST group.
5. Set up the GST Group Management extension in the GST group representative's [!INCLUDE[prod_short](includes/prod_short.md)] by using the **Set up GST Group Management** assisted setup guide. 

> [!NOTE]
> To connect to the GST group representative, group members need a user with access to the GST group representative's [!INCLUDE[prod_short](includes/prod_short.md)]. The GST group representative must create at least one user for this, however, for security reasons we recommended that you create a user for each GST group member. Make sure to distribute the credentials for these users to GST group members in a secure way.

## <a name="understanding-the-vat-group-management-setup"></a>Understanding the GST Group Management Setup

The GST group representative exposes an API that GST group members can use to connect to their [!INCLUDE[prod_short](includes/prod_short.md)] tenant and submit GST returns. GST group members will often use [!INCLUDE[prod_short](includes/prod_short.md)] in separate Azure Active Directory tenants. Therefore, more setup is needed to make a connection between the GST group member and representative's [!INCLUDE[prod_short](includes/prod_short.md)]. 
  
GST group members connect to the representative by calling a web service on the GST group representative tenant. The caller must be authenticated using OAuth. When the GST Group Management extension is set up, you will be asked to authenticate to the GST group representative to get and save an access token. This access token is used when submitting GST returns to the GST group representative. 

Authentication is handled by Azure Active Directory, so your setup must be made in the GST group representative's Azure Active Directory to allow connections. An Azure Active Directory app registration must be configured with access to the GST group representative's [!INCLUDE[prod_short](includes/prod_short.md)]. This is also true if the GST group representative is using [!INCLUDE[prod_short](includes/prod_short.md)] on-premises. Additionally, you must configure Single Sign-On if the GST group representative is using [!INCLUDE[prod_short](includes/prod_short.md)] on-premises.

> [!NOTE]
> For a limited time, authentication using a web service access key is also supported. For more information, see [Deprecated Features in 2021 release wave 1](/dynamics365/business-central/dev-itpro/upgrade/deprecated-features-w1#deprecated-features-in-2021-release-wave-1).

## <a name="requirements-for-authentication"></a>Requirements for Authentication 
When the GST group representative is using [!INCLUDE[prod_short](includes/prod_short.md)] online or on-premises, GST group members use Azure Active Directory to authenticate when they submit GST returns to the GST group representative. If the GST group members are also using [!INCLUDE[prod_short](includes/prod_short.md)] online, the GST group member can authenticate using the designated user credentials and the endpoint information. For more information, see [GST Group Member Setup](ui-extensions-vat-group.md#vat-group-member-setup).

GST group members who have [!INCLUDE[prod_short](includes/prod_short.md)] on-premises must set up an app registration in Azure Active Directory for the GST group representative's [!INCLUDE[prod_short](includes/prod_short.md)] tenant. The app registration will enable the GST group representative's [!INCLUDE[prod_short](includes/prod_short.md)] online to authenticate the group member. For more information, see [Quickstart: Register an application with the Microsoft identity platform](/azure/active-directory/develop/quickstart-register-app).

When you create the app registration in Azure Active Directory, you must specify the following.

* In the **Authentication** section, add **Web** as a platform, and use the following **Redirect URL**: https://businesscentral.dynamics.com/OAuthLanding.htm.
* In the **Authentication** section, in the option to select **Supported account types**, select **Accounts in any organisational directory (Any Azure AD directory - Multitenant)**.
* In the **Certificates & secrets** section, create a new client secret and note the value. The GST group members will need the secret when they set up the connection to the group representative.
* In the **API permissions** section, add permissions to [!INCLUDE[prod_short](includes/prod_short.md)]. Enable delegated access to **Financials.ReadWrite.All** and **user_impersonation**.
* In the **Overview** section, note the **Application (client) ID**. The GST group members will need the ID when they set up the connection to the group representative. 

## <a name="vat-group-member-setup"></a>GST Group Member Setup
Set up the GST group member by starting the **Set up GST Group Management** assisted setup guide. 

> [!NOTE]
> Before you get started, contact the GST group representative for the following information about their [!INCLUDE[prod_short](includes/prod_short.md)] tenant:
>
> * The API URL
> * The name of their company 
> * Client ID
> * Client secret
> * Sign in credentials for the dedicated user 

1. To define the company's GST group role, choose **Member**, then choose **Next**.
2. Copy the value of the **Group Member ID** field, then share it with the GST group representative so they can add your company as an approved member of the group.
3. Add the **API URL** from the GST group representative. Typically, the URL is formatted as follows: `https://api.businesscentral.dynamics.com/v2.0/[TENANT-ID]/[ENVIRONMENTNAME]`. For example, `https://api.businesscentral.dynamics.com/v2.0/907869c3-b252-4aca-b9cb-17a15d25477b/UKRepresentative`. 
4. Add the [!INCLUDE[prod_short](includes/prod_short.md)] company name of the GST group representative, such as *CRONUS UK Ltd*.
5. Choose **Authentication Type**, choose **OAuth2**, and then choose **Next**.
6. In the **Client ID** field, enter the ID provided by the GST group representative.
7. In the **Client Secret provided by the GST Group representative** field, enter the secret provided by the GST group representative.
8. In the **OAuth 2.0 Authority Endpoint** field, enter *https://login.microsoftonline.com/common/oauth2*.
9. In the **OAuth 2.0 Resource URL** field, enter *https://api.businesscentral.dynamics.com/*.
10. In the **OAuth 2.0 Redirect URL** field, enter *https://businesscentral.dynamics.com/OAuthLanding.htm*. 
11. When you have specified the various fields, choose **Next**, then enter the user credentials that were provided by the GST group representative.
12. Choose the GST report configuration that you use to report GST to authorities in your country.

  For example, in the United Kingdom, the GST report configuration would be set up to report GST to HMRC. The GST Group Management extension copies this setup but replaces the submission codeunit with one that supports submission to the GST group representative rather than the tax authorities. The codeunit is provided by Microsoft. When done, choose **Next**.

## <a name="using-the-vat-group-management-features"></a>Using the GST Group Management Features

GST group members use the standard processes to prepare GST returns. The only difference is to choose the **VATGROUP** report version, which submits the GST return to the GST group representative rather than the authorities. For more information, see [About the GST Return report](finance-how-report-vat.md#about-the-vat-return-report).

The following sections describe the tasks that GST group representatives must perform.

### <a name="vat-group-submissions"></a>GST Group Submissions

The **GST Group Submissions** page lists the GST returns that members have submitted. The page serves as a draft location for the submissions until the GST group representative includes them in a GST return for the group. You can open the submissions to review the GST for the individual boxes reported by the GST group member.

### <a name="creating-a-group-vat-return"></a>Creating a Group GST Return

To report GST on behalf of the group, on the **GST Returns** page, create a GST return for your company only. Afterwards, include the most recent GST submissions from GST group members by choosing the **Include Group GST** action.  

When the GST Group representative's GST Return has been submitted to the authorities on behalf of the entire group, you will normally run the **Calculate and Post GST Settlement** action. This action closes open GST Entries and transfers amounts to the GST Settlement account. Currently, this action does not take the group submissions into account. This means that only the GST Entries of the GST Group representative company will be posted. The GST Group member submission amounts must be posted to the GST settlement amount manually, so that the GST Group representative's GST Settlement account will reflect the liability of what was reported to authorities. This behaviour will change in an upcoming update of [!INCLUDE[prod_short](includes/prod_short.md)], so the entire group GST (the Total Amount on Report Lines on the GST Return) will be settled. 

> [!NOTE]
> GST group members can correct submitted GST returns as long as the group representative has not released the GST return for the group. To make a correction, the GST group member must create a new GST return for the GST return period and submit it to the GST group representative. On the GST group representative's side, the latest GST return will be included on the **GST Returns** page. 

> [!IMPORTANT]
> The GST group functionality is only supported in those markets where [!INCLUDE[prod_short](includes/prod_short.md)] uses a GST framework that consists of GST returns and GST return periods. You cannot use GST groups in other markets that have other implementations of local GST reporting, such as Austria, Germany, Italy, Spain, and Switzerland. 

## <a name="see-also"></a>See Also

[Work with GST on Sales and Purchases](finance-work-with-vat.md)  
[Set Up Goods and Services Tax](finance-setup-vat.md)  
[Work with GST on Sales and Purchases](finance-work-with-vat.md)  
[Making Tax Digital in the United Kingdom](LocalFunctionality/UnitedKingdom/making-tax-digital-submit-vat-return.md)  
[Norwegian GST Reporting in the Norwegian Version](LocalFunctionality/Norway/norwegian-vat-reporting.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]
