---
title: Set Up Codes for Audit Trails| Microsoft Docs
description: Learn about the tasks to set up source codes and reason codes that you can use to track audit trails.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: accounting, auditing, bookkeeping
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 6c20c57f05d17b0b52fcc1d4c9b1234cf03c6e97
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 03/31/2021
ms.locfileid: "5773855"
---
# <a name="setting-up-source-codes-and-reason-codes-for-audit-trails"></a><span data-ttu-id="f1b59-103">Setting Up Source Codes and Reason Codes for Audit Trails</span><span class="sxs-lookup"><span data-stu-id="f1b59-103">Setting Up Source Codes and Reason Codes for Audit Trails</span></span>

<span data-ttu-id="f1b59-104">All posted entries are automatically assigned a source code so that transactions can be traced to their origin.</span><span class="sxs-lookup"><span data-stu-id="f1b59-104">All posted entries are automatically assigned a source code so that transactions can be traced to their origin.</span></span> <span data-ttu-id="f1b59-105">If you want to give entries a supplementary source code, you can use reason codes.</span><span class="sxs-lookup"><span data-stu-id="f1b59-105">If you want to give entries a supplementary source code, you can use reason codes.</span></span> <span data-ttu-id="f1b59-106">Reason codes are used to indicate why an entry was created.</span><span class="sxs-lookup"><span data-stu-id="f1b59-106">Reason codes are used to indicate why an entry was created.</span></span> <span data-ttu-id="f1b59-107">When you set up reason codes, you can assign them to entire journal templates and journal batches, and you can assign them to individual journal lines and documents.</span><span class="sxs-lookup"><span data-stu-id="f1b59-107">When you set up reason codes, you can assign them to entire journal templates and journal batches, and you can assign them to individual journal lines and documents.</span></span>  

<span data-ttu-id="f1b59-108">For both source codes and reason codes, use codes that are easy to remember and descriptive.</span><span class="sxs-lookup"><span data-stu-id="f1b59-108">For both source codes and reason codes, use codes that are easy to remember and descriptive.</span></span> <span data-ttu-id="f1b59-109">The code must be unique, and you can set up as many codes as you like.</span><span class="sxs-lookup"><span data-stu-id="f1b59-109">The code must be unique, and you can set up as many codes as you like.</span></span>

## <a name="define-source-codes"></a><span data-ttu-id="f1b59-110">Define source codes</span><span class="sxs-lookup"><span data-stu-id="f1b59-110">Define source codes</span></span>

<span data-ttu-id="f1b59-111">Sometimes, you want see how a particular entry arose, such as whether it came from posting a general journal or a purchase invoice.</span><span class="sxs-lookup"><span data-stu-id="f1b59-111">Sometimes, you want see how a particular entry arose, such as whether it came from posting a general journal or a purchase invoice.</span></span> <span data-ttu-id="f1b59-112">A source code indicates where an entry was created.</span><span class="sxs-lookup"><span data-stu-id="f1b59-112">A source code indicates where an entry was created.</span></span> <span data-ttu-id="f1b59-113">Entries are created when journals and invoices are posted and when certain batch jobs are executed.</span><span class="sxs-lookup"><span data-stu-id="f1b59-113">Entries are created when journals and invoices are posted and when certain batch jobs are executed.</span></span> <span data-ttu-id="f1b59-114">Each posting type has a specific source code that is assigned when individual entries are created.</span><span class="sxs-lookup"><span data-stu-id="f1b59-114">Each posting type has a specific source code that is assigned when individual entries are created.</span></span>  

