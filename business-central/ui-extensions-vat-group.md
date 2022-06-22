---
title: The GST Group Management Extension for the United Kingdom
description: You can engage with other businesses to form a GST group where all members report GST in a single return.
author: brentholtorf
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: VAT, value added tax, report
ms.search.forms: ''
ms.date: 05/24/2022
ms.author: bholtorf
ms.openlocfilehash: c5757a78a44e3cdc2f6100c42b5105734928837b
ms.sourcegitcommit: 7a6efcbae293c024ca4f6622c82886decf86c176
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 06/02/2022
ms.locfileid: "8841936"
---
# <a name="the-vat-group-management-extension-for-the-united-kingdom"></a>The GST Group Management Extension for the United Kingdom

You can connect one or more businesses in your country to combine GST reporting under a single registration number. This type of arrangement is known as a *GST group*. You can engage with the group as a member or the group representative.

## <a name="forming-a-vat-group"></a>Forming a GST Group
GST group members and the group representative can use the **GST Group Management Setup** assisted setup guide to define their engagement with the group and create a connection between their [!INCLUDE[prod_short](includes/prod_short.md)] tenants. The group members will use the connection to submit their GST returns to the group representative. The representative will use a single GST return to submit GST to tax authorities for the group. 

## <a name="license-requirements"></a>Licence Requirements
Participants in the group must be licensed to use [!INCLUDE[prod_short](includes/prod_short.md)]. You can't use guest accounts in GST groups. 

* To calculate and submit GST returns, a user must be a full Business Central user.
* To sign in and do basic tasks, such as create accounts, you can have the Dynamics 365 Business Central Team Member licence.

## <a name="vat-group-constellations"></a>GST Group Constellations
Communication happens from group members to the representative. The group representative exposes an API URL that allows the members to submit their GST returns to the GST group representative. 
[!INCLUDE[prod_short](includes/prod_short.md)] supports inter-group GST return submissions for companies using [!INCLUDE[prod_short](includes/prod_short.md)] on-premises or online and in any combination. The setup of the communication depends on the constellation. This article describes various group constellations.

The following list shows the recommended order of the steps to set up a GST group:

