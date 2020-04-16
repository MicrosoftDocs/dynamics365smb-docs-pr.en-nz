---
title: How to Create Workflows from Workflow Templates | Microsoft Docs
description: To save time when creating new workflows, you can create workflows from workflow templates.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2020
ms.author: sgroespe
ms.openlocfilehash: 6b4d09ae0bd0f2def940e2516bdc54bc04f300ca
ms.sourcegitcommit: 88e4b30eaf6fa32af0c1452ce2f85ff1111c75e2
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 04/01/2020
ms.locfileid: "3188412"
---
# <a name="create-workflows-from-workflow-templates"></a><span data-ttu-id="80686-103">Create Workflows from Workflow Templates</span><span class="sxs-lookup"><span data-stu-id="80686-103">Create Workflows from Workflow Templates</span></span>
<span data-ttu-id="80686-104">To save time when creating new workflows, you can create workflows from workflow templates.</span><span class="sxs-lookup"><span data-stu-id="80686-104">To save time when creating new workflows, you can create workflows from workflow templates.</span></span>  

 <span data-ttu-id="80686-105">Workflow templates are non-editable workflows that exist in the generic version of [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="80686-105">Workflow templates are non-editable workflows that exist in the generic version of [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="80686-106">The codes for workflow templates that are added by Microsoft are prefixed with “MS-“.</span><span class="sxs-lookup"><span data-stu-id="80686-106">The codes for workflow templates that are added by Microsoft are prefixed with “MS-“.</span></span>  

 <span data-ttu-id="80686-107">Another way to quickly create a workflow is to import an existing workflow that you have on a file outside of [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="80686-107">Another way to quickly create a workflow is to import an existing workflow that you have on a file outside of [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="80686-108">For more information, see [Export and Import Workflows](across-how-to-export-and-import-workflows.md).</span><span class="sxs-lookup"><span data-stu-id="80686-108">For more information, see [Export and Import Workflows](across-how-to-export-and-import-workflows.md).</span></span>  

<span data-ttu-id="80686-109">On the **Workflow** page, you create a workflow by listing the involved steps on the lines.</span><span class="sxs-lookup"><span data-stu-id="80686-109">On the **Workflow** page, you create a workflow by listing the involved steps on the lines.</span></span> <span data-ttu-id="80686-110">Each step consists of a workflow event, moderated by event conditions, and a workflow response, moderated by response options.</span><span class="sxs-lookup"><span data-stu-id="80686-110">Each step consists of a workflow event, moderated by event conditions, and a workflow response, moderated by response options.</span></span> <span data-ttu-id="80686-111">You define workflow steps by filling fields on workflow lines from fixed lists of event and response values representing scenarios that are supported by the application code.</span><span class="sxs-lookup"><span data-stu-id="80686-111">You define workflow steps by filling fields on workflow lines from fixed lists of event and response values representing scenarios that are supported by the application code.</span></span> <span data-ttu-id="80686-112">For more information, see [Create Workflows](across-how-to-create-workflows.md).</span><span class="sxs-lookup"><span data-stu-id="80686-112">For more information, see [Create Workflows](across-how-to-create-workflows.md).</span></span>  

## <a name="to-create-a-workflow-from-workflow-template"></a><span data-ttu-id="80686-113">To create a workflow from workflow template</span><span class="sxs-lookup"><span data-stu-id="80686-113">To create a workflow from workflow template</span></span>  
1.  <span data-ttu-id="80686-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Workflows**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="80686-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Workflows**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="80686-115">Choose the **Create Workflow from Template** action.</span><span class="sxs-lookup"><span data-stu-id="80686-115">Choose the **Create Workflow from Template** action.</span></span> <span data-ttu-id="80686-116">The **Workflow Templates** page opens.</span><span class="sxs-lookup"><span data-stu-id="80686-116">The **Workflow Templates** page opens.</span></span>  
3.  <span data-ttu-id="80686-117">Select a workflow template, and then choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="80686-117">Select a workflow template, and then choose the **OK** button.</span></span>  

     <span data-ttu-id="80686-118">The **Workflow** page opens for a new workflow containing all the information of the selected template.</span><span class="sxs-lookup"><span data-stu-id="80686-118">The **Workflow** page opens for a new workflow containing all the information of the selected template.</span></span> <span data-ttu-id="80686-119">The value in the **Code** field is extended with, for example, “-01” to indicate that this is the first workflow that is created from the workflow template.</span><span class="sxs-lookup"><span data-stu-id="80686-119">The value in the **Code** field is extended with, for example, “-01” to indicate that this is the first workflow that is created from the workflow template.</span></span>  
4.  <span data-ttu-id="80686-120">Proceed to create the workflow by editing the workflow steps or add new steps.</span><span class="sxs-lookup"><span data-stu-id="80686-120">Proceed to create the workflow by editing the workflow steps or add new steps.</span></span> <span data-ttu-id="80686-121">For more information, see [Create Workflows](across-how-to-create-workflows.md).</span><span class="sxs-lookup"><span data-stu-id="80686-121">For more information, see [Create Workflows](across-how-to-create-workflows.md).</span></span>  

## <a name="see-also"></a><span data-ttu-id="80686-122">See Also</span><span class="sxs-lookup"><span data-stu-id="80686-122">See Also</span></span>  
 <span data-ttu-id="80686-123">[Create Workflows](across-how-to-create-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="80686-123">[Create Workflows](across-how-to-create-workflows.md) </span></span>  
 <span data-ttu-id="80686-124">[Export and Import Workflows](across-how-to-export-and-import-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="80686-124">[Export and Import Workflows](across-how-to-export-and-import-workflows.md) </span></span>  
 <span data-ttu-id="80686-125">[View Archived Workflow Step Instances](across-how-to-view-archived-workflow-step-instances.md) </span><span class="sxs-lookup"><span data-stu-id="80686-125">[View Archived Workflow Step Instances](across-how-to-view-archived-workflow-step-instances.md) </span></span>  
 <span data-ttu-id="80686-126">[Delete Workflows](across-how-to-delete-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="80686-126">[Delete Workflows](across-how-to-delete-workflows.md) </span></span>  
 <span data-ttu-id="80686-127">[Walkthrough: Setting Up and Using a Purchase Approval Workflow](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md) </span><span class="sxs-lookup"><span data-stu-id="80686-127">[Walkthrough: Setting Up and Using a Purchase Approval Workflow](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md) </span></span>  
 <span data-ttu-id="80686-128">[Setting Up Workflows](across-set-up-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="80686-128">[Setting Up Workflows](across-set-up-workflows.md) </span></span>  
 <span data-ttu-id="80686-129">[Using Workflows](across-use-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="80686-129">[Using Workflows](across-use-workflows.md) </span></span>  
 [<span data-ttu-id="80686-130">Workflow</span><span class="sxs-lookup"><span data-stu-id="80686-130">Workflow</span></span>](across-workflow.md)   
