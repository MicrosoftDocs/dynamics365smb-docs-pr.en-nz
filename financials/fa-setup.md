---
title: Set Up Fixed Assets| Microsoft Docs
description: Learn about the sequence of tasks you must do to set up fixed assets, such as machinery or buildings.
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: machinery, buildings
ms.date: 08/15/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 9dea8be0f5b0200f97082dc25dbaa2483ad6c735
ms.contentlocale: en-nz
ms.lasthandoff: 09/22/2017

---
# <a name="setting-up-fixed-assets"></a>Setting Up Fixed Assets
Before you can work with Fixed Assets, you need to define a few things:  

* How you insure, maintain, and depreciate fixed assets.  
* How you record costs and other values in the general ledger.  

The table below has links to more information. After you set those things up, you can start various activities. For more information, see [Fixed Assets](fa-manage.md).  

> [!NOTE]  
>   You can record fixed asset transactions in the **Fixed Asset G/L Journal** or **Fixed Asset Journal** windows, depending on whether the transactions are for financial reporting or for internal management. Help for Fixed Assets only describes how to use the **Fixed Asset G/L Journal** window.  

When you enable a fixed asset activity in the **G/L Integration** section in the **Depreciation Book Card** window, the **Fixed Asset G/L Journal** window is used to post transactions for the activity.

> [!NOTE]  
>  This functionality requires that the experience is set to **Suite**. For more information, see [Customizing Your Financials Experience](ui-experiences.md).  

The following table describes a sequence of tasks, with links to the topics that describe them.  

| To | See |
| --- | --- |
| Set up default G/L accounts, allocation keys, journal templates and batches for fixed asset posting, and set up fixed asset classes and subclasses, such as Tangible and Intangible. |[How to: Set Up General Fixed Assets Information](fa-how-setup-general.md) |
| Create depreciation books, define various depreciation methods, integrate with the general ledger, and enable duplication of entries in several depreciation books. |[How to: Set Up Fixed Asset Depreciation](fa-how-setup-depreciation.md) |
| Enable insurance of fixed assets, set up general insurance information, an insurance card per policy, and prepare journals to post insurance costs. |[How to: Set Up Fixed Asset Insurance](fa-how-setup-insurance.md) |
| Enable maintenance of fixed assets, set up general maintenance information, set up maintenance posting accounts, and define types of maintenance work. |[How to: Set Up Fixed Asset Maintenance](fa-how-setup-maintenance.md) |
| Learn about different fixed asset depreciation methods. |[Depreciation Methods](fa-depreciation-methods.md) |

## <a name="see-also"></a>See Also
[Fixed Assets](fa-manage.md)  
[Finance](finance.md)  
[Welcome to [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

