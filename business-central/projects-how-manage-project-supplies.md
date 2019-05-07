---
title: Purchase Items or Services for a Job and Manage Supplies| Microsoft Docs
description: Describes how to manage the supply and purchase of material and services to jobs.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: project management, material, purchase
ms.date: 04/01/2019
ms.author: sgroespe
ms.openlocfilehash: b6f60fccd9be7dbad28b1d0e190d240602720c69
ms.sourcegitcommit: bd78a5d990c9e83174da1409076c22df8b35eafd
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 03/31/2019
ms.locfileid: "934504"
---
# <a name="manage-job-supplies"></a><span data-ttu-id="ad2b4-103">Manage Job Supplies</span><span class="sxs-lookup"><span data-stu-id="ad2b4-103">Manage Job Supplies</span></span>
<span data-ttu-id="ad2b4-104">Managing project supplies of items, services, and expenses is an integral and critical aspect of the execution of all jobs.</span><span class="sxs-lookup"><span data-stu-id="ad2b4-104">Managing project supplies of items, services, and expenses is an integral and critical aspect of the execution of all jobs.</span></span> <span data-ttu-id="ad2b4-105">You can use inventory quantities or make job-specific purchases using purchase orders or purchase invoices.</span><span class="sxs-lookup"><span data-stu-id="ad2b4-105">You can use inventory quantities or make job-specific purchases using purchase orders or purchase invoices.</span></span> <span data-ttu-id="ad2b4-106">For example, a service job on a computer requires a new disk.</span><span class="sxs-lookup"><span data-stu-id="ad2b4-106">For example, a service job on a computer requires a new disk.</span></span> <span data-ttu-id="ad2b4-107">You create a purchase invoice to buy a new disk and record the job that it will be used on.</span><span class="sxs-lookup"><span data-stu-id="ad2b4-107">You create a purchase invoice to buy a new disk and record the job that it will be used on.</span></span>

<span data-ttu-id="ad2b4-108">If the purchase process does not require that the physical transaction be recorded separately, then a purchase may be processed on the **Job G/L Journal** page.</span><span class="sxs-lookup"><span data-stu-id="ad2b4-108">If the purchase process does not require that the physical transaction be recorded separately, then a purchase may be processed on the **Job G/L Journal** page.</span></span> <span data-ttu-id="ad2b4-109">For more information, see [Record Usage for Jobs](projects-how-record-job-usage.md).</span><span class="sxs-lookup"><span data-stu-id="ad2b4-109">For more information, see [Record Usage for Jobs](projects-how-record-job-usage.md).</span></span>

## <a name="to-purchase-items-or-services-for-a-job"></a><span data-ttu-id="ad2b4-110">To purchase items or services for a job</span><span class="sxs-lookup"><span data-stu-id="ad2b4-110">To purchase items or services for a job</span></span>
<span data-ttu-id="ad2b4-111">The following procedure shows how to use a purchase invoice to purchase products for a job.</span><span class="sxs-lookup"><span data-stu-id="ad2b4-111">The following procedure shows how to use a purchase invoice to purchase products for a job.</span></span> <span data-ttu-id="ad2b4-112">The same steps apply when using a purchase order.</span><span class="sxs-lookup"><span data-stu-id="ad2b4-112">The same steps apply when using a purchase order.</span></span>  

1. <span data-ttu-id="ad2b4-113">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchase Invoices**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="ad2b4-113">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchase Invoices**, and then choose the related link.</span></span>  
2. <span data-ttu-id="ad2b4-114">Choose the **New** action and fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="ad2b4-114">Choose the **New** action and fill in the fields as necessary.</span></span> <span data-ttu-id="ad2b4-115">For more information, see [Record Purchases](purchasing-how-record-purchases.md).</span><span class="sxs-lookup"><span data-stu-id="ad2b4-115">For more information, see [Record Purchases](purchasing-how-record-purchases.md).</span></span>
3. <span data-ttu-id="ad2b4-116">In the **Job No.** and **Job Task No.** fields, select the information of the job that you want to purchase items or services for.</span><span class="sxs-lookup"><span data-stu-id="ad2b4-116">In the **Job No.** and **Job Task No.** fields, select the information of the job that you want to purchase items or services for.</span></span> <span data-ttu-id="ad2b4-117">Use the **Choose Columns** function if the field is not visible.</span><span class="sxs-lookup"><span data-stu-id="ad2b4-117">Use the **Choose Columns** function if the field is not visible.</span></span> <span data-ttu-id="ad2b4-118">For more information, see [Personalising Your Workspace](ui-personalization-user.md).</span><span class="sxs-lookup"><span data-stu-id="ad2b4-118">For more information, see [Personalizing Your Workspace](ui-personalization-user.md).</span></span>

    <span data-ttu-id="ad2b4-119">The value that you select in the **Job Line Type** field defines whether a planning line is created when you post the usage of the item.</span><span class="sxs-lookup"><span data-stu-id="ad2b4-119">The value that you select in the **Job Line Type** field defines whether a planning line is created when you post the usage of the item.</span></span> <span data-ttu-id="ad2b4-120">If the field contains **Billable**, then job planning lines that are ready to be invoiced to the customer are created.</span><span class="sxs-lookup"><span data-stu-id="ad2b4-120">If the field contains **Billable**, then job planning lines that are ready to be invoiced to the customer are created.</span></span> <span data-ttu-id="ad2b4-121">For more information, see [Invoice Jobs](projects-how-invoice-jobs.md).</span><span class="sxs-lookup"><span data-stu-id="ad2b4-121">For more information, see [Invoice Jobs](projects-how-invoice-jobs.md).</span></span>
