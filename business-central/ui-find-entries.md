---
title: Finding entries | Microsoft Docs
description: This article describes how to documents and entries that are related
author: jswymer
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: find
ms.date: 10/01/2020
ms.author: jswymer
ms.openlocfilehash: 437e0c076b664ad35d5819783e98d9e91abee982
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "5393990"
---
# <a name="finding-related-entries-for-posted-documents"></a><span data-ttu-id="d622d-103">Finding Related Entries for Posted Documents</span><span class="sxs-lookup"><span data-stu-id="d622d-103">Finding Related Entries for Posted Documents</span></span> 

<span data-ttu-id="d622d-104">In this article, you learn how to find documents and entries that are related to each other based on a common information, like:</span><span class="sxs-lookup"><span data-stu-id="d622d-104">In this article, you learn how to find documents and entries that are related to each other based on a common information, like:</span></span>

- <span data-ttu-id="d622d-105">Document number or posting date</span><span class="sxs-lookup"><span data-stu-id="d622d-105">Document number or posting date</span></span>
- <span data-ttu-id="d622d-106">Business contact type, number, or external document number</span><span class="sxs-lookup"><span data-stu-id="d622d-106">Business contact type, number, or external document number</span></span>
- <span data-ttu-id="d622d-107">Item serial number or lot number</span><span class="sxs-lookup"><span data-stu-id="d622d-107">Item serial number or lot number</span></span>

<span data-ttu-id="d622d-108">This feature is useful for finding the ledger entries that resulted from certain transactions.</span><span class="sxs-lookup"><span data-stu-id="d622d-108">This feature is useful for finding the ledger entries that resulted from certain transactions.</span></span> <span data-ttu-id="d622d-109">When you search by document number, you can print the summary from the Document Entries report.</span><span class="sxs-lookup"><span data-stu-id="d622d-109">When you search by document number, you can print the summary from the Document Entries report.</span></span>

## <a name="get-started"></a><span data-ttu-id="d622d-110">Get started</span><span class="sxs-lookup"><span data-stu-id="d622d-110">Get started</span></span>

<span data-ttu-id="d622d-111">The find entries feature is readily available on most pages that display posted documents or posted documents entries - for both lists and cards.</span><span class="sxs-lookup"><span data-stu-id="d622d-111">The find entries feature is readily available on most pages that display posted documents or posted documents entries - for both lists and cards.</span></span> <span data-ttu-id="d622d-112">So the first step is open one of these pages.</span><span class="sxs-lookup"><span data-stu-id="d622d-112">So the first step is open one of these pages.</span></span> <span data-ttu-id="d622d-113">Then, either choose the **Find Entries** action or press the Alt+G keys.</span><span class="sxs-lookup"><span data-stu-id="d622d-113">Then, either choose the **Find Entries** action or press the Alt+G keys.</span></span>

<span data-ttu-id="d622d-114">The **Find Entries** page  includes all related documents and entries based on the document no. and posting date.</span><span class="sxs-lookup"><span data-stu-id="d622d-114">The **Find Entries** page  includes all related documents and entries based on the document no. and posting date.</span></span> <span data-ttu-id="d622d-115">The page is divided into three sections:</span><span class="sxs-lookup"><span data-stu-id="d622d-115">The page is divided into three sections:</span></span>

- <span data-ttu-id="d622d-116">The top section displays fields and actions that you use for filtering your search.</span><span class="sxs-lookup"><span data-stu-id="d622d-116">The top section displays fields and actions that you use for filtering your search.</span></span>
- <span data-ttu-id="d622d-117">The middle section displays related documents based on the search.</span><span class="sxs-lookup"><span data-stu-id="d622d-117">The middle section displays related documents based on the search.</span></span>
- <span data-ttu-id="d622d-118">The bottom section displays information about the source document that was found by searching.</span><span class="sxs-lookup"><span data-stu-id="d622d-118">The bottom section displays information about the source document that was found by searching.</span></span>


<!--
 There are two ways to open this page:

- Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Find Entries**, and then choose the related link.

    With this way, the **Find Entries** page might be empty, and you'll have to start searching for entries from scratch.
    
- Open a page that displays posted documents or posted documents entries, either a list or a card. Then, locate and select the **Find Entries** action.

    With this way, the **Find Entries**, page will include all related documents and entries based on the document no. and posting date.


    > [!TIP]
    > If you are on a page that has the **Find Entries** action, press crtl+G to open the **Find Entries** page directly. 
-->

## <a name="search-for-entries"></a><span data-ttu-id="d622d-119">Search for entries</span><span class="sxs-lookup"><span data-stu-id="d622d-119">Search for entries</span></span>

<span data-ttu-id="d622d-120">You can search for entries based on information about either the document, business contact, or item reference.</span><span class="sxs-lookup"><span data-stu-id="d622d-120">You can search for entries based on information about either the document, business contact, or item reference.</span></span> <span data-ttu-id="d622d-121">To change the search, select **Actions**, **Find By**, then one of the following actions:</span><span class="sxs-lookup"><span data-stu-id="d622d-121">To change the search, select **Actions**, **Find By**, then one of the following actions:</span></span>

