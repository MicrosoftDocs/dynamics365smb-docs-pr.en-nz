---
title: Workflow | Microsoft Docs
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
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: f65c0e577e839928809f7afda3dbdb4c9b7702c8
ms.contentlocale: en-nz
ms.lasthandoff: 09/22/2017

---
# <a name="workflow"></a>Workflow
You can set up and use workflows that connect business-process tasks performed by different users. System tasks, such as automatic posting, can be included as steps in workflows, preceded or followed by user tasks. Requesting and granting approval to create new records are typical workflow steps.  

 In the **Workflow** window, you create a workflow by listing the involved steps on the lines. Each step consists of a workflow event, moderated by event conditions, and a workflow response, moderated by response options. You define workflow steps by filling fields on workflow lines from fixed lists of event and response values representing scenarios that are supported by the application code.  

 The generic version of [!INCLUDE[d365fin](includes/d365fin_md.md)] includes a number of preconfigured workflows represented by workflow templates that you can copy to create workflows. The code for workflow templates that are added by Microsoft are prefixed with “MS-“. For more information, see the list of workflow templates in the Workflow Templates window.  

 If a business scenario requires a workflow event or response that is not supported, a Microsoft partner must implement them by customising the application code. For more information, see [Walkthrough: Implementing New Workflow Events and Responses](https://msdn.microsoft.com/en-us/library/mt574349.aspx) on MSDN.  

 The following table describes a sequence of tasks, with links to the topics that describe them.  

|**To**|**See**|  
|------------|-------------|  
|Set up workflow users, specify how users get notified, and create new workflows. For new workflows for unsupported scenarios, implement the required workflow elements by customising the application code.|[Setting Up Workflows](across-set-up-workflows.md)|  
|Enable workflows, act on workflow notifications, including request approvals and approve requests to perform a workflow step. Archive and delete workflows.|[Using Workflows](across-use-workflows.md)|  

## <a name="see-also"></a>See Also  
[Sales](sales-manage-sales.md)  
[Purchasing](purchasing-manage-purchasing.md)  
[Managing Projects](projects-manage-projects.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

