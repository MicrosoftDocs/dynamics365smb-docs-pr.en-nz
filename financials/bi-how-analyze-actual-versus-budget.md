---
title: Analyse Actual Versus Budget| Microsoft Docs
description: Describes how to analyse actual amounts versus budgeted amounts.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: bi, power BI, analysis, KPI
ms.date: 06/01/2017
ms.author: sgroespe
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: 126c8da9b9ef80e954510fa8e5089906d7dd6f01
ms.contentlocale: en-nz
ms.lasthandoff: 09/11/2017

---
# <a name="how-to-analyze-actual-amounts-versus-budgeted-amounts"></a><span data-ttu-id="b985b-103">How to: Analyse Actual Amounts Versus Budgeted Amounts</span><span class="sxs-lookup"><span data-stu-id="b985b-103">How to: Analyze Actual Amounts Versus Budgeted Amounts</span></span>
<span data-ttu-id="b985b-104">As a part of gathering, analysing, and sharing your company data, you view actual amounts compared to budgeted amounts for all accounts and for several periods.</span><span class="sxs-lookup"><span data-stu-id="b985b-104">As a part of gathering, analyzing, and sharing your company data, you view actual amounts compared to budgeted amounts for all accounts and for several periods.</span></span>

<span data-ttu-id="b985b-105">To analyse budgeted amounts, you must first create budgets.</span><span class="sxs-lookup"><span data-stu-id="b985b-105">To analyze budgeted amounts, you must first create budgets.</span></span> <span data-ttu-id="b985b-106">For more information, see [How to: Create Budgets](finance-how-create-budgets.md).</span><span class="sxs-lookup"><span data-stu-id="b985b-106">For more information, see [How to: Create Budgets](finance-how-create-budgets.md).</span></span>

> [!NOTE]  
>   <span data-ttu-id="b985b-107">This functionality requires that your experience is set to **Suite**.</span><span class="sxs-lookup"><span data-stu-id="b985b-107">This functionality requires that your experience is set to **Suite**.</span></span> <span data-ttu-id="b985b-108">For more information, see [Customizing Your [!INCLUDE[d365fin](includes/d365fin_md.md)] Experience](ui-experiences.md).</span><span class="sxs-lookup"><span data-stu-id="b985b-108">For more information, see [Customizing Your [!INCLUDE[d365fin](includes/d365fin_md.md)] Experience](ui-experiences.md).</span></span>

## <a name="to-view-a-budget"></a><span data-ttu-id="b985b-109">To view a budget</span><span class="sxs-lookup"><span data-stu-id="b985b-109">To view a budget</span></span>
<span data-ttu-id="b985b-110">In a budget with dimensions, you can filter the entries and see specific budgets.</span><span class="sxs-lookup"><span data-stu-id="b985b-110">In a budget with dimensions, you can filter the entries and see specific budgets.</span></span>

1. <span data-ttu-id="b985b-111">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **G/L Budgets**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="b985b-111">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **G/L Budgets**, and then choose the related link.</span></span>
2. <span data-ttu-id="b985b-112">In the **G/L Budgets** window, open the budget that you want to view.</span><span class="sxs-lookup"><span data-stu-id="b985b-112">In the **G/L Budgets** window, open the budget that you want to view.</span></span>  
3. <span data-ttu-id="b985b-113">At the top of the window, fill in the fields as necessary to define what is shown.</span><span class="sxs-lookup"><span data-stu-id="b985b-113">At the top of the window, fill in the fields as necessary to define what is shown.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

> [!NOTE]  
>   <span data-ttu-id="b985b-114">If you have selected **Period** in either the **Show as Lines** or the **Show as Columns** field, then you must fill in the **View by** field.</span><span class="sxs-lookup"><span data-stu-id="b985b-114">If you have selected **Period** in either the **Show as Lines** or the **Show as Columns** field, then you must fill in the **View by** field.</span></span> <span data-ttu-id="b985b-115">If you have not selected **Period** in either the **Show as Lines** or **Show as Columns** field, then enter the appropriate period in **Date Filter** field.</span><span class="sxs-lookup"><span data-stu-id="b985b-115">If you have not selected **Period** in either the **Show as Lines** or **Show as Columns** field, then enter the appropriate period in **Date Filter** field.</span></span>  

