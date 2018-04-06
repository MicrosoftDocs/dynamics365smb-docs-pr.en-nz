---
title: Connect Your Data with Flow| Microsoft Docs
description: You can make your Financials data available as a data source and specify an OData URL of your web services to build an automated workflow.
documentationcenter: 
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: workflow, Odata, Power App, SOAP
ms.date: 01/25/2018
ms.author: solsen
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 23e9ebbb75d23595d568d022526e551bf590a979
ms.contentlocale: en-nz
ms.lasthandoff: 03/22/2018

---
# <a name="using-included365finincludesd365finmdmd-in-an-automated-workflow"></a><span data-ttu-id="ce03e-103">Using [!INCLUDE[d365fin](includes/d365fin_md.md)] in an Automated Workflow</span><span class="sxs-lookup"><span data-stu-id="ce03e-103">Using [!INCLUDE[d365fin](includes/d365fin_md.md)] in an Automated Workflow</span></span>
<span data-ttu-id="ce03e-104">You can use your [!INCLUDE[d365fin](includes/d365fin_md.md)] data as part of a workflow in Microsoft Flow.</span><span class="sxs-lookup"><span data-stu-id="ce03e-104">You can use your [!INCLUDE[d365fin](includes/d365fin_md.md)] data as part of a workflow in Microsoft Flow.</span></span>  

> [!NOTE]  
>   <span data-ttu-id="ce03e-105">You must have a valid account with [!INCLUDE[d365fin](includes/d365fin_md.md)] and with Flow.</span><span class="sxs-lookup"><span data-stu-id="ce03e-105">You must have a valid account with [!INCLUDE[d365fin](includes/d365fin_md.md)] and with Flow.</span></span>  

