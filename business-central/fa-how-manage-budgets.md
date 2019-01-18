---
title: Manage FA Budgets| Microsoft Docs
description: You set up information about future investments, disposals, and depreciation of fixed assets to help prepare budgets and forecasts.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: forecast
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 33b900f1ac9e295921e7f3d6ea72cc93939d8a1b
ms.openlocfilehash: 12833530e37ed092cec5f410afdf7f4f52cd46b1
ms.contentlocale: en-nz
ms.lasthandoff: 11/26/2018

---
# <a name="manage-budgets-for-fixed-assets"></a><span data-ttu-id="bda43-103">Manage Budgets for Fixed Assets</span><span class="sxs-lookup"><span data-stu-id="bda43-103">Manage Budgets for Fixed Assets</span></span>
<span data-ttu-id="bda43-104">You can set up budgeted fixed assets.</span><span class="sxs-lookup"><span data-stu-id="bda43-104">You can set up budgeted fixed assets.</span></span> <span data-ttu-id="bda43-105">For example, this lets you include anticipated acquisitions and sales in reports.</span><span class="sxs-lookup"><span data-stu-id="bda43-105">For example, this lets you include anticipated acquisitions and sales in reports.</span></span>  

<span data-ttu-id="bda43-106">To prepare your budgeted income statement, budgeted balance sheet, and cash budget, you need information about future investments, disposals and depreciation of fixed assets.</span><span class="sxs-lookup"><span data-stu-id="bda43-106">To prepare your budgeted income statement, budgeted balance sheet, and cash budget, you need information about future investments, disposals and depreciation of fixed assets.</span></span> <span data-ttu-id="bda43-107">You can get this information from the **Fixed Asset - Projected Value** report.</span><span class="sxs-lookup"><span data-stu-id="bda43-107">You can get this information from the **Fixed Asset - Projected Value** report.</span></span> <span data-ttu-id="bda43-108">Before you print this report, you must prepare the budget.</span><span class="sxs-lookup"><span data-stu-id="bda43-108">Before you print this report, you must prepare the budget.</span></span>  

## <a name="to-budget-the-acquisition-cost-of-a-fixed-asset"></a><span data-ttu-id="bda43-109">To budget the acquisition cost of a fixed asset</span><span class="sxs-lookup"><span data-stu-id="bda43-109">To budget the acquisition cost of a fixed asset</span></span>
<span data-ttu-id="bda43-110">To prepare a budget, you have to set up fixed asset cards for fixed assets that you intend to buy in the future.</span><span class="sxs-lookup"><span data-stu-id="bda43-110">To prepare a budget, you have to set up fixed asset cards for fixed assets that you intend to buy in the future.</span></span> <span data-ttu-id="bda43-111">The budget fixed assets are set up as ordinary fixed assets, but it must be set up to not post to the general ledger.</span><span class="sxs-lookup"><span data-stu-id="bda43-111">The budget fixed assets are set up as ordinary fixed assets, but it must be set up to not post to the general ledger.</span></span>

<span data-ttu-id="bda43-112">When you post the acquisition cost, you enter the number of the budgeted fixed asset in the **Budgeted FA No.** field.</span><span class="sxs-lookup"><span data-stu-id="bda43-112">When you post the acquisition cost, you enter the number of the budgeted fixed asset in the **Budgeted FA No.** field.</span></span> <span data-ttu-id="bda43-113">This will post an acquisition cost with an opposite sign for the budgeted asset.</span><span class="sxs-lookup"><span data-stu-id="bda43-113">This will post an acquisition cost with an opposite sign for the budgeted asset.</span></span> <span data-ttu-id="bda43-114">This means that the total acquisition cost on the budgeted asset is the difference between the budgeted and the actual acquisition cost.</span><span class="sxs-lookup"><span data-stu-id="bda43-114">This means that the total acquisition cost on the budgeted asset is the difference between the budgeted and the actual acquisition cost.</span></span>

1. <span data-ttu-id="bda43-115">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Fixed Assets**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="bda43-115">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Fixed Assets**, and then choose the related link.</span></span>
2. <span data-ttu-id="bda43-116">Choose the **New** action to create a new fixed asset card for the budgeted fixed asset.</span><span class="sxs-lookup"><span data-stu-id="bda43-116">Choose the **New** action to create a new fixed asset card for the budgeted fixed asset.</span></span>
3. <span data-ttu-id="bda43-117">Select the **Budgeted Asset** check box to prevent posting to the general ledger.</span><span class="sxs-lookup"><span data-stu-id="bda43-117">Select the **Budgeted Asset** check box to prevent posting to the general ledger.</span></span>
4. <span data-ttu-id="bda43-118">Fill in the remaining fields, assign a depreciation book, and then post the first acquisition cost with the budgeted fixed asset entered in the **Budgeted FA No.** field on the journal line.</span><span class="sxs-lookup"><span data-stu-id="bda43-118">Fill in the remaining fields, assign a depreciation book, and then post the first acquisition cost with the budgeted fixed asset entered in the **Budgeted FA No.** field on the journal line.</span></span> <span data-ttu-id="bda43-119">For more information, see [Acquire Fixed Assets](fa-how-acquire.md).</span><span class="sxs-lookup"><span data-stu-id="bda43-119">For more information, see [Acquire Fixed Assets](fa-how-acquire.md).</span></span>

