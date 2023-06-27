---
title: Manage users and roles
description: Learn how to manage user profiles and Role Centres in Business Central. Profiles allow administrators to centrally define and manage what users can see and do.
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bholtorf
ms.service: dynamics365-business-central
ms.topic: how-to
ms.date: 01/11/2023
ms.custom: bap-template
ms.search.form: 9171
---
# <a name="manage-user-profiles" />Manage User Profiles

[!INCLUDE [2023rw1-sec-group-short](includes/2023rw1-sec-group-short.md)]

Assign all users to profiles that reflect:

* Their business role
* The department they work in
* Another type of categorisation

Profiles allow administrators to centrally define and manage what different types of users can access in [!INCLUDE[prod_short](includes/prod_short.md)].

> [!NOTE]
> The typical business use of a profile is a role. A profile is therefore named *Profile (Role)* in the UI.

As an administrator, you create and manage profiles on the **Profiles (Roles)** page. Each profile has a card where you manage settings for the related role. For example, the card contains the following information:

* Name of the role
* User settings
* The Role Centre that the profile uses

For more information about user settings and Role Centres, see [Change Basic Settings](ui-change-basic-settings.md).

Before you can manage user profiles, you must create and add the users through the Microsoft 365 Admin Centre. You can then assign permissions to each user or user group. Permissions define the features that users can access. For more information, see [Assign Permissions to Users and Groups](ui-define-granular-permissions.md).

## <a name="page-customization" />Page Customisation

You can customise page layouts for a profile so that all users assigned the profile will see the customised pages. As an administrator, you customise pages by using the same functionality as users do when they personalise. For more information, see [Customise Pages for Profiles](ui-personalization-manage.md).

## <a name="to-create-a-profile" />To create a profile

If you cannot copy an existing profile, you can create a new one manually.

