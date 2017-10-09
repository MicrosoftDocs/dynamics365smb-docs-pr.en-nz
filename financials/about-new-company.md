---
title: Create new companies using an assisted setup guide | Microsoft Docs
description: It's easy to create a new, blank company in Dynamics 365 for Financials. An assisted setup guide helps you through the steps, and you can import your existing business data.
author: edupont04
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: company, setup wizard
ms.date: 07/14/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: eea34afbee429d14ab150894729cb4ea3843bb2b
ms.openlocfilehash: 3ff3c7af87033595d64e583b62b0e0242b22d2f1
ms.contentlocale: en-nz
ms.lasthandoff: 09/22/2017

---
# <a name="creating-new-companies-in-included365finlongincludesd365finlongmdmd"></a>Creating New Companies in [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]
In [!INCLUDE[d365fin](includes/d365fin_md.md)], the containers for business data that belongs to a business unit or legal entity is referred to as a *company*. When you sign up for [!INCLUDE[d365fin](includes/d365fin_md.md)], you are given a demonstration company and an empty company, *My Company*. Switching between the companies is easy - just got to **My Settings** and move to the other company. But you can also create new companies in [!INCLUDE[d365fin](includes/d365fin_md.md)], depending on your business needs. When you create a new company, an assisted setup guide helps you get the basics in place. Then, you can import relevant data from your legacy system or another company in [!INCLUDE[d365fin](includes/d365fin_md.md)].  

## <a name="create-new-company"></a>Create New Company
If you decide to add a company to your [!INCLUDE[d365fin](includes/d365fin_md.md)], you can use the **Create New Company** assisted setup wizard to get you started. The setup wizard is available from the **Companies** window and from the lookup in the **Company** field in **My Settings**.  

The setup wizard offers three templates:

-   **Suite Evaluation**  
    This creates a company that is similar to the demonstration company with sample data and setup data.  
-   **Suite Production**  
    This creates a company that is similar to **My Company** with setup data but without sample data.  
-   **New**  
    This creates a blank company without setup data.  

If you want to get started easily with a new company, choose **Suite Production** and then import your own business data, such as customers, items, and vendors. Choose the **New** template if you want to set everything up from scratch. In that case, you can use the **Company Setup** assisted setup wizard to help you get started with essential setup data.  

> [!NOTE]  
>   When you create a new company, it takes a few minutes before you can access it in [!INCLUDE[d365fin](includes/d365fin_md.md)]. The setup status in the **Companies** window shows when the new company is ready for you. Then, you can switch to the new company by using **My Settings**.  

During your 30 day trial, you can create any number of new companies, but they will only be available during your trial. For more information, contact your [!INCLUDE[d365fin](includes/d365fin_md.md)] partner.  

## <a name="company-setup"></a>Company Setup
When you sign in to a new company, the **Company Setup** wizard runs automatically and helps you get started. You will be asked for information about your business, such as the address, bank details, and inventory costing method. We ask for this information because it is used as a basis for many areas in [!INCLUDE[d365fin](includes/d365fin_md.md)] that you will then not have to set up manually later.  

For example, your company address is included in invoices and other documents, your bank information is used in payments, and the costing method is used to calculate prices as well as inventory valuation.  

Once you have the basics in place, you can set up remaining core areas. Then, you are ready to add business data, such as customers and vendors. For more information, see [Setting Up Dynamics 365 for Financials](setup.md).  

## <a name="see-also"></a>See Also
[Setting Up Dynamics 365 for Financials](setup.md)  
[Importing Business Data from Other Finance Systems](upload-data.md)  
[Changing Basic Settings](ui-change-basic-settings.md)  
[Welcome to [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)  

