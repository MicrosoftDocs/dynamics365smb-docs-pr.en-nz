---
title: Workflows in Dynamics 365 Business Central
description: Use built-in workflow capabilities to set up approval workflows to supplement automated workflows based on Power Automate. You can set up steps to assign tasks to different people as part of different business-process tasks.
author: SorenGP
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 09/13/2022
ms.author: edupont
ms.openlocfilehash: ecaaf9bbb56e1c1b47f9f617319b32f32a2920fd
ms.sourcegitcommit: 9049f75c86dea374e5bfe297304caa32f579f6e4
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 09/23/2022
ms.locfileid: "9585638"
---
# <a name="workflows-in-dynamics-365-business-central"></a>Workflows in Dynamics 365 Business Central

You can set up and use workflows to connect business-process tasks performed by different users. System tasks, such as automatic posting, can be included as steps in workflows, preceded or followed by user tasks. Requesting and granting approval to create new records are typical workflow steps.

The default version of [!INCLUDE [prod_short](includes/prod_short.md)] supports three types of workflows:

* Approval workflows based on built-in workflow templates

  On the **Workflow Templates** page, you can see all available workflows. The trial version of [!INCLUDE[prod_short](includes/prod_short.md)] includes many pre-configured workflows represented by workflow templates you can copy to create new ones. When you open a template from the **Workflow Templates** page, and the workflow name starts with *MS-*, then the template was added by Microsoft.
  
* Power Automate flows you set up yourself

  Any workflow template you create with Microsoft Power Automate is added to the list of workflow templates within [!INCLUDE[prod_short](includes/prod_short.md)]. Learn more at [Use [!INCLUDE[prod_short](includes/prod_short.md)] in Power Automate Flows](across-how-use-financials-data-source-flow.md). 
  
* Instant flows manually triggered by the **Automate** action ([!INCLUDE [prod_short](includes/prod_short.md)] online only).

  Create and manually trigger a Power Automate flow on a [!INCLUDE[prod_short](includes/prod_short.md)] record, such as a customer, item, or sales order, with options to manipulate information both internally and externally (using integrated tools). Learn more in the [Instant flows](across-how-use-financials-data-source-flow.md#instant-flows) section.

## <a name="power-automate-flows"></a>Power Automate flows

Using [!INCLUDE [prod_short](includes/prod_short.md)] online, you can sign up for Power Automate to build powerful automated workflows. You can run those workflows from inside [!INCLUDE [prod_short](includes/prod_short.md)], connecting internal and external sources of data and tools, without coding knowledge.

Power Automate flows can be triggered by events (such as record or document creation, modification, or deletion) and run on a user-defined schedule, or on demand (known as an **Instant Flow**).

## <a name="approval-workflows"></a>Approval workflows

You create an approval workflow by listing the involved steps on the lines. Each step consists of a workflow event, moderated by event conditions, and a workflow response, moderated by response options. You define workflow steps by filling in fields on workflow lines using fixed lists of event and response values representing scenarios supported by the application code.<!--What are the "values"? Can we give an example?-->

Examples of approval workflows events include, among others, the creation of sales or purchase orders/quotes/invoices, price changes, and vendor or customer edits.

[!INCLUDE[workflow](includes/workflow.md)]

| **To** | **See** |
|--|--|
| Set up approval workflow users, specify how users get notified, and create new workflows. (To create new workflows for unsupported scenarios, implement the required workflow elements by customising the application code.) | [Set Up Approval Workflows](across-set-up-workflows.md) |
| Enable approval workflows, act on workflow notifications, including requesting and approving a workflow step. Archive and delete workflows. | [Use Approval Workflows](across-use-workflows.md) |
| Integrate company data with Power Automate workflows, using both internal and external sources and events to create and automate tasks or workflows. | [Use Power Automate Flows in [!INCLUDE[prod_short](includes/prod_short.md)]](across-how-use-financials-data-source-flow.md) |

## <a name="see-related-microsoft-training"></a>See related [Microsoft training](/training/modules/create-workflows/)

## <a name="see-also"></a>See also

[Sales](sales-manage-sales.md)  
[Purchasing](purchasing-manage-purchasing.md)  
[Managing Projects](projects-manage-projects.md)  
[Work with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  
[Troubleshoot Your [!INCLUDE[prod_short](includes/prod_short.md)] Automated Workflows](across-flow-troubleshoot.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]
