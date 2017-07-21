---
title: Approve or Reject Documents in Workflows| Microsoft Docs
description: Request, reject, or delegate an approval of, for example, a purchase or sales document, as part of a workflow.
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: reject, delegate, request
ms.date: 04/25/2017
ms.author: sgroespe
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: ffeffe725025dc03d2053333f75249679103b6a4
ms.contentlocale: en-nz
ms.lasthandoff: 07/07/2017


---
# <a name="how-to-use-approval-workflows"></a>How to: Use Approval Workflows
When a record, such as a purchase document or a customer card, needs to be approved by someone in your organisation, you send an approval request as part of a workflow. Based on how the workflow is set up, the appropriate approver is then notified that the record requires their approval.

You set up approval workflows in the **Workflow** window.

Core approval workflows for purchases documents, sales documents, payment journals, customer cards, and item cards are ready to start as assisted setup. For more information, see [Welcome to [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)](index.md).

> [!NOTE]  
>   This functionality requires that your experience is set to **Suite**. For more information, see [Customizing Your [!INCLUDE[d365fin](includes/d365fin_md.md)] Experience](ui-experiences.md).

## <a name="to-request-approval-of-a-record"></a>To request approval of a record
The following task is performed by an approval user.

1. In the window that presents the record, choose the **Send Approval Request** action.
2. To see all your approval requests, choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Approval Request Entries**, and then choose the related link.  

The status of the approval entry is updated from **Created** to **Open**. The status of the record, for example a purchase invoice, is updated from **Open** to **Pending Approval** and remains locked for processing until all approvers have approved the record.

When the approver has approved the record, the status changes to **Released**. You can then continue your tasks with the record.

## <a name="to-cancel-requests-for-approval"></a>To cancel requests for approval
The following task is performed by an approval user with approver rights.

A customer may want to change an order after it has been submitted for approval. In this case, you can cancel the approval process and make the necessary changes to the order before you request approval again.

- In the window that displays the record, choose the **Cancel Approval Request** action.

When the approval request has been cancelled, the status of the related approval entry is changed to **Cancelled**. The status of the record is updated from **Pending Approval** to **Open**. The approval process can then start again.

## <a name="to-make-minor-changes-to-approved-records"></a>To make minor changes to approved records
If you want to make a minor change to a record after it has been approved, you can reopen the record, make the change, and then release it. For minor changes, you do this with the **Reopen** and **Release** buttons.

1. Open the window that displays the record, such as a purchase invoice, and then choose the **Reopen** action.

    The **Document Status** field is changed to **Open**.
2. Make the necessary changes on the record, such as the vendor’s address.
3. Choose the **Release** action.

When you reopen the source record, the status of the related approval entry remains Approved in the **Approval Entries** window.

## <a name="to-approve-or-reject-requests-for-approval"></a>To approve or reject requests for approval
The following task is performed by an approval user with approver rights.

You can process approval requests in the **Requests to Approve** window, for example to approve multiple requests at a time. Alternatively, you can process each request on the related record, such as the **Purchase Invoice** window, by choosing the link in the notification that you receive.

1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Requests to Approve**, and then choose the related link.
2. Select one or more lines for the record or records that you want to approve or reject.
3. Choose the **Approve**, **Reject**, or **Delegate** actions.

When a record has been approved or rejected, the approval status in the **Status** field changes to **Approved** or **Rejected**.

If an approver hierarchy is set up, the record status will be **Pending Approval** until all approvers have approved the record. Then the record status will change to **Released**.

At the same time, the approval status changes from **Created** to **Open** as soon as an approval request for the record is created. If the request is rejected, the approval status changes to **Rejected**. The status remains **Open** or **Rejected** until all approvers have approved the request.

## <a name="to-delegate-requests-for-approval"></a>To delegate requests for approval
The following task is performed by an approval user with approver rights.

To prevent documents from piling up or otherwise block the workflow, the approver and the approval administrator can delegate an approval request to a substitute approver. The substitute can either be a designated substitute, the direct approver, or the approval administrator, in that order of priority. You typically use this feature if an approver is out of office and is unable to approve requests before the due date.

1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Requests to Approve**, and then choose the related link.
2. Select one or more lines for the approval requests that you want to delegate to a substitute approver, and then choose the **Delegate** action.

A notification to approve the request is sent to the substitute approver.

## <a name="to-manage-overdue-approval-requests"></a>To manage overdue approval requests
The following task is performed by an approval user with approver rights.

At regular intervals, you must remind approval workflow users of overdue approval requests that they must react on. You use the **Send Overdue Approval Notifications** function for this.

The **Send Overdue Approval Notifications** function checks for all open approval requests that are currently overdue. Each approver that has at least one overdue approval entry receives a notification with the list of all their overdue approval requests. The notification is also sent to their approver and all the requesters of the overdue approvals. This helps if the overdue approval entry must be delegated to a substitute.

1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Overdue Approval Requests**, and then choose the related link.
2. In the **Overdue Approval Requests** window, choose the **Send Overdue Approval Notifications** action.

## <a name="see-also"></a>See Also
[Sales](sales-manage-sales.md)    
[Incoming Documents](across-income-documents.md)  
[Purchasing](purchasing-manage-purchasing.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)](ui-work-product.md)