<span data-ttu-id="f1b59-115">Posting journals, orders, invoices, or credit memos, and running various batch jobs, creates entries in the financial statements.</span><span class="sxs-lookup"><span data-stu-id="f1b59-115">Posting journals, orders, invoices, or credit memos, and running various batch jobs, creates entries in the financial statements.</span></span> <span data-ttu-id="f1b59-116">The **Source Code Setup** page contains several FastTabs, one for each application area.</span><span class="sxs-lookup"><span data-stu-id="f1b59-116">The **Source Code Setup** page contains several FastTabs, one for each application area.</span></span> <span data-ttu-id="f1b59-117">Each FastTab contains the source codes that are applicable for that application area.</span><span class="sxs-lookup"><span data-stu-id="f1b59-117">Each FastTab contains the source codes that are applicable for that application area.</span></span>

<span data-ttu-id="f1b59-118">When you post or run a batch job, the correct source code is automatically attached to the entry.</span><span class="sxs-lookup"><span data-stu-id="f1b59-118">When you post or run a batch job, the correct source code is automatically attached to the entry.</span></span> <span data-ttu-id="f1b59-119">For example, when you post from the general journal, the entry is coded as *GENJNL*.</span><span class="sxs-lookup"><span data-stu-id="f1b59-119">For example, when you post from the general journal, the entry is coded as *GENJNL*.</span></span> <span data-ttu-id="f1b59-120">You can then filter the **General Ledger Entries** page to show which entries were posted from the general journal or from sales documents, for example</span><span class="sxs-lookup"><span data-stu-id="f1b59-120">You can then filter the **General Ledger Entries** page to show which entries were posted from the general journal or from sales documents, for example</span></span>

### <a name="to-define-source-codes"></a><span data-ttu-id="f1b59-121">To define source codes</span><span class="sxs-lookup"><span data-stu-id="f1b59-121">To define source codes</span></span>

1. <span data-ttu-id="f1b59-122">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Source Code Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="f1b59-122">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Source Code Setup**, and then choose the related link.</span></span>  

2. <span data-ttu-id="f1b59-123">In the **Source Code Setup** window, for each each posting type and batch job, specify the relevant source code.</span><span class="sxs-lookup"><span data-stu-id="f1b59-123">In the **Source Code Setup** window, for each each posting type and batch job, specify the relevant source code.</span></span>  

<span data-ttu-id="f1b59-124">You can change the contents of a field later, and that change will then impact future postings.</span><span class="sxs-lookup"><span data-stu-id="f1b59-124">You can change the contents of a field later, and that change will then impact future postings.</span></span>

## <a name="change-source-codes"></a><span data-ttu-id="f1b59-125">Change source codes</span><span class="sxs-lookup"><span data-stu-id="f1b59-125">Change source codes</span></span>

<span data-ttu-id="f1b59-126">You may want to change a source code.</span><span class="sxs-lookup"><span data-stu-id="f1b59-126">You may want to change a source code.</span></span> <span data-ttu-id="f1b59-127">For example, you want to change the source code *GENJNL* to *GNJ*.</span><span class="sxs-lookup"><span data-stu-id="f1b59-127">For example, you want to change the source code *GENJNL* to *GNJ*.</span></span>

### <a name="to-change-source-codes"></a><span data-ttu-id="f1b59-128">To change source codes</span><span class="sxs-lookup"><span data-stu-id="f1b59-128">To change source codes</span></span>

1. <span data-ttu-id="f1b59-129">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Source Codes**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="f1b59-129">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Source Codes**, and then choose the related link.</span></span>

2. <span data-ttu-id="f1b59-130">On the line with the code to be changed, select the code in the **Code** field.</span><span class="sxs-lookup"><span data-stu-id="f1b59-130">On the line with the code to be changed, select the code in the **Code** field.</span></span>

3. <span data-ttu-id="f1b59-131">Enter the new code, and then choose the **Yes** button.</span><span class="sxs-lookup"><span data-stu-id="f1b59-131">Enter the new code, and then choose the **Yes** button.</span></span> <span data-ttu-id="f1b59-132">You can also change the contents of the **Description** field.</span><span class="sxs-lookup"><span data-stu-id="f1b59-132">You can also change the contents of the **Description** field.</span></span>