4. <span data-ttu-id="ad2b4-122">Choose the **Post** action.</span><span class="sxs-lookup"><span data-stu-id="ad2b4-122">Choose the **Post** action.</span></span>

## <a name="to-view-the-value-of-purchases-for-a-job"></a><span data-ttu-id="ad2b4-123">To view the value of purchases for a job</span><span class="sxs-lookup"><span data-stu-id="ad2b4-123">To view the value of purchases for a job</span></span>
1. <span data-ttu-id="ad2b4-124">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Jobs**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="ad2b4-124">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Jobs**, and then choose the related link.</span></span>
2. <span data-ttu-id="ad2b4-125">Open a relevant job card.</span><span class="sxs-lookup"><span data-stu-id="ad2b4-125">Open a relevant job card.</span></span>

    <span data-ttu-id="ad2b4-126">On the **Tasks** FastTab, the **Outstanding Orders** field shows the total outstanding amount, in local currency, of inventory items and services on purchase documents for the job task line.</span><span class="sxs-lookup"><span data-stu-id="ad2b4-126">On the **Tasks** FastTab, the **Outstanding Orders** field shows the total outstanding amount, in local currency, of inventory items and services on purchase documents for the job task line.</span></span>  

    <span data-ttu-id="ad2b4-127">The **Amt. Rec. Not Invoiced** field shows the value of items delivered on purchase documents, but not yet invoiced.</span><span class="sxs-lookup"><span data-stu-id="ad2b4-127">The **Amt. Rec. Not Invoiced** field shows the value of items delivered on purchase documents, but not yet invoiced.</span></span>  
3. <span data-ttu-id="ad2b4-128">Choose either of the fields to open the **Purchase Lines** page where you can review information about the related purchase document lines, including which items or services have been received.</span><span class="sxs-lookup"><span data-stu-id="ad2b4-128">Choose either of the fields to open the **Purchase Lines** page where you can review information about the related purchase document lines, including which items or services have been received.</span></span>

## <a name="to-post-a-job-related-expense"></a><span data-ttu-id="ad2b4-129">To post a job-related expense</span><span class="sxs-lookup"><span data-stu-id="ad2b4-129">To post a job-related expense</span></span>
<span data-ttu-id="ad2b4-130">If you incur extraordinary or one-time job expenses, you can use the **Job G/L Journal** page to post them directly to the relevant job account.</span><span class="sxs-lookup"><span data-stu-id="ad2b4-130">If you incur extraordinary or one-time job expenses, you can use the **Job G/L Journal** page to post them directly to the relevant job account.</span></span>

1. <span data-ttu-id="ad2b4-131">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Job G/L Journals**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="ad2b4-131">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Job G/L Journals**, and then choose the related link.</span></span>  
2. <span data-ttu-id="ad2b4-132">Create a new line and enter information about the expense, including information in the **Job No.** and **Job Task No** fields.</span><span class="sxs-lookup"><span data-stu-id="ad2b4-132">Create a new line and enter information about the expense, including information in the **Job No.** and **Job Task No** fields.</span></span>  
3. <span data-ttu-id="ad2b4-133">When the journal is complete, choose the **Post** action.</span><span class="sxs-lookup"><span data-stu-id="ad2b4-133">When the journal is complete, choose the **Post** action.</span></span>

## <a name="see-also"></a><span data-ttu-id="ad2b4-134">See Also</span><span class="sxs-lookup"><span data-stu-id="ad2b4-134">See Also</span></span>
[<span data-ttu-id="ad2b4-135">Project Management</span><span class="sxs-lookup"><span data-stu-id="ad2b4-135">Project Management</span></span>](projects-manage-projects.md)  
[<span data-ttu-id="ad2b4-136">Finance</span><span class="sxs-lookup"><span data-stu-id="ad2b4-136">Finance</span></span>](finance.md)  
<span data-ttu-id="ad2b4-137">[Purchasing](purchasing-manage-purchasing.md)       </span><span class="sxs-lookup"><span data-stu-id="ad2b4-137">[Purchasing](purchasing-manage-purchasing.md)       </span></span>  
<span data-ttu-id="ad2b4-138">[Sales](sales-manage-sales.md)    </span><span class="sxs-lookup"><span data-stu-id="ad2b4-138">[Sales](sales-manage-sales.md)    </span></span>  
<span data-ttu-id="ad2b4-139">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="ad2b4-139">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
