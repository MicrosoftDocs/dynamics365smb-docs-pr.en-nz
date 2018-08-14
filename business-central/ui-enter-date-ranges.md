---
title: Setting date ranges in Business Central  | Microsoft Docs
description: Learn about getting a report to show data from specific time periods using date ranges in Business Central .
documentationcenter: 
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: dates, reporting, filter
ms.date: 07/05/2018
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: d7664360941313da6ea0b797ef00df2e9810ad62
ms.openlocfilehash: ff63ae71a78f956dddb7b5247ee66f9416cf7cf1
ms.contentlocale: en-nz
ms.lasthandoff: 07/09/2018

---
# <a name="entering-date-ranges"></a><span data-ttu-id="3863a-103">Entering Date Ranges</span><span class="sxs-lookup"><span data-stu-id="3863a-103">Entering Date Ranges</span></span>
<span data-ttu-id="3863a-104">You can set filters containing a start date and an end date to display only the data contained in that date range or time interval.</span><span class="sxs-lookup"><span data-stu-id="3863a-104">You can set filters containing a start date and an end date to display only the data contained in that date range or time interval.</span></span> <span data-ttu-id="3863a-105">Special rules apply to the way you set date ranges.</span><span class="sxs-lookup"><span data-stu-id="3863a-105">Special rules apply to the way you set date ranges.</span></span> <span data-ttu-id="3863a-106">Let's take the **Customer Top 10** as an example:</span><span class="sxs-lookup"><span data-stu-id="3863a-106">Let's take the **Customer Top 10** as an example:</span></span>

![Setting a date range in the request page for the Customer Top 10 list](./media/ui-enter-date-ranges/customer-top10-list.png)

<span data-ttu-id="3863a-108">Here you can limit the report to a date range such as the past 2 weeks, or a total of 6 weeks, or whatever range you want.</span><span class="sxs-lookup"><span data-stu-id="3863a-108">Here you can limit the report to a date range such as the past 2 weeks, or a total of 6 weeks, or whatever range you want.</span></span> <span data-ttu-id="3863a-109">To set date ranges, you enter dates and then use either **..**</span><span class="sxs-lookup"><span data-stu-id="3863a-109">To set date ranges, you enter dates and then use either **..**</span></span> <span data-ttu-id="3863a-110">or **|** to set the range.</span><span class="sxs-lookup"><span data-stu-id="3863a-110">or **|** to set the range.</span></span> <span data-ttu-id="3863a-111">In our example, to show the top 10 customers for the first two weeks of May, you would set the date filter to *05 01 17..05 14 17*.</span><span class="sxs-lookup"><span data-stu-id="3863a-111">In our example, to show the top 10 customers for the first two weeks of May, you would set the date filter to *05 01 17..05 14 17*.</span></span>
<span data-ttu-id="3863a-112">Here are a couple of other examples:</span><span class="sxs-lookup"><span data-stu-id="3863a-112">Here are a couple of other examples:</span></span>