1. Choose the ![Search for Page or Report.](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Profiles (Roles)**, and then choose the related link.  
2. On the **Profiles (Roles)** page, choose the **New** action.  
3. Fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

> [!TIP]
> If you want a particular profile to be available only for very specific users, you can set the **Description** field to `Navigation menu only.`. This way, the profile is excluded from the list of available roles in **My Settings**.

## <a name="to-copy-a-profile" />To copy a profile

To save time, you can create a new profile by copying an existing one. Copy one that has similar settings to the one you want to create.

> [!NOTE]
> When you copy a profile, all the involved page customisations are copied as well, both the user-created and those derived from extensions.

1. On the **Profiles (Roles)** page, select the line for the profile that you want to copy, and then choose the **Copy Profile** action.
2. Fill in the **Profile ID** and **Display Name** fields, and then choose the **OK** button.
3. On the **Profiles (Roles)** page, open the newly created profile card, and then edit other fields as necessary.

## <a name="to-edit-a-profile" />To edit a profile

You can edit a profile by changing the fields on the **Profile (Role)** page. However, the changes will not be visible to user assigned the profile until they sign out and back in.

> [!Caution]
> Do not rename a profile while users assigned the profile are signed in as users may experience that the product freezes and must be restarted.

## <a name="to-assign-a-profile-to-a-user" />To assign a profile to a user

Users can assign themselves a role (representing a profile) by choosing the **Role** field on the **My Settings** page. As an administrator, you can do the same through the **Profiles (Roles)** page.

1. On the **Profiles (Roles)** page, select the profile that you want to assign, and then choose the **User Personalisation List** action.
2. On the **User Personalisations** page, select the user that you want to assign the profile to, and then choose the **Edit** action.
3. In the **Profile ID** field, select the relevant profile.

> [!NOTE]
> If you assign another profile to a user, any personalisations made by the user with the previous profile are preserved.

## <a name="to-define-user-settings-for-a-profile" />To define user settings for a profile

On the **My Settings** page, users can define basic behaviour of their account, such as the Role Centre, the language, and which notifications they get. For more information, see [Change Basic Settings](ui-change-basic-settings.md).

As an administrator, you can define settings for a profile. The settings will apply to all users assigned to the role.

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Profiles (Roles)**, and then choose the related link.
2. Select the line for the profile that you want to change user settings for, then choose the **User Personalisations List** action.
3. On the **User Personalisations** page, open the card for the user whose settings you want to change.
4. On the **User Personalisation Card** page, edit the fields as necessary.

## <a name="to-activate-a-profile" />To activate a profile

When you create a profile, you can define if, where, and how the profile and its information are available to users.

On the **Profile (Role)** page, select the following checkboxes:

* **Enabled** to specify if the related role is visible in the **Available Roles** page for users to choose from.  
* **Use as default profile** to specify the profile that applies to users who are not assigned a specific role.
* **Disable personalisation** to specify if users of the related role can personalise their workspace.
* **Show in Role Explorer** to specify if actions to business features included in the profile are shown in the extended view of the role explorer, a feature overview. For more information, see [Finding Pages with the Role Explorer](ui-role-explorer.md).

## <a name="to-export-profiles" />To export profiles

You can export profiles from [!INCLUDE[prod_short](includes/prod_short.md)], for example to reuse them in another tenant. The profiles are exported to a zip file that contains AL files. You can reuse the AL files to develop extensions. For more information, see [Use the Client to Create Profiles and Page Customisations](/dynamics365/business-central/dev-itpro/developer/devenv-design-profiles-using-client).

* On the **Profiles (Roles)** page, choose the **Export Profiles** action.

    This action exports a zip file that contains AL files for all profiles.

## <a name="to-import-profiles" />To import profiles

You can import profiles that have been exported from [!INCLUDE[prod_short](includes/prod_short.md)]. The steps are more or less the opposite of the steps to export profiles. For more information, see [To export profiles](admin-users-profiles-roles.md#to-export-profiles).

1. On the **Profiles (Roles)** page, choose the **Import Profiles** action.
2. Follow the steps on the **Import Profiles** wizard.

    If you only want to import selected profiles, use the **Selected** check box to indicate which to import.
3. Choose the **Import selected** button.

    This action imports a zip file that contains AL files for the selected profiles.

## <a name="to-delete-a-profile" />To delete a profile

You can delete a profile by choosing the **Delete** action on the **Profiles (Roles)** page. However, the following limitations apply:

* You cannot delete a profile that is assigned to a user or a user group.
*-* You cannot delete profiles that originate from extensions. The extension must first be uninstalled.
*-* You can only delete one profile at a time.

## <a name="to-delete-all-personalizations-made-by-a-user" />To delete all personalisations made by a user

You can delete all changes that a user has made to pages. Deleting changes can be useful, for example, if an employee has changed role and no longer needs them. Deletions revert the page layout back to what's defined by the profile.

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **User Personalisations**, and then choose the related link.

    The **User Personalisations** page lists all users who have made personalisations.

2. Open the card for a user whose personalisations you want to delete.
3. On the **User Personalisation Card** page, choose the **Clear Personalised Pages** action, and then accept the message that appears.

The user will see the changes the next time they sign in.

You can also delete all page customisations for a profile. For more information, see [To delete all customisations for a profile](ui-personalization-manage.md#to-delete-all-customizations-for-a-profile).

## <a name="to-delete-personalizations-for-specific-pages" />To delete personalisations for specific pages

You can delete personalisations that one or more users have made to specific pages. Deleting personalisations can be useful, for example, if a business process change means that a personalisation can't be used. Deletions revert the page layout back to what's defined by the profile.

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **User Page Personalisations**, and then choose the related link.

    The **User Page Personalisations** page lists all the pages that have been personalised and the user that they belong to.

    > [!Note]
    > A check mark in the **Legacy Personalisation** field indicates that the personalisation was done in an older version of [!INCLUDE[prod_short](includes/prod_short.md)], which handled personalisation differently. Users who try to personalise these pages are locked from doing so unless they choose to unlock the page. For more information, see [Why a Page is Locked from Personalising](ui-personalization-locked.md).

2. Select the line for the page personalisation that you want to delete, and then choose the **Delete** action.

The user will see the changes the next time they sign-in.  

You can also delete individual page customisations for a profile. For more information, see [To delete customisation for specific pages for a profile](ui-personalization-manage.md#to-delete-customization-for-specific-pages-for-a-profile).

## <a name="managing-user-sessions" />Managing user sessions

As the administrator of [!INCLUDE[prod_short](includes/prod_short.md)] online, you can manage user sessions in the administration centre. For more information, see [Managing Sessions](/dynamics365/business-central/dev-itpro/administration/tenant-admin-center-manage-sessions) in the administration content.  

For [!INCLUDE[prod_short](includes/prod_short.md)] on-premises, you can manage sessions using SQL Server Management Studio, for example. For more information, see [SQL Server technical documentation](/sql/sql-server).  

## <a name="see-related-microsoft-training" />See related [Microsoft training](/training/modules/users-security-dynamics-365-business-central/)

## <a name="see-also" />See also

[Assign Permissions to Users and Groups](ui-define-granular-permissions.md)  
[Customise Pages for Profiles](ui-personalization-manage.md)  
[Personalise Your Workspace](ui-personalization-user.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]
