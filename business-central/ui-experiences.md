---
title: Change which features are displayed
description: 'Learn what the Essential and Premium user experience tiers mean for the user interface, application areas, and your company.'
author: brentholtorf
ms.topic: conceptual
ms.devlang: al
ms.search.keywords: 'essential, basic, user interface, application area, experience'
ms.search.form: 1
ms.date: 04/01/2021
ms.author: bholtorf
ms.service: dynamics-365-business-central
---
# <a name="change-which-features-are-displayed"></a>Change Which Features are Displayed
[!INCLUDE[prod_short](includes/prod_short.md)] is designed to help you run your business regardless of the size and complexity. At the core of the product, you find essential features, such as financial reporting, sales, purchasing, and inventory management. As business complexity increases, you can turn on functionality for manufacturing and service management, for example.

You can define the product complexity level, and thereby which features the company's users get access to, by changing the **Experience** setting on the **Company Information** page. Note that the experience setting can also be changed by adding certain extensions from AppSource. For more information, see [Customizing [!INCLUDE[prod_short](includes/prod_short.md)] Using Extensions](ui-extensions.md).

The following table lists the experiences that are currently available.

| Experience | Impact on User Interface |
| --- | --- |
| **Essential** |Shows all actions and fields for all common business functionality.|
| **Premium** |Shows all actions and fields for all business functionality, including Manufacturing and Service Management.|

The experiences that can be selected in [!INCLUDE[prod_short](includes/prod_short.md)] reflect the solution licences, called plans, that are defined for the product. For information about the Essential and Premium plans, see [Business Central](https://go.microsoft.com/fwlink/?linkid=870242) on the Microsoft Dynamics 365 marketing site. See also the [[!INCLUDE[prod_short](includes/prod_short.md)] Licensing Guide](https://go.microsoft.com/fwlink/?linkid=2068931).

> [!IMPORTANT]  
> All regular users in a solution must be assigned the same plan, Essential or Premium, before that experience can be selected for the company. Accordingly, one user cannot access Premium features if one or more other users can only access Essential features. This is not the case for non-regular users of type Team Member, Internal Admin, External Accountant, and Delegated Admin, who can each be assigned a different plan than other users in the solution.<br /><br /> Only users of type Evaluation or Premium can change the value in the **Experience** field from Essential to Premium.

Prior to defining a company's experience setting, you define users' access to specific functions and pages by assigning permission sets. For more information, see [Assign Permissions to Users and Groups](ui-define-granular-permissions.md).

The **Experience** setting applies to all users in a company, but each user can personalise their own experience further by changing page layouts and content. For more information, see [Personalise Your Workspace](ui-personalization-user.md).

## <a name="enabling-premium-features-after-upgrading-a-plan"></a>Enabling Premium Features after Upgrading a Plan
Users are assigned to plans in Microsoft 365 Admin Centre in connection with the general work to create the Business Central users. For more information, see [Add users and assign licences at the same time](/microsoft-365/admin/add-users/add-users?view=o365-worldwide&preserve-view=true).

### <a name="to-update-plan-changes-in-users-groups"></a>To update plan changes in users groups

[!INCLUDE [2023rw1-sec-group-short](includes/2023rw1-sec-group-short.md)]

When you have made a change to users plans in Microsoft 365 Admin Centre, such as assigned more users to the Premium plan, you must update [!INCLUDE[prod_short](includes/prod_short.md)] to reflect the change.

1. Sign is as an administrator.
2. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Users**, and then choose the related link.
3. On the **Users** page, choose the **Update users from Microsoft 365** action.

### <a name="to-select-the-premium-experience"></a>To select the Premium experience
You can now proceed to select the new experience.
1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Company Information**, and then choose the related link.
2. On the **Company Information** page, on the **User Experience** FastTab, select Premium  in the **Experience** field.

## <a name="help-assumes-premium-experience"></a>Help Assumes Premium Experience
All feature descriptions in user documentation for [!INCLUDE[prod_short](includes/prod_short.md)] assume the **Premium** experience, meaning the descriptions cover the full scope of UI elements.

## <a name="see-also"></a>See also
[Personalise Your Workspace](ui-personalization-user.md)  
[Customising Business Central](ui-customizing-overview.md)  
[Assign Permissions to Users and Groups](ui-define-granular-permissions.md)  
[Creating New Companies](about-new-company.md)  
[Change Basic Settings](ui-change-basic-settings.md)  
[Work with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  
[[!INCLUDE[prod_short](includes/prod_short.md)] Licensing Guide](https://go.microsoft.com/fwlink/?LinkId=871590&clcid=0x409)

## [!INCLUDE[prod_short](includes/free_trial_md.md)]  


[!INCLUDE[footer-include](includes/footer-banner.md)]