| <span data-ttu-id="3863a-113">Meaning</span><span class="sxs-lookup"><span data-stu-id="3863a-113">Meaning</span></span> | <span data-ttu-id="3863a-114">Example</span><span class="sxs-lookup"><span data-stu-id="3863a-114">Example</span></span> | <span data-ttu-id="3863a-115">Entries included</span><span class="sxs-lookup"><span data-stu-id="3863a-115">Entries included</span></span> |
|---|---|---|
|<span data-ttu-id="3863a-116">Equal to</span><span class="sxs-lookup"><span data-stu-id="3863a-116">Equal to</span></span>| <span data-ttu-id="3863a-117">12 15 16</span><span class="sxs-lookup"><span data-stu-id="3863a-117">12 15 16</span></span> |<span data-ttu-id="3863a-118">Only those posted on December 15 2016.</span><span class="sxs-lookup"><span data-stu-id="3863a-118">Only those posted on December 15 2016.</span></span>|
|<span data-ttu-id="3863a-119">Interval</span><span class="sxs-lookup"><span data-stu-id="3863a-119">Interval</span></span>| <span data-ttu-id="3863a-120">12 15 16..01 15 17</span><span class="sxs-lookup"><span data-stu-id="3863a-120">12 15 16..01 15 17</span></span><br /><br /><span data-ttu-id="3863a-121">..12 15 16</span><span class="sxs-lookup"><span data-stu-id="3863a-121">..12 15 16</span></span>|<span data-ttu-id="3863a-122">Those posted on dates between and including December 15 2016 and January 15 2017.</span><span class="sxs-lookup"><span data-stu-id="3863a-122">Those posted on dates between and including December 15 2016 and January 15 2017.</span></span><br /><br /><span data-ttu-id="3863a-123">Those posted on December 15 2016 or earlier.</span><span class="sxs-lookup"><span data-stu-id="3863a-123">Those posted on December 15 2016 or earlier.</span></span>|
|<span data-ttu-id="3863a-124">Either/or</span><span class="sxs-lookup"><span data-stu-id="3863a-124">Either/or</span></span>|<span data-ttu-id="3863a-125">12 15 16&#124;12 16 16</span><span class="sxs-lookup"><span data-stu-id="3863a-125">12 15 16&#124;12 16 16</span></span>|<span data-ttu-id="3863a-126">Those posted on either December 15 or December 16 2016.</span><span class="sxs-lookup"><span data-stu-id="3863a-126">Those posted on either December 15 or December 16 2016.</span></span> <span data-ttu-id="3863a-127">If there are entries posted on both days, they will all be displayed.</span><span class="sxs-lookup"><span data-stu-id="3863a-127">If there are entries posted on both days, they will all be displayed.</span></span>|

<span data-ttu-id="3863a-128">You can also combine the various format types.</span><span class="sxs-lookup"><span data-stu-id="3863a-128">You can also combine the various format types.</span></span>

| <span data-ttu-id="3863a-129">Example</span><span class="sxs-lookup"><span data-stu-id="3863a-129">Example</span></span> | <span data-ttu-id="3863a-130">Entries included</span><span class="sxs-lookup"><span data-stu-id="3863a-130">Entries included</span></span> |
|---|---|
|<span data-ttu-id="3863a-131">12 15 16&#124;12 01 16..05 31 17</span><span class="sxs-lookup"><span data-stu-id="3863a-131">12 15 16&#124;12 01 16..05 31 17</span></span> | <span data-ttu-id="3863a-132">Entries posted either on December 15 2016 or on dates between and including December 01 2016 and May 31 2017.</span><span class="sxs-lookup"><span data-stu-id="3863a-132">Entries posted either on December 15 2016 or on dates between and including December 01 2016 and May 31 2017.</span></span> |
|<span data-ttu-id="3863a-133">..12 14 16&#124;12 30 16..</span><span class="sxs-lookup"><span data-stu-id="3863a-133">..12 14 16&#124;12 30 16..</span></span> | <span data-ttu-id="3863a-134">Entries posted on December 14 or earlier, or entries posted on December 30 or later - that is, all entries except those posted on dates between and including December 15 and 29.</span><span class="sxs-lookup"><span data-stu-id="3863a-134">Entries posted on December 14 or earlier, or entries posted on December 30 or later - that is, all entries except those posted on dates between and including December 15 and 29.</span></span> |

<span data-ttu-id="3863a-135">Note that we have used the US date format MMDDYY here.</span><span class="sxs-lookup"><span data-stu-id="3863a-135">Note that we have used the US date format MMDDYY here.</span></span> <span data-ttu-id="3863a-136">As [!INCLUDE[d365fin](includes/d365fin_md.md)] becomes available in other markets, you'll be able to use the formats that you are used to.</span><span class="sxs-lookup"><span data-stu-id="3863a-136">As [!INCLUDE[d365fin](includes/d365fin_md.md)] becomes available in other markets, you'll be able to use the formats that you are used to.</span></span>

