---
title: Set Up Workflows (contains video)
description: Set up workflows, workflow users and approval users to connect business-process system tasks performed by these different users.
author: SorenGP
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 06/11/2021
ms.author: edupont
ms.openlocfilehash: 7676e05255c31bd2b9906951d98d1a87622a0fcf
ms.sourcegitcommit: 3acadf94fa34ca57fc137cb2296e644fbabc1a60
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 09/19/2022
ms.locfileid: "9530287"
---
# <a name="set-up-workflows"></a>Set Up Workflows

You can set up and use workflows that connect business-process tasks performed by different users. System tasks, such as automatic posting, can be included as steps in workflows, preceded or followed by user tasks. Requesting and granting approval to create new records are typical workflow steps. For more information, see [Use Workflows](across-use-workflows.md).  

Before you begin to use workflows, you must set up workflow users and approval users, specify how users receive notifications about workflow steps, and then create the workflows.  

On the **Workflow** page, you create a workflow by listing the involved steps on the lines. Each step consists of a workflow event, moderated by event conditions, and a workflow response, moderated by response options. You define workflow steps by filling fields on workflow lines from fixed lists of event and response values representing scenarios that are supported by the application code.  

[!INCLUDE[workflow](includes/workflow.md)]

The following table describes a sequence of tasks, with links to the articles that describe them.  

|**To**|**See**|  
|------------|-------------|  
|Set up workflow users and user groups.|[Set Up Workflow Users](across-how-to-set-up-workflow-users.md)|  
|Set up workflow users who take part in approval workflows.|[Set Up Approval Users](across-how-to-set-up-approval-users.md)|  
|Specify how workflow users are notified of workflow steps, including approval requests.|[Setting Up Workflow Notifications](across-setting-up-workflow-notifications.md)|  
|Specify if users are notified by email or note and how often notifications are sent.|[Specify When and How to Receive Notifications](across-how-to-specify-when-and-how-to-receive-notifications.md)|  
|Customise the content of the email notification by modifying Report 1320, Notification Email.|[Create and Modify Custom Report Layouts](ui-how-create-custom-report-layout.md)|  
|Set up an SMTP server to enable email communication in and out of [!INCLUDE[prod_short](includes/prod_short.md)]|[Set up Email](admin-how-setup-email.md)|
|Specify the different steps of a workflow by connecting workflow events with workflow responses.|[Create Workflows](across-how-to-create-workflows.md)|  
|Use workflow templates to create new workflows.|[Create Workflows from Workflow Templates](across-how-to-create-workflows-from-workflow-templates.md)|  
|Share workflows with other [!INCLUDE[prod_short](includes/prod_short.md)] databases.|[Export and Import Workflows](across-how-to-export-and-import-workflows.md)|  
|Learn how to set up a workflow for approving sales documents by following an end-to-end procedure.|[Walkthrough: Setting Up and Using a Purchase Approval Workflow](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md)|  

## <a name="example-of-an-approval-workflow"></a>Example of an approval workflow

This video shows how to set up a workflow that will require a user to request someone else's approval before they can change information about an existing customer or create a new customer.  
<br><br>  

> [!Video https://www.microsoft.com/en-us/videoplayer/embed/RE4jzHI?rel=0]

## <a name="see-related-microsoft-training"></a>See related [Microsoft training](/training/modules/create-workflows/)

## <a name="see-also"></a>See also

[Use Workflows](across-use-workflows.md)  
[Workflow](across-workflow.md)  
[Walkthrough: Setting Up and Using a Purchase Approval Workflow](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md)  
[Work with Business Central](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]