<span data-ttu-id="f1b59-133">All new entries that are posted from the general journal will have the new source code.</span><span class="sxs-lookup"><span data-stu-id="f1b59-133">All new entries that are posted from the general journal will have the new source code.</span></span>

## <a name="define-reason-codes"></a><span data-ttu-id="f1b59-134">Define reason codes</span><span class="sxs-lookup"><span data-stu-id="f1b59-134">Define reason codes</span></span>

<span data-ttu-id="f1b59-135">Reason codes supplement the source codes and are used to indicate why an entry was created.</span><span class="sxs-lookup"><span data-stu-id="f1b59-135">Reason codes supplement the source codes and are used to indicate why an entry was created.</span></span> <span data-ttu-id="f1b59-136">You can assign reason codes on individual entries, and you can assign permanent codes to specific journal templates and journal batches.</span><span class="sxs-lookup"><span data-stu-id="f1b59-136">You can assign reason codes on individual entries, and you can assign permanent codes to specific journal templates and journal batches.</span></span> <span data-ttu-id="f1b59-137">When a reason code is linked to a journal line or a sales or purchase header, all entries are marked with the reason code when they are posted.</span><span class="sxs-lookup"><span data-stu-id="f1b59-137">When a reason code is linked to a journal line or a sales or purchase header, all entries are marked with the reason code when they are posted.</span></span>  

### <a name="to-set-up-reason-codes"></a><span data-ttu-id="f1b59-138">To set up reason codes</span><span class="sxs-lookup"><span data-stu-id="f1b59-138">To set up reason codes</span></span>

1. <span data-ttu-id="f1b59-139">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon")  icon, enter **Reason Codes**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="f1b59-139">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon")  icon, enter **Reason Codes**, and then choose the related link.</span></span>

2. <span data-ttu-id="f1b59-140">In the **Reason Codes** window, enter the first code in the **Code** field.</span><span class="sxs-lookup"><span data-stu-id="f1b59-140">In the **Reason Codes** window, enter the first code in the **Code** field.</span></span> <span data-ttu-id="f1b59-141">In the **Description** field, enter an explanatory text.</span><span class="sxs-lookup"><span data-stu-id="f1b59-141">In the **Description** field, enter an explanatory text.</span></span>

<span data-ttu-id="f1b59-142">Repeat the procedure for each code you want to use.</span><span class="sxs-lookup"><span data-stu-id="f1b59-142">Repeat the procedure for each code you want to use.</span></span> <span data-ttu-id="f1b59-143">You can set up any number of codes.</span><span class="sxs-lookup"><span data-stu-id="f1b59-143">You can set up any number of codes.</span></span>

<span data-ttu-id="f1b59-144">The following procedure describes how to add a reason code to a journal template, but similar steps apply to adding a reason code to a journal line or journal batch.</span><span class="sxs-lookup"><span data-stu-id="f1b59-144">The following procedure describes how to add a reason code to a journal template, but similar steps apply to adding a reason code to a journal line or journal batch.</span></span>  

### <a name="to-assign-reason-codes-to-journal-templates"></a><span data-ttu-id="f1b59-145">To assign reason codes to journal templates</span><span class="sxs-lookup"><span data-stu-id="f1b59-145">To assign reason codes to journal templates</span></span>

1. <span data-ttu-id="f1b59-146">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon")  icon, enter **General Journal Templates**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="f1b59-146">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon")  icon, enter **General Journal Templates**, and then choose the related link.</span></span>

2. <span data-ttu-id="f1b59-147">On the line with the selected journal template, in the **Reason Code** field, specify the relevant code.</span><span class="sxs-lookup"><span data-stu-id="f1b59-147">On the line with the selected journal template, in the **Reason Code** field, specify the relevant code.</span></span>

3. <span data-ttu-id="f1b59-148">Close the journal template.</span><span class="sxs-lookup"><span data-stu-id="f1b59-148">Close the journal template.</span></span>

