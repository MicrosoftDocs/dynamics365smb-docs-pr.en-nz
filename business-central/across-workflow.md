---
title: Workflows in Dynamics 365 Business Central
description: Use built-in workflow capabilities to set up approval workflows to supplement automated workflows based on Power Automate. You can set up steps to assign tasks to different people as part of different business-process tasks.
author: jswymer
ms.author: jswymer
ms.reviewer: jswymer
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.date: 10/10/2022
ms.custom: bap-template
---
# <a name="workflows-in-dynamics-365-business-central"></a><a name="workflows-in-dynamics-365-business-central"></a><a name="workflows-in-dynamics-365-business-central"></a>Workflows in Dynamics 365 Business Central

You can set up and use workflows to connect business-process tasks performed by different users. System tasks, such as automatic posting, can be included as steps in workflows. System tasks can be preceded or followed by user tasks. Requesting and granting approval to create new records are typical workflow steps.

The default version of [!INCLUDE [prod_short](includes/prod_short.md)] supports three types of workflows:
  
* Power Automate flows

  * Automated flows that are triggered by events (such as record or document creation, modification, or deletion) in [!INCLUDE[prod_short](includes/prod_short.md)]. Also included are approval flows created in Power Automate that trigger when an approval is requested in [!INCLUDE[prod_short](includes/prod_short.md)].
  * Instant flows that are manually triggered by the **Automate** action from lists, cards, and document pages.

    Create and manually trigger a Power Automate flow on a [!INCLUDE[prod_short](includes/prod_short.md)] record, such as a customer, item, or sales order, with options to manipulate information both internally and externally (using integrated tools).

* Approval workflows based on built-in workflow templates

  On the **Workflow Templates** page, you can see all available workflows. The trial version of [!INCLUDE[prod_short](includes/prod_short.md)] includes many pre-configured workflows represented by workflow templates you can copy to create new ones. When you open a template from the **Workflow Templates** page, and the workflow name starts with *MS-*, then the template was added by Microsoft.

## <a name="power-automate-flows"></a><a name="power-automate-flows"></a><a name="power-automate-flows"></a>Power Automate flows

With [!INCLUDE [prod_short](includes/prod_short.md)] online, you can sign up for Power Automate to build powerful automated workflows. You run those workflows from inside [!INCLUDE [prod_short](includes/prod_short.md)]. The flows can connect internal and external data sources and tools, without coding knowledge.

|**To** |**See**|
|-------|-------|
|Get started with Power Automate and creating flows, running  instant flows|[Use Power Automate Flows in [!INCLUDE[prod_short](includes/prod_short.md)]](across-how-use-financials-data-source-flow.md)|
|Learn details of how to create, edit, and manage flows|[Set Up Automated Flows](/dynamics365/business-central/dev-itpro/powerplatform/automate-workflows) and [Set Up Instant Flows](/dynamics365/business-central/dev-itpro/powerplatform/instant-flows)|
|Set up Power Automate integration with [!INCLUDE[prod_short](includes/prod_short.md)] for users as an admin|[Set Up Power Automate Integration](/dynamics365/business-central/dev-itpro/powerplatform/power-automate-setup)|

## <a name="approval-workflows"></a><a name="approval-workflows"></a><a name="approval-workflows"></a>Approval workflows

Create an approval workflow by defining what starts the workflow and what happens next, as follows:

* A workflow event, which is moderated by event conditions.
* A workflow response, which is moderated by response options.

To define workflow steps, fill in fields on workflow lines using the event and response values that represent supported scenarios.

Examples of approval workflows events include the creation of sales or purchase orders/quotes/invoices, price changes, vendor or customer edits, and more.

[!INCLUDE[workflow](includes/workflow.md)]

| **To** | **See** |
|--|--|
| Set up approval workflow users, specify how users get notified, and create new workflows. (To create new workflows for unsupported scenarios, implement the required workflow elements by customising the application code.) | [Set Up Approval Workflows](across-set-up-workflows.md) |
| Enable approval workflows, act on workflow notifications, including requesting and approving a workflow step. Archive and delete workflows. | [Use Approval Workflows](across-use-workflows.md) |

<!--
| Integrate company data with Power Automate workflows, using both internal and external sources and events to create and automate tasks or workflows. | [Use Power Automate Flows in [!INCLUDE[prod_short](includes/prod_short.md)]](across-how-use-financials-data-source-flow.md) |-->

## <a name="see-related-microsoft-training"></a><a name="see-related-microsoft-training"></a><a name="see-related-microsoft-training"></a>See related [Microsoft training](/training/modules/create-workflows/)

## <a name="see-also"></a><a name="see-also"></a><a name="see-also"></a>See also

[Sales](sales-manage-sales.md)  
[Purchasing](purchasing-manage-purchasing.md)  
[Managing Projects](projects-manage-projects.md)  
[Work with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  
[Troubleshoot Your [!INCLUDE[prod_short](includes/prod_short.md)] Automated Workflows](across-flow-troubleshoot.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]
