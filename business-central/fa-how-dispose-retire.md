---
title: Dispose or Retire FA| Microsoft Docs
description: You must post a disposal value when you scrap, sell, or retire a fixed asset.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: scrap
ms.date: 01/29/2020
ms.author: sgroespe
ms.openlocfilehash: fe8b5bc5304a87fbb2cce14067e7cbd74cbf1198
ms.sourcegitcommit: 1c286468697d403b9e925186c2c05e724d612b88
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 01/31/2020
ms.locfileid: "2999751"
---
# <a name="dispose-of-or-retire-fixed-assets"></a><span data-ttu-id="d2424-103">Dispose of or Retire Fixed Assets</span><span class="sxs-lookup"><span data-stu-id="d2424-103">Dispose of or Retire Fixed Assets</span></span>
<span data-ttu-id="d2424-104">When you sell or otherwise dispose of a fixed asset, the disposal value must be posted to calculate and record the gain or loss.</span><span class="sxs-lookup"><span data-stu-id="d2424-104">When you sell or otherwise dispose of a fixed asset, the disposal value must be posted to calculate and record the gain or loss.</span></span> <span data-ttu-id="d2424-105">A disposal entry must be the last entry posted for a fixed asset.</span><span class="sxs-lookup"><span data-stu-id="d2424-105">A disposal entry must be the last entry posted for a fixed asset.</span></span> <span data-ttu-id="d2424-106">For partially disposed fixed assets, you can post more than one disposal entry.</span><span class="sxs-lookup"><span data-stu-id="d2424-106">For partially disposed fixed assets, you can post more than one disposal entry.</span></span> <span data-ttu-id="d2424-107">The total of all posted disposal amounts must be a credit amount.</span><span class="sxs-lookup"><span data-stu-id="d2424-107">The total of all posted disposal amounts must be a credit amount.</span></span>  

> [!NOTE]  
>   <span data-ttu-id="d2424-108">If you trade-in a fixed asset for another one, you must record both the sale of the old asset (disposal) and the purchase of the new one (acquisition).</span><span class="sxs-lookup"><span data-stu-id="d2424-108">If you trade-in a fixed asset for another one, you must record both the sale of the old asset (disposal) and the purchase of the new one (acquisition).</span></span> <span data-ttu-id="d2424-109">For more information, see [Acquire Fixed Assets](fa-how-acquire.md).</span><span class="sxs-lookup"><span data-stu-id="d2424-109">For more information, see [Acquire Fixed Assets](fa-how-acquire.md).</span></span>  

