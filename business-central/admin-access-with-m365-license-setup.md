---
title: Set Up Access with Microsoft 365 Licences
description: A guide to how administrators can configure access to Business Central with Microsoft 365 licences.
author: mikebc
ms.author: mikebc
ms.reviewer: jswymer
ms.service: dynamics365-business-central
ms.topic: how-to
ms.date: 11/03/2022
ms.custom: bap-template
ms.search.keywords: 'License, access, Microsoft 365, collaborate, collaboration, Teams, Microsoft Teams'
ms.search.form: 9061
---
# <a name="set-up-business-central-access-in-teams-with-microsoft-365-licenses"></a>Set Up Business Central Access in Teams with Microsoft 365 Licences

Administrators must complete multiple activities before users can access [!INCLUDE [prod_short](includes/prod_short.md)] with their Microsoft 365 licence. The steps below represent the minimum setup required to get started. To learn more about access with Microsoft 365 licences, go to [Business Central Access with Microsoft 365 Licences](admin-access-with-m365-license.md).

## <a name="guidelines"></a>Guidelines

Setting up access with Microsoft 365 licences involves the following tasks:

||Task|Required|
|-|-|-|
|1|[Configure which Business Central data the Microsoft 365 licensed users have permission to view](#configure-permissions)|![check mark](media/check.png "cheque")|
|2|[Enable access with Microsoft 365 licences on the Business Central environment](#enable-access-with-microsoft-365-licenses)|![check mark](media/check.png "cheque")|
|3|[Assign security group to the environment](#choose-who-gets-access-by-using-security-group)|
|4|[Deploy the Business Central app for Teams to users](#deploy-the-business-central-app-for-teams)|![check mark](media/check.png "cheque")|
|5|[Test the setup](#test-your-setup)||

> [!TIP]
> Except for the last task, you can complete the tasks in any order. You can do tasks separately, as described in the sections that follow or use the **Access with Microsoft 365 licences** assisted setup guide to walk you through them.
>
> To run the assisted setup, do the following steps:
>
> 1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Assisted Setup**, and then choose the related link.
> 2. On the **Assisted Setup** page, go to the **Do more with Business Central** section and select **Access with Microsoft 365 licences**.
> 3. Follow the instructions.  

## <a name="configure-permissions"></a>Configure permissions

[!INCLUDE [prod_short](includes/prod_short.md)] is secure by design and minimises risk by granting no permissions to Microsoft 365 users out of the box. Administrators must configure object permissions that determine which tables, pages and reports can be accessed in Teams with only a Microsoft 365 licence. These permissions are the starting permissions assigned when a user signs in for the first time with their Microsoft 365 licence. 

To configure starting permissions:

1. In [!INCLUDE [prod_short](includes/prod_short.md)], search for **Licence Configuration**.
2. Select the Microsoft 365 licence.
3. At the top of the **Microsoft 365** licence page, select the edit icon ![Edit icon](media/edit-pencil.png), then turn on **Customise permissions**. 
4. In the **Custom Permission Sets** section, add the appropriate permission sets and choose whether they're applicable to a single company or all companies within the environment.

With this configuration, users with only a Microsoft 365 licence are added to the **Users** list when they access [!INCLUDE [prod_short](includes/prod_short.md)] for the first time. For more information about users, go to [Creating Users According to Licences](ui-how-users-permissions.md).

> [!NOTE]
> When synchronising the users list in [!INCLUDE [prod_short](includes/prod_short.md)] with users in Microsoft 365, only users that have a [!INCLUDE [prod_short](includes/prod_short.md)] licence are added to [!INCLUDE [prod_short](includes/prod_short.md)]'s users list. For more administrative control over permissions and profiles, you can assign a security group to the environment. When environments are secured using a security group and enable access with Microsoft 365 licences, the **Update users from Microsoft 365** action in the **Users** page will also include users that only have a Microsoft 365 licence. To learn about securing environments, see [Manage access using Azure Active Directory groups](/dynamics365/business-central/dev-itpro/administration/tenant-admin-center-manage-access#manage-access-using-azure-active-directory-groups) in the developer and IT pro help.

> [!TIP]
> Looking for a quicker way to get started when trying out this feature on a sandbox or evaluation company? Assign the **D365 Read** permission set, which grants permission to most objects.  

When working with multiple environments, licence configuration must be applied to each environment and can be different on each environment.

Learn more at [Assign Permissions to Users and Groups](ui-define-granular-permissions.md) and [Composing Permission Sets](/dynamics365/business-central/dev-itpro/developer/devenv-permissionset-composing).

## <a name="enable-access-with-microsoft-365-licenses"></a>Enable access with Microsoft 365 licences

Access with Microsoft 365 licences is off by default. Access must be enabled for each environment independently, giving administrators control and allowing for staged rollout across the organisation. You turn on access by using the [!INCLUDE [prod_short](includes/prod_short.md)] admin centre: 

1. In the upper-right corner, select **Settings** ![Settings.](media/ui-experience/settings_icon_small.png "Settings icon for role centre") > **Admin Centre**.  
2. In the admin centre, select **Environments**, then select the environment on which you want to change licence access. 
3. On the **Environment details** page, select **Modify** for the **Access with Microsoft 365 licences** setting.
4. In the **Microsoft 365 licences** pane, turn on the switch. 
5. Select **Save** when done and accept the confirmation. The change comes into effect immediately.

## <a name="choose-who-gets-access-by-using-security-group"></a>Choose who gets access by using security group

In the Business Centre admin centre, an environment can be assigned to one or more security groups to control access. You can assign an Azure Active Directory (Azure AD) group to the environment. By assigning an Azure AD group to an environment, only direct and indirect members of the group are granted access to the environment. Indirect members are users in another group, which itself is a member of the group assigned to the environment. Although all licensed users in Azure AD will be added to the environment when it's synchronised with Microsoft 365, only group members can sign in. To learn more, go to [Manage access using Azure Active Directory groups](/dynamics365/business-central/dev-itpro/administration/tenant-admin-center-manage-access#manage-access-using-azure-active-directory-groups) in the developer and IT pro help.

## <a name="deploy-the-business-central-app-for-teams"></a>Deploy the Business Central app for Teams

For [!INCLUDE [prod_short](includes/prod_short.md)] licence holders to share data in Teams, and for Microsoft 365 licence holders to access that data, each must have the [!INCLUDE [prod_short](includes/prod_short.md)] app for Teams installed. Although users can install the app by themselves, it's recommended that administrators use centralised deployment. Centralised deployment lets you roll out the app to a broader audience across the organisation and minimise individual user effort. 

To learn how to centrally deploy the [!INCLUDE [prod_short](includes/prod_short.md)] app for Teams, see [Installing the Business Central app by using Centralised Deployment](admin-teams-integration.md#installing-the-business-central-app-by-using-centralized-deployment).

> [!NOTE]
> If you have run centralised deployment before and only deployed the app to the security group of licensed [!INCLUDE [prod_short](includes/prod_short.md)] users, you'll need to run it again to deploy to additional groups or the whole organisation, depending on how you are configuring access.

> [!TIP]
> Looking for a quicker way to get started when trying out this feature? Test users can install the app at [aka.ms/BCgetTeamsApp](https://aka.ms/BCgetTeamsApp).

## <a name="test-your-setup"></a>Test your setup

To verify that your setup is ready for production, the following steps will help you build the confidence that everything works as it should.

1. Create or identify two test users (A and B).

   - Test user A must have a [!INCLUDE [prod_short](includes/prod_short.md)] licence and Microsoft 365 licence with access to Teams.
   - Test user B must have only a Microsoft 365 licence with access to Teams.

2. Sign in to the [!INCLUDE [prod_short](includes/prod_short.md)] web client as test user A.

   1. Open a record that test user B should have access to, such as an **Item** card in the appropriate company and environment.
   2. Select **Share** ![!Share to other apps action on pages.](media/share-icon.png) > **Share to Teams** to bring up the Share to Teams window.
   3. In the **Share to** field, add test user B as the recipient.
   4. Wait for the link to expand to a card and select Share.

3. Sign into Microsoft Teams as test user B.

   1. Select Chat and open the conversation with test user A.
   2. In the message sent by test user A, select the Details button on the card. If the [!INCLUDE [prod_short](includes/prod_short.md)] client is displayed and is read-only, your setup was successful.

> [!TIP]
> Something went wrong? Check out [Troubleshoot Access with Microsoft 365 Licences](admin-access-with-m365-license-troubleshooting.md).

## <a name="see-also"></a>See also

[Overview of Business Central Access with Microsoft 365 licences](admin-access-with-m365-license.md#minimum-requirements)  
[Troubleshoot Access with Microsoft 365 Licences](admin-access-with-m365-license-troubleshooting.md)  
[Business Central and Microsoft Teams Integration](across-teams-overview.md)  
