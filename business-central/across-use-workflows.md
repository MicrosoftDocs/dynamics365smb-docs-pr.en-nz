---
title: Using Workflows
description: You can set up and use workflows that connect business-process tasks performed by different users. Learn about the different steps you must take to start using workflows.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: fc2917a304a5a43228f9156dffd0a9a8011f9047
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "5378914"
---
# <a name="using-workflows"></a>Using Workflows
You can set up and use workflows that connect business-process tasks performed by different users. System tasks, such as automatic posting, can be included as steps in workflows, preceded or followed by user tasks. Requesting and granting approval to create new records are typical workflow steps.  

 Before you can begin to use workflows, you must set up workflow users, create the workflows, potentially preceded by code customisation and specify how users receive notifications. For more information, see [Setting Up Workflows](across-set-up-workflows.md).  

> [!NOTE]  
>  Typical workflow steps are about users who request approval of tasks and approvers accepting or rejecting approval requests. Therefore, many topics about how to use workflows refer to approvals.  

 The following table describes a sequence of tasks, with links to the topics that describe them.  

|**To**|**See**|  
|------------|-------------|  
|Set a workflow to start when the first entry-point event occurs.|[Enable Workflows](across-how-to-enable-workflows.md)|  
|Request approval of a task, as an approver, accept, decline, or delegate approvals, and send or view approval notifications.|[Use Approval Workflows](across-how-use-approval-workflows.md)|  
|Create workflow steps that restrict a certain record type from being used before a certain event occurs, for example that the record is approved.|[Restrict and Allow Usage of a Record](across-how-to-restrict-and-allow-usage-of-a-record.md)|  
|View workflow step instances of status Completed.|[View Archived Workflow Step Instances](across-how-to-view-archived-workflow-step-instances.md)|  
|Delete a workflow that you are sure will no longer be used.|[Delete Workflows](across-how-to-delete-workflows.md)|  

## <a name="see-also"></a>See Also  
[Setting Up Workflows](across-set-up-workflows.md)   
[Workflow](across-workflow.md)   
[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]