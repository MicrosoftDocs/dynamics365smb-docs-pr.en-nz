---
title: The VAT Group Management extension for the United Kingdom
description: You can engage with other businesses to form a GST group where all members report GST in a single return.
author: brentholtorf
ms.author: bholtorf
ms.reviewer: soalex
ms.topic: conceptual
ms.search.keywords: 'VAT, value added tax, report'
ms.search.form: '4700, 4701, 4703, 4704, 4705, 4706, 4707, 4708, 4709,'
ms.date: 12/12/2023
---

# The VAT Group Management extension for the United Kingdom

[!INCLUDE[azure-ad-to-microsoft-entra-id](~/../shared-content/shared/azure-ad-to-microsoft-entra-id.md)]

You can connect one or more businesses in New Zealand to combine Goods and Services Tax (GST) reporting under a single registration number. This type of arrangement is known as a *GST group*. You can engage with the group as a member or as the group representative.

## Forming a GST group

GST group members and the group representative can use the **Set Up GST Group Management** assisted setup guide to both define their engagement with the group and create a connection between their [!INCLUDE[prod_short](includes/prod_short.md)] tenants. The group members use this connection to submit their GST returns to the group representative. The group representative then uses a single GST return to submit the group's GST to tax authorities.

[!INCLUDE[prod_short](includes/prod_short.md)] supports intra-group GST return submissions for companies using [!INCLUDE[prod_short](includes/prod_short.md)] on-premises or online, in any combination, which influences the communication setup between businesses. This article describes various group setups.

### Licence requirements

Participants in the group must be licensed to use [!INCLUDE[prod_short](includes/prod_short.md)]. You can't use guest accounts in GST groups.

* To calculate and submit GST returns, a user must be a full [!INCLUDE[prod_short](includes/prod_short.md)] user.
* To sign in and do basic tasks, such as create accounts, you need a [!INCLUDE[prod_long](includes/prod_long.md)] Team Member licence.

## Set up a GST group

The following is the recommended order of steps an administrator uses to set up a GST group:

