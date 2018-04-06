---
title: Export Positive Pay Files| Microsoft Docs
description: You can ensure your bank only clears validated checks and amounts by exporting a Positive Pay file that contains vendor and payment information.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: check, clearing
ms.date: 06/16/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: db5811c3ba22df76e2c0cab4b190777d0705f72a
ms.contentlocale: en-nz
ms.lasthandoff: 03/22/2018

---
# <a name="export-a-positive-pay-file"></a><span data-ttu-id="e9fee-103">Export a Positive Pay file</span><span class="sxs-lookup"><span data-stu-id="e9fee-103">Export a Positive Pay file</span></span>
<span data-ttu-id="e9fee-104">To make sure that your bank only clears validated cheques and amounts, you can export a Positive Pay file that contains vendor information, cheque number, and payment amount, which you send to the bank for reference when you process payments.</span><span class="sxs-lookup"><span data-stu-id="e9fee-104">To make sure that your bank only clears validated checks and amounts, you can export a Positive Pay file that contains vendor information, check number, and payment amount, which you send to the bank for reference when you process payments.</span></span>

[!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="e9fee-105"> is preconfigured to support Positive Pay files for Bank of America and City Bank.</span><span class="sxs-lookup"><span data-stu-id="e9fee-105"> is preconfigured to support Positive Pay files for Bank of America and City Bank.</span></span>

## <a name="to-set-up-a-bank-account-for-positive-pay"></a><span data-ttu-id="e9fee-106">To set up a bank account for Positive Pay</span><span class="sxs-lookup"><span data-stu-id="e9fee-106">To set up a bank account for Positive Pay</span></span>
1. <span data-ttu-id="e9fee-107">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Bank Accounts**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="e9fee-107">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Bank Accounts**, and then choose the related link.</span></span>
2. <span data-ttu-id="e9fee-108">Open the card for the bank that you want to use Positive Pay for.</span><span class="sxs-lookup"><span data-stu-id="e9fee-108">Open the card for the bank that you want to use Positive Pay for.</span></span>
3. <span data-ttu-id="e9fee-109">In the **Positive Pay Export Code** field, enter POSPAYBANK.</span><span class="sxs-lookup"><span data-stu-id="e9fee-109">In the **Positive Pay Export Code** field, enter POSPAYBANK.</span></span>
4. <span data-ttu-id="e9fee-110">Close the window.</span><span class="sxs-lookup"><span data-stu-id="e9fee-110">Close the window.</span></span>

## <a name="to-export-a-positive-pay-file"></a><span data-ttu-id="e9fee-111">To export a Positive Pay file</span><span class="sxs-lookup"><span data-stu-id="e9fee-111">To export a Positive Pay file</span></span>
1. <span data-ttu-id="e9fee-112">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Bank Accounts**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="e9fee-112">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Bank Accounts**, and then choose the related link.</span></span>
2. <span data-ttu-id="e9fee-113">Select the bank account that you want to export a Positive Pay file for.</span><span class="sxs-lookup"><span data-stu-id="e9fee-113">Select the bank account that you want to export a Positive Pay file for.</span></span>
3. <span data-ttu-id="e9fee-114">Choose **Positive Pay Export** action.</span><span class="sxs-lookup"><span data-stu-id="e9fee-114">Choose **Positive Pay Export** action.</span></span>

    <span data-ttu-id="e9fee-115">The **Positive Pay Export** window opens displaying payments that have been made for the bank account since the last upload date, as shown in the **Last Upload Date** and **Last Upload Time** fields.</span><span class="sxs-lookup"><span data-stu-id="e9fee-115">The **Positive Pay Export** window opens displaying payments that have been made for the bank account since the last upload date, as shown in the **Last Upload Date** and **Last Upload Time** fields.</span></span>
4. <span data-ttu-id="e9fee-116">In the **Cutoff Upload Date** field, specify a date before which payments are not included in the exported file.</span><span class="sxs-lookup"><span data-stu-id="e9fee-116">In the **Cutoff Upload Date** field, specify a date before which payments are not included in the exported file.</span></span>
5. <span data-ttu-id="e9fee-117">Choose the **Export** action.</span><span class="sxs-lookup"><span data-stu-id="e9fee-117">Choose the **Export** action.</span></span>
6. <span data-ttu-id="e9fee-118">In the **Export File** window, choose the **Save** button, and then save the file to a convenient location.</span><span class="sxs-lookup"><span data-stu-id="e9fee-118">In the **Export File** window, choose the **Save** button, and then save the file to a convenient location.</span></span>
7. <span data-ttu-id="e9fee-119">Upload the file to your electronic bank site.</span><span class="sxs-lookup"><span data-stu-id="e9fee-119">Upload the file to your electronic bank site.</span></span>
8. <span data-ttu-id="e9fee-120">Write down or copy the confirmation number that is displayed when the file upload is successful.</span><span class="sxs-lookup"><span data-stu-id="e9fee-120">Write down or copy the confirmation number that is displayed when the file upload is successful.</span></span>

<span data-ttu-id="e9fee-121">To view exported Positive Pay records</span><span class="sxs-lookup"><span data-stu-id="e9fee-121">To view exported Positive Pay records</span></span>

1. <span data-ttu-id="e9fee-122">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Bank Accounts**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="e9fee-122">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Bank Accounts**, and then choose the related link.</span></span>
2. <span data-ttu-id="e9fee-123">Select the bank account that you want to view Positive Pay export records for.</span><span class="sxs-lookup"><span data-stu-id="e9fee-123">Select the bank account that you want to view Positive Pay export records for.</span></span>
3. <span data-ttu-id="e9fee-124">Choose the **Positive Pay Entries** action.</span><span class="sxs-lookup"><span data-stu-id="e9fee-124">Choose the **Positive Pay Entries** action.</span></span>

    <span data-ttu-id="e9fee-125">In the **Positive Pay Entries** window, you can see all the Positive Pay export records for the bank account.</span><span class="sxs-lookup"><span data-stu-id="e9fee-125">In the **Positive Pay Entries** window, you can see all the Positive Pay export records for the bank account.</span></span>
4. <span data-ttu-id="e9fee-126">In the **Confirmation Number** field, enter, for each export record, the confirmation number that you receive when the file upload to the bank is successful.</span><span class="sxs-lookup"><span data-stu-id="e9fee-126">In the **Confirmation Number** field, enter, for each export record, the confirmation number that you receive when the file upload to the bank is successful.</span></span>
5. <span data-ttu-id="e9fee-127">To view the related payment lines, choose the **Positive Pay Entry Details** action.</span><span class="sxs-lookup"><span data-stu-id="e9fee-127">To view the related payment lines, choose the **Positive Pay Entry Details** action.</span></span>

<span data-ttu-id="e9fee-128">To reexport Positive Pay files</span><span class="sxs-lookup"><span data-stu-id="e9fee-128">To reexport Positive Pay files</span></span>

1. <span data-ttu-id="e9fee-129">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Bank Accounts**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="e9fee-129">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Bank Accounts**, and then choose the related link.</span></span>
2. <span data-ttu-id="e9fee-130">Select the bank account that you want to reexport Positive Pay files for.</span><span class="sxs-lookup"><span data-stu-id="e9fee-130">Select the bank account that you want to reexport Positive Pay files for.</span></span>
3. <span data-ttu-id="e9fee-131">Choose the **Positive Pay Entries** action.</span><span class="sxs-lookup"><span data-stu-id="e9fee-131">Choose the **Positive Pay Entries** action.</span></span>
4. <span data-ttu-id="e9fee-132">Select the line for the Positive Pay export file that you want to reexport.</span><span class="sxs-lookup"><span data-stu-id="e9fee-132">Select the line for the Positive Pay export file that you want to reexport.</span></span>
5. <span data-ttu-id="e9fee-133">In the **Positive Pay Entries** window, choose the **Reexport Positive Pay to File** action.</span><span class="sxs-lookup"><span data-stu-id="e9fee-133">In the **Positive Pay Entries** window, choose the **Reexport Positive Pay to File** action.</span></span>

## <a name="see-also"></a><span data-ttu-id="e9fee-134">See Also</span><span class="sxs-lookup"><span data-stu-id="e9fee-134">See Also</span></span>
[<span data-ttu-id="e9fee-135">Finance</span><span class="sxs-lookup"><span data-stu-id="e9fee-135">Finance</span></span>](finance.md)  
[<span data-ttu-id="e9fee-136">Setting Up Finance</span><span class="sxs-lookup"><span data-stu-id="e9fee-136">Setting Up Finance</span></span>](finance-setup-finance.md)  
[<span data-ttu-id="e9fee-137">Working with General Journals</span><span class="sxs-lookup"><span data-stu-id="e9fee-137">Working with General Journals</span></span>](ui-work-general-journals.md)  
<span data-ttu-id="e9fee-138">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="e9fee-138">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
