---
title: How to Restrict and Allow Usage of a Record
description: 'If you want to restrict a record from being used, you can incorporate two workflow responses in a workflow that controls the usage of the record.'
author: SorenGP
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: null
ms.date: 09/08/2022
ms.author: edupont
---
# <a name="restrict-and-allow-usage-of-a-record"></a>Restrict and Allow Usage of a Record

If you want to restrict a record from being used in certain activities, for example, until the record has been approved, you can incorporate two workflow responses in the workflow that controls usage of the record. One workflow response restricts usage of the record as defined by the workflow event and conditions. The other workflow response allows usage of the record as defined by the workflow event and conditions. Two responses exist in the default version of [!INCLUDE[prod_short](includes/prod_short.md)] for this purpose: **Add record restriction** and **Remove record restriction**.

> [!NOTE]  
> The default version of [!INCLUDE[prod_short](includes/prod_short.md)] offers support for restricting a record from being posted, from being exported as a payment, and from being printed as a cheque. To support other restrictions, a Microsoft partner must customise the application code.  

> [!NOTE]  
> The workflow functionality to restrict and allow records from being used is not related to the functionality to block item, customer, and vendor records from being posted.

The following procedure describes how to restrict purchase orders from being posted until they've been approved. The new workflow will be based on the existing *Purchase Invoice Approval Workflow* template.  

## <a name="create-a-workflow-step-that-restricts-posting-of-unapproved-purchase-orders"></a>Create a workflow step that restricts posting of unapproved purchase orders

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Workflows**, then choose the related link.  
2. On the **Workflows** page, choose the **New Workflow from Template** action. Learn more at [Create Workflows from Workflow Templates](across-how-to-create-workflows-from-workflow-templates.md).
3. On the **Workflow Templates** page, choose the *Purchase Invoice Approval Workflow* template.  

   Note that the first two workflow steps are about restricting and then allowing usage of purchase invoices. Change the event condition on the first step of the new workflow to specify that it applies to purchase orders.  
4. On the **Workflow Steps** FastTab, choose the **On Condition** field for the first step, then, for the **Document Type** filter, select **Order**.  
5. Proceed to edit, delete, or add other workflow steps to reflect a business process that begins by restricting unapproved purchase orders from being posted.  

## <a name="see-also"></a>See also

[Use Approval Workflows](across-use-workflows.md)  
[Create Approval Workflows](across-how-to-create-workflows.md)  
[Workflow](across-workflow.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
