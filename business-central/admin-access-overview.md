---
title: Manage Access to Business Central
description: Administrators use a layered approach to controlling access to Business Central and its capabilities.
author: brentholtorf
ms.author: bholtorf
ms.reviewer: jswymer
ms.topic: overview
ms.date: 04/04/2023
ms.custom: bap-template
---

# <a name="manage-access-to-business-central" />Manage Access to Business Central

This article gives administrators and application developers a high-level overview of how to control access to [!INCLUDE [prod_short](includes/prod_short.md)] and its features. Use the links to go to other articles that provide more details about the subjects.

## <a name="layered-access" />Layered access

[!INCLUDE [prod_short](includes/prod_short.md)] uses a layered approach to application security, as outlined in the following diagram. To learn more about each layer, go to [Application Security in Business Central](/dynamics365/business-central/dev-itpro/security/security-application).

:::image type="content" source="media/security-overview.png" alt-text="Layered application security in Business Central.":::

## <a name="licenses" />Licences

Assign [!INCLUDE [prod_short](includes/prod_short.md)] users to a **Dynamics 365 Business Central** licence so they can view, modify, and act on their business data from any user interface. To learn more about licences, go to [Licensing in Dynamics 365 Business Central](/dynamics365/business-central/dev-itpro/deployment/licensing).

However, folks who occasionally need read-only access to information in [!INCLUDE [prod_short](includes/prod_short.md)] can use a **Microsoft 365** licence. To learn more about giving limited access, go to [Business Central Access with Microsoft 365 Licences](admin-access-with-m365-license.md).

For comprehensive information about the different types of licences and how licensing works in [!INCLUDE[prod_short](includes/prod_short.md)], [download the Dynamics 365 Licensing Guide](https://go.microsoft.com/fwlink/?LinkId=866544).

## <a name="business-central-administrator-tasks" />Business Central administrator tasks

The following table lists how administrators can control access to [!INCLUDE [prod_short](includes/prod_short.md)] and the features people will use. Some of the tasks also help keep access settings up to date.

|Task| Learn more |
|--|--|--|
|Each person must have a user account before they can sign in to [!INCLUDE [prod_short](includes/prod_short.md)]. The easiest way to set up users is to add them one at a time in the [Microsoft 365 admin centre](https://go.microsoft.com/fwlink/p/?linkid=2024339). |[Add users and assign licences at the same time](/microsoft-365/admin/add-users/add-users)|
|Manage access for all users at the environment level. Create an Azure Active Directory (Azure AD) security group and assign it to the environment.<br><br> You can also use security groups to manage access for specific groups of users. | [Manage Access to Environments](/dynamics365/business-central/dev-itpro/administration/tenant-admin-center-manage-access)<br><br>[Control Access to Business Central Using Security Groups](ui-security-groups.md) |
|Create users in [!INCLUDE [prod_short](includes/prod_short.md)], and define who can sign in. | [Create Users According to Licences](ui-how-users-permissions.md) |
|In combination with user licences, permissions define the objects that a user can access within each database or environment. Specify whether people can read, modify, or enter data in database objects. |[Assign Permissions to Users and Groups](ui-define-granular-permissions.md)|
|If an external accountant manages your books and financial reporting, invite them to your [!INCLUDE [prod_short](includes/prod_short.md)]. They'll be able to work more closely with you on your fiscal data.|[Accountant Experiences in [!INCLUDE[prod_long](includes/prod_long.md)]](finance-accounting.md)|
|If you're a [!INCLUDE [prod_short](includes/prod_short.md)] reselling partner, you can send an email to a customer to request a reseller relationship. You can include delegated administration privileges for Azure Active Directory and Microsoft 365 in the email.| [Delegated Administrator Access to Business Central Online](/dynamics365/business-central/dev-itpro/administration/delegated-admin)|
|An Azure service tag represents a group of IP addresses that traffic for a service can come from or go to. Use service tags to set up firewalls to allow traffic only from certain services. The **Dynamics365BusinessCentral** tag lets you use firewall and network security group rules to restrict traffic to and from [!INCLUDE [prod_short](includes/prod_short.md)].| [Azure security service tags](/dynamics365/business-central/dev-itpro/security/security-service-tags)|
|When using Azure Active Directory authentication with [!INCLUDE [prod_short](includes/prod_short.md)], we recommend you take advantage of [Azure AD Multi-Factor Authentication (MFA)](/azure/active-directory/authentication/concept-mfa-howitworks). MFA further safeguards access to the application and data.|[Multi-Factor Authentication for Dynamics 365 Business Central](/dynamics365/business-central/dev-itpro/security/multifactor-authentication)|

## <a name="business-central-developer-tasks" />Business Central developer tasks

There's also a developer story for managing access to [!INCLUDE [prod_short](includes/prod_short.md)]. For example, developers and administrators can build and connect applications to [!INCLUDE [prod_short](includes/prod_short.md)] that benefit the business:  

* Streamline business processes
* Improve customer interactions
* Make better decisions, faster

The following table links to information about how to give apps and extensions access to [!INCLUDE [prod_short](includes/prod_short.md)] data.

| Task | Learn more |
|--|--|
|The two main concepts for defining access to features are entitlements and permissions. Entitlements give broad access to objects according to licences or Azure Active Directory roles. Permissions and permission sets let you fine-tune access to objects. |[Entitlements and Permission Sets Overview](/dynamics365/business-central/dev-itpro/developer/devenv-entitlements-and-permissionsets-overview)|

## <a name="see-also" />See Also

[Security in Business Central](/dynamics365/business-central/dev-itpro/security/security-and-protection)
