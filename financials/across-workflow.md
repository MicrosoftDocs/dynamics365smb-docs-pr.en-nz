---
title: Workflow | Microsoft Docs
description: You can set up and use workflows that connect business-process tasks performed by different users. System tasks, such as automatic posting, can be included as steps in workflows, preceded or followed by user tasks. Requesting and granting approval to create new records are typical workflow steps.
services: project-madeira
documentationcenter: 
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
ms.sourcegitcommit: a49e50213f808fb72b43dfa22a34833b306ef12d
ms.openlocfilehash: 58f2aa5a26275820d0fafcc79fec5be118857d78
ms.contentlocale: en-nz
ms.lasthandoff: 12/14/2017

---
# <a name="workflow"></a><span data-ttu-id="20028-105">Workflow</span><span class="sxs-lookup"><span data-stu-id="20028-105">Workflow</span></span>
<span data-ttu-id="20028-106">You can set up and use workflows that connect business-process tasks performed by different users.</span><span class="sxs-lookup"><span data-stu-id="20028-106">You can set up and use workflows that connect business-process tasks performed by different users.</span></span> <span data-ttu-id="20028-107">System tasks, such as automatic posting, can be included as steps in workflows, preceded or followed by user tasks.</span><span class="sxs-lookup"><span data-stu-id="20028-107">System tasks, such as automatic posting, can be included as steps in workflows, preceded or followed by user tasks.</span></span> <span data-ttu-id="20028-108">Requesting and granting approval to create new records are typical workflow steps.</span><span class="sxs-lookup"><span data-stu-id="20028-108">Requesting and granting approval to create new records are typical workflow steps.</span></span>  

 <span data-ttu-id="20028-109">In the **Workflow** window, you create a workflow by listing the involved steps on the lines.</span><span class="sxs-lookup"><span data-stu-id="20028-109">In the **Workflow** window, you create a workflow by listing the involved steps on the lines.</span></span> <span data-ttu-id="20028-110">Each step consists of a workflow event, moderated by event conditions, and a workflow response, moderated by response options.</span><span class="sxs-lookup"><span data-stu-id="20028-110">Each step consists of a workflow event, moderated by event conditions, and a workflow response, moderated by response options.</span></span> <span data-ttu-id="20028-111">You define workflow steps by filling fields on workflow lines from fixed lists of event and response values representing scenarios that are supported by the application code.</span><span class="sxs-lookup"><span data-stu-id="20028-111">You define workflow steps by filling fields on workflow lines from fixed lists of event and response values representing scenarios that are supported by the application code.</span></span>  

 <span data-ttu-id="20028-112">The generic version of [!INCLUDE[d365fin](includes/d365fin_md.md)] includes a number of preconfigured workflows represented by workflow templates that you can copy to create workflows.</span><span class="sxs-lookup"><span data-stu-id="20028-112">The generic version of [!INCLUDE[d365fin](includes/d365fin_md.md)] includes a number of preconfigured workflows represented by workflow templates that you can copy to create workflows.</span></span> <span data-ttu-id="20028-113">The code for workflow templates that are added by Microsoft are prefixed with “MS-“.</span><span class="sxs-lookup"><span data-stu-id="20028-113">The code for workflow templates that are added by Microsoft are prefixed with “MS-“.</span></span> <span data-ttu-id="20028-114">For more information, see the list of workflow templates in the Workflow Templates window.</span><span class="sxs-lookup"><span data-stu-id="20028-114">For more information, see the list of workflow templates in the Workflow Templates window.</span></span>  

 <span data-ttu-id="20028-115">If a business scenario requires a workflow event or response that is not supported, a Microsoft partner must implement them by customising the application code.</span><span class="sxs-lookup"><span data-stu-id="20028-115">If a business scenario requires a workflow event or response that is not supported, a Microsoft partner must implement them by customizing the application code.</span></span> <span data-ttu-id="20028-116">For more information, see [Walkthrough: Implementing New Workflow Events and Responses](/dynamics_nav/Walkthrough--Implementing-New-Workflow-Events-and-Responses) in the developer and IT-pro help.</span><span class="sxs-lookup"><span data-stu-id="20028-116">For more information, see [Walkthrough: Implementing New Workflow Events and Responses](/dynamics_nav/Walkthrough--Implementing-New-Workflow-Events-and-Responses) in the developer and IT-pro help.</span></span>  

 <span data-ttu-id="20028-117">The following table describes a sequence of tasks, with links to the topics that describe them.</span><span class="sxs-lookup"><span data-stu-id="20028-117">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>  

|<span data-ttu-id="20028-118">**To**</span><span class="sxs-lookup"><span data-stu-id="20028-118">**To**</span></span>|<span data-ttu-id="20028-119">**See**</span><span class="sxs-lookup"><span data-stu-id="20028-119">**See**</span></span>|  
|------------|-------------|  
|<span data-ttu-id="20028-120">Set up workflow users, specify how users get notified, and create new workflows.</span><span class="sxs-lookup"><span data-stu-id="20028-120">Set up workflow users, specify how users get notified, and create new workflows.</span></span> <span data-ttu-id="20028-121">For new workflows for unsupported scenarios, implement the required workflow elements by customising the application code.</span><span class="sxs-lookup"><span data-stu-id="20028-121">For new workflows for unsupported scenarios, implement the required workflow elements by customizing the application code.</span></span>|[<span data-ttu-id="20028-122">Setting Up Workflows</span><span class="sxs-lookup"><span data-stu-id="20028-122">Setting Up Workflows</span></span>](across-set-up-workflows.md)|  
|<span data-ttu-id="20028-123">Enable workflows, act on workflow notifications, including request approvals and approve requests to perform a workflow step.</span><span class="sxs-lookup"><span data-stu-id="20028-123">Enable workflows, act on workflow notifications, including request approvals and approve requests to perform a workflow step.</span></span> <span data-ttu-id="20028-124">Archive and delete workflows.</span><span class="sxs-lookup"><span data-stu-id="20028-124">Archive and delete workflows.</span></span>|[<span data-ttu-id="20028-125">Using Workflows</span><span class="sxs-lookup"><span data-stu-id="20028-125">Using Workflows</span></span>](across-use-workflows.md)|  

## <a name="see-also"></a><span data-ttu-id="20028-126">See Also</span><span class="sxs-lookup"><span data-stu-id="20028-126">See Also</span></span>  
[<span data-ttu-id="20028-127">Sales</span><span class="sxs-lookup"><span data-stu-id="20028-127">Sales</span></span>](sales-manage-sales.md)  
[<span data-ttu-id="20028-128">Purchasing</span><span class="sxs-lookup"><span data-stu-id="20028-128">Purchasing</span></span>](purchasing-manage-purchasing.md)  
[<span data-ttu-id="20028-129">Managing Projects</span><span class="sxs-lookup"><span data-stu-id="20028-129">Managing Projects</span></span>](projects-manage-projects.md)  
<span data-ttu-id="20028-130">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="20028-130">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