> [!NOTE]  
>   <span data-ttu-id="b985b-116">Only entries from the general ledger budget with the filter codes that you enter on the **Filters** FastTab are included in the calculation.</span><span class="sxs-lookup"><span data-stu-id="b985b-116">Only entries from the general ledger budget with the filter codes that you enter on the **Filters** FastTab are included in the calculation.</span></span> <span data-ttu-id="b985b-117">Budget entries with other filter codes or without any filter codes are not included.</span><span class="sxs-lookup"><span data-stu-id="b985b-117">Budget entries with other filter codes or without any filter codes are not included.</span></span> <span data-ttu-id="b985b-118">As long as the filter remains on the window, the budget only displays the budget entries with these filter codes.</span><span class="sxs-lookup"><span data-stu-id="b985b-118">As long as the filter remains on the window, the budget only displays the budget entries with these filter codes.</span></span>  

> [!TIP]  
>   <span data-ttu-id="b985b-119">If you want to modify the budget, you can modify the budget entries.</span><span class="sxs-lookup"><span data-stu-id="b985b-119">If you want to modify the budget, you can modify the budget entries.</span></span> <span data-ttu-id="b985b-120">Choose an amount to view the underlying general ledger budget entries.</span><span class="sxs-lookup"><span data-stu-id="b985b-120">Choose an amount to view the underlying general ledger budget entries.</span></span>