1. Create the setup in [Microsoft Entra ID setup for group members](#microsoft-entra-id-setup-for-group-members).
2. Share the technical information GST group members and the group representative need to connect their [!INCLUDE[prod_short](includes/prod_short.md)] tenants. Usually, the group representative has this information, such as the [API URL](#group-api-setup) and the name of the GST group representative's environment the GST group members submit their GST data to.
3. Create users that VAT group members use to authenticate when they connect to the VAT group representative's [!INCLUDE[prod_short](includes/prod_short.md)]. The users must have full user licences for [!INCLUDE[prod_short](includes/prod_short.md)].
4. Run the **Set Up GST Group Management** assisted setup guide to connect the GST group members.

   The GST group representative must supply certain information to group members to complete their setup. (Learn more in the [Set up GST group members](#set-up-vat-group-members) section below.) Make a note of the **Group Member ID** for each GST group member. The group representative needs these IDs to add the companies to the GST group.
5. Set up the GST group management extension in the GST group representative's [!INCLUDE[prod_short](includes/prod_short.md)] using the **Set Up GST Group Management** assisted setup guide.

> [!NOTE]
> To connect to the GST group representative, group members must have a user account that can access the GST group representative's [!INCLUDE[prod_short](includes/prod_short.md)]. The GST group representative must create at least one user for this. However, for security reasons we recommended that they create a user for each GST group member, which can be a system user account that is not related to an actual person. Make sure to distribute the user credentials to GST group members in a secure way.

### Microsoft Entra ID setup for group members

When the GST group representative is using [!INCLUDE[prod_short](includes/prod_short.md)] online or on-premises, GST group members must use Microsoft Entra ID to authenticate users when they submit GST returns to the GST group representative. For [!INCLUDE[prod_short](includes/prod_short.md)] on-premises, members must configure single sign-on. Learn more at [Configure Microsoft Entra authentication with WS-Federation](/dynamics365/business-central/dev-itpro/administration/authenticating-users-with-azure-active-directory?tabs=singletenant%2Cadmintool).

If the GST group members are also using [!INCLUDE[prod_short](includes/prod_short.md)] online, the member can authenticate with the designated user credentials and the sign-in information provided by the group representative. Learn more in the [Set up GST group members](#set-up-vat-group-members) section below.

GST group members who have [!INCLUDE[prod_short](includes/prod_short.md)] on-premises must set up an app registration in Microsoft Entra ID for the GST group representative's [!INCLUDE[prod_short](includes/prod_short.md)] tenant. The app registration enables the GST group representative's [!INCLUDE[prod_short](includes/prod_short.md)] online to authenticate the group member. Learn more at [Quickstart: Register an application with the Microsoft identity platform](/azure/active-directory/develop/quickstart-register-app).

When the GST group member's administrator creates the app registration in Microsoft Entra ID, they must specify the following information.

* In the **Authentication** section, add **Web** as a platform, and use the following **Redirect URL**: `https://businesscentral.dynamics.com/OAuthLanding.htm`.
* In the **Authentication** section, in the option to select **Supported account types**, select **Accounts in any organisational directory (Any Microsoft Entra directory - Multitenant)**.
* In the **Certificates & secrets** section, create a new client secret and note the value. The VAT group members need the secret when they set up the connection to the group representative.
* In the **API permissions** section, add permissions to [!INCLUDE[prod_short](includes/prod_short.md)]. Enable delegated access to **Financials.ReadWrite.All** and **user_impersonation**.
* In the **Overview** section, note the **Application (client) ID**. The VAT group members need the ID when they set up the connection to the group representative.

### Group API setup

The GST group representative creates and supplies an API to group members. The members use this API to connect to the representative's [!INCLUDE[prod_short](includes/prod_short.md)] tenant and submit GST returns. GST group members often use [!INCLUDE[prod_short](includes/prod_short.md)] in separate Microsoft Entra tenants. For that reason, setup is needed to connect the GST group member and the representative's [!INCLUDE[prod_short](includes/prod_short.md)].

> [!NOTE]
> This setup requires credentials for an administrator account that has a full user licence for [!INCLUDE[prod_short](includes/prod_short.md)].

1. In the Business Central admin centre for the representative's tenant, choose the **Environments** tab.
1. Choose the representative's environment.
1. In the **Details** section, copy the **URL**.
1. Open Notepad, and paste the URL. Replace `https://businesscentral.dynamics.com` with `https://api.businesscentral.dynamics.com/v2.0`.

## Set up GST group members

GST group members connect to the representative by calling a web service on the GST group representative's tenant. The caller must be authenticated using OAuth2. When the GST group management extension is set up, members are asked to authenticate to the GST group representative, during which an access token is generated and saved. This access token is used when submitting GST returns to the GST group representative.

> [!IMPORTANT]
> The member companies in the GST group do not need to connect to HMRC because they report through the group's representative.

Before GST group members start their setup (listed below), they need to contact the GST group representative for the following information about their [!INCLUDE[prod_short](includes/prod_short.md)] tenant:

* The API URL
* The name of their company
* Sign in credentials for the dedicated user

1. In the top right corner, choose the **Settings** ![Settings.](media/ui-experience/settings_icon_small.png "Settings icon for role centre") icon, then choose the **Assisted setup** action.
2. Choose the **Set Up GST Group Management** action.
3. In the **GST Group Role** field, choose **Member** then **Next**.
4. Copy the value of the **Group Member ID** field, then share it with the GST group representative so they can add your company as an approved member of the group.
5. In the **Group Representative Product Version** field, specify the version of [!INCLUDE[prod_short](includes/prod_short.md)] the representative is using.
6. In the **API URL** field, enter the API URL provided by the GST group representative. Typically, the URL is formatted as follows: `https://api.businesscentral.dynamics.com/v2.0/[TENANT-ID]/[ENVIRONMENTNAME]`. For example, `https://api.businesscentral.dynamics.com/v2.0/907869c3-b252-4aca-b9cb-17a15d25477b/UKRepresentative`.
7. In the **Group Representative Company** field, enter the company name of the GST group representative, such as, **CRONUS UK Ltd**.
8. In the **Authentication Type** field, choose **OAuth2**. If the GST group representative is using [!INCLUDE[prod_short](includes/prod_short.md)] online, enable the **Group Representative Uses Business Central Online** toggle, and then choose **Next**.

   Then, follow the steps in either the [GST Group Representative uses Business Central online](ui-extensions-vat-group.md#vat-group-representative-uses-business-central-online) or [GST Group Representative uses Business Central on-premises](ui-extensions-vat-group.md#vat-group-representative-uses-business-central-on-premises) section below.

### GST group representative uses Business Central online

1. Enter the user credentials provided by the GST group representative, and add the required permissions to generate the access token.
2. Choose the GST report configuration you use to submit GST returns to the New Zealand tax authorities. 

After you complete the setup, [!INCLUDE[prod_short](includes/prod_short.md)] will create a new configuration based on this choice that enables you to submit GST returns to the GST group representative.

### GST group representative uses Business Central on-premises

1. Enter the user credentials provided by the GST group representative and choose **Next**.
2. In the **Client ID** field, specify the client ID from the app registration in [Microsoft Entra ID setup for group members](#microsoft-entra-id-setup-for-group-members).
3. In the **Client Secret** field, specify the client secret from the app registration in Microsoft Entra ID.
4. In the **OAuth 2.0 Authority Endpoint** field, enter `https://login.microsoftonline.com/common/oauth2`.
5. In the **OAuth 2.0 Resource URL** field, enter `https://api.businesscentral.dynamics.com/`.
6. In the **OAuth 2.0 Redirect URL** field, enter `https://businesscentral.dynamics.com/OAuthLanding.htm`.
7. When you've specified the various fields, choose **Next**, and then confirm the authentication connection to generate the access token.
8. Choose the GST report configuration you use to submit GST returns to the New Zealand tax authorities.

## Set up the GST group representative

> [!NOTE]
> For on-premises, [!INCLUDE[prod_short](includes/prod_short.md)] supports only a single tenant instance of the group representative.

> [!IMPORTANT]
> The representative company must enable the **IRD GST Setup** service connection on the **Service Connections** page. Representatives must also download GST return periods from IRD.

1. In the top right corner, choose the **Settings** icon ![Settings.](media/ui-experience/settings_icon_small.png "Settings icon for role centre"), and then choose the **Assisted setup** action.
2. Choose the **Set Up GST Group Management** action.
3. In the **GST Group Role** field, choose **Representative** to act as the GST group representative, then choose **Next**.
4. In the **Group Settlement Account** field, specify the settlement account used for the group member GST US Tax amounts. This account should have **Assets** as the **Account Category**.
5. In the **GST Settlement Account** field, specify the account you use for GST settlements. This account should have **Liabilities** as the **Account Category**.
6. In the **GST Due Box No.** field, specify the box that represents the total GST amount due from a GST group submission.
7. In the **Group Settlement General Journal Template** field, specify the general journal template used to create the document with which the group representative posts the group GST to the settlement account.
8. The **Approved Members** field shows the number of group members set up to submit GST returns to the group representative. To add new members, choose the number to open the **GST Group Approved Members** page and add the following information:
    1. In the **Group Member ID** field, enter an identifier for the group member, as displayed during the group member setup (learn more in the [GST group member setup](#set-up-vat-group-members) section above).
    2. In the **Group Member Name** field, specify the name of the group member.
    3. In the **Company** field, specify the company from which the group member submits VAT returns in [!INCLUDE[prod_short](includes/prod_short.md)], such as, **CRONUS UK Ltd**.
    4. Specify contact details for the company.

## Use the GST group management features

GST group members use the standard processes to prepare GST returns. The only difference is members must choose the **GSTGROUP** report version in the **GST Return** page to submit the GST return to the GST group representative rather than the authorities. Learn more at [About the GST Return report](finance-how-report-vat.md#vatreturn).

> [!NOTE]
> GST group members can correct submitted GST returns as long as the group representative has not released the GST return for the group. To make a correction, the GST group member must create a new GST return for the GST return period and submit it to the GST group representative. On the GST group representative's side, the member's latest GST return replaces the previous and is included on the **GST Returns** page.

The following sections describe the tasks that GST group representatives must do to file the group GST return.

### Review GST member submissions

The **GST Group Submissions** page lists the GST returns that members have submitted. The page serves as a draft location for the submissions until the GST group representative includes them in a GST return for the group. The representative can open the submissions to review the individual boxes containing the amount reported by each GST group member.

> [!TIP]
> On the **GST Return Periods** page, the **Group Member Submissions** field shows how many returns members have submitted. To ensure that this number is up to date, choose the **Get GST Returns** action.

### Create a group GST return

To report GST for the group, on the **GST Returns** page, create a GST return for your company only. Afterwards, include the most recent GST submissions from GST group members by choosing the **Include Group GST** action.  

When the group representative has submitted the group's GST return to the authorities, the representative then normally runs the **Calculate and Post GST Settlement** action. This action closes open GST Entries and transfers amounts to the GST settlement account. Currently, this action doesn't take the group submissions into account. Only the GST entries of the GST group representative company are posted. The GST group member submission amounts must be posted to the GST settlement amount manually, so the GST group representative's GST settlement account reflects the liability of what was reported to the authorities. This behaviour changes in an upcoming update of [!INCLUDE[prod_short](includes/prod_short.md)], so the entire group VAT (the total amount on report lines of the VAT return) is settled.

> [!IMPORTANT]
> The GST group functionality is only supported in those markets where [!INCLUDE[prod_short](includes/prod_short.md)] uses a GST framework that consists of GST returns and GST return periods. You cannot use GST groups in markets with other implementations of local GST reporting, such as Austria, Germany, Italy, Spain and Switzerland.

## Issue with enabling Multifactor Authentication (MFA)

If you get an error message related to authorisation during the renewal of the **OAuth2 Token** on the **GST Report Setup** page after you enable MFA, complete the following steps.  

1. Sign in to the **Azure Portal** as an Authentication Administrator.  
2. Go to the **Microsoft Entra ID**.   
3. Browse to **Users**, and then select the user you want to perform an action.  
4. Select the **Authentication methods** and at the top of the page, select **Require re-register multifactor authentication**. 
5. Go back to Dynamics 365 Business Central and select to renew the token from the **GST Report Setup**.  

This should be a one-time setup after you enable multifactor authentication for the user selected in **GST Report Setup**.  

## See also

[United Kingdom Local Functionality in the British Version](LocalFunctionality/unitedkingdom/united-kingdom-local-functionality.md)  
[Making Tax Digital in the United Kingdom](LocalFunctionality/UnitedKingdom/making-tax-digital-submit-vat-return.md)  
[Work with GST on Sales and Purchases](finance-work-with-vat.md)  
[Set Up Goods and Services Tax](finance-setup-vat.md)  
[Work with GST on Sales and Purchases](finance-work-with-vat.md)  
[Consolidating Financial Data from Multiple Companies](finance-consolidated-company-reporting.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