## <a name="to-post-a-disposal-from-the-fixed-asset-gl-journal"></a><span data-ttu-id="d2424-110">To post a disposal from the fixed asset G/L journal</span><span class="sxs-lookup"><span data-stu-id="d2424-110">To post a disposal from the fixed asset G/L journal</span></span>
1. <span data-ttu-id="d2424-111">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Fixed Asset G/L Journals**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="d2424-111">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Fixed Asset G/L Journals**, and then choose the related link.</span></span>  
2. <span data-ttu-id="d2424-112">Create an initial journal line and fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="d2424-112">Create an initial journal line and fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  
3. <span data-ttu-id="d2424-113">In the **FA Posting Type** field, select **Disposal**.</span><span class="sxs-lookup"><span data-stu-id="d2424-113">In the **FA Posting Type** field, select **Disposal**.</span></span>  
4. <span data-ttu-id="d2424-114">Choose the **Insert FA Bal. Account** action.</span><span class="sxs-lookup"><span data-stu-id="d2424-114">Choose the **Insert FA Bal. Account** action.</span></span> <span data-ttu-id="d2424-115">A second journal line is created for the balancing account that is set up for disposal posting.</span><span class="sxs-lookup"><span data-stu-id="d2424-115">A second journal line is created for the balancing account that is set up for disposal posting.</span></span>  

    > [!NOTE]  
    >   <span data-ttu-id="d2424-116">Step 4 only works if you have set up the following: On the **FA Posting Group Card** page for the posting group of the fixed asset, the **Disposal Account** field contains the general ledger debit account and the **Disposal Bal. Account** field contains the general ledger account to which you want to post balancing entries for appreciation.</span><span class="sxs-lookup"><span data-stu-id="d2424-116">Step 4 only works if you have set up the following: On the **FA Posting Group Card** page for the posting group of the fixed asset, the **Disposal Account** field contains the general ledger debit account and the **Disposal Bal. Account** field contains the general ledger account to which you want to post balancing entries for appreciation.</span></span> <span data-ttu-id="d2424-117">For more information, see [To set up fixed asset posting groups](fa-how-setup-general.md#to-set-up-fixed-asset-posting-groups).</span><span class="sxs-lookup"><span data-stu-id="d2424-117">For more information, see [To set up fixed asset posting groups](fa-how-setup-general.md#to-set-up-fixed-asset-posting-groups).</span></span>  
5. <span data-ttu-id="d2424-118">Choose the **Post** action.</span><span class="sxs-lookup"><span data-stu-id="d2424-118">Choose the **Post** action.</span></span>  

<span data-ttu-id="d2424-119">If you sell or dispose of part of a fixed asset, you must split up the asset before you can record the disposal transaction.</span><span class="sxs-lookup"><span data-stu-id="d2424-119">If you sell or dispose of part of a fixed asset, you must split up the asset before you can record the disposal transaction.</span></span> <span data-ttu-id="d2424-120">For more information, see [Transfer, Split, or Combine Fixed Assets](fa-how-trans-split-combine.md).</span><span class="sxs-lookup"><span data-stu-id="d2424-120">For more information, see [Transfer, Split, or Combine Fixed Assets](fa-how-trans-split-combine.md).</span></span>  

## <a name="to-view-disposal-ledger-entries"></a><span data-ttu-id="d2424-121">To view disposal ledger entries</span><span class="sxs-lookup"><span data-stu-id="d2424-121">To view disposal ledger entries</span></span>
<span data-ttu-id="d2424-122">When you sell or dispose of a fixed asset, the disposal value is posted to the general ledger where you can view the result.</span><span class="sxs-lookup"><span data-stu-id="d2424-122">When you sell or dispose of a fixed asset, the disposal value is posted to the general ledger where you can view the result.</span></span>  

1. <span data-ttu-id="d2424-123">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Fixed Assets**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="d2424-123">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Fixed Assets**, and then choose the related link.</span></span>  
2. <span data-ttu-id="d2424-124">Select the fixed asset that you want to view entries for, and then choose the **Depreciation Books** action.</span><span class="sxs-lookup"><span data-stu-id="d2424-124">Select the fixed asset that you want to view entries for, and then choose the **Depreciation Books** action.</span></span>  
3. <span data-ttu-id="d2424-125">Select the depreciation book that you want to view entries for, and then choose the **Ledger Entries** action.</span><span class="sxs-lookup"><span data-stu-id="d2424-125">Select the depreciation book that you want to view entries for, and then choose the **Ledger Entries** action.</span></span>  
4. <span data-ttu-id="d2424-126">Select a line with **Disposal** in the **FA Posting Category** field, and then choose the **Navigate** action.</span><span class="sxs-lookup"><span data-stu-id="d2424-126">Select a line with **Disposal** in the **FA Posting Category** field, and then choose the **Navigate** action.</span></span>  
5. <span data-ttu-id="d2424-127">On the **Navigate** page, select the general ledger entry line, and then choose the **Show** action.</span><span class="sxs-lookup"><span data-stu-id="d2424-127">On the **Navigate** page, select the general ledger entry line, and then choose the **Show** action.</span></span>  

<span data-ttu-id="d2424-128">The **General Ledger Entries** page opens where you can see the entries that the disposal posting resulted in.</span><span class="sxs-lookup"><span data-stu-id="d2424-128">The **General Ledger Entries** page opens where you can see the entries that the disposal posting resulted in.</span></span>  

## <a name="see-also"></a><span data-ttu-id="d2424-129">See Also</span><span class="sxs-lookup"><span data-stu-id="d2424-129">See Also</span></span>
[<span data-ttu-id="d2424-130">Fixed Assets</span><span class="sxs-lookup"><span data-stu-id="d2424-130">Fixed Assets</span></span>](fa-manage.md)  
[<span data-ttu-id="d2424-131">Setting Up Fixed Assets</span><span class="sxs-lookup"><span data-stu-id="d2424-131">Setting Up Fixed Assets</span></span>](fa-setup.md)  
[<span data-ttu-id="d2424-132">Finance</span><span class="sxs-lookup"><span data-stu-id="d2424-132">Finance</span></span>](finance.md)  
[<span data-ttu-id="d2424-133">Getting Started</span><span class="sxs-lookup"><span data-stu-id="d2424-133">Getting Started</span></span>](product-get-started.md)  
<span data-ttu-id="d2424-134">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="d2424-134">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
