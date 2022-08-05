---
title: Using Workflows
description: You can set up and use workflows that connect business-process tasks like automatic posting or requesting and granting approval for new records.
author: SorenGP
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 06/11/2021
ms.author: edupont
ms.openlocfilehash: 4f66b334df678ff27e094858dd0cec44c1bb8e75
ms.sourcegitcommit: f1e272485a0e675d337a694aba3e35a5daf43920
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 07/09/2022
ms.locfileid: "9130243"
---
# <a name="use-workflows"></a>Use Workflows

A workflow is a sequence of tasks that are triggered by an action, a condition or a rule. Workflows are usually implemented to integrate business logic to an organisation, such as the separation of duties, unifying processes, or to increase trust and responsibilities.  

The workflows are designed to create requests for approval of a new value while keeping the old value in case the request isn't approved. The new value won't be implemented until the last request is approved.  

The business logic could be approval of:

- New master data like G/L Accounts, customers, vendors, or items
- Changes to fields in existing records containing sensible information, such as **Vendor Bank Account No.** or **Customer Credit Limit**
- Changes to fields in existing records containing business critical information, such as **Item Sales Prices**
- New users or changes to user permissions
- Purchase documents
- Sales documents
- Incoming documents
- Finance journals prior to posting

The following illustration shows an example of a workflow with sequential approval triggered by a user. By triggering the workflow, an approval request is created for the first approver.  

![Illustration of a workflow with sequential approval.](media/Workflows/approval-flow.png)

In this example, the request must be approved by the first approver before the request is sent on to the next approver. If the request isn't approved by the first approver, the request will never go to the next approver.  

The route taken from the initial triggering of the workflow can vary depending on the nature of the approval.  

The following illustration shows a parallel approval that is triggered by the user. By triggering the workflow, an approval request is sent to all approvers simultaneously.  

![Illustration of a workflow with parallel approval.](media/Workflows/approval-flow-2.png)

However, the workflow isn't approved until all requests have been approved by the approvers, as shown in the following illustration:  

![Illustration of a rejected workflow with parallel approval.](media/Workflows/approval-flow-3.png)

> [!NOTE]  
> It is not possible to create a workflow with multiple approvers and expect the whole workflow to be approved after the first request has been approved. All requests must be approved for the workflow to be approved.

You can set up and use workflows that connect business-process tasks performed by different users. It's also possible to create the same workflow more than once. Each workflow can be triggered by an event using different filters. This is useful if an approval request in one department must be approved by one approver, while approval requests in other departments must be approved by another approver. System tasks, such as automatic posting, can be included as steps in workflows, preceded or followed by user tasks. Requesting and granting approval to create new records are typical workflow steps.  

Before you can begin to use workflows, you must set up workflow users, create the workflows, potentially preceded by code customisation and specify how users receive notifications. For more information, see [Setting Up Workflows](across-set-up-workflows.md).  

> [!NOTE]  
> Typical workflow steps are about users who request approval of tasks and approvers accepting or rejecting approval requests. Therefore, many topics about how to use workflows refer to approvals.  

 The following table describes a sequence of tasks, with links to the articles that describe them.  

|**To**|**See**|  
|------------|-------------|  
|Set a workflow to start when the first entry-point event occurs.|[Enable Workflows](across-how-to-enable-workflows.md)|  
|Request approval of a task, as an approver, accept, decline, or delegate approvals, and send or view approval notifications.|[Use Approval Workflows](across-how-use-approval-workflows.md)|  
|Create workflow steps that restrict a certain record type from being used before a certain event occurs, for example that the record is approved.|[Restrict and Allow Usage of a Record](across-how-to-restrict-and-allow-usage-of-a-record.md)|  
|View workflow step instances of status **Completed**.|[View Archived Workflow Step Instances](across-how-to-view-archived-workflow-step-instances.md)|  
|Delete a workflow that you're sure will no longer be used.|[Delete Workflows](across-how-to-delete-workflows.md)|  

## <a name="see-related-training-at-microsoft-learn"></a>See related training at [Microsoft Learn](/learn/modules/create-workflows/)

## <a name="see-also"></a>See also

[Setting Up Workflows](across-set-up-workflows.md)  
[Workflow](across-workflow.md)  
[Work with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]