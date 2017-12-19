---
title: Setting Up Workflows | Microsoft Docs
description: You can set up and use workflows that connect business-process tasks performed by different users. System tasks, such as automatic posting, can be included as steps in workflows, preceded or followed by user tasks. Requesting and granting approval to create new records are typical workflow steps.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 12/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: a49e50213f808fb72b43dfa22a34833b306ef12d
ms.openlocfilehash: 6beb70ad41fa32043e9b8afea67d390929533007
ms.contentlocale: en-nz
ms.lasthandoff: 12/14/2017

---
# <a name="setting-up-workflows"></a>Setting Up Workflows
You can set up and use workflows that connect business-process tasks performed by different users. System tasks, such as automatic posting, can be included as steps in workflows, preceded or followed by user tasks. Requesting and granting approval to create new records are typical workflow steps. For more information, see [Using Workflows](across-use-workflows.md).  

 Before you begin to use workflows, you must set up workflow users and approval users, specify how users receive notifications about workflow steps, and then create the workflows, potentially preceded by code customisation.  

 In the **Workflow** window, you create a workflow by listing the involved steps on the lines. Each step consists of a workflow event, moderated by event conditions, and a workflow response, moderated by response options. You define workflow steps by filling fields on workflow lines from fixed lists of event and response values representing scenarios that are supported by the application code.  

 If a business scenario requires a workflow event or response that is not supported, a Microsoft partner must implement them by customising the application code. For more information, see [Walkthrough: Implementing New Workflow Events and Responses](/dynamics_nav/Walkthrough--Implementing-New-Workflow-Events-and-Responses) in the developer and IT-pro help.

 The following table describes a sequence of tasks, with links to the topics that describe them.  

|**To**|**See**|  
|------------|-------------|  
|Set up workflow users and user groups.|[How to: Set Up Workflow Users](across-how-to-set-up-workflow-users.md)|  
|Set up workflow users who take part in approval workflows.|[How to: Set Up Approval Users](across-how-to-set-up-approval-users.md)|  
|Specify how workflow users are notified of workflow steps, including approval requests.|[Setting Up Workflow Notifications](across-setting-up-workflow-notifications.md)|  
|Specify when users receive notifications and whether to aggregate notifications in a period to minimise the number of notifications.|[How to: Specify When and How to Receive Notifications](across-how-to-specify-when-and-how-to-receive-notifications.md)|  
|Set up the layout and general content of new workflow notifications emails, or export, modify, and reimport existing templates.|[How to: Manage Notification Templates](across-how-to-manage-notification-templates.md)|  
|Set up an SMTP server to enable email communication in and out of [!INCLUDE[d365fin](includes/d365fin_md.md)]|[How to: Set up Email](madeira-how-setup-email.md)|
|Specify the different steps of a workflow by connection workflow events with workflow responses.|[How to: Create Workflows](across-how-to-create-workflows.md)|  
|Use workflow templates to create new workflows.|[How to: Create Workflows from Workflow Templates](across-how-to-create-workflows-from-workflow-templates.md)|  
|Share workflows with other [!INCLUDE[d365fin](includes/d365fin_md.md)] databases.|[How to: Export and Import Workflows](across-how-to-export-and-import-workflows.md)|  
|Learn how to set up a workflow for approving sales documents by following an end-to-end procedure.|[Walkthrough: Setting Up and Using a Purchase Approval Workflow](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md)|  
|Add support for a business scenario that requires new workflow events or responses by customising the application code.|[Walkthrough: Implementing New Workflow Events and Responses](/dynamics_nav/Walkthrough--Implementing-New-Workflow-Events-and-Responses)|  

## <a name="see-also"></a>See Also  
 [Using Workflows](across-use-workflows.md)   
 [Workflow](across-workflow.md)   
 [Walkthrough: Setting Up and Using a Purchase Approval Workflow](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md)  
 [Working with Financials](ui-work-product.md)

