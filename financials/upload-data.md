---
title: Import Your Legacy Business Data into Financials | Microsoft Docs
description: You can migrate data for customers, vendors, and inventory, for example, from Excel, QuickBooks, or Dynamics GP, into Financials.
author: edupont04
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: migrate, initialize, implement
ms.date: 07/05/2017
ms.author: edupont
ms.translationtype: Human Translation
ms.sourcegitcommit: 2a38dc36cb9ff609c5582acd489841b20013d4bc
ms.openlocfilehash: dd6eb5a6b19bf4c8fd92674a48e8cd29ce912eee
ms.contentlocale: en-nz
ms.lasthandoff: 07/07/2017


---
# <a name="importing-business-data-from-other-finance-systems"></a>Importing Business Data from Other Finance Systems
When you sign up for [!INCLUDE[d365fin](includes/d365fin_md.md)], you can choose to create an empty company so that you can upload your own data and to test your new [!INCLUDE[d365fin](includes/d365fin_md.md)] company. Depending on the finance solution that your business uses today, you can transfer information about customers, vendors, inventory, and bank accounts.  

From Home, you can start an assisted setup guide that helps you transfer the business data from an Excel file or from other formats. The type of files you can upload depends on the extensions that are available. For example, you can migrate data from QuickBooks because [!INCLUDE[d365fin](includes/d365fin_md.md)] includes an extension that handles the conversion from QuickBooks. If you want to migrate data from other finance solutions, you must either check if an extension is available for that solution or import from Excel.  

[!INCLUDE[d365fin](includes/d365fin_md.md)] includes templates for accounts, customers, vendors, and inventory items that you can choose to apply when you import your data.  

## <a name="importing-data-from-quickbooks-or-dynamics-gp"></a>Importing Data from QuickBooks or Dynamics GP
If your business uses QuickBooks or Dynamics GP today, you can export the relevant information to a file. You can then open the assisted setup guide to transfer the data.
For example, if your file includes customers and vendors, you can choose to transfer only the customer data. You can then transfer the rest of the information later.  

The assisted setup includes an option to change the default configuration of the transfer, but we recommend that you only enter this advanced setup if you are familiar with database tables. In the vast majority of businesses, the default mapping from QuickBooks or Dynamics GP to [!INCLUDE[d365fin](includes/d365fin_md.md)] will transfer the information that you want.  

For more information, see [QuickBooks Data Migration](ui-extensions-quickbooks-data-migration.md) or [Dynamics GP Data Migration](ui-extensions-dynamicsgp-data-migration.md).

## <a name="importing-data-from-configuration-packages"></a>Importing Data from Configuration Packages
[!INCLUDE[d365fin](includes/d365fin_md.md)] includes a configuration package that you can export to Excel and set up your data there. Then, you can import the data from Excel again. The package consists of 27 tables, including master data such as customers, vendors, items, and accounts, other basic setup tables such as shipping methods, and transactions tables such as sales header and lines.  

> [!NOTE]  
>   Working with configuration packages is advanced functionality, and we recommend that you contact your administrator. For more information, see [Importing Data from Legacy Accounting Software using a Configuration Package](across-import-data-configuration-packages.md).  

## <a name="see-also"></a>See Also
[Finance](finance.md)  
[Importing Data from Legacy Accounting Software using a Configuration Package](across-import-data-configuration-packages.md)  
[QuickBooks Data Migration](ui-extensions-quickbooks-data-migration.md)  
[Dynamics GP Data Migration](ui-extensions-dynamicsgp-data-migration.md)  
[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions](ui-extensions.md)   
[Setting Up [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)

## [!INCLUDE[d365fin](includes/free_trial_md.md)]