## <a name="using-date-formulas"></a><span data-ttu-id="3863a-137">Using Date Formulas</span><span class="sxs-lookup"><span data-stu-id="3863a-137">Using Date Formulas</span></span>
<span data-ttu-id="3863a-138">A date formula is a short, abbreviated combination of letters and numbers that specifies how to calculate dates.</span><span class="sxs-lookup"><span data-stu-id="3863a-138">A date formula is a short, abbreviated combination of letters and numbers that specifies how to calculate dates.</span></span> <span data-ttu-id="3863a-139">You can enter date formulas in various date calculation fields and in recurring frequency fields in recurring journals.</span><span class="sxs-lookup"><span data-stu-id="3863a-139">You can enter date formulas in various date calculation fields and in recurring frequency fields in recurring journals.</span></span>

> [!NOTE]
>  <span data-ttu-id="3863a-140">In all data formula fields, one day is automatically included to cover today as the day when the period starts.</span><span class="sxs-lookup"><span data-stu-id="3863a-140">In all data formula fields, one day is automatically included to cover today as the day when the period starts.</span></span> <span data-ttu-id="3863a-141">Accordingly, for example, if you enter **1W**, then the period is actually eight days because today is included.</span><span class="sxs-lookup"><span data-stu-id="3863a-141">Accordingly, for example, if you enter **1W**, then the period is actually eight days because today is included.</span></span> <span data-ttu-id="3863a-142">To specify a period of seven days (one true week) including the period starting date, then you must enter **6D** or **1W\-1D**.</span><span class="sxs-lookup"><span data-stu-id="3863a-142">To specify a period of seven days (one true week) including the period starting date, then you must enter **6D** or **1W\-1D**.</span></span>

<span data-ttu-id="3863a-143">Here are some examples of how date formulas can be used:</span><span class="sxs-lookup"><span data-stu-id="3863a-143">Here are some examples of how date formulas can be used:</span></span>

-   <span data-ttu-id="3863a-144">The date formula in the recurring frequency field in recurring journals determines how often the entry on the journal line will be posted.</span><span class="sxs-lookup"><span data-stu-id="3863a-144">The date formula in the recurring frequency field in recurring journals determines how often the entry on the journal line will be posted.</span></span>

-   <span data-ttu-id="3863a-145">The date formula in the **Grace Period** field for a specified reminder level determines the period of time that must pass from the due date (or from the due date of the previous reminder) before a reminder will be created.</span><span class="sxs-lookup"><span data-stu-id="3863a-145">The date formula in the **Grace Period** field for a specified reminder level determines the period of time that must pass from the due date (or from the due date of the previous reminder) before a reminder will be created.</span></span>

-   <span data-ttu-id="3863a-146">The date formula in the **Due Date Calculation** field determines how to calculate the due date on the reminder.</span><span class="sxs-lookup"><span data-stu-id="3863a-146">The date formula in the **Due Date Calculation** field determines how to calculate the due date on the reminder.</span></span>

<span data-ttu-id="3863a-147">The date calculation formula can contain a maximum of 20 characters, both numbers and letters.</span><span class="sxs-lookup"><span data-stu-id="3863a-147">The date calculation formula can contain a maximum of 20 characters, both numbers and letters.</span></span> <span data-ttu-id="3863a-148">You can use the following letters, which are abbreviations for time specifications.</span><span class="sxs-lookup"><span data-stu-id="3863a-148">You can use the following letters, which are abbreviations for time specifications.</span></span>

