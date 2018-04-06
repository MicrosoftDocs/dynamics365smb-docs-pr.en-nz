---
title: Workflow | Microsoft Docs
description: You can set up and use workflows that connect business-process tasks performed by different users. System tasks, such as automatic posting, can be included as steps in workflows, preceded or followed by user tasks. Requesting and granting approval to create new records are typical workflow steps.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 02/20/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 06783cab93ae83111b9646de7c8577fb0669d466
ms.contentlocale: en-nz
ms.lasthandoff: 03/22/2018

---
# <a name="workflow"></a><span data-ttu-id="b9f65-105">Workflow</span><span class="sxs-lookup"><span data-stu-id="b9f65-105">Workflow</span></span>
<span data-ttu-id="b9f65-106">You can set up and use workflows that connect business-process tasks performed by different users.</span><span class="sxs-lookup"><span data-stu-id="b9f65-106">You can set up and use workflows that connect business-process tasks performed by different users.</span></span> <span data-ttu-id="b9f65-107">System tasks, such as automatic posting, can be included as steps in workflows, preceded or followed by user tasks.</span><span class="sxs-lookup"><span data-stu-id="b9f65-107">System tasks, such as automatic posting, can be included as steps in workflows, preceded or followed by user tasks.</span></span> <span data-ttu-id="b9f65-108">Requesting and granting approval to create new records are typical workflow steps.</span><span class="sxs-lookup"><span data-stu-id="b9f65-108">Requesting and granting approval to create new records are typical workflow steps.</span></span>  

 <span data-ttu-id="b9f65-109">In the **Workflow** window, you create a workflow by listing the involved steps on the lines.</span><span class="sxs-lookup"><span data-stu-id="b9f65-109">In the **Workflow** window, you create a workflow by listing the involved steps on the lines.</span></span> <span data-ttu-id="b9f65-110">Each step consists of a workflow event, moderated by event conditions, and a workflow response, moderated by response options.</span><span class="sxs-lookup"><span data-stu-id="b9f65-110">Each step consists of a workflow event, moderated by event conditions, and a workflow response, moderated by response options.</span></span> <span data-ttu-id="b9f65-111">You define workflow steps by filling fields on workflow lines from fixed lists of event and response values representing scenarios that are supported by the application code.</span><span class="sxs-lookup"><span data-stu-id="b9f65-111">You define workflow steps by filling fields on workflow lines from fixed lists of event and response values representing scenarios that are supported by the application code.</span></span>  

 <span data-ttu-id="b9f65-112">The generic version of [!INCLUDE[d365fin](includes/d365fin_md.md)] includes a number of preconfigured workflows represented by workflow templates that you can copy to create workflows.</span><span class="sxs-lookup"><span data-stu-id="b9f65-112">The generic version of [!INCLUDE[d365fin](includes/d365fin_md.md)] includes a number of preconfigured workflows represented by workflow templates that you can copy to create workflows.</span></span> <span data-ttu-id="b9f65-113">The code for workflow templates that are added by Microsoft are prefixed with “MS-“.</span><span class="sxs-lookup"><span data-stu-id="b9f65-113">The code for workflow templates that are added by Microsoft are prefixed with “MS-“.</span></span> <span data-ttu-id="b9f65-114">For more information, see the list of workflow templates in the Workflow Templates window.</span><span class="sxs-lookup"><span data-stu-id="b9f65-114">For more information, see the list of workflow templates in the Workflow Templates window.</span></span>  

 <span data-ttu-id="b9f65-115">If a business scenario requires a workflow event or response that is not supported, a Microsoft partner must implement them by customising the application code.</span><span class="sxs-lookup"><span data-stu-id="b9f65-115">If a business scenario requires a workflow event or response that is not supported, a Microsoft partner must implement them by customizing the application code.</span></span> <span data-ttu-id="b9f65-116">For more information, see [Walkthrough: Implementing New Workflow Events and Responses](/dynamics-nav/Walkthrough--Implementing-New-Workflow-Events-and-Responses) in the developer and IT-pro help.</span><span class="sxs-lookup"><span data-stu-id="b9f65-116">For more information, see [Walkthrough: Implementing New Workflow Events and Responses](/dynamics-nav/Walkthrough--Implementing-New-Workflow-Events-and-Responses) in the developer and IT-pro help.</span></span>  

 <span data-ttu-id="b9f65-117">The following table describes a sequence of tasks, with links to the topics that describe them.</span><span class="sxs-lookup"><span data-stu-id="b9f65-117">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>  

|<span data-ttu-id="b9f65-118">**To**</span><span class="sxs-lookup"><span data-stu-id="b9f65-118">**To**</span></span>|<span data-ttu-id="b9f65-119">**See**</span><span class="sxs-lookup"><span data-stu-id="b9f65-119">**See**</span></span>|  
|------------|-------------|  
|<span data-ttu-id="b9f65-120">Set up workflow users, specify how users get notified, and create new workflows.</span><span class="sxs-lookup"><span data-stu-id="b9f65-120">Set up workflow users, specify how users get notified, and create new workflows.</span></span> <span data-ttu-id="b9f65-121">For new workflows for unsupported scenarios, implement the required workflow elements by customising the application code.</span><span class="sxs-lookup"><span data-stu-id="b9f65-121">For new workflows for unsupported scenarios, implement the required workflow elements by customizing the application code.</span></span>|[<span data-ttu-id="b9f65-122">Setting Up Workflows</span><span class="sxs-lookup"><span data-stu-id="b9f65-122">Setting Up Workflows</span></span>](across-set-up-workflows.md)|  
|<span data-ttu-id="b9f65-123">Enable workflows, act on workflow notifications, including request approvals and approve requests to perform a workflow step.</span><span class="sxs-lookup"><span data-stu-id="b9f65-123">Enable workflows, act on workflow notifications, including request approvals and approve requests to perform a workflow step.</span></span> <span data-ttu-id="b9f65-124">Archive and delete workflows.</span><span class="sxs-lookup"><span data-stu-id="b9f65-124">Archive and delete workflows.</span></span>|[<span data-ttu-id="b9f65-125">Using Workflows</span><span class="sxs-lookup"><span data-stu-id="b9f65-125">Using Workflows</span></span>](across-use-workflows.md)|  

## <a name="see-also"></a><span data-ttu-id="b9f65-126">See Also</span><span class="sxs-lookup"><span data-stu-id="b9f65-126">See Also</span></span>  
[<span data-ttu-id="b9f65-127">Sales</span><span class="sxs-lookup"><span data-stu-id="b9f65-127">Sales</span></span>](sales-manage-sales.md)  
[<span data-ttu-id="b9f65-128">Purchasing</span><span class="sxs-lookup"><span data-stu-id="b9f65-128">Purchasing</span></span>](purchasing-manage-purchasing.md)  
[<span data-ttu-id="b9f65-129">Managing Projects</span><span class="sxs-lookup"><span data-stu-id="b9f65-129">Managing Projects</span></span>](projects-manage-projects.md)  
<span data-ttu-id="b9f65-130">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="b9f65-130">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

