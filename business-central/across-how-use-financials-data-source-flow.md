---
title: Use Power Automate flows in Business Central
description: Set up and use Power Automate flows to create or modify Business Central data.
author: jswymer
ms.author: jswymer
ms.reviewer: jswymer
ms.service: dynamics-365-business-central
ms.topic: conceptual
ms.search.keywords: 'workflow, OData, Power App, SOAP, Power Automate,'
ms.search.form: '1500,'
ms.date: 08/31/2023
ms.custom: bap-template
---

<!-- Line 41 says there are three cloud flow types, but the table lists four. Should line 41 change? -->


# <a name="use-power-automate-flows-in-"></a>Use Power Automate flows in [!INCLUDE[prod_short](includes/prod_short.md)]

With [!INCLUDE[prod_short](includes/prod_short.md)], you're given a licence to Microsoft Power Automate. This licence lets you use your [!INCLUDE[prod_short](includes/prod_short.md)] data as part of a workflow in Microsoft Power Automate. You create flows and connect to your data from internal and external sources through the [!INCLUDE [prod_short](includes/prod_short.md)] connector.

Power Automate flows are triggered by events, such as a record being created, modified, or deleted. Flows can also be run on a user-defined schedule or on demand.

> [!NOTE]
> Administrators can restrict access to Power Automate. If you find that you don't have access to some or all of the features described in this article, talk to your admin. If you want to learn how you can control Power Automate access as an admin, see [Set Up Power Automate Integration](/dynamics365/business-central/dev-itpro/powerplatform/power-automate-setup).

<!-- You must have a valid account with both [!INCLUDE[prod_short](includes/prod_short.md)] and Power Automate. --> 

> [!TIP]
> In addition to Power Automate, you can use approval workflow templates in [!INCLUDE[prod_short](includes/prod_short.md)]. Although they're two separate workflow systems, any approval workflow template you create with Power Automate is added to the list of workflows within [!INCLUDE[prod_short](includes/prod_short.md)]. Learn more at [Workflows](across-workflow.md).

## <a name="about-power-automate-flows"></a>About Power Automate flows

Power Automate is a service that helps you create automated workflows (or flows) between apps and services, like [!INCLUDE[prod_short](includes/prod_short.md)]. Power Automate flows require little or no coding knowledge. They can be associated with a wide range of events and responses, such as:

- Record changes
- External files updates
- Posted documents
- Different Microsoft and third-party services, like Microsoft Outlook, Excel, Dataverse, Teams, SharePoint, Power Apps, and more.

There are three different cloud flow types that you can work with:

|Flow type|Description|
|---------|-----------|
|Automated flow|This flow type is run automatically by an event. In [!INCLUDE[prod_short](includes/prod_short.md)], an event could be when a record or document is created, modified or deleted. So, for example, a new sales invoice can trigger a flow for an approval request, which can have different events set depending on the approver's reply. A negative response sends a notification and email to the approval requester. A positive reply simultaneously updates an Excel spreadsheet located in a SharePoint folder and sends an update to a Teams chat. Automated flows can be started by both internal and external events in [!INCLUDE[prod_short](includes/prod_short.md)].|
|Approval flow|Approval flows are also automated flows in Power Automate, but they're designed specifically for requesting approval when changes are made to records and data. You can use approval flows in Power Automate as an alternative to the [approval workflows feature](across-use-workflows.md) that's part of [!INCLUDE[prod_short](includes/prod_short.md)]. |
|Scheduled flow|This type of flow is also automatically run but it runs periodically at a scheduled date and time. |
|Instant flow|This flow type is run on-demand, requiring the user to run it manually from a button or action in another app or device, in this case, the [!INCLUDE[prod_short](includes/prod_short.md)] client. Instant flows work similarly to batch shortcuts, performing multiple lengthy steps with a few button presses and are launched from specific pages or tables. For example, a flow can add a button to the action menu on the **Vendors** page to block payments to a vendor and, at the same time, send customisable emails to the vendor's contact and your company's purchasers as well as update the contact in Outlook. |