## <a name="to-view-actual-and-budgeted-amounts-for-all-accounts"></a><span data-ttu-id="b985b-121">To view actual and budgeted amounts for all accounts</span><span class="sxs-lookup"><span data-stu-id="b985b-121">To view actual and budgeted amounts for all accounts</span></span>  
<span data-ttu-id="b985b-122">You can view general ledger budgets and compare them with actual figures in several areas of [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="b985b-122">You can view general ledger budgets and compare them with actual figures in several areas of [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>

1. <span data-ttu-id="b985b-123">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Chart of Accounts**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="b985b-123">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Chart of Accounts**, and then choose the related link.</span></span>  
2. <span data-ttu-id="b985b-124">In the **Chart of Accounts** window, choose the **G/L Balance/Budget** action.</span><span class="sxs-lookup"><span data-stu-id="b985b-124">In the **Chart of Accounts** window, choose the **G/L Balance/Budget** action.</span></span>
3. <span data-ttu-id="b985b-125">At the top of the window, fill in the fields as necessary to define what is shown.</span><span class="sxs-lookup"><span data-stu-id="b985b-125">At the top of the window, fill in the fields as necessary to define what is shown.</span></span>  
4. <span data-ttu-id="b985b-126">To see a specification that makes up the amount shown, choose the field.</span><span class="sxs-lookup"><span data-stu-id="b985b-126">To see a specification that makes up the amount shown, choose the field.</span></span>  

> [!NOTE]  
>   <span data-ttu-id="b985b-127">The filters you set in the window header will be applied to general ledger entries and also budget entries.</span><span class="sxs-lookup"><span data-stu-id="b985b-127">The filters you set in the window header will be applied to general ledger entries and also budget entries.</span></span>

<span data-ttu-id="b985b-128">The leftmost columns contain the chart of accounts.</span><span class="sxs-lookup"><span data-stu-id="b985b-128">The leftmost columns contain the chart of accounts.</span></span> <span data-ttu-id="b985b-129">Of the five columns on the rightmost side, the first four columns show actual and budgeted debit and credit amounts for each account.</span><span class="sxs-lookup"><span data-stu-id="b985b-129">Of the five columns on the rightmost side, the first four columns show actual and budgeted debit and credit amounts for each account.</span></span> <span data-ttu-id="b985b-130">The fifth column shows the proportional relationship between the actual and the budgeted amounts on the general ledger account.</span><span class="sxs-lookup"><span data-stu-id="b985b-130">The fifth column shows the proportional relationship between the actual and the budgeted amounts on the general ledger account.</span></span>  

> [!TIP]  
>   <span data-ttu-id="b985b-131">Use the **View by** field in the **G/L Balance/Budget** window to select the period length.</span><span class="sxs-lookup"><span data-stu-id="b985b-131">Use the **View by** field in the **G/L Balance/Budget** window to select the period length.</span></span> <span data-ttu-id="b985b-132">Use the **View as** field to select the way the amounts will be calculated, **Net Change** or **Balance at Date**.</span><span class="sxs-lookup"><span data-stu-id="b985b-132">Use the **View as** field to select the way the amounts will be calculated, **Net Change** or **Balance at Date**.</span></span> <span data-ttu-id="b985b-133">Choose the **Previous Period** or **Next Period** action to change the period.</span><span class="sxs-lookup"><span data-stu-id="b985b-133">Choose the **Previous Period** or **Next Period** action to change the period.</span></span>  

## <a name="to-view-actual-and-budgeted-amounts-for-several-periods"></a><span data-ttu-id="b985b-134">To view actual and budgeted amounts for several periods</span><span class="sxs-lookup"><span data-stu-id="b985b-134">To view actual and budgeted amounts for several periods</span></span>  
<span data-ttu-id="b985b-135">Instead of viewing the actual and budgeted amounts for all accounts within a single period, you can view a number of periods for a single account.</span><span class="sxs-lookup"><span data-stu-id="b985b-135">Instead of viewing the actual and budgeted amounts for all accounts within a single period, you can view a number of periods for a single account.</span></span>  

1. <span data-ttu-id="b985b-136">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Chart of Accounts**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="b985b-136">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Chart of Accounts**, and then choose the related link.</span></span>  
2. <span data-ttu-id="b985b-137">In the **Chart of Accounts** window, select the relevant general ledger account, and then choose the **G/L Account Balance/Budget** action.</span><span class="sxs-lookup"><span data-stu-id="b985b-137">In the **Chart of Accounts** window, select the relevant general ledger account, and then choose the **G/L Account Balance/Budget** action.</span></span>  
3. <span data-ttu-id="b985b-138">At the top of the window, fill in the fields as necessary to define what is shown.</span><span class="sxs-lookup"><span data-stu-id="b985b-138">At the top of the window, fill in the fields as necessary to define what is shown.</span></span>   
4. <span data-ttu-id="b985b-139">To see a specification of an amount shown, choose the field.</span><span class="sxs-lookup"><span data-stu-id="b985b-139">To see a specification of an amount shown, choose the field.</span></span>  

## <a name="see-also"></a><span data-ttu-id="b985b-140">See Also</span><span class="sxs-lookup"><span data-stu-id="b985b-140">See Also</span></span>
<span data-ttu-id="b985b-141">[Business Intelligence](bi.md)
[How to: Work with Account Schedules](bi-how-work-account-schedule.md)</span><span class="sxs-lookup"><span data-stu-id="b985b-141">[Business Intelligence](bi.md)
[How to: Work with Account Schedules](bi-how-work-account-schedule.md)</span></span>  
[<span data-ttu-id="b985b-142">Finance</span><span class="sxs-lookup"><span data-stu-id="b985b-142">Finance</span></span>](finance.md)  
[<span data-ttu-id="b985b-143">Setting Up Finance</span><span class="sxs-lookup"><span data-stu-id="b985b-143">Setting Up Finance</span></span>](finance-setup-finance.md)  
[<span data-ttu-id="b985b-144">The General Ledger and the Chart of Accounts</span><span class="sxs-lookup"><span data-stu-id="b985b-144">The General Ledger and the Chart of Accounts</span></span>](finance-general-ledger.md)  
<span data-ttu-id="b985b-145">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="b985b-145">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  

