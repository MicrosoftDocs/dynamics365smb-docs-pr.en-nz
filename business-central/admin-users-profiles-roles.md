---
title: Manage users and roles | Microsoft Docs
description: Learn how to manage users and Role Centres in Business Central.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: profiles, users
ms.date: 08/02/2019
ms.author: edupont
ms.openlocfilehash: 27a57490101195f8dc05cc39538260e7db5e46af
ms.sourcegitcommit: 5bcc5f95e450ee9a3d9f7a380e592a5e75c4185b
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 08/05/2019
ms.locfileid: "1858236"
---
# <a name="understanding-users-roles-and-profiles"></a>Understanding Users, Roles, and Profiles

In [!INCLUDE[d365fin](includes/d365fin_md.md)], users are added by an administrator who also gives users access to the areas of [!INCLUDE[d365fin](includes/d365fin_md.md)] that they need in their work.  

Access to functionality is managed through *user groups* and *profiles (roles)*. As an administrator, you can add and remove users as part of your [!INCLUDE[d365fin](includes/d365fin_md.md)] subscription, and you can assign users permissions through user groups.  

## <a name="adding-users"></a>Adding Users

To add users in [!INCLUDE[d365fin](includes/d365fin_md.md)] online, your company's Office 365 administrator must first create the users in the Office 365 Admin Centre. For more information, see [Add Users to Office 365 for business](https://aka.ms/CreateOffice365Users).

Then, the administrator can assign permissions to each user and groups of users. For more information, see [Managing Users and Permissions](ui-how-users-permissions.md).  

The most powerful permissions that a user can have is the SUPER permission set. Each company must have at least one user with this permission set, but it is a best practice to give each user permissions that match their work needs in [!INCLUDE[prodshort](includes/prodshort.md)] and not more than that. This helps ensure that users only have access to data that is relevant to their work, for example.  

> [!TIP]
> It's a best practice to make sure that the Office 365 administrator also has the SUPER permission set in [!INCLUDE[prodshort](includes/prodshort.md)] because that makes many administrative tasks easier, including setting up integration with other apps.

### <a name="users-of-on-premises-deployments"></a>Users of on-premises deployments

For on-premises deployments of [!INCLUDE[d365fin](includes/d365fin_md.md)], the administrator can choose between different credential authorisation mechanisms for users. Then, when you create a user, you provide different information depending on the credential type that you are using in the specific [!INCLUDE[server](includes/server.md)] instance. For more information, see the [Authentication and Credential Types](/dynamics365/business-central/dev-itpro/administration/users-credential-types) in the Administration section of the developer and ITPro content for [!INCLUDE[d365fin](includes/d365fin_md.md)].  

## <a name="profiles-roles"></a>Profiles (Roles)

The people in your company who have access to [!INCLUDE[d365fin](includes/d365fin_md.md)] are all assigned a role that gives them access to a *Role Centre*.

Profiles are collections of [!INCLUDE[d365fin](includes/d365fin_md.md)] users who share the same role. A Role Centre is the entry point and home page for [!INCLUDE[d365fin](includes/d365fin_md.md)] that gives you quick access to your most important tasks and displays various insights and key performance indicators (KPIs) about your work.  

> [!NOTE]  
>  In the current version of [!INCLUDE[d365fin](includes/d365fin_md.md)] online, you cannot add, edit, or delete profiles.  

### <a name="CreateProfile"></a>To create a profile

1.  Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Profiles**, and then choose the related link.  

2.  On the **Profiles** page, choose the **New** action to open the **New Profile Card** page.  

3.  In the **Profile ID** field, enter a name that describes the intended role of the users.  

4.  In the **Description** field, enter a description of the Profile ID, for example, **Order Processor**.  

5.  Set the **Role Centre ID** field to the Role Centre that you want to assign to the profile.  

The procedure for modifying an existing profile is the same, except you select an existing profile on the **Profiles** page instead of choosing the **New** action.  


### <a name="copy-a-profile"></a>Copy a profile
Copying a profile can save you time if you want to use similar settings on a profile and you only want to change a few settings.

1.  Open the profile that you want to copy, and then choose the **Copy Profile** action.

2.  In **New Profile ID** field, enter a name for the profile that you want to copy.

3.  Set the **New Profile Scope** field to one of the following:

    - **System** to make the new profile available to all tenant databases that use the application.
    - **Tenant** to make the new profile available to just the current tenant database.
4. Choose the **OK** button when done.

### <a name="ExportImportProfile"></a>Export and import profiles

You can export and import profiles as XML files to and from the a [!INCLUDE[d365fin](includes/d365fin_md.md)] database. Exporting and importing a profile can save you time when configuring the user interface because you reuse an existing profile configuration instead of having to configure a profile from scratch. If you have a profile that is configured in a [!INCLUDE[d365fin](includes/d365fin_md.md)] database and you would like to reuse all or some of the same profile configurations in another database, you can export the profile to an XML file. Then, you can import the profile XML file into the other database.

-   To export a profile, you can either choose the **Export Profiles** action from the **Profile List** or **Profile Card** page or you can search for and open the **Export Profiles** page. Save the XML file to a location on your computer or network.

-   To import a profile, you can either choose the **Import Profile** action from the **Profile List** page, or you can search for and open the **Import Profiles** page.

    > [!NOTE]  
    >  You cannot import a profile that already exists in the database, even though the XML file is named differently or has different content. You must delete the existing profile before you can import the new profile.


## <a name="configuration-and-personalization"></a>Configuration and Personalisation
<!--The concept of UI customization in [!INCLUDE[d365fin](includes/d365fin_md.md)] is divided in two:  

-   Configuration, performed by the administrator  

-   Personalization, performed by users  

The administrator configures the user interface for multiple users by customizing the user interface for a profile that the users are assigned to.  -->

Users personalise the user interface of their personal version by customising the user interface under their own user logon. This personalisation can be deleted by the administrator. For more information, see [Personalising Your Workspace](ui-personalization-user.md).  

## <a name="see-also"></a>See Also  
[Managing Users and Permissions](ui-how-users-permissions.md)  
[Managing Personalisation as an Administrator](ui-personalization-manage.md)  
[Personalising Your Workspace](ui-personalization-user.md)  
