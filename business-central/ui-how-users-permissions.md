---
title: Create Users According to Licences
description: Describes how to add users to Business Central online or on-premises based on licences.
author: jswymer
ms.topic: conceptual
ms.search.keywords: 'access, right, security'
ms.search.form: '119, 6300, 6301, 6302, 8930, 9800, 9807, 9808, 9830, 9831, 9838, 9818, 9062, 9061, 9069, 9173'
ms.date: 03/24/2023
ms.author: jswymer
ms.reviewer: jswymer
---
# <a name="create-users-according-to-licenses"></a>Create Users According to Licences

[!INCLUDE [2023rw1-sec-group-short](includes/2023rw1-sec-group-short.md)]

This article describes how administrators create users and define who can sign in to [!INCLUDE[prod_short](includes/prod_short.md)]. You'll also learn how to assign permissions to different users according to your product licences.

When you create users in [!INCLUDE[prod_short](includes/prod_short.md)], you grant permissions to them through permission sets. You can also organise users in user groups. User groups make it easier to manage permissions and other settings for multiple users at the same time. For more information, see [Assign Permissions to Users and Groups](ui-define-granular-permissions.md).  

For more information about the different types of licences and how licensing works in [!INCLUDE[prod_short](includes/prod_short.md)], [download the Dynamics 365 Licensing Guide](https://go.microsoft.com/fwlink/?LinkId=866544).

> [!NOTE]
> The process of managing users and licences varies depending on whether [!INCLUDE[prod_short](includes/prod_short.md)] is deployed online or on-premises. For [!INCLUDE [prod_short](includes/prod_short.md)] online, you must add users from Microsoft 365. In on-premises deployments, you can create, edit, and delete users directly.  

## <a name="manage-users-and-licenses-in-online-tenants"></a>Manage users and licences in online tenants

User accounts in [!INCLUDE[prod_short](includes/prod_short.md)] must be first created in the Microsoft 365 admin centre. These user accounts aren't exclusive to Business Central. If you subscribe to other plans, they can be used to sign in to other applications, such as Power BI. For information about creating users in the Microsoft 365 admin centre, go to [Add users in Microsoft admin centre](/microsoft-365/admin/add-users/add-users).

Your subscription to [!INCLUDE[prod_short](includes/prod_short.md)] online defines how many [!INCLUDE[prod_short](includes/prod_short.md)] user licences you're allowed. Users are added to your tenant in the Microsoft Partner Centre, typically by your Microsoft partner. For more information, see [Administration of Business Central Online](/dynamics365/business-central/dev-itpro/administration/tenant-administration).

You assign licences to users according to the work each user will do in [!INCLUDE[prod_short](includes/prod_short.md)]. You can assign licences in several ways:

- Your company's Microsoft 365 administrator can do it in the [Microsoft 365 Admin Centre](https://admin.microsoft.com). For more information, see [Add users individually or in bulk to Microsoft 365](/microsoft-365/admin/add-users/add-users).  
- A Microsoft partner can assign licences in the Microsoft 365 Admin Centre or in the Microsoft Partner Centre. For more information, see [User management tasks for customer accounts](/partner-center/assign-licenses-to-users) in the Microsoft Partner Centre Help.

For more information, see [Administration of Business Central Online](/dynamics365/business-central/dev-itpro/administration/tenant-administration) in the administration Help.

After user accounts are created in the Microsoft 365 admin centre, there are two ways to import them to Business Central:

- A user account is imported automatically when the user signs in to [!INCLUDE [prod_short](includes/prod_short.md)] the first time.

- The administrator can import users by choosing the **Update Users from Microsoft 365** action on the **Users* page.

Both approaches have their own advantages, and you can use them simultaneously. Each approach allows administrators to proactively configure [!INCLUDE [prod_short](includes/prod_short.md)] to assign the starting permissions, user groups, and user profiles. Using the **Update Users from Microsoft 365** action gives administrators more control to adjust permissions, user groups, and profiles. It's an ideal approach when you're setting up [!INCLUDE [prod_short](includes/prod_short.md)] the first time, before any users sign in, or when adding a new team of users.

> [!NOTE]
> After you add users in the Microsoft 365 Admin Centre, we recommend that you update the user information in [!INCLUDE[prod_short](includes/prod_short.md)] as soon as possible. Keeping user information current is easy to do, and helps ensure that people can always sign in. For more information, see [To add users or update user information and licence assignments in Business Central](#adduser).<br>
>
> Updating user information is especially important if you've customised permission sets for the licence. If a new user tries to sign in to [!INCLUDE[prod_short](includes/prod_short.md)] before you've added them, they might not be able to. For more information, see [Configure permissions based on licences](#licensespermissions).
>
> However, users who experience this problem aren't actually blocked. They can either use the **Go back home** action, or simply sign in again to resolve the issue.

[!INCLUDE [admin-gdap-users](includes/admin-gdap-users.md)]

For more information, see [Delegated administrator access to Business Central Online](/dynamics365/business-central/dev-itpro/administration/delegated-admin).  

### <a name="configure-permissions-based-on-licenses"></a><a name="licensespermissions"></a>Configure permissions based on licences

[!INCLUDE [2022_releasewave1](includes/2022_releasewave1.md)]

Admins can configure permissions sets and user groups for each licence.<!--Note to translators: The names in *italics* or capitalized in this section must not be translated.-->  

For example, the commonly used licence, *Dynamics 365 Business Central Team Member*, has the following permissions sets by default:

- D365 READ
- D365 TEAM MEMBER
- EDIT IN EXCEL - VIEW
- EXPORT REPORT EXCEL
- LOCAL

Other permission sets are added automatically based on the user groups assigned to the licence. When creating a new user based on this licence, [!INCLUDE[prod_short](includes/prod_short.md)] assigns the permission sets originating from the user groups and the permission sets from the licence. The same starting permissions are assigned to the user if their user account was created automatically in [!INCLUDE[prod_short](includes/prod_short.md)] or if the administrator used the **Update Users from Microsoft 365** action in the **Users** page.

If this default configuration isn't the right setup for a particular environment, the admin can change that configuration. However, customised permissions will affect only new users who are assigned that licence. Permissions for existing users who are assigned the licence won't be affected.  

1. Sign in to [!INCLUDE[prod_short](includes/prod_short.md)] using an administrator account.  
2. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Licence Configuration**, and then choose the related link.  

    <!--Alternatively, if you're already in the **Users** page, you can run the **Update Users from Microsoft 365** guide, and then, on the first page of the guide, choose the **Configure permissions per license** link.-->  
3. In the **Licence Configuration** page, choose the licence that you want to customise, and then choose the **Configure** action.  
4. Choose the **Customise permissions** field to switch on customisation, and then make the relevant changes.  

    In our example, the admin wants to remove the permission to edit in Excel, so they remove the *Excel Export Action* user group from the Team Member licence. Going forward, new users that are assigned the Team Member licence won't get the option to export data to Excel. If the organisation changes their minds on the subject, they can just go back to the **Licence Configuration** page and switch off the customisation for that licence type.  

> [!IMPORTANT]
> This customisation of permissions only takes effect for new users that you assign the relevant licence. Existing users are not updated. We recommend that you customise permissions before you start assigning users licences in the Microsoft 365 admin centre.

### <a name="to-add-users-or-update-user-information-and-license-assignments-in-business-central"></a><a name="adduser"></a>To add users or update user information and licence assignments in Business Central

After you add users or change user information in the Microsoft 365 Admin Centre, you can quickly import the user information to [!INCLUDE[prod_short](includes/prod_short.md)]. The import includes licence assignments.  

1. Sign in to [!INCLUDE[prod_short](includes/prod_short.md)] using an administrator account.
2. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Users**, and then choose the related link.  
3. Choose **Update Users from Microsoft 365**.

> [!IMPORTANT]  
> Running the synchronisation of users from Microsoft 365 using the **Update Users from Microsoft 365** guide, requires the SUPER permission set.

> [!NOTE]
> The **Update Users from Microsoft 365** guide doesn't update users that are not assigned a licence, such as someone who is Global Admin and Dynamics 365 Admin. Those users will update the next time they sign in to the environment.

The next step for newly created users is to assign user groups and permissions. Go to [Assign Permissions to Users and Groups](ui-define-granular-permissions.md) for information. If you're updating a user, and the update includes a licence change, users are assigned to the appropriate user group and their permission sets are updated. For more information, see [To manage permissions through user groups](ui-define-granular-permissions.md).  

> [!NOTE]
> All users in an environment must be assigned to the same licence, either Essentials or Premium. For more information about licensing, go to [Business Central](https://dynamics.microsoft.com/business-central/overview/) website.

For more information about synchronising user information with Microsoft 365, go to the [Synchronisation with Microsoft 365](#m365) section.

> [!NOTE]
> If you use an external accountant to manage your books and financial reporting, you can invite them to your [!INCLUDE[prod_short](includes/prod_short.md)] so they can work with you on your fiscal data. For more information, see [Inviting Your External Accountant to Your Business Central](finance-accounting.md#inviteaccountant).

### <a name="to-remove-a-users-access-to-the-system"></a>To remove a user's access to the system

You can remove a user's access to [!INCLUDE[prod_short](includes/prod_short.md)] online. All references to the user are kept. However, the user can't sign in and active sessions for the user are stopped.

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Users**, and then choose the related link.
2. Open the **User Card** page for the relevant user, and then, in the **Status** field, select **Disabled**.
3. To give the user access again, set the **Status** field to **Enabled**.

You can also remove the licence from a user in the Microsoft 365 Admin Centre. The user is then unable to sign in. For more information, see [Remove licences from users](/microsoft-365/admin/manage/remove-licenses-from-users).

### <a name="synchronization-with-microsoft-365"></a><a name="m365"></a>Synchronisation with Microsoft 365

When you assign a licence for [!INCLUDE[prod_short](includes/prod_short.md)] to a user in Microsoft 365, there are two ways to create the user in [!INCLUDE[prod_short](includes/prod_short.md)].  

- The administrator can add the user by choosing the **Update Users from Microsoft 365** action on the **Users** page as described in the [To add a user or update user information in Business Central](#adduser) section.
- The licence information will update automatically when the user signs in for the first time.

In both cases, several settings are applied automatically. These settings are listed in the second and third columns in the table below.

If you change user information in Microsoft 365, you can update [!INCLUDE[prod_short](includes/prod_short.md)] to reflect the change. Depending on what you want to update, use one of the actions on the **Users** page. The actions are described in the last two columns in the table below.

|What happens when:|First user, first sign-in|Update Users from Microsoft 365|Restore User Default User Groups|
|-|-|-|-|
|Scope:|Current user|Multiple selected users|Single selected user (except current)|
|Create the new user and assign SUPER permission set.<br /><br /><!--Platform-->|**X**|**X** | | 
|Update the user based on information in Microsoft 365: Status, Full Name, Contact Email, Authentication Email.<!--<br /><br />Codeunit "Azure AD   Graph User".UpdateUserFromAzureGraph-->|**X**|**X**|**X**|
|Synchronise user plans (licences) with licences and roles assigned in Microsoft 365.<!--<br /><br />Codeunit "Azure AD   Graph User".UpdateUserPlans-->|**X**|**X**|**X**|
|Add the user to user groups according to the current user plans. Remove the SUPER permission set for all users other than the first user to sign in and [administrators](/dynamics365/business-central/dev-itpro/administration/tenant-administration). At least one SUPER is required.<!--<br /><br />Codeunit "Permission Manager". AddUserToDefaultUserGroups-->|**X**|**X**|**X**<br /><br />Removes manually assigned user groups and permissions.|

Users can access [!INCLUDE[prod_short](includes/prod_short.md)] records in Teams using only their Microsoft 365 licence. When access is enabled for an environment, synchronising using the **Update users from Microsoft 365** action won't include users that only have a Microsoft 365 licence. To include these users in synchronisation, you must first update environment settings by assigning a security group that contains users with a [!INCLUDE[prod_short](includes/prod_short.md)] licence and users with only a Microsoft 365 licence.

Learn about securing access to environments using security groups at [Manage access using Azure Active Directory groups](/dynamics365/business-central/dev-itpro/administration/tenant-admin-center-manage-access#manage-access-using-azure-active-directory-groups).

Get an overview of accessing [!INCLUDE[prod_short](includes/prod_short.md)] in Teams with Microsoft 365 licences at [admin-access-with-m365-licence](admin-access-with-m365-license.md).

## <a name="manage-users-and-licenses-in-on-premises-deployments"></a>Manage users and licences in on-premises deployments

For on-premises deployments, the number of user licences is specified in the licence file (.bclicense or .flf). When an administrator or Microsoft partner uploads the licence file, they can specify which users can sign in to [!INCLUDE[prod_short](includes/prod_short.md)].

For on-premises deployments, the administrator creates, edits, and deletes users directly from the **Users** page.

### <a name="to-edit-or-delete-a-user-in-an-on-premises-deployment"></a>To edit or delete a user in an on-premises deployment

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Users**, and then choose the related link.
2. Select the user that you want to edit, and then choose the **Edit** action.
3. On the **User Card** page, change the information as necessary.  
4. To delete a user, select the user that you want to delete, and then choose the **Delete** action.

> [!NOTE]
> For on-premises deployments an administrator can specify how to authenticate user credentials in the [!INCLUDE[server](includes/server.md)] instance. When you create a user, you provide the credential type that you are using.
>
> For more information, see the [Authentication and Credential Types](/dynamics365/business-central/dev-itpro/administration/users-credential-types) in the administration Help for [!INCLUDE[prod_short](includes/prod_short.md)].

## <a name="see-also"></a>See Also

[Assign Permissions to Users and Groups](ui-define-granular-permissions.md)  
[Manage Profiles](admin-users-profiles-roles.md)  
[Change Which Features are Displayed](ui-experiences.md)  
[Customising [!INCLUDE[prod_short](includes/prod_short.md)]](ui-customizing-overview.md)  
[Getting Ready for Doing Business](ui-get-ready-business.md)  
[Administration](admin-setup-and-administration.md)  
[Licensing in Dynamics 365 Business Central](/dynamics365/business-central/dev-itpro/deployment/licensing)  
[Add Users to Microsoft 365 for business](/microsoft-365/admin/add-users/add-users)  
[Security and Protection in Business Central (administration content)](/dynamics365/business-central/dev-itpro/security/security-and-protection)  
[Assign a telemetry ID to users](/dynamics365/business-central/dev-itpro/administration/telemetry-enable-application-insights#assign-a-telemetry-id-to-users)  


[!INCLUDE[footer-include](includes/footer-banner.md)]
