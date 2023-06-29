---
title: Specify When and How to Receive Workflow Notifications
description: 'When you set users up in approval workflows, you can specify how and when each approval user receives notifications.'
author: brentholtorf
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: null
ms.search.form: '663, 1500, 1512, 1513,'
ms.date: 09/09/2022
ms.author: bholtorf
---
# <a name="specify-when-and-how-to-receive-workflow-notifications"></a><a name="specify-when-and-how-to-receive-workflow-notifications"></a>Specify When and How to Receive Workflow Notifications

When you set up approval users in workflows where you want someone to approve changes, such as when new records are created or when someone requests an approval, you must specify how and when to notify the approval user. For example, you can specify that an approval user will immediately receive an email when someone creates a new customer. Alternatively, you can schedule the notifications to be held and then delivered together, for example, on a weekly or monthly basis.

People can also change their notification setup by choosing **Change Notification Settings** on any notification.  

> [!NOTE]
> Notifications are delivered according to the notification settings for the receiver, not the sender. That's an important distinction because it means that when someone requests an approval as part of a workflow, their request is not necessarily sent immediately. Instead, it will be delivered according to the notification schedule specified in the approver's notification settings.

Before you can set up an approval user's notification preferences, you must set up the user as an approval user. Learn more at [Set Up Approval Users](across-how-to-set-up-approval-users.md).  

> [!NOTE]
> If you want to use email as the notification method, you must set email up for both the sender and the receiver in [!INCLUDE [prod_short](includes/prod_short.md)]. Learn more at [Set up Email](admin-how-setup-email.md).

## <a name="steps-in-workflows"></a><a name="steps-in-workflows"></a>Steps in workflows

Many approval workflow steps are about notifying users that an event they must act on has occurred. For example, on one workflow step, the event can be that User 1 requests approval of a new record. The related response is that a notification is sent to User 2, the approver. On the next workflow step, the event can be that User 2 approves the record. The related response is that a notification is sent to User 3 to start a process with the approved record. For workflow steps involving approvals, each notification is tied to an approval entry. Learn more at [Workflow](across-workflow.md).  

## <a name="specify-when-and-how-approval-users-receive-notifications"></a><a name="specify-when-and-how-approval-users-receive-notifications"></a>Specify when and how approval users receive notifications

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Approval User Setup**, then choose the related link.  
2. Select the line for the user you want to set up notification preferences for, then choose the **Notification Setup** action.  
3. On the **Workflow Notification Setup** page, fill in the fields as described in the following table.  

   > [!NOTE]
   > If you open the **Workflow Notification Setup** page from the **Approval User Setup** page the notification setup is linked to the approval user. The approval user will always receive workflow notifications according to that notification setup. If you use the *Tell Me* feature to open the **Workflow Notification Setup** page, the notification setup applies to all users.

   |Field|Description|
   |-----|-----------|
   |**Notification Type**|Specify the type of event the notification is about.<br /><br /> Select one of the following options:<br /><br /> -   **New Record** specifies that the notification is about a new record, such as a document, that the user must act on.<br />-   **Approval** specifies that the notification is about one or more approval requests.<br />-   **Overdue** specifies that the notification is to remind users that they're late in acting on an event.|
   |**Notification Method**|Specify if the notification is an email or an internal note.|

   You can define the layout of email notifications by customising Report 1320, Notification Email. Learn more at [Create and Modify Custom Report Layouts](ui-how-create-custom-report-layout.md).

   You've now specified how the user receives notifications. Proceed to specify when the user receives notifications.  
4. Choose the **Notification Schedule** action.  
5. On the **Notification Schedule** page, fill in the fields as described in the following table.  

   |Field|Description|
   |-----|-----------|
   |**Recurrence**|Specify the recurring pattern in which notifications are sent to the user.|
   |**Time**|Specify what time of day notifications are sent to the user when the value in the **Recurrence** field is anything other than **Instantly**.|
   |**Daily Frequency**|Specify on which type of days the user receives notifications when the value in the **Recurrence** field is **Daily**.<br /><br /> Select **Weekday** to receive notifications every day of the work week. Select **Daily** to receive notifications every day of the week, including weekends.|
   |**Monday** through **Sunday**|Specify on which days the user receives notifications when the value in the **Recurrence** field is **Weekly**.|
   |**Date of Month**|Specify if the user receives notifications on the first, last, or a specific date of the month.|
   |**Monthly Notification Date**|Specify the date of the month on which the user receives notifications when the value in the **Date of Month** field is **Custom**.|

## <a name="change-when-and-how-you-receive-notifications"></a><a name="change-when-and-how-you-receive-notifications"></a>Change when and how you receive notifications

1. On one of the notifications you've received, either as an email or a note, choose **Change Notification Settings**.  
2. On the **Workflow Notification Setup** page, change your notification preferences as described in steps 3-5 above.
   1. Confirm that the correct notification is chosen under the **Notification Type** field.
   2. Choose whether to receive an email or note notification under the  **Notification Method** field.
   3. Select the **Notification Schedule** to change the frequency and recurrence in which notifications are sent.

## <a name="see-also"></a><a name="see-also"></a>See also

[Set Up Approval Users](across-how-to-set-up-approval-users.md)  
[Create and Modify Custom Report Layouts](ui-how-create-custom-report-layout.md)  
[Setting Up Approval Workflow Notifications](across-setting-up-workflow-notifications.md)  
[Setting Up Approval Workflows](across-set-up-workflows.md)  
[Use Approval Workflows](across-use-workflows.md)

[!INCLUDE[footer-include](includes/footer-banner.md)]
