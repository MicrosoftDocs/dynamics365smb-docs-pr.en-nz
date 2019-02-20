---
title: Choosing the User Experience to Show or Hide Advanced Features | Microsoft Docs
description: Learn what the Essential and Premium user experience tiers mean for the user interface, application areas, and your company.
documentationcenter: 
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: essential, basic, user interface, application area, experience
ms.date: 02/04/2019
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: ce612d546349d05883016646fe14a35553c2f55a
ms.openlocfilehash: 3317df5f54a359e5b143d5b288a378a350d49440
ms.contentlocale: en-nz
ms.lasthandoff: 02/04/2019

---
# <a name="changing-which-features-are-displayed"></a>Changing Which Features are Displayed
[!INCLUDE[d365fin](includes/d365fin_md.md)] is designed to help you run your business, regardless which line of business you are in. At the core of [!INCLUDE[d365fin](includes/d365fin_md.md)], you find financial reporting and sales and purchasing processes. You add experiences to that according to your business needs by adding extensions from AppSource or by changing the Experience setting for your company. For more information, see [Customising [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions](ui-extensions.md), or the "Choosing a User Experience to Show or Hide Features" section below.

## <a name="choosing-a-user-experience-to-show-or-hide-features"></a>Choosing a User Experience to Show or Hide Features
The user experience determines how much of the core functionality is available when you and your colleagues use [!INCLUDE[d365fin](includes/d365fin_md.md)]. You can choose the user experience for your company on the **Company Information** page, in the **Experience** field.

> [!NOTE]  
> This setting applies to all users in your company. Users can customise their own experience even further by changing page layouts and content. For more information, see [Personalising Your Workspace and Pages](ui-personalization-user.md).  

The following table lists the experiences that are currently available.

| Experience | Impact on User Interface |
| --- | --- |
| **Essential** |Shows all actions and fields for all common business functionality.|
| **Premium** |Shows all actions and fields for all business functionality, including Manufacturing and Service Management.|

> [!NOTE]  
> The experiences that you can select from in [!INCLUDE[d365fin](includes/d365fin_md.md)] depend on your solution licence, called a plan. For information about the **Essential** and **Premium** plans, see [Business Central](https://go.microsoft.com/fwlink/?linkid=870242) on the Microsoft Dynamics 365 marketing site. See also the [[!INCLUDE[d365fin](includes/d365fin_md.md)] Licensing Guide](https://go.microsoft.com/fwlink/?linkid=2068931) (requires access to CustomerSource or PartnerSource).

> [!IMPORTANT]  
> All regular users in a solution must be assigned the same plan, Essential or Premium, before that experience can be selected for the company. Accordingly, one user cannot access Premium features if one or more other users can only access Essential features. This is not the case for non-regular users of type Team Member, Internal Admin, External Accountant, and Delegated Admin, who can each be assigned a different plan than other users in the solution.

## <a name="enabling-premium-features-after-upgrading-a-plan"></a>Enabling Premium Features after Upgrading a Plan
Users are assigned to plans in Office 365 Admin Centre in connection with the general work to create the Business Central users. For more information, see [Add Users to Office 365 for business](https://support.office.com/en-us/article/Add-users-to-Office-365-for-business-435ccec3-09dd-4587-9ebd-2f3cad6bc2bc).

You can then define which specific functions and pages within the experience those users are allowed to access by assigning permission sets. For more information, see [Managing Users and Permissions](ui-how-users-permissions.md).

### <a name="to-update-plan-changes-in-users-groups"></a>To update plan changes in users groups
When you have made a change to users plans in Office 365 Admin Centre, such as assigned more users to the Premium plan, you must reflect the change in [!INCLUDE[d365fin](includes/d365fin_md.md)].

1. Sign is as an administrator.
2. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Users**, and then choose the related link.
3. On the **Users** page, choose the **Refresh all User Groups** action.

All new information about the users’ plans and their assigned user groups are now updated according to the plan changes.

### <a name="to-select-the-premium-experience"></a>To select the Premium experience
You can now proceed to select the new experience.
1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Company Information**, and then choose the related link.
2. On the **Company Information** page, on the **User Experience** FastTab, select Premium  in the **Experience** field.

## <a name="help-assumes-premium-experience"></a>Help Assumes Premium Experience
All feature descriptions in user documentation for [!INCLUDE[d365fin](includes/d365fin_md.md)] assume the **Premium** experience, meaning the descriptions cover the full scope of UI elements. A text note is inserted in high-level help topics for the Manufacturing and Service Managements feature areas stating that they require the **Premium** experience.

## <a name="see-also"></a>See also 
[Creating New Companies](about-new-company.md)  
[Managing Users and Permissions](ui-how-users-permissions.md)    
[Changing Basic Settings](ui-change-basic-settings.md)  
[Customising [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions](ui-extensions.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  
[[!INCLUDE[d365fin](includes/d365fin_md.md)] Licensing Guide](https://go.microsoft.com/fwlink/?LinkId=871590&clcid=0x409)

## [!INCLUDE[d365fin](includes/free_trial_md.md)]  

