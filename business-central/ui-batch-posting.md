---
title: How to Post Multiple Documents at the Same Time | Microsoft Docs
description: Instead of posting individual documents one by one, you can select multiple non-posted documents in a list for batch posting, either for immediate posting or scheduled to, for example, the end of the day.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.reviewer: edupont
ms.date: 10/01/2019
ms.author: sgroespe
ms.openlocfilehash: 15b0afcf04ad279000de227523f977fdb695fe01
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 10/01/2019
ms.locfileid: "2316803"
---
# <a name="post-multiple-documents-at-the-same-time"></a><span data-ttu-id="cb39e-103">Post Multiple Documents at the Same Time</span><span class="sxs-lookup"><span data-stu-id="cb39e-103">Post Multiple Documents at the Same Time</span></span>
<span data-ttu-id="cb39e-104">Instead of posting individual documents one by one, you can select multiple non-posted documents in a list for immediate posting or for batch posting according to a schedule, such as at the end of the day.</span><span class="sxs-lookup"><span data-stu-id="cb39e-104">Instead of posting individual documents one by one, you can select multiple non-posted documents in a list for immediate posting or for batch posting according to a schedule, such as at the end of the day.</span></span> <span data-ttu-id="cb39e-105">This may be useful if only a supervisor can post documents created by other users or to avoid system performance issues from posting during work hours.</span><span class="sxs-lookup"><span data-stu-id="cb39e-105">This may be useful if only a supervisor can post documents created by other users or to avoid system performance issues from posting during work hours.</span></span>

## <a name="to-post-multiple-purchase-orders-immediately"></a><span data-ttu-id="cb39e-106">To post multiple purchase orders immediately</span><span class="sxs-lookup"><span data-stu-id="cb39e-106">To post multiple purchase orders immediately</span></span>
<span data-ttu-id="cb39e-107">The following procedure explains how to post multiple purchase orders immediately.</span><span class="sxs-lookup"><span data-stu-id="cb39e-107">The following procedure explains how to post multiple purchase orders immediately.</span></span> <span data-ttu-id="cb39e-108">The steps are similar for all purchase and sales documents.</span><span class="sxs-lookup"><span data-stu-id="cb39e-108">The steps are similar for all purchase and sales documents.</span></span>

1. <span data-ttu-id="cb39e-109">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchase Orders**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="cb39e-109">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchase Orders**, and then choose the related link.</span></span>
2. <span data-ttu-id="cb39e-110">On the **Purchase Orders** page, proceed to select all orders to be posted:</span><span class="sxs-lookup"><span data-stu-id="cb39e-110">On the **Purchase Orders** page, proceed to select all orders to be posted:</span></span>
3. <span data-ttu-id="cb39e-111">In the **No.**</span><span class="sxs-lookup"><span data-stu-id="cb39e-111">In the **No.**</span></span> <span data-ttu-id="cb39e-112">field, choose the three vertical dots to open the context menu, and then choose the **Select More** action.</span><span class="sxs-lookup"><span data-stu-id="cb39e-112">field, choose the three vertical dots to open the context menu, and then choose the **Select More** action.</span></span>
4. <span data-ttu-id="cb39e-113">Select the check box for all the lines representing orders that you want to post at the same time.</span><span class="sxs-lookup"><span data-stu-id="cb39e-113">Select the check box for all the lines representing orders that you want to post at the same time.</span></span>
5. <span data-ttu-id="cb39e-114">Choose the **Posting** action, and then choose the **Post** action.</span><span class="sxs-lookup"><span data-stu-id="cb39e-114">Choose the **Posting** action, and then choose the **Post** action.</span></span>
6. <span data-ttu-id="cb39e-115">Choose the **Yes** button on the confirmation message.</span><span class="sxs-lookup"><span data-stu-id="cb39e-115">Choose the **Yes** button on the confirmation message.</span></span>

## <a name="to-batch-post-multiple-purchase-orders"></a><span data-ttu-id="cb39e-116">To batch post multiple purchase orders</span><span class="sxs-lookup"><span data-stu-id="cb39e-116">To batch post multiple purchase orders</span></span>
<span data-ttu-id="cb39e-117">The following procedure explains how to batch post purchase orders.</span><span class="sxs-lookup"><span data-stu-id="cb39e-117">The following procedure explains how to batch post purchase orders.</span></span> <span data-ttu-id="cb39e-118">The steps are similar for all purchase and sales documents where the **Batch Post** action is available.</span><span class="sxs-lookup"><span data-stu-id="cb39e-118">The steps are similar for all purchase and sales documents where the **Batch Post** action is available.</span></span>

> [!NOTE]
> <span data-ttu-id="cb39e-119">Batch posting of documents happens in the background as defined by a job queue entry, which must first be set up.</span><span class="sxs-lookup"><span data-stu-id="cb39e-119">Batch posting of documents happens in the background as defined by a job queue entry, which must first be set up.</span></span> <span data-ttu-id="cb39e-120">For more information, see [Use Job Queues to Schedule Tasks](admin-job-queues-schedule-tasks.md).</span><span class="sxs-lookup"><span data-stu-id="cb39e-120">For more information, see [Use Job Queues to Schedule Tasks](admin-job-queues-schedule-tasks.md).</span></span>

