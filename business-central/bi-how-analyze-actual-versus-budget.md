---
title: Analyse Actual Versus Budget| Microsoft Docs
description: Describes how to analyse actual amounts versus budgeted amounts.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: bi, power BI, analysis, KPI
ms.date: 04/01/2020
ms.author: edupont
ms.openlocfilehash: cc0497b4e0add53ce983883cd58c10475c9d9a6e
ms.sourcegitcommit: a80afd4e5075018716efad76d82a54e158f1392d
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 09/09/2020
ms.locfileid: "3783507"
---
# <a name="analyze-actual-amounts-versus-budgeted-amounts"></a><span data-ttu-id="8d5b1-103">Analyse Actual Amounts Versus Budgeted Amounts</span><span class="sxs-lookup"><span data-stu-id="8d5b1-103">Analyze Actual Amounts Versus Budgeted Amounts</span></span>
<span data-ttu-id="8d5b1-104">As a part of gathering, analysing, and sharing your company data, you view actual amounts compared to budgeted amounts for all accounts and for several periods.</span><span class="sxs-lookup"><span data-stu-id="8d5b1-104">As a part of gathering, analyzing, and sharing your company data, you view actual amounts compared to budgeted amounts for all accounts and for several periods.</span></span>

<span data-ttu-id="8d5b1-105">To analyse budgeted amounts, you must first create G(L budgets.</span><span class="sxs-lookup"><span data-stu-id="8d5b1-105">To analyze budgeted amounts, you must first create G(L budgets.</span></span> <span data-ttu-id="8d5b1-106">For more information, see [Create G/L Budgets](finance-how-create-budgets.md).</span><span class="sxs-lookup"><span data-stu-id="8d5b1-106">For more information, see [Create G/L Budgets](finance-how-create-budgets.md).</span></span>

## <a name="to-view-a-gl-budget"></a><span data-ttu-id="8d5b1-107">To view a G/L budget</span><span class="sxs-lookup"><span data-stu-id="8d5b1-107">To view a G/L budget</span></span>
<span data-ttu-id="8d5b1-108">In a budget with dimensions, you can filter the entries and see specific budgets.</span><span class="sxs-lookup"><span data-stu-id="8d5b1-108">In a budget with dimensions, you can filter the entries and see specific budgets.</span></span>

1. <span data-ttu-id="8d5b1-109">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **G/L Budgets**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="8d5b1-109">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **G/L Budgets**, and then choose the related link.</span></span>
2. <span data-ttu-id="8d5b1-110">On the **G/L Budgets** page, open the budget that you want to view.</span><span class="sxs-lookup"><span data-stu-id="8d5b1-110">On the **G/L Budgets** page, open the budget that you want to view.</span></span>  
3. <span data-ttu-id="8d5b1-111">At the top of the page, fill in the fields as necessary to define what is shown.</span><span class="sxs-lookup"><span data-stu-id="8d5b1-111">At the top of the page, fill in the fields as necessary to define what is shown.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

> [!NOTE]  
>   <span data-ttu-id="8d5b1-112">If you have selected **Period** in either the **Show as Lines** or the **Show as Columns** field, then you must fill in the **View by** field.</span><span class="sxs-lookup"><span data-stu-id="8d5b1-112">If you have selected **Period** in either the **Show as Lines** or the **Show as Columns** field, then you must fill in the **View by** field.</span></span> <span data-ttu-id="8d5b1-113">If you have not selected **Period** in either the **Show as Lines** or **Show as Columns** field, then enter the appropriate period in **Date Filter** field.</span><span class="sxs-lookup"><span data-stu-id="8d5b1-113">If you have not selected **Period** in either the **Show as Lines** or **Show as Columns** field, then enter the appropriate period in **Date Filter** field.</span></span>  

> [!NOTE]  
>   <span data-ttu-id="8d5b1-114">Only entries from the general ledger budget with the filter codes that you enter on the **Filters** FastTab are included in the calculation.</span><span class="sxs-lookup"><span data-stu-id="8d5b1-114">Only entries from the general ledger budget with the filter codes that you enter on the **Filters** FastTab are included in the calculation.</span></span> <span data-ttu-id="8d5b1-115">Budget entries with other filter codes or without any filter codes are not included.</span><span class="sxs-lookup"><span data-stu-id="8d5b1-115">Budget entries with other filter codes or without any filter codes are not included.</span></span> <span data-ttu-id="8d5b1-116">As long as the filter remains on the page, the budget only displays the budget entries with these filter codes.</span><span class="sxs-lookup"><span data-stu-id="8d5b1-116">As long as the filter remains on the page, the budget only displays the budget entries with these filter codes.</span></span>  

> [!TIP]  
>   <span data-ttu-id="8d5b1-117">If you want to modify the budget, you can modify the budget entries.</span><span class="sxs-lookup"><span data-stu-id="8d5b1-117">If you want to modify the budget, you can modify the budget entries.</span></span> <span data-ttu-id="8d5b1-118">Choose an amount to view the underlying general ledger budget entries.</span><span class="sxs-lookup"><span data-stu-id="8d5b1-118">Choose an amount to view the underlying general ledger budget entries.</span></span>

## <a name="to-view-actual-and-budgeted-amounts-for-all-accounts"></a><span data-ttu-id="8d5b1-119">To view actual and budgeted amounts for all accounts</span><span class="sxs-lookup"><span data-stu-id="8d5b1-119">To view actual and budgeted amounts for all accounts</span></span>  
<span data-ttu-id="8d5b1-120">You can view general ledger budgets and compare them with actual figures in several areas of [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="8d5b1-120">You can view general ledger budgets and compare them with actual figures in several areas of [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>

1. <span data-ttu-id="8d5b1-121">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Chart of Accounts**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="8d5b1-121">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Chart of Accounts**, and then choose the related link.</span></span>  
2. <span data-ttu-id="8d5b1-122">On the **Chart of Accounts** page, choose the **G/L Balance/Budget** action.</span><span class="sxs-lookup"><span data-stu-id="8d5b1-122">On the **Chart of Accounts** page, choose the **G/L Balance/Budget** action.</span></span>
3. <span data-ttu-id="8d5b1-123">At the top of the page, fill in the fields as necessary to define what is shown.</span><span class="sxs-lookup"><span data-stu-id="8d5b1-123">At the top of the page, fill in the fields as necessary to define what is shown.</span></span>  
4. <span data-ttu-id="8d5b1-124">To see a specification that makes up the amount shown, choose the field.</span><span class="sxs-lookup"><span data-stu-id="8d5b1-124">To see a specification that makes up the amount shown, choose the field.</span></span>  

> [!NOTE]  
>   <span data-ttu-id="8d5b1-125">The filters you set on the page header will be applied to general ledger entries and also budget entries.</span><span class="sxs-lookup"><span data-stu-id="8d5b1-125">The filters you set on the page header will be applied to general ledger entries and also budget entries.</span></span>

<span data-ttu-id="8d5b1-126">The leftmost columns contain the chart of accounts.</span><span class="sxs-lookup"><span data-stu-id="8d5b1-126">The leftmost columns contain the chart of accounts.</span></span> <span data-ttu-id="8d5b1-127">Of the five columns on the rightmost side, the first four columns show actual and budgeted debit and credit amounts for each account.</span><span class="sxs-lookup"><span data-stu-id="8d5b1-127">Of the five columns on the rightmost side, the first four columns show actual and budgeted debit and credit amounts for each account.</span></span> <span data-ttu-id="8d5b1-128">The fifth column shows the proportional relationship between the actual and the budgeted amounts on the general ledger account.</span><span class="sxs-lookup"><span data-stu-id="8d5b1-128">The fifth column shows the proportional relationship between the actual and the budgeted amounts on the general ledger account.</span></span>  

> [!TIP]  
>   <span data-ttu-id="8d5b1-129">Use the **View by** field on the **G/L Balance/Budget** page to select the period length.</span><span class="sxs-lookup"><span data-stu-id="8d5b1-129">Use the **View by** field on the **G/L Balance/Budget** page to select the period length.</span></span> <span data-ttu-id="8d5b1-130">Use the **View as** field to select the way the amounts will be calculated, **Net Change** or **Balance at Date**.</span><span class="sxs-lookup"><span data-stu-id="8d5b1-130">Use the **View as** field to select the way the amounts will be calculated, **Net Change** or **Balance at Date**.</span></span> <span data-ttu-id="8d5b1-131">Choose the **Previous Period** or **Next Period** action to change the period.</span><span class="sxs-lookup"><span data-stu-id="8d5b1-131">Choose the **Previous Period** or **Next Period** action to change the period.</span></span>  

## <a name="to-view-actual-and-budgeted-amounts-for-several-periods"></a><span data-ttu-id="8d5b1-132">To view actual and budgeted amounts for several periods</span><span class="sxs-lookup"><span data-stu-id="8d5b1-132">To view actual and budgeted amounts for several periods</span></span>  
<span data-ttu-id="8d5b1-133">Instead of viewing the actual and budgeted amounts for all accounts within a single period, you can view a number of periods for a single account.</span><span class="sxs-lookup"><span data-stu-id="8d5b1-133">Instead of viewing the actual and budgeted amounts for all accounts within a single period, you can view a number of periods for a single account.</span></span>  

1. <span data-ttu-id="8d5b1-134">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Chart of Accounts**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="8d5b1-134">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Chart of Accounts**, and then choose the related link.</span></span>  
2. <span data-ttu-id="8d5b1-135">On the **Chart of Accounts** page, select the relevant general ledger account, and then choose the **G/L Account Balance/Budget** action.</span><span class="sxs-lookup"><span data-stu-id="8d5b1-135">On the **Chart of Accounts** page, select the relevant general ledger account, and then choose the **G/L Account Balance/Budget** action.</span></span>  
3. <span data-ttu-id="8d5b1-136">At the top of the page, fill in the fields as necessary to define what is shown.</span><span class="sxs-lookup"><span data-stu-id="8d5b1-136">At the top of the page, fill in the fields as necessary to define what is shown.</span></span>   
4. <span data-ttu-id="8d5b1-137">To see a specification of an amount shown, choose the field.</span><span class="sxs-lookup"><span data-stu-id="8d5b1-137">To see a specification of an amount shown, choose the field.</span></span>  

## <a name="see-related-training-at-microsoft-learn"></a><span data-ttu-id="8d5b1-138">See Related Training at [Microsoft Learn](/learn/modules/budgets-exchange-rates-dynamics-365-business-central/index)</span><span class="sxs-lookup"><span data-stu-id="8d5b1-138">See Related Training at [Microsoft Learn](/learn/modules/budgets-exchange-rates-dynamics-365-business-central/index)</span></span>

## <a name="see-also"></a><span data-ttu-id="8d5b1-139">See Also</span><span class="sxs-lookup"><span data-stu-id="8d5b1-139">See Also</span></span>
[<span data-ttu-id="8d5b1-140">Business Intelligence</span><span class="sxs-lookup"><span data-stu-id="8d5b1-140">Business Intelligence</span></span>](bi.md)  
[<span data-ttu-id="8d5b1-141">Work with Account Schedules</span><span class="sxs-lookup"><span data-stu-id="8d5b1-141">Work with Account Schedules</span></span>](bi-how-work-account-schedule.md)  
[<span data-ttu-id="8d5b1-142">Finance</span><span class="sxs-lookup"><span data-stu-id="8d5b1-142">Finance</span></span>](finance.md)  
[<span data-ttu-id="8d5b1-143">Setting Up Finance</span><span class="sxs-lookup"><span data-stu-id="8d5b1-143">Setting Up Finance</span></span>](finance-setup-finance.md)  
[<span data-ttu-id="8d5b1-144">The General Ledger and the Chart of Accounts</span><span class="sxs-lookup"><span data-stu-id="8d5b1-144">The General Ledger and the Chart of Accounts</span></span>](finance-general-ledger.md)  
<span data-ttu-id="8d5b1-145">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="8d5b1-145">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
