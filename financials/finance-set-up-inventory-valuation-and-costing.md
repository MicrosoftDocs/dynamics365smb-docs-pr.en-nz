---
title: Set Up Inventory Valuation and Costing | Microsoft Docs
description: The following table describes a sequence of tasks, with links to the topics that describe them.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/06/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: f6d1d0da42bbc6bf186845648552eb639731759f
ms.contentlocale: en-nz
ms.lasthandoff: 03/22/2018

---
# <a name="setting-up-inventory-valuation-and-costing"></a><span data-ttu-id="ac370-103">Setting Up Inventory Valuation and Costing</span><span class="sxs-lookup"><span data-stu-id="ac370-103">Setting Up Inventory Valuation and Costing</span></span>
<span data-ttu-id="ac370-104">To make sure that inventory costs are recorded correctly, you must set up various fields and windows before you begin to make item transactions.</span><span class="sxs-lookup"><span data-stu-id="ac370-104">To make sure that inventory costs are recorded correctly, you must set up various fields and windows before you begin to make item transactions.</span></span>

<span data-ttu-id="ac370-105">The following table describes a sequence of tasks, with links to the topics that describe them.</span><span class="sxs-lookup"><span data-stu-id="ac370-105">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>

|<span data-ttu-id="ac370-106">**To**</span><span class="sxs-lookup"><span data-stu-id="ac370-106">**To**</span></span>|<span data-ttu-id="ac370-107">**See**</span><span class="sxs-lookup"><span data-stu-id="ac370-107">**See**</span></span>|  
|------------|-------------|  
|<span data-ttu-id="ac370-108">Set a costing method for each item to govern how its incoming cost is used to assess inventory value and the cost of goods sold.</span><span class="sxs-lookup"><span data-stu-id="ac370-108">Set a costing method for each item to govern how its incoming cost is used to assess inventory value and the cost of goods sold.</span></span>|[<span data-ttu-id="ac370-109">Register New Items</span><span class="sxs-lookup"><span data-stu-id="ac370-109">Register New Items</span></span>](inventory-how-register-new-items.md)|  
|<span data-ttu-id="ac370-110">Ensure that the cost is automatically posted to the general ledger whenever an inventory transaction is posted.</span><span class="sxs-lookup"><span data-stu-id="ac370-110">Ensure that the cost is automatically posted to the general ledger whenever an inventory transaction is posted.</span></span>|<span data-ttu-id="ac370-111">**Automatic Cost Posting** field in the **Inventory Setup** page</span><span class="sxs-lookup"><span data-stu-id="ac370-111">**Automatic Cost Posting** field in the **Inventory Setup** page</span></span>|  
|<span data-ttu-id="ac370-112">Ensure that expected costs are posted to the general ledger to see from the interim G/L accounts an estimate of the amounts due and the cost of the traded items before they are actually invoiced.</span><span class="sxs-lookup"><span data-stu-id="ac370-112">Ensure that expected costs are posted to the general ledger to see from the interim G/L accounts an estimate of the amounts due and the cost of the traded items before they are actually invoiced.</span></span>|<span data-ttu-id="ac370-113">**Expected Cost Posting to G/L** field in the **Inventory Setup** page</span><span class="sxs-lookup"><span data-stu-id="ac370-113">**Expected Cost Posting to G/L** field in the **Inventory Setup** page</span></span>|  
|<span data-ttu-id="ac370-114">Set the system up to adjust for any cost changes automatically every time you post inventory transactions.</span><span class="sxs-lookup"><span data-stu-id="ac370-114">Set the system up to adjust for any cost changes automatically every time you post inventory transactions.</span></span>|[<span data-ttu-id="ac370-115">Adjust Item Costs</span><span class="sxs-lookup"><span data-stu-id="ac370-115">Adjust Item Costs</span></span>](inventory-how-adjust-item-costs.md)|  
|<span data-ttu-id="ac370-116">Define if the average cost is to be calculated per item only or per item for each stockkeping unit and for each variant of the item.</span><span class="sxs-lookup"><span data-stu-id="ac370-116">Define if the average cost is to be calculated per item only or per item for each stockkeping unit and for each variant of the item.</span></span>|<span data-ttu-id="ac370-117">**Average Cost Calc. Type** field in the **Inventory Setup** page</span><span class="sxs-lookup"><span data-stu-id="ac370-117">**Average Cost Calc. Type** field in the **Inventory Setup** page</span></span>|  
|<span data-ttu-id="ac370-118">Select the period of time you would like the program to use for calculating the weighted average cost of items that use the average costing method.</span><span class="sxs-lookup"><span data-stu-id="ac370-118">Select the period of time you would like the program to use for calculating the weighted average cost of items that use the average costing method.</span></span>|<span data-ttu-id="ac370-119">**Average Cost Period** field in the **Inventory Setup** page</span><span class="sxs-lookup"><span data-stu-id="ac370-119">**Average Cost Period** field in the **Inventory Setup** page</span></span>|  
|<span data-ttu-id="ac370-120">Define inventory periods to control inventory value over time by disallowing transaction posting in closed inventory periods.</span><span class="sxs-lookup"><span data-stu-id="ac370-120">Define inventory periods to control inventory value over time by disallowing transaction posting in closed inventory periods.</span></span>|[<span data-ttu-id="ac370-121">Work with Inventory Periods</span><span class="sxs-lookup"><span data-stu-id="ac370-121">Work with Inventory Periods</span></span>](finance-how-to-work-with-inventory-periods.md)|  
|<span data-ttu-id="ac370-122">Ensure that sales returns are applied to the original outbound transaction to preserve inventory value.</span><span class="sxs-lookup"><span data-stu-id="ac370-122">Ensure that sales returns are applied to the original outbound transaction to preserve inventory value.</span></span>|<span data-ttu-id="ac370-123">**Exact Cost Reversing Mandatory** field in the **Sales & Receivables** page</span><span class="sxs-lookup"><span data-stu-id="ac370-123">**Exact Cost Reversing Mandatory** field in the **Sales & Receivables** page</span></span>|  
|<span data-ttu-id="ac370-124">Ensure that purchase returns are applied to the original inbound transaction to preserve inventory value.</span><span class="sxs-lookup"><span data-stu-id="ac370-124">Ensure that purchase returns are applied to the original inbound transaction to preserve inventory value.</span></span>|<span data-ttu-id="ac370-125">**Exact Cost Reversing Mandatory** field in the **´Purchases & Payables** page</span><span class="sxs-lookup"><span data-stu-id="ac370-125">**Exact Cost Reversing Mandatory** field in the **´Purchases & Payables** page</span></span>|
|<span data-ttu-id="ac370-126">Set up the rounding rules to apply when adjusting or suggesting item prices and when adjusting or suggesting standard costs.</span><span class="sxs-lookup"><span data-stu-id="ac370-126">Set up the rounding rules to apply when adjusting or suggesting item prices and when adjusting or suggesting standard costs.</span></span>|<span data-ttu-id="ac370-127">**Rounding Method** page</span><span class="sxs-lookup"><span data-stu-id="ac370-127">**Rounding Method** page</span></span>|  

## <a name="see-also"></a><span data-ttu-id="ac370-128">See Also</span><span class="sxs-lookup"><span data-stu-id="ac370-128">See Also</span></span>  
[<span data-ttu-id="ac370-129">Managing Inventory Costs</span><span class="sxs-lookup"><span data-stu-id="ac370-129">Managing Inventory Costs</span></span>](finance-manage-inventory-costs.md)  
[<span data-ttu-id="ac370-130">Working with Finance and Operations, Business edition</span><span class="sxs-lookup"><span data-stu-id="ac370-130">Working with Finance and Operations, Business edition</span></span>](ui-work-product.md)  
[<span data-ttu-id="ac370-131">Finance</span><span class="sxs-lookup"><span data-stu-id="ac370-131">Finance</span></span>](finance.md)  

