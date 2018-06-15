---
title: Build financial reports using account schedules
description: Describes how to use account schedules to create various views and report for analysing financial performance data.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: bi, power BI, analysis, KPI
ms.date: 04/16/2018
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 7c346455a9e27d7274b116754f1d594484b95d67
ms.openlocfilehash: f9f5b3a25a24d4d10c80d048153e68030733bf9e
ms.contentlocale: en-nz
ms.lasthandoff: 04/18/2018

---
# <a name="work-with-account-schedules"></a><span data-ttu-id="1e85f-103">Work with Account Schedules</span><span class="sxs-lookup"><span data-stu-id="1e85f-103">Work with Account Schedules</span></span>
<span data-ttu-id="1e85f-104">Use account schedules to get insight into the financial data stored in your chart of accounts.</span><span class="sxs-lookup"><span data-stu-id="1e85f-104">Use account schedules to get insight into the financial data stored in your chart of accounts.</span></span> <span data-ttu-id="1e85f-105">Account schedules analyse figures in G/L accounts, and compare general ledger entries with general ledger budget entries.</span><span class="sxs-lookup"><span data-stu-id="1e85f-105">Account schedules analyze figures in G/L accounts, and compare general ledger entries with general ledger budget entries.</span></span> <span data-ttu-id="1e85f-106">The results display in charts on your Role Centre, such as the Cash Flow chart.</span><span class="sxs-lookup"><span data-stu-id="1e85f-106">The results display in charts on your Role Center, such as the Cash Flow chart.</span></span>  

