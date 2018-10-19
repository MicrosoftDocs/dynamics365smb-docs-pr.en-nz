---
title: How to Archive Sales and Purchase Documents | Microsoft Docs
description: You can archive sales and purchase orders, quotes, return orders, and blanket orders, and you can use the archived document to recreate the document that it was archived from.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: 6b1b23c062fdb1c4558a292c7aa454ae24ff3c71
ms.contentlocale: en-nz
ms.lasthandoff: 09/28/2018

---
# <a name="archive-documents"></a><span data-ttu-id="cd530-103">Archive Documents</span><span class="sxs-lookup"><span data-stu-id="cd530-103">Archive Documents</span></span>
<span data-ttu-id="cd530-104">You can archive sales and purchase orders, quotes, return orders, and blanket orders, and you can use the archived document to recreate the document that it was archived from.</span><span class="sxs-lookup"><span data-stu-id="cd530-104">You can archive sales and purchase orders, quotes, return orders, and blanket orders, and you can use the archived document to recreate the document that it was archived from.</span></span>

## <a name="to-set-up-automatic-document-archiving"></a><span data-ttu-id="cd530-105">To set up automatic document archiving</span><span class="sxs-lookup"><span data-stu-id="cd530-105">To set up automatic document archiving</span></span>  
<span data-ttu-id="cd530-106">You can set up automatic archiving of sales and purchase orders, quotes, blanket orders, and return orders, before you delete documents.</span><span class="sxs-lookup"><span data-stu-id="cd530-106">You can set up automatic archiving of sales and purchase orders, quotes, blanket orders, and return orders, before you delete documents.</span></span>

<span data-ttu-id="cd530-107">The following procedure describes how to set up automatic archiving of sales documents.</span><span class="sxs-lookup"><span data-stu-id="cd530-107">The following procedure describes how to set up automatic archiving of sales documents.</span></span> <span data-ttu-id="cd530-108">The steps are similar for purchase documents.</span><span class="sxs-lookup"><span data-stu-id="cd530-108">The steps are similar for purchase documents.</span></span>
1.  <span data-ttu-id="cd530-109">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales & Receivables Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="cd530-109">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales & Receivables Setup**, and then choose the related link.</span></span>
2. <span data-ttu-id="cd530-110">In the **Sales & Receivables Setup** window, fill in the fields as follows.</span><span class="sxs-lookup"><span data-stu-id="cd530-110">In the **Sales & Receivables Setup** window, fill in the fields as follows.</span></span>

|<span data-ttu-id="cd530-111">Field</span><span class="sxs-lookup"><span data-stu-id="cd530-111">Field</span></span>|<span data-ttu-id="cd530-112">Description</span><span class="sxs-lookup"><span data-stu-id="cd530-112">Description</span></span>|
|-----|-----------|
|<span data-ttu-id="cd530-113">**Archiving Sales Quotes**</span><span class="sxs-lookup"><span data-stu-id="cd530-113">**Archiving Sales Quotes**</span></span>|<span data-ttu-id="cd530-114">**Never** to never archive sales quotes when they are deleted.</span><span class="sxs-lookup"><span data-stu-id="cd530-114">**Never** to never archive sales quotes when they are deleted.</span></span> <span data-ttu-id="cd530-115">**Question** to prompt the user to choose whether to archive sales quotes when they are deleted.</span><span class="sxs-lookup"><span data-stu-id="cd530-115">**Question** to prompt the user to choose whether to archive sales quotes when they are deleted.</span></span> <span data-ttu-id="cd530-116">**Always** to archive sales quotes automatically when they are deleted.</span><span class="sxs-lookup"><span data-stu-id="cd530-116">**Always** to archive sales quotes automatically when they are deleted.</span></span>|
|<span data-ttu-id="cd530-117">**Archiving Blanket Sales Orders**</span><span class="sxs-lookup"><span data-stu-id="cd530-117">**Archiving Blanket Sales Orders**</span></span>|<span data-ttu-id="cd530-118">Select to archive blanket sales orders automatically each time they are deleted.</span><span class="sxs-lookup"><span data-stu-id="cd530-118">Select to archive blanket sales orders automatically each time they are deleted.</span></span>|
|<span data-ttu-id="cd530-119">**Arch. Orders and Ret. Orders**</span><span class="sxs-lookup"><span data-stu-id="cd530-119">**Arch. Orders and Ret. Orders**</span></span>|<span data-ttu-id="cd530-120">Select to automatically archive sales orders each time they are deleted.</span><span class="sxs-lookup"><span data-stu-id="cd530-120">Select to automatically archive sales orders each time they are deleted.</span></span>|