## <a name="to-add-included365finincludesd365finmdmd-as-a-data-source-in-flow"></a><span data-ttu-id="ce03e-106">To add [!INCLUDE[d365fin](includes/d365fin_md.md)] as a data source in Flow</span><span class="sxs-lookup"><span data-stu-id="ce03e-106">To add [!INCLUDE[d365fin](includes/d365fin_md.md)] as a data source in Flow</span></span>
1. <span data-ttu-id="ce03e-107">In your browser, navigate to [flow.microsoft.com](https://flow.microsoft.com/en-us/), and then sign in.</span><span class="sxs-lookup"><span data-stu-id="ce03e-107">In your browser, navigate to [flow.microsoft.com](https://flow.microsoft.com/en-us/), and then sign in.</span></span>
2. <span data-ttu-id="ce03e-108">Choose **My Flows** from the ribbon at the top of the page.</span><span class="sxs-lookup"><span data-stu-id="ce03e-108">Choose **My Flows** from the ribbon at the top of the page.</span></span>
3. <span data-ttu-id="ce03e-109">In the **My Flows** window, choose the **Create from blank** option.</span><span class="sxs-lookup"><span data-stu-id="ce03e-109">In the **My Flows** window, choose the **Create from blank** option.</span></span>
4. <span data-ttu-id="ce03e-110">From the list of available triggers, select one of the [!INCLUDE[d365fin](includes/d365fin_md.md)] triggers available:</span><span class="sxs-lookup"><span data-stu-id="ce03e-110">From the list of available triggers, select one of the [!INCLUDE[d365fin](includes/d365fin_md.md)] triggers available:</span></span>  
    <span data-ttu-id="ce03e-111">*When a customer approval is requested*,</span><span class="sxs-lookup"><span data-stu-id="ce03e-111">*When a customer approval is requested*,</span></span>  
    <span data-ttu-id="ce03e-112">*When a general journal batch approval is requested*,</span><span class="sxs-lookup"><span data-stu-id="ce03e-112">*When a general journal batch approval is requested*,</span></span>  
    <span data-ttu-id="ce03e-113">*When a general journal line approval is requested*,</span><span class="sxs-lookup"><span data-stu-id="ce03e-113">*When a general journal line approval is requested*,</span></span>  
    <span data-ttu-id="ce03e-114">*When an item approval is requested*,</span><span class="sxs-lookup"><span data-stu-id="ce03e-114">*When an item approval is requested*,</span></span>  
    <span data-ttu-id="ce03e-115">*When a purchase document approval is requested*,</span><span class="sxs-lookup"><span data-stu-id="ce03e-115">*When a purchase document approval is requested*,</span></span>  
    <span data-ttu-id="ce03e-116">*When a sales document approval is requested*, or</span><span class="sxs-lookup"><span data-stu-id="ce03e-116">*When a sales document approval is requested*, or</span></span>  
    <span data-ttu-id="ce03e-117">*When a vendor aproval is requested*.</span><span class="sxs-lookup"><span data-stu-id="ce03e-117">*When a vendor aproval is requested*.</span></span>
5. <span data-ttu-id="ce03e-118">Flow will prompt you to select a company within your [!INCLUDE[d365fin](includes/d365fin_md.md)] tenant.</span><span class="sxs-lookup"><span data-stu-id="ce03e-118">Flow will prompt you to select a company within your [!INCLUDE[d365fin](includes/d365fin_md.md)] tenant.</span></span> <span data-ttu-id="ce03e-119">Because each step in the Flow is independent of the next, you may be required to define the company multiple times when using a [!INCLUDE[d365fin](includes/d365fin_md.md)] template.</span><span class="sxs-lookup"><span data-stu-id="ce03e-119">Because each step in the Flow is independent of the next, you may be required to define the company multiple times when using a [!INCLUDE[d365fin](includes/d365fin_md.md)] template.</span></span>

<span data-ttu-id="ce03e-120">At this point, you have successfully connected to your Business Central data and are ready to begin building your flow.</span><span class="sxs-lookup"><span data-stu-id="ce03e-120">At this point, you have successfully connected to your Business Central data and are ready to begin building your flow.</span></span> <span data-ttu-id="ce03e-121">For more information, see the [Flow documentation](https://flow.microsoft.com/documentation/getting-started/).</span><span class="sxs-lookup"><span data-stu-id="ce03e-121">For more information, see the [Flow documentation](https://flow.microsoft.com/documentation/getting-started/).</span></span>

<span data-ttu-id="ce03e-122">For troubleshooting your Microsoft Flow, see [Troubleshooting Integration with Microsoft Flow](across-troubleshooting-how-use-financials-data-source-flow.md).</span><span class="sxs-lookup"><span data-stu-id="ce03e-122">For troubleshooting your Microsoft Flow, see [Troubleshooting Integration with Microsoft Flow](across-troubleshooting-how-use-financials-data-source-flow.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="ce03e-123">See Also</span><span class="sxs-lookup"><span data-stu-id="ce03e-123">See Also</span></span>
<span data-ttu-id="ce03e-124">[Welcome to [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)</span><span class="sxs-lookup"><span data-stu-id="ce03e-124">[Welcome to [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)</span></span>  
[<span data-ttu-id="ce03e-125">Importing Business Data from Other Finance Systems</span><span class="sxs-lookup"><span data-stu-id="ce03e-125">Importing Business Data from Other Finance Systems</span></span>](upload-data.md)  
<span data-ttu-id="ce03e-126">[Manage Users and Permissions](ui-how-users-permissions.md)  </span><span class="sxs-lookup"><span data-stu-id="ce03e-126">[Manage Users and Permissions](ui-how-users-permissions.md)  </span></span>  
<span data-ttu-id="ce03e-127">[Setting Up [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)</span><span class="sxs-lookup"><span data-stu-id="ce03e-127">[Setting Up [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)</span></span>  
[<span data-ttu-id="ce03e-128">Finance</span><span class="sxs-lookup"><span data-stu-id="ce03e-128">Finance</span></span>](finance.md)  
