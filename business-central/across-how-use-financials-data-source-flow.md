---
title: Connect Your Data with Flow| Microsoft Docs
description: You can make your Business Central data available as a data source and specify an OData URL of your web services to build an automated workflow.
documentationcenter: ''
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: workflow, Odata, Power App, SOAP
ms.date: 04/01/2019
ms.author: solsen
ms.openlocfilehash: 1652c4bc22425bd6df4ac303a96a2ab1b28bfaf9
ms.sourcegitcommit: bd78a5d990c9e83174da1409076c22df8b35eafd
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 03/31/2019
ms.locfileid: "936475"
---
# <a name="using-included365finincludesd365finmdmd-in-an-automated-workflow"></a>Using [!INCLUDE[d365fin](includes/d365fin_md.md)] in an Automated Workflow
You can use your [!INCLUDE[d365fin](includes/d365fin_md.md)] data as part of a workflow in Microsoft Flow.

> [!NOTE]
> In addition to Microsoft Flow, you can use the Workflow functionality within [!INCLUDE[d365fin](includes/d365fin_md.md)]. Note that although they are two separate workflow systems, any Flow template that you create with Microsoft Flow is added to the list of workflow templates within [!INCLUDE[d365fin](includes/d365fin_md.md)]. For more information, see [Workflow](across-workflow.md).  

> [!NOTE]  
>   You must have a valid account with [!INCLUDE[d365fin](includes/d365fin_md.md)] and with Flow.  

## <a name="to-add-included365finincludesd365finmdmd-as-a-data-source-in-flow"></a>To add [!INCLUDE[d365fin](includes/d365fin_md.md)] as a data source in Flow
1. In your browser, navigate to [flow.microsoft.com](https://flow.microsoft.com/en-us/), and then sign in.
2. Choose **My Flows** from the ribbon at the top of the page.
3. There are 2 ways to create a Flow; **Create from template** and **Create from blank**. A template is a predefined Flow that has been created for you.  To use a template, simply select it and create a connection for each service the template uses. A blank template enables you to create a new Flow completely from scratch.
4. To Create from blank, on the **My Flows** page, choose the **Create from blank** option.
5. Search for **Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)]** connector.
6. From the list of available triggers, select one of the [!INCLUDE[d365fin](includes/d365fin_md.md)] triggers available:  
    *When a customer approval is requested*,  
    *When a general journal batch approval is requested*,  
    *When a general journal line approval is requested*,  
    *When an item approval is requested*,  
    *When a purchase document approval is requested*,  
    *When a sales document approval is requested*, or  
    *When a vendor approval is requested*.
7. Flow will prompt you to select a company within your [!INCLUDE[d365fin](includes/d365fin_md.md)] tenant, as well as any conditions in your data that you want to listen for.

At this point, you have successfully connected to your Business Central data and are ready to begin building your flow.

8. To Create from a template, choose the **Create from template** option.
9. Search for **Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)]** templates.
10. From the list of available templates, select one of the templates.  
    *Request Approval for Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] sales order*,  
    *Request Approval for Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] sales quote*,  
    *Request Approval for Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] sales invoice*,  
    *Request Approval for Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] sales credit memo*,  
    *Request Approval for Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] customer*,  
    *Request Approval for Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] purchase order*,  
    *Request Approval for Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] purchase invoice*,  
    *Request Approval for Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] purchase credit memo*,  
    *Request Approval for Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] item*,  
    *Request Approval for Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] vendor*,  
    *Request Approval for Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] general journal batch*,  
    *Request Approval for Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] general journal lines*.  
11. Flow will prompt you to select a company within your [!INCLUDE[d365fin_md](includes/d365fin_md.md)] tenant. Because each step in the flow is independent of the next, you may be required to define the company multiple times when using a [!INCLUDE[d365fin_md](includes/d365fin_md.md)] Flow template.

For more information, see the [Flow Documentation](https://docs.microsoft.com/en-us/flow/getting-started).

For troubleshooting your Microsoft Flow, see [Troubleshooting Integration with Microsoft Flow](across-troubleshooting-how-use-financials-data-source-flow.md).

## <a name="see-also"></a>See Also
[Getting Started](product-get-started.md)  
[Workflow](across-workflow.md)  
[Importing Business Data from Other Finance Systems](across-import-data-configuration-packages.md)  
[Managing Users and Permissions](ui-how-users-permissions.md)   
[Manage [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)] Workflows](across-use-workflows.md)  
[Approval User Setup](across-how-to-set-up-approval-users.md)  
[Setting Up [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)  
[Finance](finance.md)  
