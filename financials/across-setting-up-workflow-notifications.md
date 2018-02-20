---
title: Setting Up Workflow Notifications | Microsoft Docs
description: Many workflow responses are about notifying a user that an event has occurred that they must act on. For example, on one workflow step, the event can be that User 1 requests approval of a new record, and the response is that a notification is sent to User 2, the approver. On the next workflow step, the event can be that User 2 approves the record, and the response is that a notification is sent to User 3 to start a related processing of the approved record. For workflow steps that are about approval, each notification is tied to an approval entry.
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
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: 351c079df25516a83de42d5fa12954b25ba5e63e
ms.contentlocale: en-nz
ms.lasthandoff: 01/30/2018

---
# <a name="setting-up-workflow-notifications"></a>Setting Up Workflow Notifications
Many workflow responses are about notifying a user that an event has occurred that they must act on. For example, on one workflow step, the event can be that User 1 requests approval of a new record, and the response is that a notification is sent to User 2, the approver. On the next workflow step, the event can be that User 2 approves the record, and the response is that a notification is sent to User 3 to start a related processing of the approved record. For workflow steps that are about approval, each notification is tied to an approval entry. For more information, see [Workflow](across-workflow.md).  

> [!NOTE]  
>  The generic version of [!INCLUDE[d365fin](includes/d365fin_md.md)] supports notifications as email and as internal notes.  

> [!IMPORTANT]  
>  All workflow notifications are sent through a job queue. Make sure that the job queue in your solution. For more information, see [Use Job Queues to Schedule Tasks](admin-job-queues-schedule-tasks.md).

You set up different aspects of workflow notifications in the following places:  

1.  For approval workflows, you set up the recipients of workflow notifications by filling a line in the **Approval User Setup** window for each user that takes part in the workflow. For example, if User 2 is specified in the **Approver ID** field on the line for User 1, then the approval request notification is sent to User 1. For more information, see [Set Up Approval Users](across-how-to-set-up-approval-users.md).  
2.  You set when and how users receive workflow notifications by filling the **Notification Schedule** window for each workflow user. For more information, see [Specify When and How to Receive Notifications](across-how-to-specify-when-and-how-to-receive-notifications.md).  
3.  You set up the general content and layout of notifications, including notifications about overdue workflow responses, by setting up notification templates in the **Notification Templates** window. You can use the default templates provided with [!INCLUDE[d365fin](includes/d365fin_md.md)].  
4.  You set up specific content and rules of a workflow notification when you create the workflow in question. You do this by selecting options in the **Workflow Response Options** window for the workflow response that represents the notification. For more information, see step 9 in [Create Workflows](across-how-to-create-workflows.md).  

## <a name="see-also"></a>See Also  
 [Set Up Approval Users](across-how-to-set-up-approval-users.md)   
 [Set Up Workflow Users](across-how-to-set-up-workflow-users.md)   
 [Specify When and How to Receive Notifications](across-how-to-specify-when-and-how-to-receive-notifications.md)   
 [Create Workflows](across-how-to-create-workflows.md)   
 [Manage Notification Templates](across-how-to-manage-notification-templates.md)   
 [Use Job Queues to Schedule Tasks](admin-job-queues-schedule-tasks.md)   
 [Set up Email](madeira-how-setup-email.md)   
 [Walkthrough: Setting Up and Using a Purchase Approval Workflow](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md)   
 [Workflow](across-workflow.md)   

