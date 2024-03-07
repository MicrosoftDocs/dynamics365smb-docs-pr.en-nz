---
title: Define Granular Permissions
description: This article describes how to define granular permissions and assign each user the permission sets that they need to do their jobs.
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bholtorf
ms.topic: conceptual
ms.search.keywords: 'access, right, security'
ms.search.form: '1, 119, 8930, 9800, 9807, 9808, 9830, 9831, 9802, 9855, 9862'
ms.date: 02/08/2023
ms.service: dynamics-365-business-central
---

# Assign Permissions to Users and Groups

[!INCLUDE [2023rw1-sec-group-long](includes/2023rw1-sec-group-long.md)]

The [!INCLUDE[prod_short](includes/prod_short.md)] security system controls which objects a user can access within each database or environment, in combination with the user's licence. For each user you can specify whether they're able to read, modify, or enter data in database objects. For more information, see [Data Security](/dynamics365/business-central/dev-itpro/security/data-security?tabs=object-level) in the developer and administration content for [!INCLUDE[prod_short](includes/prod_short.md)].

Before you assign permissions to users and user groups, you must define who can sign in by creating users according to their licence. For more information, see [Create Users According to Licences](ui-how-users-permissions.md).

In [!INCLUDE[prod_short](includes/prod_short.md)], there are two levels of permissions to database objects:

- Overall permissions according to the licence, also referred to as the entitlement.

  The licences include default permission sets. Starting in 2022 release wave 1, admins can customise these default permissions for the relevant licence types. For more information, see [Configure permissions based on licences](ui-how-users-permissions.md#licensespermissions).  

- Detailed permissions that you assign in [!INCLUDE[prod_short](includes/prod_short.md)].

This article describes how to define, use, and apply permissions in [!INCLUDE [prod_short](includes/prod_short.md)] to change the default configuration.  

[!INCLUDE [admin-gdap-users](includes/admin-gdap-users.md)]  
For more information, see [Delegated administrator access to Business Central Online](/dynamics365/business-central/dev-itpro/administration/delegated-admin).  

[!INCLUDE [prod_short](includes/prod_short.md)] online includes default user groups that are assigned to users automatically based on their licence. You can change the default configuration by modifying or adding security groups, permission sets, and permissions. The following table outlines key scenarios for modifying the default permissions.  

|To  |See  |
|---------|---------|
|To make it easier to manage permissions for multiple users, you can organise them in security groups and then assign or change one permission set for many users in one action.| [To manage permissions through user groups](#to-manage-permissions-through-user-groups) |
|To manage permission sets for specific users | [To assign permission sets to users](#to-assign-permission-sets-to-users) |
|To learn how to define a permission set|[To create a permission set](#to-create-a-permission-set)|
|To view or troubleshoot a user's permissions|[To get an overview of a user's permissions](#to-get-an-overview-of-a-users-permissions)|
|To learn about record-level security|[Security filters limit a user's access to specific records in a table](#security-filters-limit-a-users-access-to-specific-records-in-a-table)|

> [!NOTE]
> An broader way to define which features users have access to is by setting the **Experience** field on the **Company Information** page. For more information, see [Change Which Features are Displayed](ui-experiences.md).
>
> You can also define the features that are available to users in the user interface and how they interact with them through pages. You do this through profiles that you assign to different types of users according to their job role or department. For more information, see [Manage Profiles](admin-users-profiles-roles.md) and [Customising [!INCLUDE[prod_short](includes/prod_short.md)]](ui-customizing-overview.md).

## To create a permission set

> [!NOTE]
> In 2022 release wave 2 we made it easier to add permissions to permission sets. Rather than adding permissions individually, you can add entire permission sets. If needed, you can then exclude individual permissions in them. For more information, see [To add other permission sets](#to-add-other-permission-sets). To make that possible, we replaced the Permission Set page with a new one. The key differences are the new **Permission Sets** and **Results** panes, and the **Included permissions** FactBox. To continue using the replaced Permissions page, on the **Permission Sets** page, choose the **Permissions (legacy)** action.

Maintenance is also easier. When you add a system permission, your user-defined permission set will be automatically updated with any changes that Microsoft makes to those permissions.

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Permission Sets**, and then choose the related link.
2. Choose the **New** action.
3. On the new line, fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4. Choose the **Permissions** action.
5. On the **Permission Set** page, in the **Type** field, include or exclude permissions to the object as follows:

  To include the permission, choose **Include**, and then choose level of access to give in the **Read Permission**, **Insert Permission**, **Modify Permission**, **Delete Permission**, and **Execute Permission** fields. The following table describes the options.

  |Option|Description|Ranking|
  |------|-----------|-------|
  |**Blank**|The user can't perform the action on the object.|Lowest|  
  |**Yes**|The user can perform the action on the object.|Highest|
  |**Indirect**|The user can perform the action on the object, but only through another related object that the user has full access to. For more information, see [Example - Indirect Permission](#example---indirect-permission) in this article, and [Permissions Property](/dynamics365/business-central/dev-itpro/developer/properties/devenv-permissions-property#example---indirect-permission) in Developer and IT-Pro Help.|Second highest|
  
  To exclude the permission, or one or more access levels, choose **Exclude**, and then choose the level of access to give. The following table describes the options.

  |Option|Description|
  |------|-----------|-------|
  |**Blank**|Use the access level based on the hierarchy of permissions in the set.  |
  |**Exclude**|Remove the specific access level for the object.|
  |**Reduce to indirect**|Change the access level to Indirect if any permission sets give Direct access to the object. For example, choose this option if the permission set gives Direct access to G/L entries but you don't want users to have full access to the entries.|
  
  > [!NOTE]
  > If a permission is in a permission set that is included, and is also in a permission set that is excluded, the permission will be excluded.

6. Use the **Object Type** and **Object ID** fields to specify the object you're giving access to.

  > [!TIP]
  > New lines show default values. For example, the **Object Type** field contains **Table Data**, and the **Object ID** field contains **0**. The default values are just placeholders, and aren't used. You must choose a type of object and an object in the **Object ID** field before you can create another new line.

7. Optional: If you're defining permissions for a Table Data object type, in the **Security Filter** field you can filter the data that a user can access in fields on the selected table. For example, you might want to let a user access only records that contain information about a particular customer. For more information, see [Security filters limit a user's access to specific records in a table](#security-filters-limit-a-users-access-to-specific-records-in-a-table) and [Using Security Filters](/dynamics365/business-central/dev-itpro/security/security-filters).
8. Optional: On the **Permission Sets** pane, add one or more other permission sets. For more information, see [To add other permission sets](#to-add-other-permission-sets).

> [!IMPORTANT]
> Use caution when assigning **Insert Permission** or **Modify Permission** to the **9001 User Group Member** or **9003 User Group Permission Set** table. Any users assigned to the permission set could potentially assign themselves to other user groups, which in turn might give them unintended permissions.

### Example - Indirect Permission

You can assign Indirect permission to allow a user to use an object, but only through another object. For example, a user has permission to run codeunit 80, Sales-Post. The Sales-Post codeunit performs many tasks, including modifying table 37, Sales Line. When the user posts a sales document using the Sales-Post codeunit, [!INCLUDE[prod_short](includes/prod_short.md)] checks whether the user has permission to modify the Sales Line table. If not, the codeunit can't complete its tasks, and the user receives an error message. If so, the codeunit runs successfully.

However, the user doesn't need to have full access to the Sales Line table to run the codeunit. If the user has Indirect permission for the Sales Line table, the Sales-Post codeunit runs successfully. When a user has Indirect permission, they can only modify the Sales Line table by running the Sales-Post codeunit or another object that has permission to modify the Sales Line table. The user can only modify the Sales Line table when doing so from supported application areas. The user can't run the feature inadvertently or maliciously by other methods.

### To add other permission sets

Expand a permission set by adding other permission sets to it. Afterward, you can include or exclude specific permissions, or entire permission sets, in each set you add. This includes permissions in the Extension and System type permission sets, which otherwise isn't allowed. Exclusions apply only to the permission set you're expanding. The original set isn't affected.

On the **Permission Set** page, add a permission set on the **Permission Sets** pane. The **Result** pane lists all added permission sets. To explore the permissions that are included in a set you've added, choose the set on the Result pane and the **Included permissions** FactBox will show the permissions.

On the **Result** pane, use the **Inclusion Status** field to identify the permission sets in which you've excluded permissions or permission sets. If something's been excluded, the status will be **Partial**.

For an overall view of permissions in the permission set, choose the **View all permissions** action. The **Expanded Permissions** page shows all permissions that were already assigned to the permission set and the permissions in the added permission sets.

To fully exclude all permissions from a permission set, on the **Result** pane, select the line, choose **Show more options**, and then choose **Exclude**. When you exclude a permission set, a line is created on the **Permission Sets** pane of the type Excluded. If you've excluded a permission set, but want to include it again, delete the line on the **Permission Sets** pane.

To fully or partially exclude a specific permission in a set you've added, under **Permissions**, create a line for the object. The access level fields, Insert Permission, Modify Permission, and so on, will all contain **Exclude**. To allow a certain access level, choose the appropriate option.

Excluding a permission set excludes all of the permissions in the set. [!INCLUDE [prod_short](includes/prod_short.md)] calculates permissions as follows:

1. Calculate the full list of included permissions
2. Calculate the full list of excluded permissions
3. Remove excluded permissions from the list of included permissions (removing an indirect permission is the same as Reduce to Indirect)

## To copy a permission set

Create a new permission set by copying another. The new set will include all of the permissions and permission sets from the set you copied. How the permissions and permission sets are arranged in the new permission set differs, depending on your choice in the **Copy operation** field. The following table describes the options.

|Option  |Description  |
|---------|---------|
|**Copy by reference**     | The original permission set and all of the permission sets that were added to it are listed on the **Results** pane.       |
|**Flat permission copy**  | All permissions from all permission sets are included in a flat list on the **Permissions pane**. Permissions are not organised by permission set.        |
|**Clone**     | Create an exact copy of the original permission set.        |

1. On the **Permission Sets** page, select the line for a permission set that you want to copy, and then choose the **Copy Permission Set** action.
2. On the **Copy Permission Set** page, specify the name of the new permission set.
3. In the **Copy operation** field, specify how to arrange permission in the new permission set.
4. Optional: If you're adding a System permission set, you might want to be notified if the name or content of the original permission set changes in a future version. This lets you consider whether to update your user-defined permission set. To receive a notification, turn on the **Notify on Changed Permission Set** toggle.

> [!NOTE]
> The notification requires that the **Original System permission set changed** notification is enabled on the **My Notifications** page.

## To create or modify permissions by recording your actions

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Permission Sets**, and then choose the related link.

    Alternatively, on the **Users** page, choose the **Permission Sets** action.
2. On the **Permission Sets** page, choose the **New** Action.
3. On a new line, fill in the fields as necessary.
4. Choose the **Permissions** action.
5. On the **Permissions** page, choose the **Record Permissions** action, and then choose the **Start** action.  
    Recording must be done either by using the **Open this page in a new windows** (pop-out) feature to have the **Permissions** recording window side-by-side, or by working within the same tab.  
    A recording process now starts and captures all of your actions in the user interface.
6. Go to the various pages and activities in [!INCLUDE[prod_short](includes/prod_short.md)] that you want users with this permission set to access. You must carry out the tasks that you want to record permissions for.
7. When you want to finish the recording, return to the **Permissions** page, and then choose the **Stop** action.
8. Choose the **Yes** button to add the recorded permissions to the new permission set.
9. For each object in the recorded list, specify whether users are able to insert, modify, or delete records in the recorded tables.

### To export and import a permission set

To quickly set up permissions, you can import permission sets that you exported from another [!INCLUDE[prod_short](includes/prod_short.md)] tenant.

In multi-tenant environments, a permission set will be imported into a specific tenant. In other words, the scope of the import is *Tenant*.

1. In tenant 1, on the **Permission Sets** page, select the line or lines for the permission sets to export, and then choose the **Export Permission Sets** action.

    An XML file is created in the download folder on your machine. By default, the name is *Export Permission Sets.xml*.

2. In tenant 2, on the **Permission Sets** page, select the **Import Permission Sets** action.
3. On the **Import Permission Sets** dialogue page, consider if you want to merge existing permission sets with any new permission sets in the XML file.

    If you select the **Update existing permissions** checkbox, existing permission sets that match names in the XML file will be merged with the imported permission sets.

    If you don't select the **Update existing permissions** checkbox, permission sets that match names in the XML file will be skipped during import. In that case, you'll be notified about permission sets that are skipped.

4. From the **Import** dialogue page, find and select the XML file to be imported, and then choose the **Open** action.

The permission sets are imported.

## To remove obsolete permissions from all permission sets

On the **Permission Sets** page, choose the **Remove Obsolete Permissions** action.

## To set up time constraints for users

Administrators can define periods of time during which specified users are able to post. Administrators can also specify if the system logs how much time users are signed in. Similarly, administrators can assign responsibility centres to users. For more information, see [Work with Responsibility Centres](inventory-responsibility-centers.md).

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **User Setup**, and then choose the related link.
2. On the **User Setup** page opens, choose the **New** action.
3. In the **User ID** field, enter the ID of a user, or choose the field to see all current Windows users in the system.
4. Fill in the fields as necessary.

## To manage permissions through user groups

User groups help you manage permission sets across the company. [!INCLUDE [prod_short](includes/prod_short.md)] online includes default user groups that are assigned to users automatically based on their licence. You can add users manually to a user group, and you can create new user groups as copies of existing ones.  

You start by creating a user group. Then you assign permission sets to the group to define which object users of the group can access. When you add user to the group, the permission sets defined for the group will apply to the user.

Permission sets assigned to a user through a user group stay synchronised. A change to the user group permissions is automatically propagated to the users. If you remove a user from a user group, the involved permissions are automatically revoked.

### To add users to a user group

The following procedure explains how to create user groups manually. To create user groups automatically, see [To copy a user group and all its permission sets](#to-copy-a-user-group-and-all-its-permission-sets).

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **User Groups**, and then choose the related link.

    1. Alternatively, on the **Users** page, choose the **User Groups** action.
2. On the **User Group** page, choose the **User Group Members** action.
3. On the **User Group Members** page, choose the **Add Users** action.

### To copy a user group and all its permission sets

To quickly define a new user group, you can copy all permission sets from an existing user group to your new user group.

> [!NOTE]
> The user group members are not copied to the new user group. You must add them manually afterwards. For more information, see the [To add users to a user group](#to-add-users-to-a-user-group) section.

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **User Groups**, and then choose the related link.
2. Select the user group that you want to copy, and then choose the **Copy User Group** action.
3. In the **New User Group Code** field, enter a name for the group, and then choose the **OK** button.

The new user group is added to the **User Groups** page. Proceed to add users. For more information, see the [To add users to a user group](#to-add-users-to-a-user-group) section.  

> [!IMPORTANT]
> You'll get a validation error if you're trying to assign a user group to the user that refers to a permission set which was defined in an uninstalled extension. It's because the App ID of the extension is validated whenever it's referenced. To assign that user group to a user, you can either re-install the extension, remove the reference of the uninstalled extension from the permission set, or remove that permission set from the user group.

### To assign permission sets to user groups

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **User Groups**, and then choose the related link.
2. Select the user group that you want to assign permission to.  

    Any permission sets that are already assigned to the user are displayed in the **Permission Sets** FactBox.
3. Choose the **User Permission Sets** action to open the **User Permission Sets** page.
4. On the **User Permission Sets** page, on a new line, fill in the fields as necessary.

### To assign a permission set on the **Permission Set by User Group** page

The following procedure explains how to assign permission sets to a user group on the **Permission Set by User Group** page.

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Users**, and then choose the related link.
2. On the **Users** page, select the relevant user, and then choose the **Permission Set by User Group** action.
3. On the **Permission Set by User Group** page, select the **[user group name]** field on a line for the relevant permission set to assign the set to the user group.
4. Select the **All User Groups** checkbox to assign the permission set to all user groups.

You can also assign permissions sets directly to a user.

## To assign permission sets to users

A permission set is a collection of permissions for specific database objects. All users must be assigned one or more permission sets before they can access [!INCLUDE[prod_short](includes/prod_short.md)].  

A [!INCLUDE[prod_short](includes/prod_short.md)] solution contains predefined permission sets that are added by Microsoft or by your solution provider. You can also add new permission sets tailored to meet the needs of your organisation. For more information, see the [To create a permission set](#to-create-a-permission-set) section.

> [!NOTE]
> If you do not want to restrict a user's access more than already defined by the licence, you can assign a special permission set called SUPER to the user. This permission set ensures that the user can access all objects specified in the licence.
>
> A user with the Essential licence and the SUPER permission set has access to more functionality than users with the Team Member licence and the SUPER permission set.

You can assign permissions sets to users in two ways:

- From the **User Card** page by selecting permission sets to assign to the user.
- From the **Permission Set by User** page by selecting users that a permission set is assigned to.

### To assign a permission set on a user card

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Users**, and then choose the related link.
2. Select the user that you want to assign permission to.
Any permission sets that are already assigned to the user are displayed in the **Permission Sets** FactBox.
3. Choose the **Edit** action to open the **User Card** page.
4. On the **User Permission Sets** FastTab, on a new line, fill in the fields as necessary. For more information, see [To create or edit a permission set](ui-define-granular-permissions.md#to-create-a-permission-set).

   Use the **Company** field to apply to permission set to a specific company. If you leave the field blank, then it applies to all companies.

## To assign a permission set on the Permission Set by User page

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Users**, and then choose the related link.
2. On the **Users** page, choose the **Permission Set by User** action.
3. On the **Permission Set by User** page, select the **[user name]** checkbox on a line for the relevant permission set to assign the set to the user.

    Select the **All Users** checkbox to assign the permission set to all users.

## To get an overview of a user's permissions

You can view other users' effective permissions only if you're assigned to the SECURITY or SUPER permissions. 

The **Effective Permissions** page offers additional information about the source of each permission. For example, whether the source is a security group, or a permission is inherited. The page also contains a column where administrators can review the security filters that are applied. To learn more about security filters, go to [Security filters limit a user's access to specific records in a table](#security-filters-limit-a-users-access-to-specific-records-in-a-table).

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Users**, and then choose the related link.
2. Open the card of the relevant user.
3. Choose the **Effective Permissions** action.

    The **Permissions** part lists all the database objects that the user has access to. You can't edit this section.

    The **By Permission Set** part shows the assigned permission sets through which the permissions are granted to the user, the source and type of the permission set, and to which extent the different access types are permitted.

    For each row that you select in the **Permissions** section, the **By Permission Set** section shows which permission set or sets that the permission is granted through. In this section, you can edit the value in each of the five access type fields, **Read Permission**, **Insert Permission**, **Modify Permission**, **Delete Permission**, **Execute Permission**.

    > [!NOTE]  
    > Only permission sets of type **User-Defined** can be edited.
    >
    > Rows of source Entitlement originate from the subscription licence. The permission values of the entitlement overrule values in other permission sets if they have a higher ranking. A value in a non-entitlement permission set that has a higher ranking than the related value in the entitlement will be surrounded by brackets to indicate that it is not effective as it is overruled by the entitlement.
    >
    > For an explanation of ranking, see [To create a permission set](ui-define-granular-permissions.md#to-create-a-permission-set).  

4. To edit a permission set, in the **By Permission Set** part, on the line for a relevant permission set of type **User-Defined**, choose one of the five access type fields and select a different value.

5. To edit individual permissions within the permission set, choose the value in the **Permission Set** field to open the **Permissions** page.

> [!NOTE]  
> When you edit a permission set, the changes will also apply to other users that have the permission set assigned.

### Security filters limit a user's access to specific records in a table

For record-level security in [!INCLUDE[prod_short](includes/prod_short.md)], use security filters to limit a user's access to data in a table. You create security filters on table data. A security filter describes a set of records in a table that a user has permission to access. You can specify, for example, that a user can only read the records that contain information about a particular customer. In this way, the user can't access the records that contain information about other customers. For more information, see [Using Security Filters](/dynamics365/business-central/dev-itpro/security/security-filters) in the administration content.

## Viewing permission changes telemetry

You can set up [!INCLUDE[prod_short](includes/prod_short.md)] to send changes that are done to permission to an Application Insights resource in Microsoft Azure. Then, using Azure Monitor, you create reports and set up alerts on the gathered data. For more information, see the following articles in the [!INCLUDE[prod_short](includes/prod_short.md)] Developer and admin help:

- [Monitoring and Analysing Telemetry - Enabling Application Insights](/dynamics365/business-central/dev-itpro/administration/telemetry-overview#enable)
- [Analysing Field Monitoring Telemetry](/dynamics365/business-central/dev-itpro/administration/telemetry-permission-changes-trace)

## Delegated admin users

[!INCLUDE [admin-gdap-users](includes/admin-gdap-users.md)]

## See Also

[Create Users According to Licences](ui-how-users-permissions.md)  
[Manage Profiles](admin-users-profiles-roles.md)  
[Change Which Features are Displayed](ui-experiences.md)  
[Customising [!INCLUDE[prod_short](includes/prod_short.md)]](ui-customizing-overview.md)  
[Getting Ready for Doing Business](ui-get-ready-business.md)  
[Administration](admin-setup-and-administration.md)  
[Add Users to Microsoft 365 for business](/microsoft-365/admin/add-users/add-users)  
[Security and Protection in Business Central](/dynamics365/business-central/dev-itpro/security/security-and-protection) in Developer and IT-pro Help  
[Assign a telemetry ID to users](/dynamics365/business-central/dev-itpro/administration/telemetry-enable-application-insights#assign-a-telemetry-id-to-users)  


[!INCLUDE[footer-include](includes/footer-banner.md)]
