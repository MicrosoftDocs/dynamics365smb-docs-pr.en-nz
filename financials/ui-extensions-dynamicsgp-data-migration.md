---
title: Microsoft Dynamics GP Data Migration | Microsoft Docs
description: Provides information about the Dynamics GP Data Migration extension
documentationcenter: 
author: edupont04
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: app, add-in, manifest, customize, import, implement
ms.date: 03/29/2017
ms.author: edupont
ms.translationtype: Human Translation
ms.sourcegitcommit: a31be0f9d07e2abb591e26f6bae34c6f6e4dcda6
ms.openlocfilehash: a94afbd0ee689f6bd9157d0b441959f252230f08
ms.contentlocale: en-nz
ms.lasthandoff: 05/04/2017


---
# <a name="the-dynamics-gp-data-migration-extension-for-dynamics-365-for-financials"></a>The Dynamics GP Data Migration Extension for Dynamics 365 for Financials
This extension makes it easy to migrate customers, vendors, inventory items, and accounts from Dynamics GP to [!INCLUDE[d365fin](includes/d365fin_md.md)]. If your business uses Dynamics GP today, you can export the relevant master records and then open an assisted setup guide to add the data to [!INCLUDE[d365fin](includes/d365fin_md.md)]. For more information, see [Migrate Business Data from Other Finance Systems](upload-data.md).

## <a name="exporting-data-from-dynamics-gp"></a>Exporting Data from Dynamics GP
You must have exported some or all of your existing customers, vendors, inventory items, and accounts to a file, using the Dynamics GP functionality for data export. For the purposes of [!INCLUDE[d365fin](includes/d365fin_md.md)], you can export the following types of data:

* Account  
* Customer  
* Item  
* Vendor  

The Dynamics GP Data Migration extension automatically maps the exported data so that your data is quickly available to you in your new [!INCLUDE[d365fin](includes/d365fin_md.md)] company. During the process, supporting setup information is created, such as posting groups. Inventory items will be brought into the system with FIFO as the cost valuation method. Accounts will be set up as the main account segment from Dynamics GP with dimensions, because [!INCLUDE[d365fin](includes/d365fin_long_md.md)] does not have account segments.

## <a name="see-also"></a>See Also
[Importing Business Data from Other Finance Systems](upload-data.md)  
[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions ](ui-extensions.md)  