## <a name="to-budget-the-disposal-of-a-fixed-asset"></a><span data-ttu-id="bda43-120">To budget the disposal of a fixed asset</span><span class="sxs-lookup"><span data-stu-id="bda43-120">To budget the disposal of a fixed asset</span></span>
<span data-ttu-id="bda43-121">If you plan to sell assets within the budget period, you can enter information about sales price and sales date.</span><span class="sxs-lookup"><span data-stu-id="bda43-121">If you plan to sell assets within the budget period, you can enter information about sales price and sales date.</span></span>

1. <span data-ttu-id="bda43-122">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Fixed Assets**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="bda43-122">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Fixed Assets**, and then choose the related link.</span></span>
2. <span data-ttu-id="bda43-123">Select the fixed asset to be disposed of, and then choose the **Depreciation Books** action.</span><span class="sxs-lookup"><span data-stu-id="bda43-123">Select the fixed asset to be disposed of, and then choose the **Depreciation Books** action.</span></span>
3. <span data-ttu-id="bda43-124">On the **FA Depreciation Books** page, fill in the **Projected Disposal Date** and **Projected Proceeds on Disposal** fields.</span><span class="sxs-lookup"><span data-stu-id="bda43-124">On the **FA Depreciation Books** page, fill in the **Projected Disposal Date** and **Projected Proceeds on Disposal** fields.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="to-view-projected-disposal-values"></a><span data-ttu-id="bda43-125">To view projected disposal values</span><span class="sxs-lookup"><span data-stu-id="bda43-125">To view projected disposal values</span></span>
<span data-ttu-id="bda43-126">To see the projected disposal values and have the gain and loss calculated, you can use the **FA Projected Value** report.</span><span class="sxs-lookup"><span data-stu-id="bda43-126">To see the projected disposal values and have the gain and loss calculated, you can use the **FA Projected Value** report.</span></span>

1. <span data-ttu-id="bda43-127">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **FA Projected Value**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="bda43-127">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **FA Projected Value**, and then choose the related link.</span></span>
2. <span data-ttu-id="bda43-128">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="bda43-128">Fill in the fields as necessary.</span></span>
3. <span data-ttu-id="bda43-129">Choose the **Print** or **Preview** button.</span><span class="sxs-lookup"><span data-stu-id="bda43-129">Choose the **Print** or **Preview** button.</span></span>

## <a name="to-budget-depreciation"></a><span data-ttu-id="bda43-130">To budget depreciation</span><span class="sxs-lookup"><span data-stu-id="bda43-130">To budget depreciation</span></span>
<span data-ttu-id="bda43-131">You can use the **Fixed Asset - Projected Value** report to calculate future depreciation.</span><span class="sxs-lookup"><span data-stu-id="bda43-131">You can use the **Fixed Asset - Projected Value** report to calculate future depreciation.</span></span> <span data-ttu-id="bda43-132">The report shows the book value and accumulated depreciation at the start of the selected period, changes during the period, and the book value and accumulated depreciation at the end of the selected period.</span><span class="sxs-lookup"><span data-stu-id="bda43-132">The report shows the book value and accumulated depreciation at the start of the selected period, changes during the period, and the book value and accumulated depreciation at the end of the selected period.</span></span>

1. <span data-ttu-id="bda43-133">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **FA Projected Value**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="bda43-133">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **FA Projected Value**, and then choose the related link.</span></span>
2. <span data-ttu-id="bda43-134">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="bda43-134">Fill in the fields as necessary.</span></span>
3. <span data-ttu-id="bda43-135">To see total values for all assets, clear the **Print per Fixed Asset** check box.</span><span class="sxs-lookup"><span data-stu-id="bda43-135">To see total values for all assets, clear the **Print per Fixed Asset** check box.</span></span>
4. <span data-ttu-id="bda43-136">Leave the **Fixed Asset** FastTab blank to have all assets included.</span><span class="sxs-lookup"><span data-stu-id="bda43-136">Leave the **Fixed Asset** FastTab blank to have all assets included.</span></span> <span data-ttu-id="bda43-137">In the **Budgeted Asset** field, enter **No** to exclude budgeted assets or **Yes** to see budgeted assets only.</span><span class="sxs-lookup"><span data-stu-id="bda43-137">In the **Budgeted Asset** field, enter **No** to exclude budgeted assets or **Yes** to see budgeted assets only.</span></span>
5. <span data-ttu-id="bda43-138">Choose the **Print** or **Preview** button.</span><span class="sxs-lookup"><span data-stu-id="bda43-138">Choose the **Print** or **Preview** button.</span></span>

## <a name="see-also"></a><span data-ttu-id="bda43-139">See Also</span><span class="sxs-lookup"><span data-stu-id="bda43-139">See Also</span></span>
[<span data-ttu-id="bda43-140">Fixed Assets</span><span class="sxs-lookup"><span data-stu-id="bda43-140">Fixed Assets</span></span>](fa-manage.md)  
[<span data-ttu-id="bda43-141">Setting Up Fixed Assets</span><span class="sxs-lookup"><span data-stu-id="bda43-141">Setting Up Fixed Assets</span></span>](fa-setup.md)  
[<span data-ttu-id="bda43-142">Finance</span><span class="sxs-lookup"><span data-stu-id="bda43-142">Finance</span></span>](finance.md)  
[<span data-ttu-id="bda43-143">Getting Started</span><span class="sxs-lookup"><span data-stu-id="bda43-143">Getting Started</span></span>](product-get-started.md)  
<span data-ttu-id="bda43-144">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="bda43-144">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

