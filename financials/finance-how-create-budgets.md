---
title: Creating G/L Budgets| Microsoft Docs
description: Describes hos to create G/L budgets to forecast different financial activities and assign dimensions for business intelligence purposes.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: postpone
ms.date: 12/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: cfe0eed4090ef458e774da8d0bc03910247570d7
ms.openlocfilehash: 34642192e74992953b569cabeb5dbeb4112a0f44
ms.contentlocale: en-nz
ms.lasthandoff: 12/14/2017

---
# <a name="how-to-create-gl-budgets"></a><span data-ttu-id="415e2-103">How to: Create G/L Budgets</span><span class="sxs-lookup"><span data-stu-id="415e2-103">How to: Create G/L Budgets</span></span>
<span data-ttu-id="415e2-104">You can have multiple budgets for identical time periods by creating budgets with separate names.</span><span class="sxs-lookup"><span data-stu-id="415e2-104">You can have multiple budgets for identical time periods by creating budgets with separate names.</span></span> <span data-ttu-id="415e2-105">First, you set up the budget name and enter the budget figures.</span><span class="sxs-lookup"><span data-stu-id="415e2-105">First, you set up the budget name and enter the budget figures.</span></span> <span data-ttu-id="415e2-106">The budget name is then included on all the budget entries you create.</span><span class="sxs-lookup"><span data-stu-id="415e2-106">The budget name is then included on all the budget entries you create.</span></span>  

 <span data-ttu-id="415e2-107">When you create a budget, you can define four dimensions for each budget.</span><span class="sxs-lookup"><span data-stu-id="415e2-107">When you create a budget, you can define four dimensions for each budget.</span></span> <span data-ttu-id="415e2-108">These budget-specific dimensions are called budget dimensions.</span><span class="sxs-lookup"><span data-stu-id="415e2-108">These budget-specific dimensions are called budget dimensions.</span></span> <span data-ttu-id="415e2-109">You select the budget dimensions for each budget from among the dimensions you have already set up.</span><span class="sxs-lookup"><span data-stu-id="415e2-109">You select the budget dimensions for each budget from among the dimensions you have already set up.</span></span> <span data-ttu-id="415e2-110">Budget dimensions can be used to set filters on a budget and to add dimension information to budget entries.</span><span class="sxs-lookup"><span data-stu-id="415e2-110">Budget dimensions can be used to set filters on a budget and to add dimension information to budget entries.</span></span> <span data-ttu-id="415e2-111">For more information, see [Working with Dimensions](finance-dimensions.md).</span><span class="sxs-lookup"><span data-stu-id="415e2-111">For more information, see [Working with Dimensions](finance-dimensions.md).</span></span>

 <span data-ttu-id="415e2-112">Budgets play an important role in business intelligence, such as in financial statement based on account schedules that include budget entries or when analysing budgeted versus actual amounts in the chart of accounts.</span><span class="sxs-lookup"><span data-stu-id="415e2-112">Budgets play an important role in business intelligence, such as in financial statement based on account schedules that include budget entries or when analyzing budgeted versus actual amounts in the chart of accounts.</span></span> <span data-ttu-id="415e2-113">For more information, see [Business Intelligence](bi.md).</span><span class="sxs-lookup"><span data-stu-id="415e2-113">For more information, see [Business Intelligence](bi.md).</span></span>

 <span data-ttu-id="415e2-114">Budgets play an important role in business intelligence, such as in financial statement based on account schedules that include budget entries or when analysing budgeted versus actual amounts in the chart of accounts.</span><span class="sxs-lookup"><span data-stu-id="415e2-114">Budgets play an important role in business intelligence, such as in financial statement based on account schedules that include budget entries or when analyzing budgeted versus actual amounts in the chart of accounts.</span></span> <span data-ttu-id="415e2-115">For more information, see [Business Intelligence](bi.md).</span><span class="sxs-lookup"><span data-stu-id="415e2-115">For more information, see [Business Intelligence](bi.md).</span></span>

<span data-ttu-id="415e2-116">In cost accounting, you work with cost budgets in a similar way.</span><span class="sxs-lookup"><span data-stu-id="415e2-116">In cost accounting, you work with cost budgets in a similar way.</span></span> <span data-ttu-id="415e2-117">For more information, see [Creating Cost Budgets](finance-create-cost-budgets.md).</span><span class="sxs-lookup"><span data-stu-id="415e2-117">For more information, see [Creating Cost Budgets](finance-create-cost-budgets.md).</span></span>    

 > [!NOTE]  
