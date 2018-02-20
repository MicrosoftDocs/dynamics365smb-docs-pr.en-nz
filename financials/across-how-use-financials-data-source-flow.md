---
title: Connect Your Data with Flow| Microsoft Docs
description: You can make your Financials data available as a data source and specify an OData URL of your web services to build an automated workflow.
documentationcenter: 
author: edupont04
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: workflow, Odata, Power App, SOAP
ms.date: 01/25/2018
ms.author: solsen
ms.translationtype: HT
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: ef4d841723b6bb0af37695a8c3ed1d805319be78
ms.contentlocale: en-nz
ms.lasthandoff: 01/30/2018

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
    *When a record is created*,  
    *When a record is deleted*,  
    *When a record is modified*,  
    *When a customer approval is requested*,  
    *When a general journal batch approval is requested*,  
    *When a general journal line approval is requested*,  
    *When an item approval is requested*,  
    *When a purchase document approval is requested*,  
    *When a sales document approval is requested*, or  
    *When a vendor aproval is requested*.
5. Flow will prompt you for the information that is required to connect to your [!INCLUDE[d365fin](includes/d365fin_md.md)] data. If you selected one of the following triggers: *When a record is created*, *When a record is modified*, or *When a record is deleted*, you must select a company name and table name. With any other trigger, only the company name is required to connect.

   Flow will show a list of companies and tables that are available from [!INCLUDE[d365fin](includes/d365fin_md.md)]. These tables, or end points, represent all the web services that you have published from [!INCLUDE[d365fin](includes/d365fin_md.md)].

   Alternatively, create a new web service URL in [!INCLUDE[d365fin](includes/d365fin_md.md)] by using the **Create Data Set** action in the **Web Services** page, using the **Set Up Reporting** Assisted Setup guide, or by choosing the **Edit in Excel** action in any lists.

At this point, you have successfully connected to your Finance and Operations, Business edition data and are ready to begin building your flow. For more information, see the [Flow documentation](https://flow.microsoft.com/documentation/getting-started/).

For troubleshooting your Microsoft Flow, see [Troubleshooting Integration with Microsoft Flow](across-troubleshooting-how-use-financials-data-source-flow.md).

## <a name="see-also"></a>See Also
[Welcome to [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)  
[Importing Business Data from Other Finance Systems](upload-data.md)  
[Manage Users and Permissions](ui-how-users-permissions.md)    
[Setting Up [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)  
[Finance](finance.md)  

