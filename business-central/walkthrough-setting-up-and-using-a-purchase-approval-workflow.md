---
title: Setting Up and Using a Purchase Approval Workflow
description: This walkthrough takes you through all the stages involved in setting up and using a purchase approval workflow in Business Central.
author: SorenGP
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: null
ms.date: 09/13/2022
ms.author: edupont
---
# <a name="walkthrough-setting-up-and-using-a-purchase-approval-workflow"></a><a name="walkthrough-setting-up-and-using-a-purchase-approval-workflow"></a>Walkthrough: Setting Up and Using a Purchase Approval Workflow

You can automate the process of approving new or changed records, such as documents, journal lines, and customer cards, by creating workflows with steps for the approvals in question.

Before you create approval workflows, you must set up an approver and substitute approver for each approval user. You can also set approvers' amount limits to define which sales and purchase records they're qualified to approve. Approval requests and other notifications can be sent as an email or internal note. For each approval user setup, you can also set up when they receive notifications.

> [!NOTE]
> In addition to the Workflow functionality within [!INCLUDE[prod_short](includes/prod_short.md)], you can use Power Automate to define workflows for events in [!INCLUDE[prod_short](includes/prod_short.md)]. Note that although they are two separate workflow systems, any flow template that you create with Power Automate is added to the list of workflow templates within [!INCLUDE[prod_short](includes/prod_short.md)]. Learn more at [Use Business Central in an Automated Workflow](across-how-use-financials-data-source-flow.md).  

You can set up and use workflows that connect business-process tasks performed by different users. System tasks, such as automatic posting, can be included as steps in workflows, preceded or followed by user tasks. Requesting and granting approval to create new records are typical workflow steps. Learn more at [Workflow](across-workflow.md).  

## <a name="about-this-walkthrough"></a><a name="about-this-walkthrough"></a>About this walkthrough

This walkthrough is a scenario illustrating the following tasks:  

- Setting up approval users  
- Setting up notifications for approval users  
- Modifying and enabling an approval workflow  
- Requesting approval of a purchase order (as Alicia)  
- Receiving a notification and then approving the request (as Sean)  

## <a name="story"></a><a name="story"></a>Story

Sean is a super user at CRONUS and creates two approval users. One is Alicia who represents a purchasing agent. The other is Sean themself, representing Alicia's approver. Sean then gives themself unlimited purchase approval rights and specifies that they'll receive notifications by internal note as soon as a relevant event occurs. Finally, Sean creates the required approval workflow as a copy of the existing *Purchase Order Approval Workflow* template, leaves all existing event conditions and response options unchanged, and then enables the workflow.  

To test the approval workflow, Sean signs in to [!INCLUDE[prod_short](includes/prod_short.md)] as Alicia and then requests approval of a purchase order. Sean then signs in as themself, sees the note in the Role Centre, follows the link to the approval request for the purchase order, and approves the request.  

## <a name="users"></a><a name="users"></a>Users

Before you can set up approval users and their notification method, you must make sure that those users exist in [!INCLUDE[prod_short](includes/prod_short.md)]: One user will represent Alicia. The other user, yourself, will represent Sean. Learn more at [Create Users According to Licences](ui-how-users-permissions.md).

### <a name="setting-up-approval-users"></a><a name="setting-up-approval-users"></a>Setting up approval users

When signed in as yourself, set up Alicia as an approval user whose approver is yourself. Set up your approval rights and specify how and when you're notified of approval requests.  

#### <a name="to-set-up-yourself-and-alicia-as-approval-users"></a><a name="to-set-up-yourself-and-alicia-as-approval-users"></a>To set up yourself and Alicia as approval users

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Approval User Setup**, and then choose the related link.  
2. On the **Approval User Setup** page, choose the **New** action.  

    > [!NOTE]  
    >  You must set up an approver before you can set up users who require that approver's approval. That means you must set yourself up before you can set Alicia up.  

3. Set up the two approval users by filling the fields as described in the following table.  

    |User ID|Approver ID|Unlimited Purchase Approval|  
    |-------|-----------|---------------------------|  
    |YOU||Selected|
    |ALICIA|YOU||

### <a name="setting-up-notifications"></a><a name="setting-up-notifications"></a>Setting up notifications

In this walkthrough, the user is notified by an internal note about requests to approve. Approval notifications can also be sent by email, and you can add a workflow response step that notifies the sender when a request is approved or rejected. Learn more at [Specify When and How to Receive Notifications](across-how-to-specify-when-and-how-to-receive-notifications.md).