>   <span data-ttu-id="415e2-118">This functionality requires that your experience is set to **Suite**.</span><span class="sxs-lookup"><span data-stu-id="415e2-118">This functionality requires that your experience is set to **Suite**.</span></span> <span data-ttu-id="415e2-119">For more information, see [Customizing Your [!INCLUDE[d365fin](includes/d365fin_md.md)] Experience](ui-experiences.md).</span><span class="sxs-lookup"><span data-stu-id="415e2-119">For more information, see [Customizing Your [!INCLUDE[d365fin](includes/d365fin_md.md)] Experience](ui-experiences.md).</span></span>  

## <a name="to-create-a-new-gl-budget"></a><span data-ttu-id="415e2-120">To create a new G/L budget</span><span class="sxs-lookup"><span data-stu-id="415e2-120">To create a new G/L budget</span></span>  
1. <span data-ttu-id="415e2-121">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **G/L Budgets**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="415e2-121">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **G/L Budgets**, and then choose the related link.</span></span>  
2. <span data-ttu-id="415e2-122">Choose the **Edit List** action, and then fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="415e2-122">Choose the **Edit List** action, and then fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  
3. <span data-ttu-id="415e2-123">Choose the **Edit Budget** action.</span><span class="sxs-lookup"><span data-stu-id="415e2-123">Choose the **Edit Budget** action.</span></span>
4. <span data-ttu-id="415e2-124">At the top of the **Budget** window, fill in the fields as necessary to define what is displayed.</span><span class="sxs-lookup"><span data-stu-id="415e2-124">At the top of the **Budget** window, fill in the fields as necessary to define what is displayed.</span></span>  

    <span data-ttu-id="415e2-125">Only entries that contain the budget name that you entered in the **budget Name** field are shown.</span><span class="sxs-lookup"><span data-stu-id="415e2-125">Only entries that contain the budget name that you entered in the **budget Name** field are shown.</span></span> <span data-ttu-id="415e2-126">Because the budget name has just been created, there are no entries that match the filter.</span><span class="sxs-lookup"><span data-stu-id="415e2-126">Because the budget name has just been created, there are no entries that match the filter.</span></span> <span data-ttu-id="415e2-127">Therefore, the window is empty.</span><span class="sxs-lookup"><span data-stu-id="415e2-127">Therefore, the window is empty.</span></span>  
5. <span data-ttu-id="415e2-128">To enter an amount, choose the relevant cell in the matrix.</span><span class="sxs-lookup"><span data-stu-id="415e2-128">To enter an amount, choose the relevant cell in the matrix.</span></span> <span data-ttu-id="415e2-129">The **G/L Budget Entries** window opens.</span><span class="sxs-lookup"><span data-stu-id="415e2-129">The **G/L Budget Entries** window opens.</span></span>  
6. <span data-ttu-id="415e2-130">Create a new line and fill in the **Amount** field.</span><span class="sxs-lookup"><span data-stu-id="415e2-130">Create a new line and fill in the **Amount** field.</span></span> <span data-ttu-id="415e2-131">Close the **G/L Budget Entries** window.</span><span class="sxs-lookup"><span data-stu-id="415e2-131">Close the **G/L Budget Entries** window.</span></span>  
7. <span data-ttu-id="415e2-132">Repeat steps 5 and 6 until you have entered all of the budget amounts.</span><span class="sxs-lookup"><span data-stu-id="415e2-132">Repeat steps 5 and 6 until you have entered all of the budget amounts.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="415e2-133">On the **Filters** FastTab, you can filter the budget information by budget dimensions you have set up under the budget name.</span><span class="sxs-lookup"><span data-stu-id="415e2-133">On the **Filters** FastTab, you can filter the budget information by budget dimensions you have set up under the budget name.</span></span>   

## <a name="see-also"></a><span data-ttu-id="415e2-134">See Also</span><span class="sxs-lookup"><span data-stu-id="415e2-134">See Also</span></span>
[<span data-ttu-id="415e2-135">Finance</span><span class="sxs-lookup"><span data-stu-id="415e2-135">Finance</span></span>](finance.md)  
[<span data-ttu-id="415e2-136">Business Intelligence</span><span class="sxs-lookup"><span data-stu-id="415e2-136">Business Intelligence</span></span>](bi.md)  
[<span data-ttu-id="415e2-137">Setting Up Finance</span><span class="sxs-lookup"><span data-stu-id="415e2-137">Setting Up Finance</span></span>](finance-setup-finance.md)  
[<span data-ttu-id="415e2-138">The General Ledger and the Chart of Accounts</span><span class="sxs-lookup"><span data-stu-id="415e2-138">The General Ledger and the Chart of Accounts</span></span>](finance-general-ledger.md)  
<span data-ttu-id="415e2-139">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="415e2-139">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  

