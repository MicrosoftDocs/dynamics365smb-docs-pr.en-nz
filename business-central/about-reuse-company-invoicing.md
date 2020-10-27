---
title: Use Invoicing and Business Central | Microsoft Docs
description: Workaround for accessing Microsoft Invoicing when you have signed up for Dynamics 365 Business Central.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: Invoicing, Microsoft 365
ms.date: 10/01/2020
ms.author: bholtorf
ms.openlocfilehash: 90f5f913fdaa96b2d4c4a057cc675e3a9edcc95c
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 10/01/2020
ms.locfileid: "3914455"
---
# <a name="using-the-same-microsoft-365-account-in-d365fin-and-microsoft-invoicing"></a>Using the same Microsoft 365 Account in [!INCLUDE[d365fin](includes/d365fin_long_md.md)] and Microsoft Invoicing
When you sign up for a trial with [!INCLUDE[d365fin](includes/d365fin_md.md)], you can move to a 30-day evaluation phase, you can start a subscription, or you can stop using [!INCLUDE[d365fin](includes/d365fin_md.md)]. In all cases, you may at some point have seen something called **Microsoft Invoicing** and clicked it. This was an app that was part of what is now Microsoft 365 Business Standard and was formerly known as Microsoft 365 Business Premium subscription, so not everyone will have seen that tile in their Microsoft 365 experience.  

Microsoft Invoicing is no longer available, but if you need to sign into Invoicing to retrieve your data, you might see a message that you cannot access Microsoft Invoicing because your account is used in [!INCLUDE[d365fin](includes/d365fin_md.md)].  

You see a similar message if you install the mobile app for Invoicing.  

## <a name="workaround"></a>Workaround
Invoicing and [!INCLUDE[d365fin](includes/d365fin_md.md)] have a shared platform. That means that you are recognised as an existing user of [!INCLUDE[d365fin](includes/d365fin_md.md)] when you click Invoicing in the Microsoft 365 admin centre. The reason is that Invoicing cannot use the same company as [!INCLUDE[d365fin](includes/d365fin_md.md)].  

So you will have to sign in to [!INCLUDE[d365fin](includes/d365fin_md.md)] and rename your existing company, and then create a new company that you can then use in Invoicing. No data is moved or overwritten during this workaround.

### <a name="to-rename-your-company"></a>To rename your company
1. Sign in to [!INCLUDE[d365fin](includes/d365fin_md.md)].
2. In the top right corner, choose the **Settings** icon ![Settings](media/ui-experience/settings_icon_small.png "Settings icon for role centre"), and then choose **My Settings** .
3. In the **Company** field, choose a different company.
4. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Companies** , and then choose the related link.  
5. On the **Companies** page, choose **Edit List** .  
6. Change the name of the *My Company* entry to something else.  

    Wait a number of minutes. We’ll be making a number of changes in the underlying database, and that takes a while.
7.  When the system is ready again, choose the **Create New Company** button.  
8.  In the dialogue that appears, specify the name as *My Company* , and choose the **Production – Setup Data Only** option.  

This again takes a number of minutes. When the process completes, you will be able to access Invoicing as part of your Microsoft 365 Business Standard experience. but only to export data since the Invoicing app is deprecated.  

### <a name="what-about-my-data"></a>What about my data?
When you rename the original My Company, the database tables that store your existing [!INCLUDE[d365fin](includes/d365fin_md.md)] data are renamed, but the data itself is not touched.  

If you use both Invoicing and [!INCLUDE[d365fin](includes/d365fin_md.md)], the data is stored in two different containers (the two companies). Nothing is shared, so you'll have to manage customers and items in both companies.  

## <a name="see-also"></a>See Also
[Frequently Asked Questions](across-faq.md)  
[Administration](admin-setup-and-administration.md)  