1. <span data-ttu-id="cb39e-121">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchase Orders**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="cb39e-121">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchase Orders**, and then choose the related link.</span></span>  
2. <span data-ttu-id="cb39e-122">On the **Purchase Orders** page, proceed to select all orders to be posted:</span><span class="sxs-lookup"><span data-stu-id="cb39e-122">On the **Purchase Orders** page, proceed to select all orders to be posted:</span></span>
3. <span data-ttu-id="cb39e-123">In the **No.**</span><span class="sxs-lookup"><span data-stu-id="cb39e-123">In the **No.**</span></span> <span data-ttu-id="cb39e-124">field, choose the three vertical dots to open the context menu, and then choose the **Select More** action.</span><span class="sxs-lookup"><span data-stu-id="cb39e-124">field, choose the three vertical dots to open the context menu, and then choose the **Select More** action.</span></span>
4. <span data-ttu-id="cb39e-125">Select the check box for all the lines representing orders that you want to post at the same time.</span><span class="sxs-lookup"><span data-stu-id="cb39e-125">Select the check box for all the lines representing orders that you want to post at the same time.</span></span>
5. <span data-ttu-id="cb39e-126">Choose the **Posting** action, and then choose the **Post Batch** action.</span><span class="sxs-lookup"><span data-stu-id="cb39e-126">Choose the **Posting** action, and then choose the **Post Batch** action.</span></span>
6. <span data-ttu-id="cb39e-127">On the **Batch Post Purchase Order** page, fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="cb39e-127">On the **Batch Post Purchase Order** page, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

    > [!NOTE]
    > <span data-ttu-id="cb39e-128">To print related reports when posting, such as the **Order Confirmation** report for sales orders, select the **Print** check box.</span><span class="sxs-lookup"><span data-stu-id="cb39e-128">To print related reports when posting, such as the **Order Confirmation** report for sales orders, select the **Print** check box.</span></span><br /><br /> <span data-ttu-id="cb39e-129">In the **Report Output Type** field on the **Sales and Receivables Setup** page or **Purchases and Payables Setup** page, you define if the report will be printed or output as a PDF.</span><span class="sxs-lookup"><span data-stu-id="cb39e-129">In the **Report Output Type** field on the **Sales and Receivables Setup** page or **Purchases and Payables Setup** page, you define if the report will be printed or output as a PDF.</span></span><br /><br /> <span data-ttu-id="cb39e-130">Note also that direct printing to a selected printer is only possible in on-premises installations.</span><span class="sxs-lookup"><span data-stu-id="cb39e-130">Note also that direct printing to a selected printer is only possible in on-premises installations.</span></span>

7. <span data-ttu-id="cb39e-131">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="cb39e-131">Choose the **OK** button.</span></span>
8. <span data-ttu-id="cb39e-132">To view potential issues that occurred during batch posting of documents, open the **Error Message Register** page.</span><span class="sxs-lookup"><span data-stu-id="cb39e-132">To view potential issues that occurred during batch posting of documents, open the **Error Message Register** page.</span></span>

<span data-ttu-id="cb39e-133">The purchase orders will now be added to a dedicated job queue entry, which defines when the documents are posted.</span><span class="sxs-lookup"><span data-stu-id="cb39e-133">The purchase orders will now be added to a dedicated job queue entry, which defines when the documents are posted.</span></span> <span data-ttu-id="cb39e-134">For more information, see [Use Job Queues to Schedule Tasks](admin-job-queues-schedule-tasks.md).</span><span class="sxs-lookup"><span data-stu-id="cb39e-134">For more information, see [Use Job Queues to Schedule Tasks](admin-job-queues-schedule-tasks.md).</span></span>

<span data-ttu-id="cb39e-135">If you select **PDF** in the **Report Output Type** field, successfully posted purchase orders will be available in the **Report Inbox** part on your Role Centre.</span><span class="sxs-lookup"><span data-stu-id="cb39e-135">If you select **PDF** in the **Report Output Type** field, successfully posted purchase orders will be available in the **Report Inbox** part on your Role Center.</span></span>

## <a name="see-also"></a><span data-ttu-id="cb39e-136">See Also</span><span class="sxs-lookup"><span data-stu-id="cb39e-136">See Also</span></span>
[<span data-ttu-id="cb39e-137">Posting Documents and Journals</span><span class="sxs-lookup"><span data-stu-id="cb39e-137">Posting Documents and Journals</span></span>](ui-post-documents-journals.md)  
[<span data-ttu-id="cb39e-138">Use Job Queues to Schedule Tasks</span><span class="sxs-lookup"><span data-stu-id="cb39e-138">Use Job Queues to Schedule Tasks</span></span>](admin-job-queues-schedule-tasks.md)  
[<span data-ttu-id="cb39e-139">Edit Posted Documents</span><span class="sxs-lookup"><span data-stu-id="cb39e-139">Edit Posted Documents</span></span>](across-edit-posted-document.md)  
[<span data-ttu-id="cb39e-140">Correct or Cancel Unpaid Purchase Invoices</span><span class="sxs-lookup"><span data-stu-id="cb39e-140">Correct or Cancel Unpaid Purchase Invoices</span></span>](purchasing-how-correct-cancel-unpaid-purchase-invoices.md)  
[<span data-ttu-id="cb39e-141">Finding Pages and Information with Tell Me</span><span class="sxs-lookup"><span data-stu-id="cb39e-141">Finding Pages and Information with Tell Me</span></span>](ui-search.md)  
<span data-ttu-id="cb39e-142">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="cb39e-142">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
