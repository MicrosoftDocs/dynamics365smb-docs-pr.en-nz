---
title: How to Create Workflows from Workflow Templates
description: To save time when creating new workflows, you can create non-editable workflows from workflow templates prefixed with "MS".
author: SorenGP
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 06/11/2021
ms.author: edupont
ms.openlocfilehash: 18a9d4ba7e2865e41d660261a598b1b755c68023
ms.sourcegitcommit: f1e272485a0e675d337a694aba3e35a5daf43920
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 07/09/2022
ms.locfileid: "9129739"
---
# <a name="create-workflows-from-workflow-templates"></a>Create Workflows from Workflow Templates

To save time when creating new workflows, you can create workflows from workflow templates.  

Workflow templates are non-editable workflows that exist in the default version of [!INCLUDE[prod_short](includes/prod_short.md)]. The codes for workflow templates created by Microsoft are prefixed with "MS-".  

Another way to quickly create a workflow is to import an existing workflow that you have on a file outside of [!INCLUDE[prod_short](includes/prod_short.md)]. For more information, see [Export and Import Workflows](across-how-to-export-and-import-workflows.md).  

On the **Workflow** page, you create a workflow by listing the involved steps on the lines. Each step consists of a workflow event, moderated by event conditions, and a workflow response, moderated by response options. You define workflow steps by filling fields on workflow lines from fixed lists of event and response values representing scenarios that are supported by the application code. For more information, see [Create Workflows](across-how-to-create-workflows.md).  

## <a name="to-create-a-workflow-from-a-workflow-template"></a>To create a workflow from a workflow template

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Workflows**, and then choose the related link.  
2. Choose the **New Workflow from Template** action. The **Workflow Templates** page opens.  
3. Select a workflow template, and then choose the **OK** button.  

   The **Workflow** page opens for a new workflow containing all the information of the selected template. The value in the **Code** field is extended with, for example, "-01" to indicate that this is the first workflow that is created from the workflow template.  
4. Proceed to create the workflow by editing the workflow steps or add new steps. For more information, see [Create Workflows](across-how-to-create-workflows.md).  

## <a name="see-related-training-at-microsoft-learn"></a>See related training at [Microsoft Learn](/learn/modules/create-workflows/)

## <a name="see-also"></a>See also

[Create Workflows](across-how-to-create-workflows.md)  
[Export and Import Workflows](across-how-to-export-and-import-workflows.md)  
[View Archived Workflow Step Instances](across-how-to-view-archived-workflow-step-instances.md)  
[Delete Workflows](across-how-to-delete-workflows.md)  
[Walkthrough: Setting Up and Using a Purchase Approval Workflow](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md)  
[Setting Up Workflows](across-set-up-workflows.md)  
[Use Workflows](across-use-workflows.md)  
[Workflow](across-workflow.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]