## <a name="power-automate-features"></a>Power Automate features

You can explore all Power Automate flows currently available to you by signing in to [Power Automate](https://powerautomate.com) and selecting **My flows** from the navigation bar on the left. Here you find any flows you have already created yourself and flows shared with you by an admin or coworker.

- Instant flows are also made available for running directly from most list, card, and document pages in [!INCLUDE[prod_short](includes/prod_short.md)]. You find the instant flows in the **Automate** action group in the action bar of pages. To run a flow, select it, and follow the instructions presented to you. Learn more in the sections that follow.

- With automated flows in [!INCLUDE[prod_short](includes/prod_short.md)], there's nothing for you to do, unless you want to change them, or turn them off. Otherwise, they just work when triggered. 
<!--

## <a name="automated-flows"></a>Automated flows

With Power Automate, you can create business flows directly in-house and rely on citizen developers. Automated workflows can be started by both internal and external events in [!INCLUDE[prod_short](includes/prod_short.md)], and also be set to run periodically. Learn more and get instructions on how to create flows in the [Set Up Automated Workflows](/dynamics365/business-central/dev-itpro/powerplatform/automate-workflows) article in the administration content.

-->

## <a name="run-instant-flows"></a>Run instant flows

Instant flows open inside [!INCLUDE [prod_short](includes/prod_short.md)] online so you can remain within the context of the business process you were in the middle of doing. You can run an instant flow from most lists, cards, or documents.

1. In the action bar, select **Automate**, then choose a flow from the list of available flows under the **Power Automate** action.

    :::image type="content" source="media/power-automate-instant-menu.svg" alt-text="Shows the Automate action with instant flow actions.":::

    On some pages, **Automate** is nested under **More options (...)**. 
2. In the **Run Flow** pane, fill in any required fields, then select **Continue** to run the flow.

> [!NOTE]
> The first time you use the **Automate** item, you may see only the **Get started with Power Automate** action. You see this action because you haven't agreed to the privacy notice for Microsoft Power Automate. To continue, select **Get started with Power Automate** and follow the instructions to agree or disagree.  
>
> :::image type="content" source="media/power-automate-action.png" alt-text="Shows the Automate item in the action bar.":::

<!--

[!INCLUDE [prod_short](includes/prod_short.md)] can run a Power Automate flow from most list, card, and document pages. Once the admin has connected [!INCLUDE [prod_short](includes/prod_short.md)] with Power Automate, you'll see any flows your organization has added when you choose the **Automate** action on the relevant pages. Instant flows are run without leaving [!INCLUDE [prod_short](includes/prod_short.md)]. Learn more in the [Set Up Automated Workflows](/dynamics365/business-central/dev-itpro/powerplatform/automate-workflows) article in the administration content.

These instant flows open on a page inside [!INCLUDE [prod_short](includes/prod_short.md)] online so you can remain within the context of the business process you were in the middle of. Choose the **Automate** action—on some pages nested under the **More Options** menu—choose the **Power Automate** menu item, then choose the relevant link to trigger the workflow. The connection to Power Automate is already set up for you.

Most flows require you to fill in a field or two before you choose the **Run flow** action.

> [!TIP]
> If you don't see an **Automate** action, then your [!INCLUDE [prod_short](includes/prod_short.md)] probably hasn't yet been set up to use Power Automate. Learn more from your admin.-->

## <a name="create-edit-and-manage-flows"></a>Create, edit, and manage flows

Creating new flows or modifying and managing existing ones (like turning them on or off) can be done directly in Power Automate. But you can initiate some of these tasks from the Automate action menu in  [!INCLUDE[prod_short](includes/prod_short.md)]:

:::image type="content" source="media/power-automate-menu.svg" alt-text="Shows the Automate action in the action bar with expanded actions.":::

- To create an automated flow from a list, card, or document page, select **Automate** > **Create automated flow**.
- To create an approval workflow from a card or document page, select **Automate** > **Create approval flow**.

  > [!TIP]
  > This action is only available on card and document type pages; not lists.
- To create an instant flow from a list, card, or document page, select **Automate** > **Create action based on a flow**.
- To open Power Automate from a list, card, or document page, select **Automate** > **Manage flows**.
<!--- To create new flows or manage existing flows from inside [!INCLUDE[prod_short](includes/prod_short.md)], got to the **Manage Power Automate Flows** page.-->

These tasks are typically done by an admin or super user. The tasks require a broader knowledge of the business processes in [!INCLUDE[prod_short](includes/prod_short.md)]. To learn more, go to the following articles in the Business Central Dev and IT Pro help:

- [Power Automate integration](/dynamics365/business-central/dev-itpro/powerplatform/power-automate-overview)
- [Create automated flows](/dynamics365/business-central/dev-itpro/powerplatform/instant-flows) (also covers approval flows)
- [Create instant flows](/dynamics365/business-central/dev-itpro/powerplatform/instant-flows)
- [Manage Power Automate flows](/dynamics365/business-central/dev-itpro/powerplatform/manage-power-automate-flows)
<!-- 

## <a name="add-more-automated-flows-and-instant-flows"></a>Add more automated flows and instant flows

You can create flows through the [powerautomate.microsoft.com](https://powerautomate.microsoft.com) website. However, if your admin has switched on the capability to run Power Automate flows from inside [!INCLUDE [prod_short](includes/prod_short.md)] online, you can start the process of building a flow from the **Automate** action on the relevant pages, which can be found under the **More Options** menu depending on the page. Then choose the **Power Automate** menu item, and then choose the **Create a flow** action. Power Automate then opens in a new browser tab, and you're signed in automatically.

You can find sample templates to adapt to your company and all available trigger events, using both [!INCLUDE [prod_short](includes/prod_short.md)] and external tools, by choosing the **Connectors** menu on the Power Automate website. Learn more about available templates and triggers in the [Set Up Automated Workflows](/dynamics365/business-central/dev-itpro/powerplatform/automate-workflows) article in the administration content.

## <a name="create-and-manage-power-automate-flows"></a>Create and manage Power Automate flows

You can create new flows or manage existing Power Automate flows in [!INCLUDE [prod_short](includes/prod_short.md)] on the **Manage Power Automate Flows** page. Learn more in the [Manage Power Automate Flows](/dynamics365/business-central/dev-itpro/powerplatform/manage-power-automate-flows) article in the administration content.

<!--
You can also manage available Power Automate workflows on the **Workflows** page in [!INCLUDE[prod_short](includes/prod_short.md)]. The page lists both the built-in approval and Power Automate workflows, with options for the latter to enable/disable, delete, and view the workflow on the Power Automate website.-->

## <a name="see-also"></a>See also

[Troubleshoot Your [!INCLUDE[prod_short](includes/prod_short.md)] Automated Workflows](across-flow-troubleshoot.md)  
[Get Ready for Doing Business](ui-get-ready-business.md)  
[Workflows](across-workflow.md)  
[Import Business Data from Other Finance Systems](across-import-data-configuration-packages.md)  
[Assign Permissions to Users and Groups](ui-define-granular-permissions.md)  
[Set Up [!INCLUDE[prod_short](includes/prod_short.md)]](setup.md)  
[Financial Management](finance.md)  
[Manage Power Automate Flows](/dynamics365/business-central/dev-itpro/powerplatform/manage-power-automate-flows)  
[Set Up Automated Workflows](/dynamics365/business-central/dev-itpro/powerplatform/automate-workflows)  
[Switch on Instant Flows](/dynamics365/business-central/dev-itpro/powerplatform/instant-flows)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
