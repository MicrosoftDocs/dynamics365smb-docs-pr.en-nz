---
title: Connect Your Data with Flow| Microsoft Docs
description: You can make your Financials data available as a data source and specify an OData URL of your web services to build an automated workflow.
documentationcenter: 
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: workflow, Odata, Power App, SOAP
ms.date: 01/25/2018
ms.author: solsen
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 23e9ebbb75d23595d568d022526e551bf590a979
ms.contentlocale: en-nz
ms.lasthandoff: 03/22/2018

---
# <a name="using-included365finincludesd365finmdmd-in-an-automated-workflow"></a>Using [!INCLUDE[d365fin](includes/d365fin_md.md)] in an Automated Workflow
You can use your [!INCLUDE[d365fin](includes/d365fin_md.md)] data as part of a workflow in Microsoft Flow.  

> [!NOTE]  
>   You must have a valid account with [!INCLUDE[d365fin](includes/d365fin_md.md)] and with Flow.  

## <a name="to-add-included365finincludesd365finmdmd-as-a-data-source-in-flow"></a>To add [!INCLUDE[d365fin](includes/d365fin_md.md)] as a data source in Flow
1. In your browser, navigate to [flow.microsoft.com](https://flow.microsoft.com/en-us/), and then sign in.
2. Choose **My Flows** from the ribbon at the top of the page.
3. In the **My Flows** window, choose the **Create from blank** option.
4. From the list of available triggers, select one of the [!INCLUDE[d365fin](includes/d365fin_md.md)] triggers available:  
    *When a customer approval is requested*,  
    *When a general journal batch approval is requested*,  
    *When a general journal line approval is requested*,  
    *When an item approval is requested*,  
    *When a purchase document approval is requested*,  
    *When a sales document approval is requested*, or  
    *When a vendor aproval is requested*.
5. Flow will prompt you to select a company within your [!INCLUDE[d365fin](includes/d365fin_md.md)] tenant. Because each step in the Flow is independent of the next, you may be required to define the company multiple times when using a [!INCLUDE[d365fin](includes/d365fin_md.md)] template.

At this point, you have successfully connected to your Business Central data and are ready to begin building your flow. For more information, see the [Flow documentation](https://flow.microsoft.com/documentation/getting-started/).

For troubleshooting your Microsoft Flow, see [Troubleshooting Integration with Microsoft Flow](across-troubleshooting-how-use-financials-data-source-flow.md).

## <a name="see-also"></a>See Also
[Welcome to [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)  
[Importing Business Data from Other Finance Systems](upload-data.md)  
[Manage Users and Permissions](ui-how-users-permissions.md)    
[Setting Up [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)  
[Finance](finance.md)  

