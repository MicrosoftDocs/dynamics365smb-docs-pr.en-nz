---
title: How to Export and Import Workflows | Microsoft Docs
description: To transfer workflows to other Finance and Operations, Business edition databases, for example to save time when creating new workflows, you can export and import workflows.
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: 6da772f9eefab9aa0ef8b9f47f6ea7656ebef1b4
ms.contentlocale: en-nz
ms.lasthandoff: 03/22/2018

---
# <a name="export-and-import-workflows"></a>Export and Import Workflows
To transfer workflows to other [!INCLUDE[d365fin](includes/d365fin_md.md)] databases, for example to save time when creating new workflows, you can export and import workflows.  

 Another way to quickly create workflows is to create workflows from workflow templates. For more information, see [Create Workflows from Workflow Templates](across-how-to-create-workflows-from-workflow-templates.md).  

 In the **Workflow** window, you create a workflow by listing the involved steps on the lines. Each step consists of a workflow event, moderated by event conditions, and a workflow response, moderated by response options. You define workflow steps by filling fields on workflow lines from fixed lists of event and response values representing scenarios that are supported by the application code. For more information, see [Create Workflows](across-how-to-create-workflows.md).  

## <a name="to-export-a-workflow"></a>To export a workflow  
1.  Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Workflows**, and then choose the related link.  
2.  Select a workflow, and then choose the **Export to File** action.  
3.  In the **Export File** window, choose the **Save** button.  
4.  In the **Export** window, select a file location, and then choose the **Save** button.  

## <a name="to-import-a-workflow"></a>To import a workflow  
1.  Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Workflows**, and then choose the related link.  
2.  Choose the **Import from File** action.  
3.  In the **Import** window, choose the XML file that contains the workflow, and then choose the **Open** button.  

> [!CAUTION]  
>  If the workflow code already exists in the database, the workflow steps will be overwritten with the steps in the imported workflow.  

## <a name="see-also"></a>See Also  
 [Create Workflows](across-how-to-create-workflows.md)   
 [Create Workflows from Workflow Templates](across-how-to-create-workflows-from-workflow-templates.md)   
 [View Archived Workflow Step Instances](across-how-to-view-archived-workflow-step-instances.md)   
 [Delete Workflows](across-how-to-delete-workflows.md)   
 [Walkthrough: Setting Up and Using a Purchase Approval Workflow](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md)   
 [Setting Up Workflows](across-set-up-workflows.md)   
 [Using Workflows](across-use-workflows.md)   
 [Workflow](across-workflow.md)   

