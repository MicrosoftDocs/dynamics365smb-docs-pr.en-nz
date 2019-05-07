---
title: Viewing and Editing Basic Settings | Microsoft Docs
description: Learn how to change some basic settings, for example, the Role Centre, company, or the work date.
author: SusanneWindfeldPedersen
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: change Role Center, notification, change company, change work date
ms.date: 04/01/2019
ms.author: solsen
ms.openlocfilehash: d95d2f609129e4bdba35deda726323dbed2ba67a
ms.sourcegitcommit: bd78a5d990c9e83174da1409076c22df8b35eafd
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 03/31/2019
ms.locfileid: "916238"
---
# <a name="changing-basic-settings"></a>Changing Basic Settings
In the [**My Settings**](https://businesscentral.dynamics.com?page=9176 "Go directly to your user settings page in Business Central") page, you can see and change basic settings for [!INCLUDE[d365fin](includes/d365fin_md.md)]. The changes that you make will only affect your workspace; not the workspaces of other users.  

## <a name="role-center"></a> Role Centre
The Role Centre represents the home page, a starting screen that is designed for the needs of a specific role in an organisation. Depending on your role, the Role Centre gives you an overview of the business, your department, or your personal tasks. It also helps you navigate to your daily tasks and find work that is assigned to you.

-   At the top, the navigation allows you to switch between customers, vendors, items, and other important lists of information. Similarly, actions allow you to initiate tasks, such as create a new sales invoice, directly from the Role Centre.

-   In the centre, you find **Activities**. Activities show current data and can be clicked or tapped to view more detailed information. Key Performance Indicators can be set up to display a selected chart for a visual representation of, for example, cash flow or income and expenses. You can also build up a list of favourite customers on the home page for accounts that you do business with often or need to pay special attention to.

### <a name="to-change-role-center"></a>To change Role Centre
The default Role Centre is **Business Manager**, but you can select another Role Centre that fits your needs better.
1. In the top right corner, choose the **Settings** icon ![Settings](media/ui-experience/settings_icon_small.png "Settings icon for role center"), and then choose **My Settings**.
2. On the **My Settings** page, in the **Role Centre** field, select the Role Centre that you want to set as the standard. For example, select **Accountant**.
3. Choose the **OK** button.

## <a name="company"></a>Company
A company functions as a container for data in [!INCLUDE[d365fin](includes/d365fin_md.md)]. There can be multiple companies in a database, but only one can be selected at a time.

The default company is called CRONUS and contains demonstration data only.

> [!TIP]  
>   If you want to display a different name for your company in the application (such as on the Role Centre), set the **Name** field on the **Company Information** page or the **Display Name** field on the **Companies** page.  

## <a name="work-date"></a>Work Date
The default work date is usually today's date. You may have to temporarily change the work date to be able to perform tasks, such as completing transactions for a date that is not the current date.

> [!TIP]  
>   Type **w** to quickly enter the work date in a date field. Write **t** to quickly enter the current date in the date field.

> [!IMPORTANT]  
>   After you change the work date, if you sign out or switch to another company, the work data reverts to the default work date. So the next time you sign in or switch back to the original company, you may have to set the work date again. 

### <a name="work-date-indication"></a>Work Date Indication
<!--
Whenever the work date is not set to the current day (today), there are two indicators on pages that you open for editing:

- A reminder appears at the top of the page that tells you what the work date is set to. The reminder provides a direct link to the work date setting on the **My Settings** page so you change the date if you want. From the reminder, you can also choose to dismiss the reminder for the rest of your session. Unless you change the work date to "today", the reminder will appear the next time you sign in. 

- If you dismiss the reminder, the work date will appear in the title of the page.  
-->
If the work date is not set to the current day (today), then on all pages where you can edit data, the current work date is shown in the upper-left corner of the page.
  
## <a name="region"></a> Region

The **Region** setting determines how dates, times, numbers, and currencies are shown or formatted.


## <a name="language"></a> Language
Changes the display language. This field appears only when there is more than one language to choose from. 

The initial language is either determined by the administrator or by your browser settings when you sign up for [!INCLUDE[d365fin](includes/d365fin_md.md)]. The language that you set will be used on all devices that you sign in from, such as a phone or tablet.

## <a name="changing-when-i-receive-notifications"></a>Changing When I Receive Notifications
Choose this link to view or change the notifications that you get about certain events or changes in status, such as when you are about to invoice a customer who has an overdue balance, or the available inventory is lower than the quantity you are about to sell. For more information, see [Smart Notifications](ui-smart-notifications.md).

## <a name="see-also"></a>See Also
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  
[Changing Which Features are Displayed](ui-experiences.md)  
