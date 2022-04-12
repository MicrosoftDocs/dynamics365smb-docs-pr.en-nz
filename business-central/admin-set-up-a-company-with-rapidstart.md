---
title: Set Up a Company With RapidStart Services
description: You can set up a new company in Business Central with RapidStart services to enhance productivity by automating and simplifying recurring tasks.
author: SorenGP
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.search.form: 8610, 8614, 8615, 8620, 8632
ms.date: 03/28/2022
ms.author: edupont
ms.openlocfilehash: b2d3378e9c06221bc91977883a53bba8514c6afc
ms.sourcegitcommit: 8a12074b170a14d98ab7ffdad77d66aed64e5783
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 03/31/2022
ms.locfileid: "8518327"
---
# <a name="set-up-a-company-with-rapidstart-services"></a>Set Up a Company with RapidStart Services

You can set up a new company in [!INCLUDE[prod_short](includes/prod_short.md)] with RapidStart Services, which is a tool designed to shorten deployment times, improve quality of implementation, introduce a repeatable approach to implementations, and enhance productivity by automating and simplifying recurring tasks.  

Use these capabilities to scale your business as a reseller. Most of the relevant pages apply to both [!INCLUDE [prod_short](includes/prod_short.md)] online and on-premises. However, some processes rely on access to files on disk and are too complex to use for [!INCLUDE [prod_short](includes/prod_short.md)] online. For [!INCLUDE [prod_short](includes/prod_short.md)] on-premises, you probably want to use Windows PowerShell to help you deploy. For more information, see [Administration of Business Central On-Premises](/dynamics365/business-central/dev-itpro/administration/administration) and [Administration of Business Central Online](/dynamics365/business-central/dev-itpro/administration/tenant-administration), respectively.  

RapidStart Services helps you gain an overview of the setup process of your new company by providing a worksheet in which you can set up the tables often involved in the configuration process of new companies. As you do this, you can create a questionnaire to guide your customers through the collection of setup information. Your customers have the option of using the questionnaire to set up application areas, or they can open the setup page directly and do the setup there. Most importantly, RapidStart Services helps you, as a customer, prepare the company with default setup data that you can fine-tune and customise. Lastly, when you use RapidStart Services, you can configure and migrate existing customer data, such as a list of customers or items, into the new company.

You can use the following components to speed up your company setup:  

- Configuration wizard  
- Configuration worksheet  
- Configuration packages  
- Configuration templates  
- Configuration questionnaire  

> [!Note]  
> There are areas of [!INCLUDE[prod_short](includes/prod_short.md)] that you must set up manually. These include adding users, setting up accounting periods, and setting up dimensions for business intelligence. For more information, see [Setting Up [!INCLUDE[prod_short](includes/prod_short.md)]](setup.md).

 The following table describes a sequence of tasks with links to topics that describe them.

|**To**|**See**|  
|------------|-------------|  
|Create a new company and import basic setup data and templates.|[Set Up Company Configuration](admin-set-up-company-configuration.md)|  
|Deploy the configured package to your customer for implementation.|[Apply Configurations to New Companies](admin-apply-configuration-to-new-companies.md)|
|Define and validate your customer's setup values for all core areas, such as company information, general ledger, inventory, sales, or manufacturing.|[Gather Customer Setup Values](admin-gather-customer-setup-values.md)|  
|Configure core master data records using templates to prepare to migrate existing customer data.|[Prepare to Migrate Customer Data](admin-use-templates-to-prepare-customer-data-for-migration.md)|  
|Define tables and fields, validate existing customer data, and migrate data into the [!INCLUDE[prod_short](includes/prod_short.md)] database.|[Migrate Customer Data](admin-migrate-customer-data.md)|
|Prepare to reuse company configurations in other companies (in the developer and administration content).|[Create Custom Company Configuration Packages](/dynamics365/business-central/dev-itpro/administration/set-up-standard-company-configuration-packages)|
|Find solutions to known issues in the RapidStart Services toolkit.|[Tips and Tricks: RapidStart Services](admin-tips-and-tricks-rapidstart-services.md)|  

## <a name="see-also"></a>See Also

[Administration](admin-setup-and-administration.md)  
[Setting Up [!INCLUDE[prod_short](includes/prod_short.md)]](setup.md)  
[Set Up Complex Application Areas Using Best Practices](set-up-complex-application-areas-using-best-practices.md)   


[!INCLUDE[footer-include](includes/footer-banner.md)]