<span data-ttu-id="f1b59-149">The selected reason code will be copied to new journal batches created under this journal template.</span><span class="sxs-lookup"><span data-stu-id="f1b59-149">The selected reason code will be copied to new journal batches created under this journal template.</span></span> <span data-ttu-id="f1b59-150">You assign reason codes to journal templates in the other application areas in the same way.</span><span class="sxs-lookup"><span data-stu-id="f1b59-150">You assign reason codes to journal templates in the other application areas in the same way.</span></span>

### <a name="to-use-reason-codes-on-sales-and-purchase-documents"></a><span data-ttu-id="f1b59-151">To use reason codes on sales and purchase documents</span><span class="sxs-lookup"><span data-stu-id="f1b59-151">To use reason codes on sales and purchase documents</span></span>

1. <span data-ttu-id="f1b59-152">Open the relevant sales or purchase document.</span><span class="sxs-lookup"><span data-stu-id="f1b59-152">Open the relevant sales or purchase document.</span></span>

2. <span data-ttu-id="f1b59-153">On the sales or purchase header, enter the code in the **Reason Code** field.</span><span class="sxs-lookup"><span data-stu-id="f1b59-153">On the sales or purchase header, enter the code in the **Reason Code** field.</span></span>

<span data-ttu-id="f1b59-154">When the invoice is posted, the reason code is copied to each general ledger, customer, and vendor entry.</span><span class="sxs-lookup"><span data-stu-id="f1b59-154">When the invoice is posted, the reason code is copied to each general ledger, customer, and vendor entry.</span></span> <span data-ttu-id="f1b59-155">You cannot assign different reason codes to the individual purchase and sales lines because all lines are posted as one entry.</span><span class="sxs-lookup"><span data-stu-id="f1b59-155">You cannot assign different reason codes to the individual purchase and sales lines because all lines are posted as one entry.</span></span>

## <a name="see-related-training-at-microsoft-learn"></a><span data-ttu-id="f1b59-156">See Related Training at [Microsoft Learn](/learn/paths/set-up-financial-management-dynamics-365-business-central/)</span><span class="sxs-lookup"><span data-stu-id="f1b59-156">See Related Training at [Microsoft Learn](/learn/paths/set-up-financial-management-dynamics-365-business-central/)</span></span>

## <a name="see-also"></a><span data-ttu-id="f1b59-157">See Also</span><span class="sxs-lookup"><span data-stu-id="f1b59-157">See Also</span></span>

[<span data-ttu-id="f1b59-158">Finance</span><span class="sxs-lookup"><span data-stu-id="f1b59-158">Finance</span></span>](finance.md)  
[<span data-ttu-id="f1b59-159">Reconciling Bank Accounts</span><span class="sxs-lookup"><span data-stu-id="f1b59-159">Reconciling Bank Accounts</span></span>](bank-manage-bank-accounts.md)  
[<span data-ttu-id="f1b59-160">Working with Dimensions</span><span class="sxs-lookup"><span data-stu-id="f1b59-160">Working with Dimensions</span></span>](finance-dimensions.md)  
[<span data-ttu-id="f1b59-161">Importing Business Data from Other Finance Systems</span><span class="sxs-lookup"><span data-stu-id="f1b59-161">Importing Business Data from Other Finance Systems</span></span>](across-import-data-configuration-packages.md)  
[<span data-ttu-id="f1b59-162">Analysing Cash Flow in Your Company</span><span class="sxs-lookup"><span data-stu-id="f1b59-162">Analyzing Cash Flow in Your Company</span></span>](finance-analyze-cash-flow.md)  
<span data-ttu-id="f1b59-163">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="f1b59-163">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>  

## [!INCLUDE[prod_short](includes/free_trial_md.md)]  


[!INCLUDE[footer-include](includes/footer-banner.md)]