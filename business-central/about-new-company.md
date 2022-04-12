---
title: Create new companies using an assisted setup guide
description: It's easy to create a new, blank company in Business Central. An assisted setup guide helps you through the steps, and you can import your existing business data.
author: edupont04
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: company, setup wizard
ms.search.form: 1803, 9020, 9022, 9026, 9027, 9030, 9000, 9004, 9005, 9018, 9006, 9007, 9010, 9016, 9017
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: bef90a9dab30391f310458cb0dde58cc4fac5268
ms.sourcegitcommit: 8a12074b170a14d98ab7ffdad77d66aed64e5783
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 03/31/2022
ms.locfileid: "8519371"
---
# <a name="create-new-companies-in-prod_short"></a>Create New Companies in [!INCLUDE[prod_short](includes/prod_short.md)]

In [!INCLUDE[prod_short](includes/prod_short.md)], the container for business data that belongs to a business unit or legal entity is referred to as a *company*. When you sign up for [!INCLUDE[prod_short](includes/prod_short.md)], you are given a demonstration company and an empty company, *My Company*. Switching between the companies is easy: just go to **My Settings** and move to the other company. But you can also create new companies in [!INCLUDE[prod_short](includes/prod_short.md)] depending on your business needs.  

When you create a new company, an assisted setup guide helps you get the basics in place. Then, you can import relevant data from your legacy system or another company in [!INCLUDE[prod_short](includes/prod_short.md)].  

## <a name="choose-the-right-template"></a>Choose the right template

If you decide to add a company to your [!INCLUDE[prod_short](includes/prod_short.md)], you can use the **Create New Company** assisted setup guide to get you started. The setup wizard is available from the **Companies** page and from the lookup in the **Company** field on the **My Settings** page.  

The setup wizard offers two templates and a blank option:

- **Evaluation - Sample Data**  
    This creates a company that is similar to the demonstration company with sample data and setup data. This type of company is available to you without switching to [a 30-day trial period](across-preview.md#add-your-own-data-to-an-empty-trial-company), which the other types do.  
- **Production - Setup Data Only**  
    This creates a company that is similar to **My Company** with setup data but without sample data. You will be able to use this company for [a 30-day trial period](across-preview.md#add-your-own-data-to-an-empty-trial-company).  
- **Create New - No Data**  
    This creates a blank company without setup data. You will be able to use this company for [a 30-day trial period](across-preview.md#add-your-own-data-to-an-empty-trial-company).  

If you want to get started easily with a new company, choose **Production - Setup Data Only** and then import your own business data, such as customers, items, and vendors. Choose the **New** template if you want to set everything up from scratch. In that case, you can use the **Company Setup** assisted setup guide to help you get started with essential setup data.  

> [!NOTE]  
> When you create a new company, it takes a few minutes before you can access it in [!INCLUDE[prod_short](includes/prod_short.md)]. The setup status on the **Companies** page shows when the new company is ready for you. Then, you can switch to the new company by using **My Settings**.  

During your 30 day trial, you can create any number of new companies, but they will only be available during your trial. For more information, contact your [!INCLUDE[prod_short](includes/prod_short.md)] partner. See also the [Dynamics 365 Business Central trial FAQ](trial-faq.md) article.  

## <a name="copy-a-company"></a>Copy a company

On the **Companies** page, you can use the **Copy** action to create a second company based on the contents of an existing company. This is useful, for example, when you want to test a company without disrupting production data.

> [!Important]
> This function cannot be used to take a backup of a company. Taking a company backup begins by exporting the database as a .bacpac file. For more information, see [Exporting Databases](/dynamics365/business-central/dev-itpro/administration/tenant-admin-center-database-export) in the development and administration help.

## <a name="set-up-the-company"></a>Set up the company

When you sign in to a new company, the **Company Setup** wizard runs automatically and helps you get started. You will be asked for information about your business, such as the address, bank details, and inventory costing method. We ask for this information because it is used as a basis for many areas in [!INCLUDE[prod_short](includes/prod_short.md)] that you will then not have to set up manually later.  

For example, your company address is included in invoices and other documents, your bank information is used in payments, and the costing method is used to calculate prices as well as inventory valuation.  

Once you have the basics in place, you can set up remaining core areas. Then, you are ready to add business data, such as customers and vendors. For more information, see [Setting Up [!INCLUDE[prod_short](includes/prod_short.md)]](setup.md).  

## <a name="companies-and-environments"></a>Companies and environments

[!INCLUDE [company_environment](includes/company_environment.md)]

For more information, see [Switching to Another Company or Environment](ui-organization-switch.md). For more information about environments, see [Understanding the Infrastructure of Business Central Online](/dynamics365/business-central/dev-itpro/administration/tenant-environment-topology) (in English only).  

## <a name="changing-a-companys-name"></a>Changing a company's name

Once a company has been created, you can't change it's name. But you can change its **Display Name**, which is text that will be shown for the company throughout the application.  

> [!TIP]
> You can rename a company if you're using [!INCLUDE[prod_short](includes/prod_short.md)] on-premises.

## <a name="add-contoso-coffee"></a>Add Contoso Coffee

The Contoso Coffee app provides demonstration data that can help you explore the advanced capabilities of [!INCLUDE [prod_short](includes/prod_short.md)]. Find the app in AppSource, and install it in an empty company, for example a company in a sandbox environment. For more information, see [Introduction to Contoso Coffee Demo Data](contoso-coffee/contoso-coffee-intro.md).  

## <a name="see-also"></a>See Also

[Customising Business Central](ui-customizing-overview.md)  
[Setting Up [!INCLUDE[prod_short](includes/prod_short.md)]](setup.md)  
[Importing Business Data from Other Finance Systems](across-import-data-configuration-packages.md)  
[Change Basic Settings](ui-change-basic-settings.md)  
[Getting Ready for Doing Business](ui-get-ready-business.md)  
[Trials and Subscriptions](across-preview.md)  
[Understanding the Infrastructure of Business Central Online (English only)](/dynamics365/business-central/dev-itpro/administration/tenant-environment-topology)  

[!INCLUDE[footer-include](includes/footer-banner.md)]