[!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="1e85f-107"> provides a few sample account schedules that you can use right away, or you can set up your own rows and columns to specify the figures to compare.</span><span class="sxs-lookup"><span data-stu-id="1e85f-107"> provides a few sample account schedules that you can use right away, or you can set up your own rows and columns to specify the figures to compare.</span></span> <span data-ttu-id="1e85f-108">For example, you can create account schedules to calculate profit margins on dimensions like departments or customer groups.</span><span class="sxs-lookup"><span data-stu-id="1e85f-108">For example, you can create account schedules to calculate profit margins on dimensions like departments or customer groups.</span></span> <span data-ttu-id="1e85f-109">You can create as many customised financial statements as you want.</span><span class="sxs-lookup"><span data-stu-id="1e85f-109">You can create as many customized financial statements as you want.</span></span>  

<span data-ttu-id="1e85f-110">Setting up account schedules requires an understanding of the financial data in the chart of accounts.</span><span class="sxs-lookup"><span data-stu-id="1e85f-110">Setting up account schedules requires an understanding of the financial data in the chart of accounts.</span></span> <span data-ttu-id="1e85f-111">For example, you can view general ledger entries as percentages of budget entries.</span><span class="sxs-lookup"><span data-stu-id="1e85f-111">For example, you can view general ledger entries as percentages of budget entries.</span></span> <span data-ttu-id="1e85f-112">This requires that budgets are created.</span><span class="sxs-lookup"><span data-stu-id="1e85f-112">This requires that budgets are created.</span></span> <span data-ttu-id="1e85f-113">For more information, see [Create G/L Budgets](finance-how-create-budgets.md).</span><span class="sxs-lookup"><span data-stu-id="1e85f-113">For more information, see [Create G/L Budgets](finance-how-create-budgets.md).</span></span>

## <a name="account-categories-and-account-schedules"></a><span data-ttu-id="1e85f-114">Account Categories and Account Schedules</span><span class="sxs-lookup"><span data-stu-id="1e85f-114">Account Categories and Account Schedules</span></span>
<span data-ttu-id="1e85f-115">You can use account categories to change the layout of your financial statements.</span><span class="sxs-lookup"><span data-stu-id="1e85f-115">You can use account categories to change the layout of your financial statements.</span></span> <span data-ttu-id="1e85f-116">After you set up your account categories in the **G/L Account Categories** window, and you choose the **Generate Account Schedules** action, the underlying account schedules for the core financial reports are updated.</span><span class="sxs-lookup"><span data-stu-id="1e85f-116">After you set up your account categories in the **G/L Account Categories** window, and you choose the **Generate Account Schedules** action, the underlying account schedules for the core financial reports are updated.</span></span> <span data-ttu-id="1e85f-117">The next time you run one of these reports, such as the balance statement, new totals and subentries are added, based on your changes.</span><span class="sxs-lookup"><span data-stu-id="1e85f-117">The next time you run one of these reports, such as the balance statement, new totals and subentries are added, based on your changes.</span></span> <span data-ttu-id="1e85f-118">For more information, see [The General Ledger and the Chart of Accounts](finance-general-ledger.md).</span><span class="sxs-lookup"><span data-stu-id="1e85f-118">For more information, see [The General Ledger and the Chart of Accounts](finance-general-ledger.md).</span></span>  

## <a name="to-create-new-account-schedules"></a><span data-ttu-id="1e85f-119">To create new account schedules</span><span class="sxs-lookup"><span data-stu-id="1e85f-119">To create new account schedules</span></span>  
 <span data-ttu-id="1e85f-120">You use account schedules to analyse figures in general ledger accounts or to compare general ledger entries with general ledger budget entries.</span><span class="sxs-lookup"><span data-stu-id="1e85f-120">You use account schedules to analyze figures in general ledger accounts or to compare general ledger entries with general ledger budget entries.</span></span> <span data-ttu-id="1e85f-121">For example, you can view the general ledger entries as percentages of the budget entries.</span><span class="sxs-lookup"><span data-stu-id="1e85f-121">For example, you can view the general ledger entries as percentages of the budget entries.</span></span>

1. <span data-ttu-id="1e85f-122">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Account Schedules**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="1e85f-122">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Account Schedules**, and then choose the related link.</span></span>  
2. <span data-ttu-id="1e85f-123">In the **Account Schedule Names** window, choose the **New** action to create a new account schedule name.</span><span class="sxs-lookup"><span data-stu-id="1e85f-123">In the **Account Schedule Names** window, choose the **New** action to create a new account schedule name.</span></span>
3. <span data-ttu-id="1e85f-124">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="1e85f-124">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4. <span data-ttu-id="1e85f-125">Choose the **Edit Account Schedule** action.</span><span class="sxs-lookup"><span data-stu-id="1e85f-125">Choose the **Edit Account Schedule** action.</span></span>
5. <span data-ttu-id="1e85f-126">In the **Account Schedule** window, fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="1e85f-126">In the **Account Schedule** window, fill in the fields as necessary.</span></span>  

    <span data-ttu-id="1e85f-127">When you have created a new account schedule and set up the rows, you must set up columns.</span><span class="sxs-lookup"><span data-stu-id="1e85f-127">When you have created a new account schedule and set up the rows, you must set up columns.</span></span> <span data-ttu-id="1e85f-128">You can either set them up manually or assign a predefined column layout to your account schedule.</span><span class="sxs-lookup"><span data-stu-id="1e85f-128">You can either set them up manually or assign a predefined column layout to your account schedule.</span></span>
6. <span data-ttu-id="1e85f-129">Choose the **Edit Column Layout Setup** action.</span><span class="sxs-lookup"><span data-stu-id="1e85f-129">Choose the **Edit Column Layout Setup** action.</span></span>
7. <span data-ttu-id="1e85f-130">In the **Column Layout** window, fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="1e85f-130">In the **Column Layout** window, fill in the fields as necessary.</span></span>

> [!NOTE]  
>   <span data-ttu-id="1e85f-131">If you did not assign a default column layout to the account schedule, you must set the columns up manually.</span><span class="sxs-lookup"><span data-stu-id="1e85f-131">If you did not assign a default column layout to the account schedule, you must set the columns up manually.</span></span>   

### <a name="to-create-a-column-that-calculates-percentages"></a><span data-ttu-id="1e85f-132">To create a column that calculates percentages</span><span class="sxs-lookup"><span data-stu-id="1e85f-132">To create a column that calculates percentages</span></span>  
<span data-ttu-id="1e85f-133">Sometimes you may want to include a column in an account schedule to calculate percentages of a total.</span><span class="sxs-lookup"><span data-stu-id="1e85f-133">Sometimes you may want to include a column in an account schedule to calculate percentages of a total.</span></span> <span data-ttu-id="1e85f-134">For example, if you have a number of rows that break down sales by dimension, you may want a column to indicate the percentage of total sales that each row represents.</span><span class="sxs-lookup"><span data-stu-id="1e85f-134">For example, if you have a number of rows that break down sales by dimension, you may want a column to indicate the percentage of total sales that each row represents.</span></span>

1. <span data-ttu-id="1e85f-135">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Account Schedules**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="1e85f-135">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Account Schedules**, and then choose the related link.</span></span>
2. <span data-ttu-id="1e85f-136">In the **Account Schedule Names** window, select an account schedule.</span><span class="sxs-lookup"><span data-stu-id="1e85f-136">In the **Account Schedule Names** window, select an account schedule.</span></span>  
3. <span data-ttu-id="1e85f-137">Choose the **Edit Account Schedule** action to set up an account schedule row to calculate the total on which the percentages will be based.</span><span class="sxs-lookup"><span data-stu-id="1e85f-137">Choose the **Edit Account Schedule** action to set up an account schedule row to calculate the total on which the percentages will be based.</span></span>  
4. <span data-ttu-id="1e85f-138">Insert a line immediately above the first row for which you want to display a percentage.</span><span class="sxs-lookup"><span data-stu-id="1e85f-138">Insert a line immediately above the first row for which you want to display a percentage.</span></span>  
5. <span data-ttu-id="1e85f-139">Fill in the fields on the line as follows: In the **Totaling Type** field, enter **Set Base for Percent**.</span><span class="sxs-lookup"><span data-stu-id="1e85f-139">Fill in the fields on the line as follows: In the **Totaling Type** field, enter **Set Base for Percent**.</span></span> <span data-ttu-id="1e85f-140">In the **Totalling** field, enter a formula for the total that the percentage will be based on.</span><span class="sxs-lookup"><span data-stu-id="1e85f-140">In the **Totaling** field, enter a formula for the total that the percentage will be based on.</span></span> <span data-ttu-id="1e85f-141">For example, if row 11 contains the total sales, enter **11**.</span><span class="sxs-lookup"><span data-stu-id="1e85f-141">For example, if row 11 contains the total sales, enter **11**.</span></span>  
6. <span data-ttu-id="1e85f-142">Choose the **Edit Column Layout Setup** action to set up a column.</span><span class="sxs-lookup"><span data-stu-id="1e85f-142">Choose the **Edit Column Layout Setup** action to set up a column.</span></span>  
7. <span data-ttu-id="1e85f-143">Fill in the fields on the line as follows: In the **Column Type** field, select **Formula**.</span><span class="sxs-lookup"><span data-stu-id="1e85f-143">Fill in the fields on the line as follows: In the **Column Type** field, select **Formula**.</span></span> <span data-ttu-id="1e85f-144">In the **Formula** field, enter a formula for the amount that you want to calculate a percentage for, followed by %.</span><span class="sxs-lookup"><span data-stu-id="1e85f-144">In the **Formula** field, enter a formula for the amount that you want to calculate a percentage for, followed by %.</span></span> <span data-ttu-id="1e85f-145">For example, if column number N contains the net change, enter **N%**.</span><span class="sxs-lookup"><span data-stu-id="1e85f-145">For example, if column number N contains the net change, enter **N%**.</span></span>  
8. <span data-ttu-id="1e85f-146">Repeat steps 4 through 7 for each group of rows that you want to break down by percentage.</span><span class="sxs-lookup"><span data-stu-id="1e85f-146">Repeat steps 4 through 7 for each group of rows that you want to break down by percentage.</span></span>

## <a name="to-set-up-account-schedules-with-overviews"></a><span data-ttu-id="1e85f-147">To set up account schedules with overviews</span><span class="sxs-lookup"><span data-stu-id="1e85f-147">To set up account schedules with overviews</span></span>  
<span data-ttu-id="1e85f-148">You can use an account schedule to create a statement comparing general ledger figures and general leger budget figures.</span><span class="sxs-lookup"><span data-stu-id="1e85f-148">You can use an account schedule to create a statement comparing general ledger figures and general leger budget figures.</span></span>

1. <span data-ttu-id="1e85f-149">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Account Schedules**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="1e85f-149">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Account Schedules**, and then choose the related link.</span></span>
2. <span data-ttu-id="1e85f-150">In the **Account Schedule Names** window, select an account schedule.</span><span class="sxs-lookup"><span data-stu-id="1e85f-150">In the **Account Schedule Names** window, select an account schedule.</span></span>  
3. <span data-ttu-id="1e85f-151">Choose the **Edit Account Schedule** action</span><span class="sxs-lookup"><span data-stu-id="1e85f-151">Choose the **Edit Account Schedule** action</span></span>  
4. <span data-ttu-id="1e85f-152">In the **Account Schedule** window, in the **Name** field, select the default account schedule name.</span><span class="sxs-lookup"><span data-stu-id="1e85f-152">In the **Account Schedule** window, in the **Name** field, select the default account schedule name.</span></span>
5. <span data-ttu-id="1e85f-153">Choose the **Insert Accounts** action.</span><span class="sxs-lookup"><span data-stu-id="1e85f-153">Choose the **Insert Accounts** action.</span></span>  
6. <span data-ttu-id="1e85f-154">Select the accounts that you want to include in your statement, and then choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="1e85f-154">Select the accounts that you want to include in your statement, and then choose the **OK** button.</span></span>

    <span data-ttu-id="1e85f-155">The accounts are now inserted into your account schedule.</span><span class="sxs-lookup"><span data-stu-id="1e85f-155">The accounts are now inserted into your account schedule.</span></span> <span data-ttu-id="1e85f-156">If you want you can also change the column layout.</span><span class="sxs-lookup"><span data-stu-id="1e85f-156">If you want you can also change the column layout.</span></span>  
7. <span data-ttu-id="1e85f-157">Choose the **Overview** action.</span><span class="sxs-lookup"><span data-stu-id="1e85f-157">Choose the **Overview** action.</span></span>  
8. <span data-ttu-id="1e85f-158">On the **Dimension Filters** FastTab, set the budget filter to the desired filter name.</span><span class="sxs-lookup"><span data-stu-id="1e85f-158">On the **Dimension Filters** FastTab, set the budget filter to the desired filter name.</span></span>  
9. <span data-ttu-id="1e85f-159">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="1e85f-159">Choose the **OK** button.</span></span>  

<span data-ttu-id="1e85f-160">Now you can copy and paste your budget statement into a spreadsheet.</span><span class="sxs-lookup"><span data-stu-id="1e85f-160">Now you can copy and paste your budget statement into a spreadsheet.</span></span>  

## <a name="comparing-accounting-periods-using-period-formulas"></a><span data-ttu-id="1e85f-161">Comparing Accounting Periods using Period Formulas</span><span class="sxs-lookup"><span data-stu-id="1e85f-161">Comparing Accounting Periods using Period Formulas</span></span>
<span data-ttu-id="1e85f-162">Your account schedule can compare the results of different accounting periods, such as this month versus same month last year.</span><span class="sxs-lookup"><span data-stu-id="1e85f-162">Your account schedule can compare the results of different accounting periods, such as this month versus same month last year.</span></span> <span data-ttu-id="1e85f-163">To do that, you add a column with the **Comparison Period Formula** field, and then set that field to a period formula.</span><span class="sxs-lookup"><span data-stu-id="1e85f-163">To do that, you add a column with the **Comparison Period Formula** field, and then set that field to a period formula.</span></span>  

<span data-ttu-id="1e85f-164">An accounting period does not have to match the calendar, but each fiscal year must have the same number of accounting periods, even though each period can be different in length.</span><span class="sxs-lookup"><span data-stu-id="1e85f-164">An accounting period does not have to match the calendar, but each fiscal year must have the same number of accounting periods, even though each period can be different in length.</span></span>   

[!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="1e85f-165"> uses the period formula to calculate the amount from the comparison period in relation to the period represented by the date filter on the report request.</span><span class="sxs-lookup"><span data-stu-id="1e85f-165"> uses the period formula to calculate the amount from the comparison period in relation to the period represented by the date filter on the report request.</span></span> <span data-ttu-id="1e85f-166">The comparison period is based on the period of the start date of the date filter.</span><span class="sxs-lookup"><span data-stu-id="1e85f-166">The comparison period is based on the period of the start date of the date filter.</span></span> <span data-ttu-id="1e85f-167">The abbreviations for period specifications are:</span><span class="sxs-lookup"><span data-stu-id="1e85f-167">The abbreviations for period specifications are:</span></span>


<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="1e85f-168">Abbreviation</span><span class="sxs-lookup"><span data-stu-id="1e85f-168">Abbreviation</span></span></th>
<th><span data-ttu-id="1e85f-169">Description</span><span class="sxs-lookup"><span data-stu-id="1e85f-169">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><span data-ttu-id="1e85f-170">P</span><span class="sxs-lookup"><span data-stu-id="1e85f-170">P</span></span></p></td>
<td><p><span data-ttu-id="1e85f-171">Period</span><span class="sxs-lookup"><span data-stu-id="1e85f-171">Period</span></span></p></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="1e85f-172">LP</span><span class="sxs-lookup"><span data-stu-id="1e85f-172">LP</span></span></p></td>
<td><p><span data-ttu-id="1e85f-173">Last period of a fiscal year, half-year or quarter.</span><span class="sxs-lookup"><span data-stu-id="1e85f-173">Last period of a fiscal year, half-year or quarter.</span></span></p></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="1e85f-174">CP</span><span class="sxs-lookup"><span data-stu-id="1e85f-174">CP</span></span></p></td>
<td><p><span data-ttu-id="1e85f-175">Current period of a fiscal year, half-year or quarter.</span><span class="sxs-lookup"><span data-stu-id="1e85f-175">Current period of a fiscal year, half-year or quarter.</span></span></p></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="1e85f-176">FY</span><span class="sxs-lookup"><span data-stu-id="1e85f-176">FY</span></span></p></td>
<td><p><span data-ttu-id="1e85f-177">Fiscal year.</span><span class="sxs-lookup"><span data-stu-id="1e85f-177">Fiscal year.</span></span> <span data-ttu-id="1e85f-178">For example, FY[1..3] denotes first quarter of the current fiscal year</span><span class="sxs-lookup"><span data-stu-id="1e85f-178">For example, FY[1..3] denotes first quarter of the current fiscal year</span></span></p></td>
</tr>
</tbody>
</table>

<span data-ttu-id="1e85f-179">Examples of formulas:</span><span class="sxs-lookup"><span data-stu-id="1e85f-179">Examples of formulas:</span></span>


<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="1e85f-180">Formula</span><span class="sxs-lookup"><span data-stu-id="1e85f-180">Formula</span></span></th>
<th><span data-ttu-id="1e85f-181">Description</span><span class="sxs-lookup"><span data-stu-id="1e85f-181">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><span data-ttu-id="1e85f-182">&lt;Blank&gt;</span><span class="sxs-lookup"><span data-stu-id="1e85f-182">&lt;Blank&gt;</span></span></p></td>
<td><p><span data-ttu-id="1e85f-183">Current period</span><span class="sxs-lookup"><span data-stu-id="1e85f-183">Current period</span></span></p></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="1e85f-184">-1P</span><span class="sxs-lookup"><span data-stu-id="1e85f-184">-1P</span></span></p></td>
<td><p><span data-ttu-id="1e85f-185">Previous period</span><span class="sxs-lookup"><span data-stu-id="1e85f-185">Previous period</span></span></p></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="1e85f-186">-1FY[1..LP]</span><span class="sxs-lookup"><span data-stu-id="1e85f-186">-1FY[1..LP]</span></span></p></td>
<td><p><span data-ttu-id="1e85f-187">Entire previous fiscal year</span><span class="sxs-lookup"><span data-stu-id="1e85f-187">Entire previous fiscal year</span></span></p></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="1e85f-188">-1FY</span><span class="sxs-lookup"><span data-stu-id="1e85f-188">-1FY</span></span></p></td>
<td><p><span data-ttu-id="1e85f-189">Current period in previous fiscal year</span><span class="sxs-lookup"><span data-stu-id="1e85f-189">Current period in previous fiscal year</span></span></p></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="1e85f-190">-1FY[1..3]</span><span class="sxs-lookup"><span data-stu-id="1e85f-190">-1FY[1..3]</span></span></p></td>
<td><p><span data-ttu-id="1e85f-191">First quarter of previous fiscal year</span><span class="sxs-lookup"><span data-stu-id="1e85f-191">First quarter of previous fiscal year</span></span></p></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="1e85f-192">-1FY[1..CP]</span><span class="sxs-lookup"><span data-stu-id="1e85f-192">-1FY[1..CP]</span></span></p></td>
<td><p><span data-ttu-id="1e85f-193">From the beginning of previous fiscal year to current period in previous fiscal year, inclusive</span><span class="sxs-lookup"><span data-stu-id="1e85f-193">From the beginning of previous fiscal year to current period in previous fiscal year, inclusive</span></span></p></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="1e85f-194">-1FY[CP..LP]</span><span class="sxs-lookup"><span data-stu-id="1e85f-194">-1FY[CP..LP]</span></span></p></td>
<td><p><span data-ttu-id="1e85f-195">From current period in previous fiscal year to last period of previous fiscal year, inclusive</span><span class="sxs-lookup"><span data-stu-id="1e85f-195">From current period in previous fiscal year to last period of previous fiscal year, inclusive</span></span></p></td>
</tr>
</tbody>
</table>

<span data-ttu-id="1e85f-196">If you want to calculate by regular time periods, you must enter a formula in the **Comparison Date Formula** field instead.</span><span class="sxs-lookup"><span data-stu-id="1e85f-196">If you want to calculate by regular time periods, you must enter a formula in the **Comparison Date Formula** field instead.</span></span>

> [!NOTE]
> <span data-ttu-id="1e85f-197">It is not always transparent which periods you are comparing because you can set a date filter on a report that spans different dates than the accounting periods that are reflected in the data in the chart of accounts.</span><span class="sxs-lookup"><span data-stu-id="1e85f-197">It is not always transparent which periods you are comparing because you can set a date filter on a report that spans different dates than the accounting periods that are reflected in the data in the chart of accounts.</span></span> <span data-ttu-id="1e85f-198">For example, you create an account schedule where you want to compare this period with the same period last year, so you set the **Comparison Date Period Filter** field to *-1FY*.</span><span class="sxs-lookup"><span data-stu-id="1e85f-198">For example, you create an account schedule where you want to compare this period with the same period last year, so you set the **Comparison Date Period Filter** field to *-1FY*.</span></span> <span data-ttu-id="1e85f-199">Then, you run the report on February 28th and set the date filter to January and February.</span><span class="sxs-lookup"><span data-stu-id="1e85f-199">Then, you run the report on February 28th and set the date filter to January and February.</span></span> <span data-ttu-id="1e85f-200">As a result, the account schedule compares January and February this year to January last year, which is the only completed accounting period of the two for last year.</span><span class="sxs-lookup"><span data-stu-id="1e85f-200">As a result, the account schedule compares January and February this year to January last year, which is the only completed accounting period of the two for last year.</span></span>  


## <a name="see-also"></a><span data-ttu-id="1e85f-201">See Also</span><span class="sxs-lookup"><span data-stu-id="1e85f-201">See Also</span></span>
[<span data-ttu-id="1e85f-202">Business Intelligence</span><span class="sxs-lookup"><span data-stu-id="1e85f-202">Business Intelligence</span></span>](bi.md)  
[<span data-ttu-id="1e85f-203">Finance</span><span class="sxs-lookup"><span data-stu-id="1e85f-203">Finance</span></span>](finance.md)  
[<span data-ttu-id="1e85f-204">Setting Up Finance</span><span class="sxs-lookup"><span data-stu-id="1e85f-204">Setting Up Finance</span></span>](finance-setup-finance.md)  
[<span data-ttu-id="1e85f-205">The General Ledger and the Chart of Accounts</span><span class="sxs-lookup"><span data-stu-id="1e85f-205">The General Ledger and the Chart of Accounts</span></span>](finance-general-ledger.md)  
<span data-ttu-id="1e85f-206">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="1e85f-206">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  