|  <span data-ttu-id="3863a-149">Letter</span><span class="sxs-lookup"><span data-stu-id="3863a-149">Letter</span></span>  |  <span data-ttu-id="3863a-150">Time specification</span><span class="sxs-lookup"><span data-stu-id="3863a-150">Time specification</span></span>  |
|----------|----------------------|
|<span data-ttu-id="3863a-151">C</span><span class="sxs-lookup"><span data-stu-id="3863a-151">C</span></span>|<span data-ttu-id="3863a-152">Current</span><span class="sxs-lookup"><span data-stu-id="3863a-152">Current</span></span>|
|<span data-ttu-id="3863a-153">D</span><span class="sxs-lookup"><span data-stu-id="3863a-153">D</span></span>|<span data-ttu-id="3863a-154">Day\(s\)</span><span class="sxs-lookup"><span data-stu-id="3863a-154">Day\(s\)</span></span>|
|<span data-ttu-id="3863a-155">W</span><span class="sxs-lookup"><span data-stu-id="3863a-155">W</span></span>|<span data-ttu-id="3863a-156">Week\(s\)</span><span class="sxs-lookup"><span data-stu-id="3863a-156">Week\(s\)</span></span>|
|<span data-ttu-id="3863a-157">M</span><span class="sxs-lookup"><span data-stu-id="3863a-157">M</span></span>|<span data-ttu-id="3863a-158">Month\(s\)</span><span class="sxs-lookup"><span data-stu-id="3863a-158">Month\(s\)</span></span>|
|<span data-ttu-id="3863a-159">Q</span><span class="sxs-lookup"><span data-stu-id="3863a-159">Q</span></span>|<span data-ttu-id="3863a-160">Quarter\(s\)</span><span class="sxs-lookup"><span data-stu-id="3863a-160">Quarter\(s\)</span></span>|
|<span data-ttu-id="3863a-161">Y</span><span class="sxs-lookup"><span data-stu-id="3863a-161">Y</span></span>|<span data-ttu-id="3863a-162">Year\(s\)</span><span class="sxs-lookup"><span data-stu-id="3863a-162">Year\(s\)</span></span>|

<span data-ttu-id="3863a-163">You can construct a date formula in three ways.</span><span class="sxs-lookup"><span data-stu-id="3863a-163">You can construct a date formula in three ways.</span></span>

<span data-ttu-id="3863a-164">The following example shows how to use **C**, for current, and a time unit.</span><span class="sxs-lookup"><span data-stu-id="3863a-164">The following example shows how to use **C**, for current, and a time unit.</span></span>

|  <span data-ttu-id="3863a-165">Expression</span><span class="sxs-lookup"><span data-stu-id="3863a-165">Expression</span></span>  |  <span data-ttu-id="3863a-166">Meaning</span><span class="sxs-lookup"><span data-stu-id="3863a-166">Meaning</span></span>  |
|--------------|-----------|
|<span data-ttu-id="3863a-167">CW</span><span class="sxs-lookup"><span data-stu-id="3863a-167">CW</span></span>|<span data-ttu-id="3863a-168">Current week</span><span class="sxs-lookup"><span data-stu-id="3863a-168">Current week</span></span>|
|<span data-ttu-id="3863a-169">CM</span><span class="sxs-lookup"><span data-stu-id="3863a-169">CM</span></span>|<span data-ttu-id="3863a-170">Current month</span><span class="sxs-lookup"><span data-stu-id="3863a-170">Current month</span></span>|

<span data-ttu-id="3863a-171">The following example shows how to use a number and a time unit.</span><span class="sxs-lookup"><span data-stu-id="3863a-171">The following example shows how to use a number and a time unit.</span></span> <span data-ttu-id="3863a-172">A number cannot be larger than 9999.</span><span class="sxs-lookup"><span data-stu-id="3863a-172">A number cannot be larger than 9999.</span></span>

|  <span data-ttu-id="3863a-173">Expression</span><span class="sxs-lookup"><span data-stu-id="3863a-173">Expression</span></span>  |  <span data-ttu-id="3863a-174">Meaning</span><span class="sxs-lookup"><span data-stu-id="3863a-174">Meaning</span></span>  |
|--------------|-----------|
|<span data-ttu-id="3863a-175">10D</span><span class="sxs-lookup"><span data-stu-id="3863a-175">10D</span></span>|<span data-ttu-id="3863a-176">10 days from today</span><span class="sxs-lookup"><span data-stu-id="3863a-176">10 days from today</span></span>|
|<span data-ttu-id="3863a-177">2W</span><span class="sxs-lookup"><span data-stu-id="3863a-177">2W</span></span>|<span data-ttu-id="3863a-178">2 weeks from today</span><span class="sxs-lookup"><span data-stu-id="3863a-178">2 weeks from today</span></span>|

<span data-ttu-id="3863a-179">The following example shows how to use a time unit and a number.</span><span class="sxs-lookup"><span data-stu-id="3863a-179">The following example shows how to use a time unit and a number.</span></span>