1. Create the setup in Azure Active Directory. For more information, see [Requirements for Authentication](ui-extensions-vat-group.md#requirements-for-authentication).
2. Share the technical information that GST group members and the representative need to connect their [!INCLUDE[prod_short](includes/prod_short.md)] tenants. Usually, the GST group representative has this information, such as the name of the GST group representative's environment to which the GST group members will submit GST.
3. Create users that GST group members can use to authenticate when they connect to the GST group representative's [!INCLUDE[prod_short](includes/prod_short.md)]. The users must have full user licences for [!INCLUDE[prod_short](includes/prod_short.md)].
4. Run the **Set Up GST Group Management** assisted setup guide to connect the GST group members.

  The guide requires some information from the GST group representative. For more information, see [Set Up GST Group Members](#set-up-vat-group-members). Make a note of the **Group Member ID** for each GST group member. The representative needs these IDs to add the companies to the GST group.
5. Set up the GST Group Management extension in the GST group representative's [!INCLUDE[prod_short](includes/prod_short.md)] by using the **Set Up GST Group Management** assisted setup guide. 

> [!NOTE]
> To connect to the GST group representative, group members must have a user account that can access the GST group representative's [!INCLUDE[prod_short](includes/prod_short.md)]. The GST group representative must create at least one user for this, however, for security reasons we recommended that you create a user for each GST group member. Make sure to distribute the credentials for these users to GST group members in a secure way. This be a system user account that is not related to an actual person.

## <a name="about-the-vat-group-management-setup"></a>About the GST Group Management Setup

The GST group representative exposes an API to group members. The members use the API to connect to the representative's [!INCLUDE[prod_short](includes/prod_short.md)] tenant and submit GST returns. GST group members often use [!INCLUDE[prod_short](includes/prod_short.md)] in separate Azure Active Directory tenants. Therefore, setup is needed to connect the GST group member and representative's [!INCLUDE[prod_short](includes/prod_short.md)]. 
  
GST group members connect to the representative by calling a web service on the GST group representative's tenant. The caller must be authenticated using OAuth2. When the GST Group Management extension is set up, you'll be asked to authenticate to the GST group representative to get and save an access token. This access token is used when submitting GST returns to the GST group representative. 

## <a name="construct-the-api-url"></a>Construct the API URL
1. In the Business Central admin centre for the representative's tenant, choose the **Environments** tab.
2. In the **Details** section, copy the **URL**.
3. Open Notepad, and paste the URL. Replace **https://businesscentral.dynamics.com** with **https://api.businesscentral.dynamics.com/v2.0**.

## <a name="requirements-for-authentication"></a>Requirements for Authentication 
> [!NOTE]
> This requires credentials for an administrator account that has a full user licence for [!INCLUDE[prod_short](includes/prod_short.md)].

When the GST group representative is using [!INCLUDE[prod_short](includes/prod_short.md)] online or on-premises, GST group members must use Azure Active Directory to authenticate users when they submit GST returns to the GST group representative. For [!INCLUDE[prod_short](includes/prod_short.md)] on-premises, members must configure single sign-on. For more information, see [Configure Azure Active Directory Authentication with WS-Federation](/dynamics365/business-central/dev-itpro/administration/authenticating-users-with-azure-active-directory?tabs=singletenant%2Cadmintool). If the GST group members are also using [!INCLUDE[prod_short](includes/prod_short.md)] online, the GST group member can authenticate using the designated user credentials and the endpoint information. For more information, see [Set Up GST Group Members](ui-extensions-vat-group.md#set-up-vat-group-members).

GST group members who have [!INCLUDE[prod_short](includes/prod_short.md)] on-premises must set up an app registration in Azure Active Directory for the GST group representative's [!INCLUDE[prod_short](includes/prod_short.md)] tenant. The app registration enables the GST group representative's [!INCLUDE[prod_short](includes/prod_short.md)] online to authenticate the group member. For more information, see [Quickstart: Register an application with the Microsoft identity platform](/azure/active-directory/develop/quickstart-register-app).

When you create the app registration in Azure Active Directory, you must specify the following information.

* In the **Authentication** section, add **Web** as a platform, and use the following **Redirect URL**: https://businesscentral.dynamics.com/OAuthLanding.htm.
* In the **Authentication** section, in the option to select **Supported account types**, select **Accounts in any organisational directory (Any Azure AD directory - Multitenant)**.
* In the **Certificates & secrets** section, create a new client secret and note the value. The GST group members will need the secret when they set up the connection to the group representative.
* In the **API permissions** section, add permissions to [!INCLUDE[prod_short](includes/prod_short.md)]. Enable delegated access to **Financials.ReadWrite.All** and **user_impersonation**.
* In the **Overview** section, note the **Application (client) ID**. The GST group members will need the ID when they set up the connection to the group representative. 

## <a name="set-up-vat-group-members"></a>Set Up GST Group Members
> [!IMPORTANT]
> The member companies in the GST group do not need to connect to HMRC because they report through the group's representative.

Before you get started, contact the GST group representative for the following information about their [!INCLUDE[prod_short](includes/prod_short.md)] tenant:

* The API URL
* The name of their company 
* Client ID
* Client secret
* Sign in credentials for the dedicated user 

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Set Up GST Group Management**, and then choose the related link.
2. In the **GST Group Role** field, specify whether you're a member of the group or the group's representative. Choose **Member** to act as a group member and submit your GST returns to the group representative rather than the tax authorities, and then choose **Next**.
3. Copy the value of the **Group Member ID** field, then share it with the GST group representative so they can add your company as an approved member of the group.
4. In the **Group Representative Product Version** field, specify the version of [!INCLUDE[prod_short](includes/prod_short.md)] that the representative is using.
5. In the **Group Representative Company** field, enter the company name of the GST group representative. For example, **CRONUS UK Ltd**.
6. In the **Authentication Type** field, choose **OAuth2**. If the GST group representative is using [!INCLUDE[prod_short](includes/prod_short.md)] online, specify that **Group Representative Uses Business Central Online**, and then choose **Next**. Depending on whether the representative is using [!INCLUDE[prod_short](includes/prod_short.md)] online or on-premises, follow the steps in either the [GST Group Representative Uses Business Central Online](ui-extensions-vat-group.md#vat-group-representative-uses-business-central-online) or [GST Group Representative Uses Business Central On-Premesis](ui-extensions-vat-group.md#vat-group-representative-uses-business-central-on-premesis) sections.

### <a name="vat-group-representative-uses-business-central-online"></a>GST Group Representative Uses Business Central Online
1. Enter the user credentials that were provided by the GST group representative, and add the required permissions.
2. Choose the GST Report Configuration that is currently being used to submit GST returns to the tax authorities. After you complete the setup, [!INCLUDE[prod_short](includes/prod_short.md)] will create a new configuration based on this choice and use the configuration to submit GST returns to the GST group representative.  
3. Add the **API URL** from the GST group representative. Typically, the URL is formatted as follows: `https://api.businesscentral.dynamics.com/v2.0/[TENANT-ID]/[ENVIRONMENTNAME]`. For example, `https://api.businesscentral.dynamics.com/v2.0/907869c3-b252-4aca-b9cb-17a15d25477b/UKRepresentative`.

### <a name="vat-group-representative-uses-business-central-on-premesis"></a>GST Group Representative Uses Business Central On-Premesis
1. In the **Client ID** field, specify the client ID from the app registration in Azure Active Directory.
2. In the **Client Secret** field, specify the client secret from the app registration in Azure Active Directory.
3. In the **OAuth 2.0 Authority Endpoint** field, enter `https://login.microsoftonline.com/common/oauth2`.
4. In the **OAuth 2.0 Resource URL** field, enter `https://api.businesscentral.dynamics.com/`.
5. In the **OAuth 2.0 Redirect URL** field, enter `https://businesscentral.dynamics.com/OAuthLanding.htm`.
6. When you've specified the various fields, choose **Next**, and then enter the user credentials that were provided by the GST group representative.
7. Choose the GST report configuration that you use to report GST to authorities in your country.

## <a name="set-up-the-vat-group-representative"></a>Set Up the GST Group Representative
> [!NOTE]
> For on-premesis, we support only a single tenant instance of the group representative.

> [!IMPORTANT]
> The representative company must enable the **IRD GST Setup** service connection on the **Service Connections** page. Representatives must also download GST return periods from IRD.

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Set Up GST Group Management**, and then choose the related link.
2. In the **GST Group Role** field, specify whether you're a member of the group or the group's representative. Choose **Representative** to act as the GST group representative and submit GST returns to the tax authorities for the group, and then choose **Next**.
3. In the **GST Settlement Account** field, specify the account you use for GST settlements.
4. In the **GST Due Box No.** field, specify the box that represents the total GST amount that is due from a GST group submission.
5. In the **Group Settlement General Journal Template** field, specify the general journal template used for the document to post the group GST to the settlement account.
6. The **Approved Members** field shows the number of group members that are set up to submit GST returns to the representative. To add new members, choose the number to open the **Approved Members** page.
7. To add new members, add the following information on the **GST Group Approved Members** page:
    1. In the **Group Member ID** field, enter an identifier for the group member.
    2. In the **Group Member Name** field, specify the name of the group member. 
    3. In the **Company** field, specify the company from which the group member will submit GST returns in [!INCLUDE[prod_short](includes/prod_short.md)]. For example, **CRONUS UK Ltd**.
    4. Specify contact details for the company.

## <a name="use-the-vat-group-management-features"></a>Use the GST Group Management Features
GST group members use the standard processes to prepare GST returns. The only difference is to choose the **VATGROUP** report version, which submits the GST return to the GST group representative rather than the authorities. For more information, see [About the GST Return report](finance-how-report-vat.md#vatreturn).

The following sections describe the tasks that GST group representatives must do.

### <a name="vat-group-submissions"></a>GST Group Submissions

The **GST Group Submissions** page lists the GST returns that members have submitted. The page serves as a draft location for the submissions until the GST group representative includes them in a GST return for the group. You can open the submissions to review the GST for the individual boxes reported by the GST group member. 

> [!TIP]
> On the **GST Return Periods** page, the **Group Member Submissions** field shows how many returns members have submitted. To ensure that this number is up to date, choose the **Get GST Returns** action.

### <a name="creating-a-group-vat-return"></a>Creating a Group GST Return

To report GST for the group, on the **GST Returns** page, create a GST return for your company only. Afterwards, include the most recent GST submissions from GST group members by choosing the **Include Group GST** action.  

When the GST group representative's GST return has been submitted to the authorities for the entire group, you'll normally run the **Calculate and Post GST Settlement** action. This action closes open GST Entries and transfers amounts to the GST Settlement account. Currently, this action doesn't take the group submissions into account. <!--Has this changed?--> Only the GST entries of the GST Group representative company will be posted. The GST group member submission amounts must be posted to the GST settlement amount manually, so that the GST group representative's GST settlement account will reflect the liability of what was reported to authorities. This behaviour will change in an upcoming update of [!INCLUDE[prod_short](includes/prod_short.md)], so the entire group GST (the Total Amount on Report Lines on the GST return) will be settled. <!--Has this behavior changed?-->

> [!NOTE]
> GST group members can correct submitted GST returns as long as the group representative has not released the GST return for the group. To make a correction, the GST group member must create a new GST return for the GST return period and submit it to the GST group representative. On the GST group representative's side, the latest GST return will be included on the **GST Returns** page. 

> [!IMPORTANT]
> The GST group functionality is only supported in those markets where [!INCLUDE[prod_short](includes/prod_short.md)] uses a GST framework that consists of GST returns and GST return periods. You cannot use GST groups in other markets that have other implementations of local GST reporting, such as Austria, Germany, Italy, Spain, and Switzerland. 

## <a name="see-also"></a>See Also
[United Kingdom Local Functionality in the British Version](LocalFunctionality/unitedkingdom/united-kingdom-local-functionality.md)  
[Making Tax Digital in the United Kingdom](LocalFunctionality/UnitedKingdom/making-tax-digital-submit-vat-return.md)  
[Work with GST on Sales and Purchases](finance-work-with-vat.md)  
[Set Up Goods and Services Tax](finance-setup-vat.md)  
[Work with GST on Sales and Purchases](finance-work-with-vat.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]
