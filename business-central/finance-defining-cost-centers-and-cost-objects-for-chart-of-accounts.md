---
title: Defining Cost Centres and Cost Objects for Chart of Accounts | Microsoft Docs
description: You can automatically transfer the expense and income entries from the general ledger to cost accounting either for each general ledger posting or with a batch job. When you do the transfer, the system only transfers the entries that are already linked to a cost centre or a cost object. To establish a meaningful transfer, you must ensure that the cost centres and cost objects are correctly defined.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2019
ms.author: sgroespe
redirect_url: finance-set-up-cost-accounting
ms.openlocfilehash: 1a9178f80f6c16659509f1ae22b9225b1b6d2f70
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 10/01/2019
ms.locfileid: "2302444"
---
# <a name="defining-cost-centers-and-cost-objects-for-chart-of-accounts"></a><span data-ttu-id="f7025-105">Defining Cost Centres and Cost Objects for Chart of Accounts</span><span class="sxs-lookup"><span data-stu-id="f7025-105">Defining Cost Centers and Cost Objects for Chart of Accounts</span></span>
<span data-ttu-id="f7025-106">You can automatically transfer the expense and income entries from the general ledger to cost accounting either for each general ledger posting or with a batch job.</span><span class="sxs-lookup"><span data-stu-id="f7025-106">You can automatically transfer the expense and income entries from the general ledger to cost accounting either for each general ledger posting or with a batch job.</span></span> <span data-ttu-id="f7025-107">When you do the transfer, [!INCLUDE[d365fin](includes/d365fin_md.md)] only transfers the entries that are already linked to a cost centre or a cost object.</span><span class="sxs-lookup"><span data-stu-id="f7025-107">When you do the transfer, [!INCLUDE[d365fin](includes/d365fin_md.md)] only transfers the entries that are already linked to a cost center or a cost object.</span></span> <span data-ttu-id="f7025-108">To establish a meaningful transfer, you must ensure that the cost centres and cost objects are correctly defined.</span><span class="sxs-lookup"><span data-stu-id="f7025-108">To establish a meaningful transfer, you must ensure that the cost centers and cost objects are correctly defined.</span></span>  

## <a name="defining-default-dimension-values-for-general-ledger-accounts"></a><span data-ttu-id="f7025-109">Defining Default Dimension Values for General Ledger Accounts</span><span class="sxs-lookup"><span data-stu-id="f7025-109">Defining Default Dimension Values for General Ledger Accounts</span></span>  
<span data-ttu-id="f7025-110">For each general ledger account, you can define default dimension values in the **Default Dimension** table.</span><span class="sxs-lookup"><span data-stu-id="f7025-110">For each general ledger account, you can define default dimension values in the **Default Dimension** table.</span></span> <span data-ttu-id="f7025-111">The following example shows how to define that there should always be a DEPARTMENT cost centre, but never be a PROJECT cost object when posting to a general ledger account.</span><span class="sxs-lookup"><span data-stu-id="f7025-111">The following example shows how to define that there should always be a DEPARTMENT cost center, but never be a PROJECT cost object when posting to a general ledger account.</span></span>  

|<span data-ttu-id="f7025-112">**Dimension Code**</span><span class="sxs-lookup"><span data-stu-id="f7025-112">**Dimension Code**</span></span>|<span data-ttu-id="f7025-113">**Value Posting**</span><span class="sxs-lookup"><span data-stu-id="f7025-113">**Value Posting**</span></span>|  
|------------------------------------------|-----------------------------------------|  
|<span data-ttu-id="f7025-114">Department</span><span class="sxs-lookup"><span data-stu-id="f7025-114">Department</span></span>|<span data-ttu-id="f7025-115">Code Mandatory</span><span class="sxs-lookup"><span data-stu-id="f7025-115">Code Mandatory</span></span>|  
|<span data-ttu-id="f7025-116">Project</span><span class="sxs-lookup"><span data-stu-id="f7025-116">Project</span></span>|<span data-ttu-id="f7025-117">No Code</span><span class="sxs-lookup"><span data-stu-id="f7025-117">No Code</span></span>|  

## <a name="defining-dimension-values-for-overhead-costs-and-direct-costs"></a><span data-ttu-id="f7025-118">Defining Dimension Values for Overhead Costs and Direct Costs</span><span class="sxs-lookup"><span data-stu-id="f7025-118">Defining Dimension Values for Overhead Costs and Direct Costs</span></span>  
 <span data-ttu-id="f7025-119">You can transfer overhead costs to a cost centre and direct costs to a cost object.</span><span class="sxs-lookup"><span data-stu-id="f7025-119">You can transfer overhead costs to a cost center and direct costs to a cost object.</span></span> <span data-ttu-id="f7025-120">The following table shows the optimal combination of the dimension setup values.</span><span class="sxs-lookup"><span data-stu-id="f7025-120">The following table shows the optimal combination of the dimension setup values.</span></span>  

|<span data-ttu-id="f7025-121">Transfer To</span><span class="sxs-lookup"><span data-stu-id="f7025-121">Transfer To</span></span>|<span data-ttu-id="f7025-122">Cost Centre Posting</span><span class="sxs-lookup"><span data-stu-id="f7025-122">Cost Center Posting</span></span>|<span data-ttu-id="f7025-123">Cost Object Posting</span><span class="sxs-lookup"><span data-stu-id="f7025-123">Cost Object Posting</span></span>|  
|-----------------|-------------------------|-------------------------|  
|<span data-ttu-id="f7025-124">Cost Centre</span><span class="sxs-lookup"><span data-stu-id="f7025-124">Cost Center</span></span>|<span data-ttu-id="f7025-125">Code Mandatory</span><span class="sxs-lookup"><span data-stu-id="f7025-125">Code Mandatory</span></span>|<span data-ttu-id="f7025-126">No Code</span><span class="sxs-lookup"><span data-stu-id="f7025-126">No Code</span></span>|  
|<span data-ttu-id="f7025-127">Cost Object</span><span class="sxs-lookup"><span data-stu-id="f7025-127">Cost Object</span></span>|<span data-ttu-id="f7025-128">No Code</span><span class="sxs-lookup"><span data-stu-id="f7025-128">No Code</span></span>|<span data-ttu-id="f7025-129">Code Mandatory</span><span class="sxs-lookup"><span data-stu-id="f7025-129">Code Mandatory</span></span>|  

> [!NOTE]  
>  <span data-ttu-id="f7025-130">To make sure that the predefined cost centre and cost object that you set up in the general ledger are automatically carried over to cost accounting, select the **Check G/L Postings** check box in the Cost Accounting Setup page.</span><span class="sxs-lookup"><span data-stu-id="f7025-130">To make sure that the predefined cost center and cost object that you set up in the general ledger are automatically carried over to cost accounting, select the **Check G/L Postings** check box in the Cost Accounting Setup page.</span></span>  

## <a name="see-also"></a><span data-ttu-id="f7025-131">See Also</span><span class="sxs-lookup"><span data-stu-id="f7025-131">See Also</span></span>  
[<span data-ttu-id="f7025-132">Accounting for Costs</span><span class="sxs-lookup"><span data-stu-id="f7025-132">Accounting for Costs</span></span>](finance-manage-cost-accounting.md)  
[<span data-ttu-id="f7025-133">Setting Up Cost Accounting</span><span class="sxs-lookup"><span data-stu-id="f7025-133">Setting Up Cost Accounting</span></span>](finance-set-up-cost-accounting.md)  
<span data-ttu-id="f7025-134">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="f7025-134">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
