---
title: Control Access Using Security Groups
description: This article describes how to use security groups to define user permissions.
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bholtorf
ms.topic: conceptual
ms.search.keywords: 'access, right, security, permissions'
ms.search.form: '1, 119, 8930, 9800, 9807, 9808, 9830, 9831, 9802, 9855, 9862'
ms.date: 02/08/2023
---

# Control Access to Business Central Using Security Groups

Security groups make it easier for administrators to manage user permissions. For example, for [!INCLUDE [prod_short](includes/prod_short.md)] online, they're reusable across Dynamics 365 applications, such as SharePoint Online, CRM Online, and [!INCLUDE [prod_short](includes/prod_short.md)]. Administrators add permissions to their [!INCLUDE [prod_short](includes/prod_short.md)] security groups, and when they add users to the group the permissions apply to all members. For example, an administrator can create a [!INCLUDE [prod_short](includes/prod_short.md)] security group that gives salespeople the ability to create and post sales orders. Or, let purchasers do the same for purchase orders.

## Business Central online and on-premises

You can use security groups for the online and on-premises versions of [!INCLUDE [prod_short](includes/prod_short.md)]. Depending on your version, create groups in one of the following ways:

* For the online version, use Microsoft Entra security groups. To learn more about creating the group, go to [Create, edit, or delete a security group in the Microsoft 365 admin centre](/microsoft-365/admin/email/create-edit-or-delete-a-security-group).
* For on-premises, use Windows Active Directory groups. To learn more, go to [Create a Group Account in Active Directory](/windows/security/operating-system-security/network-security/windows-firewall/create-a-group-account-in-active-directory).

Afterward, create a corresponding security group in [!INCLUDE [prod_short](includes/prod_short.md)], and then link it to the group you created. To learn more, go to [Add a security group in Business Central](#add-a-security-group-in-business-central).

> [!NOTE]
> If you've set up a special type of user with a Windows Group licence type in a version of [!INCLUDE [prod_short](includes/prod_short.md)] on-prem that's earlier than 2023 release wave 1, when you upgrade [!INCLUDE [prod_short](includes/prod_short.md)] converts the user to a security group. The new security group has the same name as the Windows group name. The security group gives you a better overview of the group members and their effective permissions.

## Add a security group in Business Central

1. Choose the ![Lightbulb that opens the Tell Me feature 1.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Security Groups**, and then choose the related link.
1. Choose **New** to create a group.
1. Create the link to your group, as follows:

    * For [!INCLUDE [prod_short](includes/prod_short.md)] online, choose the group in the **AAD security group name** field.
    * For [!INCLUDE [prod_short](includes/prod_short.md)] on-premises, choose the group in the **Windows group name** field.

> [!NOTE]
> The users show in the **Members** card on the FactBox pane or the **Security Group Members** page only if they're added as users in [!INCLUDE [prod_short](includes/prod_short.md)]. To learn more about adding users, go to [To add users or update user information and licence assignments in Business Central](ui-how-users-permissions.md#adduser).  

### Assign permissions to a security group

1. On the **Security Groups** page, choose the group, and then choose the **Permissions** action.
1. Assign permissions in the following ways:

    * To assign permission sets individually, in the **Permission Set** field, choose the permissions to assign.
    * To assign multiple permission sets, choose the **Select Permission Sets** action, and then choose the sets to assign.

## Review the permissions in a security group

On the **Security Groups** page, the FactBox pane shows the **Permission Sets** that are assigned to the group. Each user listed in the **Members** card has those permissions. The **Permission Set by Security Group** action provides a more detailed view. There you can also explore the individual permissions in each security group.

Permissions are also available on the **Users** page. The FactBox pane shows the **Permission Sets from Security Group** and **Security Group Memberships** cards for the selected user.

## Security groups and user groups

> [!NOTE]
> User groups will no longer be available in a future release.

Security groups are very similar to the user groups that are currently available. However, user groups are only relevant for [!INCLUDE [prod_short](includes/prod_short.md)]. Security groups are based on groups in Azure Active Directory or Windows Active Directory, depending on whether you're using [!INCLUDE [prod_short](includes/prod_short.md)] online or on-premises, respectively. Groups benefit administrators because they can use them with other Dynamics 365 apps. For example, if salespeople use [!INCLUDE [prod_short](includes/prod_short.md)]and SharePoint, administrators don't have to recreate the group and its members.

### Optional: Convert user groups to permission sets

In 2023 release wave 1 and later, you can convert user groups to permission sets in your tenant. The permission sets provide the same functionality as user groups. Here are some examples:

* You can use the **Users** FactBox to manage permissions for users.
* You can drill down on the permission set name to add other permission sets to the set you're working on. To learn more, go to [To add other permission sets](ui-define-granular-permissions.md#to-add-other-permission-sets).

Use the **User Group Migration** assisted setup guide to convert your groups. To start the guide, on the **Feature Management** page, find **Feature: Convert user group permissions**, and then choose **All Users** in the **Enabled For** field. The assisted setup guide offers the following options for the conversion.

|Option  |Description  |
|---------|---------|
|Assign to user     | Assign the permissions in user groups directly to the users who were assigned to the group, and remove their user group assignments.        |
|Convert to a permission set     | Create a new permission for the permissions in each user group. The new permission set is assigned to all members of each user group.          |

### Licence configurations still apply

You can configure permissions in [!INCLUDE [prod_short](includes/prod_short.md)] based on licences. Those permissions are directly assigned to new users. These configurations still apply, even if you start using security groups.

To use security groups exclusively, we recommend that you remove the licence configurations. To learn more about licence configurations, go to [Create Users According to Licences](ui-how-users-permissions.md).

You can remove licence configurations on the **Licence Configuration** page. Choose a licence, and then delete all permission sets assigned to it.

## See Also

[Create Users According to Licences](ui-how-users-permissions.md)  
[Set Up Business Central Access in Teams with Microsoft 365 Licences](admin-access-with-m365-license-setup.md)  
[Learn about groups and access rights in Azure Active Directory](/azure/active-directory/fundamentals/concept-learn-about-groups)  
[Active Directory security groups](/windows-server/identity/ad-ds/manage/understand-security-groups)  