## <a name="to-archive-a-sales-order"></a><span data-ttu-id="cd530-121">To archive a sales order</span><span class="sxs-lookup"><span data-stu-id="cd530-121">To archive a sales order</span></span>
<span data-ttu-id="cd530-122">The following procedure describes how to archive a sales order.</span><span class="sxs-lookup"><span data-stu-id="cd530-122">The following procedure describes how to archive a sales order.</span></span> <span data-ttu-id="cd530-123">The steps are similar for all orders, blanket orders, return orders, and quotes.</span><span class="sxs-lookup"><span data-stu-id="cd530-123">The steps are similar for all orders, blanket orders, return orders, and quotes.</span></span>

1.  <span data-ttu-id="cd530-124">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="cd530-124">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="cd530-125">Open a sales order that you want to archive.</span><span class="sxs-lookup"><span data-stu-id="cd530-125">Open a sales order that you want to archive.</span></span>  
3.  <span data-ttu-id="cd530-126">Choose the **Archive Document** action.</span><span class="sxs-lookup"><span data-stu-id="cd530-126">Choose the **Archive Document** action.</span></span>

<span data-ttu-id="cd530-127">The sales order is archived.</span><span class="sxs-lookup"><span data-stu-id="cd530-127">The sales order is archived.</span></span> <span data-ttu-id="cd530-128">You can view it in the **Archived Sales orders** window.</span><span class="sxs-lookup"><span data-stu-id="cd530-128">You can view it in the **Archived Sales orders** window.</span></span> <span data-ttu-id="cd530-129">From here, you can also use it to recreate the sales order that it was archived from.</span><span class="sxs-lookup"><span data-stu-id="cd530-129">From here, you can also use it to recreate the sales order that it was archived from.</span></span>

## <a name="to-recreate-a-sales-order-from-the-archive"></a><span data-ttu-id="cd530-130">To recreate a sales order from the archive</span><span class="sxs-lookup"><span data-stu-id="cd530-130">To recreate a sales order from the archive</span></span>
<span data-ttu-id="cd530-131">The following procedure describes how to recreate a sales order.</span><span class="sxs-lookup"><span data-stu-id="cd530-131">The following procedure describes how to recreate a sales order.</span></span> <span data-ttu-id="cd530-132">The steps are similar for all orders, blanket orders, return orders, and quotes.</span><span class="sxs-lookup"><span data-stu-id="cd530-132">The steps are similar for all orders, blanket orders, return orders, and quotes.</span></span>

1.  <span data-ttu-id="cd530-133">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Archived Sales Orders**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="cd530-133">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Archived Sales Orders**, and then choose the related link.</span></span>
2.  <span data-ttu-id="cd530-134">Select the archived sales order that you want to recreate, and then choose the **Restore** action.</span><span class="sxs-lookup"><span data-stu-id="cd530-134">Select the archived sales order that you want to recreate, and then choose the **Restore** action.</span></span>  

<span data-ttu-id="cd530-135">The sales order is created and added to the **Sales Orders** window.</span><span class="sxs-lookup"><span data-stu-id="cd530-135">The sales order is created and added to the **Sales Orders** window.</span></span>

## <a name="to-delete-archived-sales-orders"></a><span data-ttu-id="cd530-136">To delete archived sales orders</span><span class="sxs-lookup"><span data-stu-id="cd530-136">To delete archived sales orders</span></span>
<span data-ttu-id="cd530-137">The following procedure describes how to delete archived sales orders.</span><span class="sxs-lookup"><span data-stu-id="cd530-137">The following procedure describes how to delete archived sales orders.</span></span> <span data-ttu-id="cd530-138">The steps are similar for other archived sales and purchase documents.</span><span class="sxs-lookup"><span data-stu-id="cd530-138">The steps are similar for other archived sales and purchase documents.</span></span>

1.  <span data-ttu-id="cd530-139">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Delete Archived Sales Order Versions**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="cd530-139">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Delete Archived Sales Order Versions**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="cd530-140">In the **Delete Archived Sales Order Versions** window, select the appropriate filters.</span><span class="sxs-lookup"><span data-stu-id="cd530-140">In the **Delete Archived Sales Order Versions** window, select the appropriate filters.</span></span>  
3.  <span data-ttu-id="cd530-141">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="cd530-141">Choose the **OK** button.</span></span>

## <a name="see-also"></a><span data-ttu-id="cd530-142">See Also</span><span class="sxs-lookup"><span data-stu-id="cd530-142">See Also</span></span>
[<span data-ttu-id="cd530-143">Track Document Lines</span><span class="sxs-lookup"><span data-stu-id="cd530-143">Track Document Lines</span></span>](across-how-to-track-document-lines.md)  
[<span data-ttu-id="cd530-144">Sales</span><span class="sxs-lookup"><span data-stu-id="cd530-144">Sales</span></span>](sales-manage-sales.md)  
[<span data-ttu-id="cd530-145">General Business Functionality</span><span class="sxs-lookup"><span data-stu-id="cd530-145">General Business Functionality</span></span>](ui-across-business-areas.md)  
<span data-ttu-id="cd530-146">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="cd530-146">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

