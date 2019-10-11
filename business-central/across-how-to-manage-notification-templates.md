---
title: How to Manage Notification Templates | Microsoft Docs
description: Notifications are sent to workflow users to notify them about steps they must make or to inform them about the status of workflow steps. You set up who receives notification and when by setting up approval users, the users’ notification schedule, and the involved workflow responses to define the notification recipient.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2019
ms.author: sgroespe
redirect_url: across-how-to-specify-when-and-how-to-receive-notifications
ms.openlocfilehash: c195ffa8b798f13d92f78896f101a84b07728d08
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 10/01/2019
ms.locfileid: "2305372"
---
# <a name="manage-notification-templates"></a>Manage Notification Templates
Notifications are sent to workflow users to notify them about steps they must make or to inform them about the status of workflow steps. You set up who receives notification and when by setting up approval users, the users’ notification schedule, and the involved workflow responses to define the notification recipient. For more information, see [Setting Up Workflow Notifications](across-setting-up-workflow-notifications.md).  

 Notifications are based on templates that define the content and layout of the notification. You can export the content of a notification template, edit it, and then import into the same or a new notification template. This is described in the following procedures.  

 The generic version of [!INCLUDE[d365fin](includes/d365fin_md.md)] contains three notification templates, one for notifying about approval requests, one for notifying about new records, and one for notifying about overdue approval requests. The three predefined notification templates support **Email** and **Note** as notification method. To view the content of the three notification templates, see the “Content of the Notification Templates” section in this topic.

## <a name="to-create-a-new-notification-template"></a>To create a new notification template  
1.  Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Notification Templates**, and then choose the related link.  
2.  On the **Notification Templates** page, choose the **New** action.  
3.  Fill the fields as described in the following table.  

    |Field|Description|  
    |---------------------------------|---------------------------------------|  
    |**Code**|Identify the notification template.|  
    |**Description**|Describe the notification template.|  
    |**Notification Method**|Specify if the notification is sent as an email or as a note.|  
    |**Type**|Specify the business process that the notification will be used for.<br /><br /> Select one of the following types:<br /><br /> -   **Approval** specifies that the template is used to notify users in approval workflows.<br />-   **New Record** specifies that the template is to notify approvers when a new record, such as a customer card, needs their approval.<br />-   **Overdue** specifies that the template is used to notify users about overdue approval requests.|  
    |**Default**|Specify if the notification template will be used by default.|  

## <a name="to-modify-a-notification-template"></a>To modify a notification template  
1.  Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Notification Templates**, and then choose the related link.  
2.  On the **Notification Templates** page, select the notification template that you want to modify.  
3.  Choose the **Export Template Content** action.  
4.  On the **Export File** page, choose the **Save** button, and then name and save the HTML file in an appropriate location.  
5.  Right-click the file, choose **Open with**, and then choose the relevant program.  

    > [!NOTE]  
    >  Content for notification templates of type Email are in HTML format. Content for notification templates of type Note are in TXT format.  
6.  Edit the content of the notification template by adding, changing, or removing parameter variables to define the content that you want, and then save it. For more information, see the “Content of the Notification Templates” section.  

    Proceed to import the modified content back into the same or a new notification template.  
7.  To modify the notification template that you exported, on the **Notification Templates** page, select the template that you selected in step 2.  

    Alternatively, to import the modified template content into a new notification template, follow the “To create a new notification template” procedure, and then select the new notification template.  
8.  Choose the **Import Template Content** action.  
9. If you are modifying an existing notification template, choose the **Yes** button on the message about overwriting the existing template.  
10. On the **Select a file to import** page, choose the HTML file that you modified in step 6, and then choose the **Open** button.  

The existing or new notification template on the **Notification Templates** page is now updated with the modified content.  

### <a name="content-of-the-notification-templates"></a>Content of the Notification Templates  
The three notification template types, **New Record**, **Approval**, and **Overdue**, have different content.  

Parameter values are automatically inserted in notifications according to the notification template type.  

#### <a name="new-record"></a>New Record  
 ![NAV&#95;notification&#95;template&#95;new&#95;record&#95;type](media/nav_notification_template_new_record.png "NAV_notification_template_new_record")  

#### <a name="approval"></a>Approval  
 ![NAV&#95;notification&#95;template&#95;approval&#95;type](media/nav_notification_template_approval_type.png "NAV_notification_template_approval_type")  

#### <a name="overdue"></a>Overdue  
 ![NAV&#95;notification&#95;overdue&#95;type](media/nav_notification_overdue_type.png "NAV_notification_overdue_type")  

## <a name="see-also"></a>See Also  
 [Setting Up Workflow Notifications](across-setting-up-workflow-notifications.md)   
 [Set up Email](admin-how-setup-email.md)   
 [Set Up Workflow Users](across-how-to-set-up-workflow-users.md)   
 [Set Up Approval Users](across-how-to-set-up-approval-users.md)   
 [Create Workflows](across-how-to-create-workflows.md)   
 [Use Job Queues to Schedule Tasks](admin-job-queues-schedule-tasks.md)   
 [Workflow](across-workflow.md)   