|  <span data-ttu-id="3863a-180">Expression</span><span class="sxs-lookup"><span data-stu-id="3863a-180">Expression</span></span>  |  <span data-ttu-id="3863a-181">Meaning</span><span class="sxs-lookup"><span data-stu-id="3863a-181">Meaning</span></span>  |
|--------------|-----------|
|<span data-ttu-id="3863a-182">D10</span><span class="sxs-lookup"><span data-stu-id="3863a-182">D10</span></span>|<span data-ttu-id="3863a-183">The next 10th day of a month</span><span class="sxs-lookup"><span data-stu-id="3863a-183">The next 10th day of a month</span></span>|
|<span data-ttu-id="3863a-184">WD4</span><span class="sxs-lookup"><span data-stu-id="3863a-184">WD4</span></span>|<span data-ttu-id="3863a-185">The next 4th day of a week \(Thursday\)</span><span class="sxs-lookup"><span data-stu-id="3863a-185">The next 4th day of a week \(Thursday\)</span></span>|

<span data-ttu-id="3863a-186">The following example shows how you can combine these three forms as needed.</span><span class="sxs-lookup"><span data-stu-id="3863a-186">The following example shows how you can combine these three forms as needed.</span></span>

|  <span data-ttu-id="3863a-187">Expression</span><span class="sxs-lookup"><span data-stu-id="3863a-187">Expression</span></span>  |  <span data-ttu-id="3863a-188">Meaning</span><span class="sxs-lookup"><span data-stu-id="3863a-188">Meaning</span></span>  |
|--------------|-----------|
|<span data-ttu-id="3863a-189">CM\+10D</span><span class="sxs-lookup"><span data-stu-id="3863a-189">CM\+10D</span></span>|<span data-ttu-id="3863a-190">Current month \+ 10 days</span><span class="sxs-lookup"><span data-stu-id="3863a-190">Current month \+ 10 days</span></span>|

<span data-ttu-id="3863a-191">The following example shows how you can use a minus sign to indicate a date in the past.</span><span class="sxs-lookup"><span data-stu-id="3863a-191">The following example shows how you can use a minus sign to indicate a date in the past.</span></span>

|  <span data-ttu-id="3863a-192">Expression</span><span class="sxs-lookup"><span data-stu-id="3863a-192">Expression</span></span>  |  <span data-ttu-id="3863a-193">Meaning</span><span class="sxs-lookup"><span data-stu-id="3863a-193">Meaning</span></span>  |
|--------------|-----------|
|<span data-ttu-id="3863a-194">-1Y</span><span class="sxs-lookup"><span data-stu-id="3863a-194">-1Y</span></span>|<span data-ttu-id="3863a-195">1 year ago from today</span><span class="sxs-lookup"><span data-stu-id="3863a-195">1 year ago from today</span></span>|

> [!IMPORTANT]
>  <span data-ttu-id="3863a-196">If the location uses a base calendar, then the date formula that you enter in, for example, the **Shipping Time** field is interpreted according to the calendar working days.</span><span class="sxs-lookup"><span data-stu-id="3863a-196">If the location uses a base calendar, then the date formula that you enter in, for example, the **Shipping Time** field is interpreted according to the calendar working days.</span></span> <span data-ttu-id="3863a-197">For example, **1W**  means seven working days.</span><span class="sxs-lookup"><span data-stu-id="3863a-197">For example, **1W**  means seven working days.</span></span>

## <a name="see-also"></a><span data-ttu-id="3863a-198">See Also</span><span class="sxs-lookup"><span data-stu-id="3863a-198">See Also</span></span>
<span data-ttu-id="3863a-199">[Working with [!INCLUDE[d365fin](includes/d365fin_long_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="3863a-199">[Working with [!INCLUDE[d365fin](includes/d365fin_long_md.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="3863a-200">Date Calculation for Purchases</span><span class="sxs-lookup"><span data-stu-id="3863a-200">Date Calculation for Purchases</span></span>](purchasing-date-calculation-for-purchases.md)  
[<span data-ttu-id="3863a-201">Entering Criteria in Filters</span><span class="sxs-lookup"><span data-stu-id="3863a-201">Entering Criteria in Filters </span></span>](ui-enter-criteria-filters.md)  