|<span data-ttu-id="d622d-122">Action</span><span class="sxs-lookup"><span data-stu-id="d622d-122">Action</span></span>|<span data-ttu-id="d622d-123">Description</span><span class="sxs-lookup"><span data-stu-id="d622d-123">Description</span></span>|
|------|-----------|
|<span data-ttu-id="d622d-124">Find by Document</span><span class="sxs-lookup"><span data-stu-id="d622d-124">Find by Document</span></span>|<span data-ttu-id="d622d-125">View entries based on a specific document number or posting date.</span><span class="sxs-lookup"><span data-stu-id="d622d-125">View entries based on a specific document number or posting date.</span></span>|
|<span data-ttu-id="d622d-126">Business Contact</span><span class="sxs-lookup"><span data-stu-id="d622d-126">Business Contact</span></span> |<span data-ttu-id="d622d-127">View entries based on a specific contact type, contact number, anr/or external document number.</span><span class="sxs-lookup"><span data-stu-id="d622d-127">View entries based on a specific contact type, contact number, anr/or external document number.</span></span> <span data-ttu-id="d622d-128">You can enter document information that was assigned by a vendor or a customer.</span><span class="sxs-lookup"><span data-stu-id="d622d-128">You can enter document information that was assigned by a vendor or a customer.</span></span> <span data-ttu-id="d622d-129">Use the available fields to search for vendor documents by using the numbers that the vendor has assigned the documents.</span><span class="sxs-lookup"><span data-stu-id="d622d-129">Use the available fields to search for vendor documents by using the numbers that the vendor has assigned the documents.</span></span>|
|<span data-ttu-id="d622d-130">Item reference</span><span class="sxs-lookup"><span data-stu-id="d622d-130">Item reference</span></span>|<span data-ttu-id="d622d-131">View entires based on a serial number or lot number.</span><span class="sxs-lookup"><span data-stu-id="d622d-131">View entires based on a serial number or lot number.</span></span> <span data-ttu-id="d622d-132">You can enter the lot number or serial number, or filter on the lot number or serial number that you want to search for.</span><span class="sxs-lookup"><span data-stu-id="d622d-132">You can enter the lot number or serial number, or filter on the lot number or serial number that you want to search for.</span></span> <span data-ttu-id="d622d-133">This action is useful to see where a specific item tracking number was used, what vendor it came from, or what customer it was sold to.</span><span class="sxs-lookup"><span data-stu-id="d622d-133">This action is useful to see where a specific item tracking number was used, what vendor it came from, or what customer it was sold to.</span></span>|

<span data-ttu-id="d622d-134">After you make a selection, enter the relevant search information in the fields at the top.</span><span class="sxs-lookup"><span data-stu-id="d622d-134">After you make a selection, enter the relevant search information in the fields at the top.</span></span> <span data-ttu-id="d622d-135">Use the tooltips on the fields to help.</span><span class="sxs-lookup"><span data-stu-id="d622d-135">Use the tooltips on the fields to help.</span></span> <span data-ttu-id="d622d-136">When you're finished, choose **Find** to start the search.</span><span class="sxs-lookup"><span data-stu-id="d622d-136">When you're finished, choose **Find** to start the search.</span></span> <span data-ttu-id="d622d-137">If you change any of the filters, you have to choose **Find** again.</span><span class="sxs-lookup"><span data-stu-id="d622d-137">If you change any of the filters, you have to choose **Find** again.</span></span>

> [!TIP]
> <span data-ttu-id="d622d-138">For a couple examples about using **Find Entries**, see [Trace Item-Tracked Items](inventory-how-to-trace-item-tracked-items.md) and [Walkthrough: Tracing Serial-Lot Numbers](walkthrough-tracing-serial-lot-numbers.md).</span><span class="sxs-lookup"><span data-stu-id="d622d-138">For a couple examples about using **Find Entries**, see [Trace Item-Tracked Items](inventory-how-to-trace-item-tracked-items.md) and [Walkthrough: Tracing Serial-Lot Numbers](walkthrough-tracing-serial-lot-numbers.md).</span></span>

## <a name="see-related-training-at-microsoft-learn"></a><span data-ttu-id="d622d-139">See Related Training at [Microsoft Learn](/learn/modules/user-interface-dynamics-365-business-central/index)</span><span class="sxs-lookup"><span data-stu-id="d622d-139">See Related Training at [Microsoft Learn](/learn/modules/user-interface-dynamics-365-business-central/index)</span></span>

## <a name="see-also"></a><span data-ttu-id="d622d-140">See Also</span><span class="sxs-lookup"><span data-stu-id="d622d-140">See Also</span></span>

[<span data-ttu-id="d622d-141">Working with Business Central</span><span class="sxs-lookup"><span data-stu-id="d622d-141">Working with Business Central</span></span>](ui-work-product.md)  
[<span data-ttu-id="d622d-142">Add a Page Action to Your Role Centre</span><span class="sxs-lookup"><span data-stu-id="d622d-142">Add a Page Action to Your Role Center</span></span>](ui-bookmarks.md)  
[<span data-ttu-id="d622d-143">Trace Item-Tracked Items</span><span class="sxs-lookup"><span data-stu-id="d622d-143">Trace Item-Tracked Items</span></span>](inventory-how-to-trace-item-tracked-items.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]