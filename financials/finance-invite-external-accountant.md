---
title: Add your external accountant to your Financials | Microsoft Docs
description: Learn how you can invite your external accountant to your Dynamics 365 for Financials.
author: edupont04
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: accountant, accounting
ms.date: 06/23/2017
ms.author: edupont
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: 1b9f88f02b198ae8da0f3359a3ce7799b9535739
ms.contentlocale: en-nz
ms.lasthandoff: 07/07/2017


---
# <a name="invite-your-external-accountant-to-your-included365finincludesd365finmdmd"></a>Invite Your External Accountant to Your [!INCLUDE[d365fin](includes/d365fin_md.md)]
If you use an external accountant to manage your books and financial reporting, you can invite them to your [!INCLUDE[d365fin](includes/d365fin_md.md)] so they can work with you on your fiscal data.

Once your accountant has gained access to your [!INCLUDE[d365fin](includes/d365fin_md.md)], they can use the **Accountant** Role Center that gives easy access to the most relevant windows for their work.  

> [!NOTE]  
>  This functionality requires that the experience is set to **Suite**. For more information, see [Customizing Your Financials Experience](ui-experiences.md).  

## <a name="invite-your-accountant-to-your-included365finincludesd365finmdmd"></a>Invite Your Accountant to Your [!INCLUDE[d365fin](includes/d365fin_md.md)]
In the current version of [!INCLUDE[d365fin](includes/d365fin_md.md)], inviting your external accountant requires an administrator to add them to your Active Directory tenant. The steps for doing this depends on the type of account that you used when you signed up for [!INCLUDE[d365fin](includes/d365fin_md.md)]. This topic is based on the use of an Office 365 account, which uses Microsoft Azure Active Directory.  

> [!TIP]  
>  We recommend that you contact your [!INCLUDE[d365fin](includes/d365fin_md.md)] partner for assistance.  

If you have activated your subscription of [!INCLUDE[d365fin](includes/d365fin_md.md)] and are no longer using the evaluation company, you have an Azure Active Directory tenant. Your administrator or [!INCLUDE[d365fin](includes/d365fin_md.md)] partner manages this tenant in the [Azure portal](https://portal.azure.com). This is where new users are added and licenses are applied and removed. For more information, see the [Microsoft Azure portal overview](https://docs.microsoft.com/en-us/azure/azure-portal-overview).  

### <a name="separate-license"></a>Separate Licence
One of the license types for [!INCLUDE[d365fin](includes/d365fin_md.md)] is the *External Accountant* license. This licence type is intended for use by users such as external accountants. This means that you do not have to buy an extra seat in your current Active Directory or use one of your existing [!INCLUDE[d365fin](includes/d365fin_md.md)] user accounts on your external accountant. For example, if your current Office 365 subscription includes 10 users for [!INCLUDE[d365fin](includes/d365fin_md.md)], and you are currently using 10 *Full User* licenses, your administrator can simply add your external accountant as a guest user in the Azure portal and assign this user the *External Accountant* license at no additional cost. However, you can only have one user with the *External Accountant* license. If you want to add more users, you must update your Office 365 subscription accordingly.  

## <a name="see-also"></a>See Also
[Finance](finance.md)  
[Accountant Experiences in Dynamics 365 for Financials](finance-accounting.md)  
[Financials for Accountants on Microsoft.com](https://www.microsoft.com/en-us/dynamics365/financial-insights-for-accountants)  