#### <a name="to-set-up-how-and-when-you-are-notified"></a><a name="to-set-up-how-and-when-you-are-notified"></a>To set up how and when you are notified

1. On the **Approval User Setup** page, select the line for yourself, and then choose the **Notification Setup** action.  
2. On the **Notification Setup** page, in the **Notification Type** field, choose **Approval**.  
3. In the **Notification Method** field, choose **Note**.  
4. On the **Notification Setup** page, choose the **Notification Schedule** action.  
5. On the **Notification Schedule** page, in the **Recurrence** field, select **Instantly**.  

## <a name="creating-the-approval-workflow"></a><a name="creating-the-approval-workflow"></a>Creating the approval workflow

Create the purchase order approval workflow by copying the steps from the **Purchase Order Approval Workflow** template. Leave the existing workflow steps unchanged, and then enable the workflow.  

> [!TIP]
> Optionally, add a workflow response step to notify the sender when their request is approved or rejected. Learn more at [Specify When and How to Receive Notifications](across-how-to-specify-when-and-how-to-receive-notifications.md).

### <a name="to-create-and-enable-a-purchase-order-approval-workflow"></a><a name="to-create-and-enable-a-purchase-order-approval-workflow"></a>To create and enable a purchase order approval workflow

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Workflows**, then choose the related link.  
2. On the **Workflows** page, select **Actions**, then select **New**, and then choose the **New Workflow from Template** action.  
3. On the **Workflow Templates** page, select the workflow template named **Purchase Order Approval Workflow**.  

   The **Workflow** page opens for a new workflow containing all the information of the selected template. The value in the **Code** field is extended with *-01* to indicate this is the first workflow created from the **Purchase Order Approval Workflow** template.  
4. On the header of the **Workflow** page, turn on the **Enabled** toggle.  

## <a name="use-the-approval-workflow"></a><a name="use-the-approval-workflow"></a>Use the approval workflow

Use the new Purchase Order Approval Workflow by first signing in to [!INCLUDE[prod_short](includes/prod_short.md)] as Alicia to request approval of a purchase order. Then sign in as yourself, view the note on the Role Centre, follow the link to the approval request, then approve the request.  

### <a name="to-request-approval-of-a-purchase-order-as-alicia"></a><a name="to-request-approval-of-a-purchase-order-as-alicia"></a>To request approval of a purchase order, as Alicia

1. Sign in as Alicia.
2. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchase Orders**, then choose the related link.  
3. Select the line to open *Purchase Order 106001*.  
4. On the **Purchase Order** page, choose **Actions**, then **Request Approval**, and then choose the **Send Approval Request** action.  

Notice that the value in the **Status** field has changed to **Pending Approval**.  

### <a name="to-approve-the-purchase-order-as-sean"></a><a name="to-approve-the-purchase-order-as-sean"></a>To approve the purchase order, as Sean

1. Sign in as Sean.
2. On the Role Centre, in the **Self Service** area, choose **Requests to Approve**.
3. On the **Requests to Approve** page, select the line about the purchase order from Alicia, then choose the **Approve** action.  

The value in the **Status** field on Alicia's purchase order changes to **Released**.  

You have now set up and tested a simple approval workflow based on the first two steps of the **Purchase Order Approval Workflow**. You can easily extend this workflow to automatically post Alicia's purchase order when Sean approves it. To do this, you must enable the **Purchase Invoice Workflow**, so the response to a released purchase invoice is to post it. First you must change the event condition on the first workflow step from (purchase) **Invoice** to **Order**.  

The generic version of [!INCLUDE[prod_short](includes/prod_short.md)] includes many workflow templates for scenarios that are supported by the application code. Most of these templates are for approval workflows.  

You define variations of workflows by filling in fields on workflow lines using fixed lists of event and response values representing scenarios that are supported by the application code. Learn more at [Create Workflows](across-how-to-create-workflows.md).  

[!INCLUDE[workflow](includes/workflow.md)]

## <a name="see-related-microsoft-training"></a><a name="see-related-microsoft-training"></a>See related [Microsoft training](/training/modules/use-approval-workflows/)

## <a name="see-also"></a><a name="see-also"></a>See also

[Set Up Approval Users](across-how-to-set-up-approval-users.md)  
[Setting Up Workflow Notifications](across-setting-up-workflow-notifications.md)  
[Create Approval Workflows](across-how-to-create-workflows.md)  
[Use Approval Workflows](across-how-use-approval-workflows.md)  
[Workflow](across-workflow.md)  
[Use Business Central in an Automated Workflow](across-how-use-financials-data-source-flow.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]
