---
title: Import Your Legacy Business Data into Business Central | Microsoft Docs
description: You can migrate data for customers, vendors, and inventory, for example, from Excel, QuickBooks, or Dynamics GP, into Business Central.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: QuickBooks, transfer, import, migrate, initialize, implement
ms.date: 03/07/2018
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 25005f972cf541f12419ad34c76d1997c070a6d8
ms.contentlocale: en-nz
ms.lasthandoff: 03/22/2018

---
# <a name="importing-business-data-from-other-finance-systems"></a>Importing Business Data from Other Finance Systems
When you sign up for [!INCLUDE[d365fin](includes/d365fin_md.md)], you can choose to create an empty company so that you can upload your own data and to test your new [!INCLUDE[d365fin](includes/d365fin_md.md)] company. Depending on the finance solution that your business uses today, you can transfer information about customers, vendors, inventory, and bank accounts.  

From the Role Centre, you can start an assisted setup guide that helps you transfer the business data from an Excel file or from other formats. The type of files you can upload depends on the extensions that are available. For example, you can migrate data from QuickBooks because [!INCLUDE[d365fin](includes/d365fin_md.md)] includes an extension that handles the conversion from QuickBooks. If you want to migrate data from other finance solutions, you must either check if an extension is available for that solution or import from Excel.  

[!INCLUDE[d365fin](includes/d365fin_md.md)] includes templates for accounts, customers, vendors, and inventory items that you can choose to apply when you import your data.

> [!NOTE]  
> For larger implementation work, you can use RapidStart Services for [!INCLUDE[d365fin](includes/d365fin_md.md)], which is an extensive toolkit for setting up new solutions based on customers' business requirements and setup data. RapidStart Services also offers functionality for import of business data. For more information, see [Setting Up a Company With RapidStart Services](admin-set-up-a-company-with-rapidstart.md).  

## <a name="importing-data-from-quickbooks-desktop-quickbooks-online-or-dynamics-gp"></a>Importing Data from QuickBooks Desktop, QuickBooks Online, or Dynamics GP
If your business uses QuickBooks or Dynamics GP today, you can export the relevant information to a file. You can then open the assisted setup guide to transfer the data.
For example, if your file includes customers and vendors, you can choose to transfer only the customer data. You can then transfer the rest of the information later.  

The assisted setup includes an option to change the default configuration of the transfer, but we recommend that you only enter this advanced setup if you are familiar with database tables. In the vast majority of businesses, the default mapping from QuickBooks or Dynamics GP to [!INCLUDE[d365fin](includes/d365fin_md.md)] will transfer the information that you want.  

For more information, see [QuickBooks Desktop Data Migration](ui-extensions-quickbooks-data-migration.md), [QuickBooks Online Data Migration](ui-extensions-quickbooks-online-data-migration.md), or [Dynamics GP Data Migration](ui-extensions-dynamicsgp-data-migration.md).  

## <a name="importing-data-from-configuration-packages"></a>Importing Data from Configuration Packages
[!INCLUDE[d365fin](includes/d365fin_md.md)] includes a configuration package that you can export to Excel and set up your data there. Then, you can import the data from Excel again. The package consists of 27 tables, including master data such as customers, vendors, items, and accounts, other basic setup tables such as shipping methods, and transactions tables such as sales header and lines.  

> [!NOTE]  
>   Working with configuration packages is advanced functionality, and we recommend that you contact your administrator. For more information, see [Importing Data from Legacy Accounting Software using a Configuration Package](across-import-data-configuration-packages.md).  

## <a name="see-also"></a>See Also
[Finance](finance.md)  
[Importing Data from Legacy Accounting Software using a Configuration Package](across-import-data-configuration-packages.md)  
[Setting Up a Company With RapidStart Services](admin-set-up-a-company-with-rapidstart.md)  
[QuickBooks Desktop Data Migration](ui-extensions-quickbooks-data-migration.md)  
[QuickBooks Online Data Migration](ui-extensions-quickbooks-online-data-migration.md)  
[Dynamics GP Data Migration](ui-extensions-dynamicsgp-data-migration.md)  
[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions](ui-extensions.md)   
[Setting Up [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)

## [!INCLUDE[d365fin](includes/free_trial_md.md)]  
## [!INCLUDE[d365fin](includes/training_link_md.md)]

