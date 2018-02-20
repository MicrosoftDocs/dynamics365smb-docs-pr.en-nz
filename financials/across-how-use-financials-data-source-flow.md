---
title: Connect Your Data with Flow| Microsoft Docs
description: You can make your Financials data available as a data source and specify an OData URL of your web services to build an automated workflow.
documentationcenter: 
author: edupont04
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: workflow, Odata, Power App, SOAP
ms.date: 01/25/2018
ms.author: solsen
ms.translationtype: HT
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: ef4d841723b6bb0af37695a8c3ed1d805319be78
ms.contentlocale: en-nz
ms.lasthandoff: 01/30/2018

---
# <a name="using-included365finincludesd365finmdmd-in-an-automated-workflow"></a><span data-ttu-id="59491-103">Using [!INCLUDE[d365fin](includes/d365fin_md.md)] in an Automated Workflow</span><span class="sxs-lookup"><span data-stu-id="59491-103">Using [!INCLUDE[d365fin](includes/d365fin_md.md)] in an Automated Workflow</span></span>
<span data-ttu-id="59491-104">You can use your [!INCLUDE[d365fin](includes/d365fin_md.md)] data as part of a workflow in Microsoft Flow.</span><span class="sxs-lookup"><span data-stu-id="59491-104">You can use your [!INCLUDE[d365fin](includes/d365fin_md.md)] data as part of a workflow in Microsoft Flow.</span></span>  

> [!NOTE]  
>   <span data-ttu-id="59491-105">You must have a valid account with [!INCLUDE[d365fin](includes/d365fin_md.md)] and with Flow.</span><span class="sxs-lookup"><span data-stu-id="59491-105">You must have a valid account with [!INCLUDE[d365fin](includes/d365fin_md.md)] and with Flow.</span></span>  

## <a name="to-add-included365finincludesd365finmdmd-as-a-data-source-in-flow"></a><span data-ttu-id="59491-106">To add [!INCLUDE[d365fin](includes/d365fin_md.md)] as a data source in Flow</span><span class="sxs-lookup"><span data-stu-id="59491-106">To add [!INCLUDE[d365fin](includes/d365fin_md.md)] as a data source in Flow</span></span>
1. <span data-ttu-id="59491-107">In your browser, navigate to [flow.microsoft.com](https://flow.microsoft.com/en-us/), and then sign in.</span><span class="sxs-lookup"><span data-stu-id="59491-107">In your browser, navigate to [flow.microsoft.com](https://flow.microsoft.com/en-us/), and then sign in.</span></span>
2. <span data-ttu-id="59491-108">Choose **My Flows** from the ribbon at the top of the page.</span><span class="sxs-lookup"><span data-stu-id="59491-108">Choose **My Flows** from the ribbon at the top of the page.</span></span>
3. <span data-ttu-id="59491-109">In the **My Flows** window, choose the **Create from blank** option.</span><span class="sxs-lookup"><span data-stu-id="59491-109">In the **My Flows** window, choose the **Create from blank** option.</span></span>
4. <span data-ttu-id="59491-110">From the list of available triggers, select one of the [!INCLUDE[d365fin](includes/d365fin_md.md)] triggers available:</span><span class="sxs-lookup"><span data-stu-id="59491-110">From the list of available triggers, select one of the [!INCLUDE[d365fin](includes/d365fin_md.md)] triggers available:</span></span>  
    <span data-ttu-id="59491-111">*When a record is created*,</span><span class="sxs-lookup"><span data-stu-id="59491-111">*When a record is created*,</span></span>  
    <span data-ttu-id="59491-112">*When a record is deleted*,</span><span class="sxs-lookup"><span data-stu-id="59491-112">*When a record is deleted*,</span></span>  
    <span data-ttu-id="59491-113">*When a record is modified*,</span><span class="sxs-lookup"><span data-stu-id="59491-113">*When a record is modified*,</span></span>  
    <span data-ttu-id="59491-114">*When a customer approval is requested*,</span><span class="sxs-lookup"><span data-stu-id="59491-114">*When a customer approval is requested*,</span></span>  
    <span data-ttu-id="59491-115">*When a general journal batch approval is requested*,</span><span class="sxs-lookup"><span data-stu-id="59491-115">*When a general journal batch approval is requested*,</span></span>  
    <span data-ttu-id="59491-116">*When a general journal line approval is requested*,</span><span class="sxs-lookup"><span data-stu-id="59491-116">*When a general journal line approval is requested*,</span></span>  
    <span data-ttu-id="59491-117">*When an item approval is requested*,</span><span class="sxs-lookup"><span data-stu-id="59491-117">*When an item approval is requested*,</span></span>  
    <span data-ttu-id="59491-118">*When a purchase document approval is requested*,</span><span class="sxs-lookup"><span data-stu-id="59491-118">*When a purchase document approval is requested*,</span></span>  
    <span data-ttu-id="59491-119">*When a sales document approval is requested*, or</span><span class="sxs-lookup"><span data-stu-id="59491-119">*When a sales document approval is requested*, or</span></span>  
    <span data-ttu-id="59491-120">*When a vendor aproval is requested*.</span><span class="sxs-lookup"><span data-stu-id="59491-120">*When a vendor aproval is requested*.</span></span>
5. <span data-ttu-id="59491-121">Flow will prompt you for the information that is required to connect to your [!INCLUDE[d365fin](includes/d365fin_md.md)] data.</span><span class="sxs-lookup"><span data-stu-id="59491-121">Flow will prompt you for the information that is required to connect to your [!INCLUDE[d365fin](includes/d365fin_md.md)] data.</span></span> <span data-ttu-id="59491-122">If you selected one of the following triggers: *When a record is created*, *When a record is modified*, or *When a record is deleted*, you must select a company name and table name.</span><span class="sxs-lookup"><span data-stu-id="59491-122">If you selected one of the following triggers: *When a record is created*, *When a record is modified*, or *When a record is deleted*, you must select a company name and table name.</span></span> <span data-ttu-id="59491-123">With any other trigger, only the company name is required to connect.</span><span class="sxs-lookup"><span data-stu-id="59491-123">With any other trigger, only the company name is required to connect.</span></span>

   <span data-ttu-id="59491-124">Flow will show a list of companies and tables that are available from [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="59491-124">Flow will show a list of companies and tables that are available from [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="59491-125">These tables, or end points, represent all the web services that you have published from [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="59491-125">These tables, or end points, represent all the web services that you have published from [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>

   <span data-ttu-id="59491-126">Alternatively, create a new web service URL in [!INCLUDE[d365fin](includes/d365fin_md.md)] by using the **Create Data Set** action in the **Web Services** page, using the **Set Up Reporting** Assisted Setup guide, or by choosing the **Edit in Excel** action in any lists.</span><span class="sxs-lookup"><span data-stu-id="59491-126">Alternatively, create a new web service URL in [!INCLUDE[d365fin](includes/d365fin_md.md)] by using the **Create Data Set** action in the **Web Services** page, using the **Set Up Reporting** Assisted Setup guide, or by choosing the **Edit in Excel** action in any lists.</span></span>

<span data-ttu-id="59491-127">At this point, you have successfully connected to your Finance and Operations, Business edition data and are ready to begin building your flow.</span><span class="sxs-lookup"><span data-stu-id="59491-127">At this point, you have successfully connected to your Finance and Operations, Business edition data and are ready to begin building your flow.</span></span> <span data-ttu-id="59491-128">For more information, see the [Flow documentation](https://flow.microsoft.com/documentation/getting-started/).</span><span class="sxs-lookup"><span data-stu-id="59491-128">For more information, see the [Flow documentation](https://flow.microsoft.com/documentation/getting-started/).</span></span>

<span data-ttu-id="59491-129">For troubleshooting your Microsoft Flow, see [Troubleshooting Integration with Microsoft Flow](across-troubleshooting-how-use-financials-data-source-flow.md).</span><span class="sxs-lookup"><span data-stu-id="59491-129">For troubleshooting your Microsoft Flow, see [Troubleshooting Integration with Microsoft Flow](across-troubleshooting-how-use-financials-data-source-flow.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="59491-130">See Also</span><span class="sxs-lookup"><span data-stu-id="59491-130">See Also</span></span>
<span data-ttu-id="59491-131">[Welcome to [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)</span><span class="sxs-lookup"><span data-stu-id="59491-131">[Welcome to [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)</span></span>  
[<span data-ttu-id="59491-132">Importing Business Data from Other Finance Systems</span><span class="sxs-lookup"><span data-stu-id="59491-132">Importing Business Data from Other Finance Systems</span></span>](upload-data.md)  
<span data-ttu-id="59491-133">[Manage Users and Permissions](ui-how-users-permissions.md)  </span><span class="sxs-lookup"><span data-stu-id="59491-133">[Manage Users and Permissions](ui-how-users-permissions.md)  </span></span>  
<span data-ttu-id="59491-134">[Setting Up [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)</span><span class="sxs-lookup"><span data-stu-id="59491-134">[Setting Up [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)</span></span>  
[<span data-ttu-id="59491-135">Finance</span><span class="sxs-lookup"><span data-stu-id="59491-135">Finance</span></span>](finance.md)  

