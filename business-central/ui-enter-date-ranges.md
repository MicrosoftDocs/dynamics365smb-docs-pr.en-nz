---
title: Entering dates and times in Business Central  | Microsoft Docs
description: Learn how to enter dates and times including various productivity tips such as shorthand, expressions and ranges. Filter lists or reports down to specific date or time periods.
documentationcenter: ''
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: dates, reporting, filter, calendar, shorthand, range
ms.date: 04/01/2019
ms.author: jswymer
ms.openlocfilehash: c7e80edfd796056176d37ad12a56c76e64bb44e6
ms.sourcegitcommit: bd78a5d990c9e83174da1409076c22df8b35eafd
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 03/31/2019
ms.locfileid: "932994"
---
# <a name="working-with-calendar-dates-and-times"></a><span data-ttu-id="c040d-104">Working with Calendar Dates and Times</span><span class="sxs-lookup"><span data-stu-id="c040d-104">Working with Calendar Dates and Times</span></span>

[!INCLUDE[d365fin](includes/d365fin_long_md.md)] <span data-ttu-id="c040d-105">offers multiple ways to enter dates and times, including powerful features that accelerate data entry, or help you write complex calendar expressions.</span><span class="sxs-lookup"><span data-stu-id="c040d-105">offers multiple ways to enter dates and times, including powerful features that accelerate data entry, or help you write complex calendar expressions.</span></span> <span data-ttu-id="c040d-106">There are various places throughout the application where you can enter dates and times in fields.</span><span class="sxs-lookup"><span data-stu-id="c040d-106">There are various places throughout the application where you can enter dates and times in fields.</span></span> <span data-ttu-id="c040d-107">For example, on a sales order, you can set the shipment date.</span><span class="sxs-lookup"><span data-stu-id="c040d-107">For example, on a sales order, you can set the shipment date.</span></span> <span data-ttu-id="c040d-108">When filtering lists or report data, you can enter dates and times to pinpoint only the data that you are interested in.</span><span class="sxs-lookup"><span data-stu-id="c040d-108">When filtering lists or report data, you can enter dates and times to pinpoint only the data that you are interested in.</span></span>

## <a name="check-your-region-and-language-settings"></a><span data-ttu-id="c040d-109">Check your region and language settings</span><span class="sxs-lookup"><span data-stu-id="c040d-109">Check your region and language settings</span></span>

<span data-ttu-id="c040d-110">The [**My Settings**](https://businesscentral.dynamics.com?page=9176 "Go directly to your user settings page in Business Central") page specifies the **Region** and **Language** that you are using in the application.</span><span class="sxs-lookup"><span data-stu-id="c040d-110">The [**My Settings**](https://businesscentral.dynamics.com?page=9176 "Go directly to your user settings page in Business Central") page specifies the **Region** and **Language** that you are using in the application.</span></span> <span data-ttu-id="c040d-111">These settings influence how you enter dates and times.</span><span class="sxs-lookup"><span data-stu-id="c040d-111">These settings influence how you enter dates and times.</span></span> 

-   <span data-ttu-id="c040d-112">The **Region** setting determines how dates, times, numbers, and currencies are shown or formatted.</span><span class="sxs-lookup"><span data-stu-id="c040d-112">The **Region** setting determines how dates, times, numbers, and currencies are shown or formatted.</span></span>

-   <span data-ttu-id="c040d-113">For date patterns that involve words, the language of the words that you use must correspond to the **Language** setting.</span><span class="sxs-lookup"><span data-stu-id="c040d-113">For date patterns that involve words, the language of the words that you use must correspond to the **Language** setting.</span></span>

> [!NOTE]
> [!INCLUDE[d365fin](includes/d365fin_long_md.md)] <span data-ttu-id="c040d-114">uses the Gregorian calendar system.</span><span class="sxs-lookup"><span data-stu-id="c040d-114">uses the Gregorian calendar system.</span></span>

<!-- 
The following sections describe how you can enter dates, times, datetimes, durations, date ranges, and how you use date formulas.
-->

## <a name="entering-dates"></a><span data-ttu-id="c040d-115">Entering Dates</span><span class="sxs-lookup"><span data-stu-id="c040d-115">Entering Dates</span></span>

<span data-ttu-id="c040d-116">In a date field, you can enter a date using the standard format for your region setting.</span><span class="sxs-lookup"><span data-stu-id="c040d-116">In a date field, you can enter a date using the standard format for your region setting.</span></span> <span data-ttu-id="c040d-117">Different regions can use different separators between the days, months and years.</span><span class="sxs-lookup"><span data-stu-id="c040d-117">Different regions can use different separators between the days, months and years.</span></span> <span data-ttu-id="c040d-118">For example, some regions use dashes (mm-dd-yyyy) and others use forward slashes (mm/dd/yyyy).</span><span class="sxs-lookup"><span data-stu-id="c040d-118">For example, some regions use dashes (mm-dd-yyyy) and others use forward slashes (mm/dd/yyyy).</span></span> <span data-ttu-id="c040d-119">However, you can use any separators, even a space, and the date will automatically be changed to use separators that match your region.</span><span class="sxs-lookup"><span data-stu-id="c040d-119">However, you can use any separators, even a space, and the date will automatically be changed to use separators that match your region.</span></span>

<span data-ttu-id="c040d-120">Note that the format in which dates are displayed on printed reports or emailed documents is not influenced by your personal choice of region setting.</span><span class="sxs-lookup"><span data-stu-id="c040d-120">Note that the format in which dates are displayed on printed reports or emailed documents is not influenced by your personal choice of region setting.</span></span>

<span data-ttu-id="c040d-121">To work more productively with dates and times, you can use any of the methods or formats that are described in the following sections.</span><span class="sxs-lookup"><span data-stu-id="c040d-121">To work more productively with dates and times, you can use any of the methods or formats that are described in the following sections.</span></span> 

### <a name="picking-dates-from-the-calendar"></a><span data-ttu-id="c040d-122">Picking dates from the calendar</span><span class="sxs-lookup"><span data-stu-id="c040d-122">Picking dates from the calendar</span></span>

<span data-ttu-id="c040d-123">Any field displaying a calendar icon can be set using the calendar date picker.</span><span class="sxs-lookup"><span data-stu-id="c040d-123">Any field displaying a calendar icon can be set using the calendar date picker.</span></span> <span data-ttu-id="c040d-124">To display the calendar date picker, activate the calendar icon or press the Ctrl + Home keyboard shortcut in the field.</span><span class="sxs-lookup"><span data-stu-id="c040d-124">To display the calendar date picker, activate the calendar icon or press the Ctrl + Home keyboard shortcut in the field.</span></span>

<span data-ttu-id="c040d-125">![Date fields](media/ui-date-field.png "Example of a date field")</span><span class="sxs-lookup"><span data-stu-id="c040d-125">![Date fields](media/ui-date-field.png "Example of a date field")</span></span>

<span data-ttu-id="c040d-126">See also [Keyboard Shortcuts in the calendar date picker](keyboard-shortcuts.md#calendarshortcuts)</span><span class="sxs-lookup"><span data-stu-id="c040d-126">See also [Keyboard Shortcuts in the calendar date picker](keyboard-shortcuts.md#calendarshortcuts)</span></span>

### <a name="day-week-year-pattern"></a><span data-ttu-id="c040d-127">Day\-week\-year pattern</span><span class="sxs-lookup"><span data-stu-id="c040d-127">Day\-week\-year pattern</span></span>

<span data-ttu-id="c040d-128">You can enter a date as a weekday followed by a week number and, optionally, a year.</span><span class="sxs-lookup"><span data-stu-id="c040d-128">You can enter a date as a weekday followed by a week number and, optionally, a year.</span></span> <span data-ttu-id="c040d-129">For example, `Mon25` or `mon25` means Monday in week 25.</span><span class="sxs-lookup"><span data-stu-id="c040d-129">For example, `Mon25` or `mon25` means Monday in week 25.</span></span> <span data-ttu-id="c040d-130">If you do not enter a year, the year of the work date is used.</span><span class="sxs-lookup"><span data-stu-id="c040d-130">If you do not enter a year, the year of the work date is used.</span></span>

<span data-ttu-id="c040d-131">Instead of entering the entire word for the day of the week, you can enter part of the word, starting from the beginning.</span><span class="sxs-lookup"><span data-stu-id="c040d-131">Instead of entering the entire word for the day of the week, you can enter part of the word, starting from the beginning.</span></span> <span data-ttu-id="c040d-132">In case of conflicts (such as with `s` which could be Saturday or Sunday), the days are evaluated according to the region setting.</span><span class="sxs-lookup"><span data-stu-id="c040d-132">In case of conflicts (such as with `s` which could be Saturday or Sunday), the days are evaluated according to the region setting.</span></span> <span data-ttu-id="c040d-133">The input is first evaluated against `workdate` and `today` as well, so keep this in mind when abbreviating.</span><span class="sxs-lookup"><span data-stu-id="c040d-133">The input is first evaluated against `workdate` and `today` as well, so keep this in mind when abbreviating.</span></span> <span data-ttu-id="c040d-134">For example, `t` already means today, so it cannot mean Tuesday or Thursday.</span><span class="sxs-lookup"><span data-stu-id="c040d-134">For example, `t` already means today, so it cannot mean Tuesday or Thursday.</span></span>

<span data-ttu-id="c040d-135">The week number scheme is always ISO 8601, where week 1 is the week with 4 January in it, or the week with the first Thursday of the year.</span><span class="sxs-lookup"><span data-stu-id="c040d-135">The week number scheme is always ISO 8601, where week 1 is the week with 4 January in it, or the week with the first Thursday of the year.</span></span>

### <a name="digit-patterns"></a><span data-ttu-id="c040d-136">Digit patterns</span><span class="sxs-lookup"><span data-stu-id="c040d-136">Digit patterns</span></span>

<span data-ttu-id="c040d-137">In a date field you can enter two, four, six, or eight digits:</span><span class="sxs-lookup"><span data-stu-id="c040d-137">In a date field you can enter two, four, six, or eight digits:</span></span>

-   <span data-ttu-id="c040d-138">If you enter only two digits, this is interpreted as the day, and it will add the month and the year of the work date.</span><span class="sxs-lookup"><span data-stu-id="c040d-138">If you enter only two digits, this is interpreted as the day, and it will add the month and the year of the work date.</span></span>

-   <span data-ttu-id="c040d-139">If you enter four digits, this is interpreted as the day and the month, and it will add the year of the work date.</span><span class="sxs-lookup"><span data-stu-id="c040d-139">If you enter four digits, this is interpreted as the day and the month, and it will add the year of the work date.</span></span> <span data-ttu-id="c040d-140">The order of the day and month is determined by your region settings.</span><span class="sxs-lookup"><span data-stu-id="c040d-140">The order of the day and month is determined by your region settings.</span></span> <span data-ttu-id="c040d-141">Even if your region settings have the year before the day and month, four digits are interpreted as the day and month.</span><span class="sxs-lookup"><span data-stu-id="c040d-141">Even if your region settings have the year before the day and month, four digits are interpreted as the day and month.</span></span>

-   <span data-ttu-id="c040d-142">If the date you want to enter is in the range 01/01/1930 through 12/31/2029, you can enter the year with two digits; otherwise, enter the year with four digits.</span><span class="sxs-lookup"><span data-stu-id="c040d-142">If the date you want to enter is in the range 01/01/1930 through 12/31/2029, you can enter the year with two digits; otherwise, enter the year with four digits.</span></span>

### <a name="today"></a><span data-ttu-id="c040d-143">Today</span><span class="sxs-lookup"><span data-stu-id="c040d-143">Today</span></span>

<span data-ttu-id="c040d-144">Enter the word for `today`, in the language set by **Language** setting, that will set the date to the current date.</span><span class="sxs-lookup"><span data-stu-id="c040d-144">Enter the word for `today`, in the language set by **Language** setting, that will set the date to the current date.</span></span> <span data-ttu-id="c040d-145">Instead of entering the entire word, you can enter part of the word, starting from the beginning, such as `t` or `tod`, as long as it is not also the start of another word.</span><span class="sxs-lookup"><span data-stu-id="c040d-145">Instead of entering the entire word, you can enter part of the word, starting from the beginning, such as `t` or `tod`, as long as it is not also the start of another word.</span></span>

### <a name="period"></a><span data-ttu-id="c040d-146">Period</span><span class="sxs-lookup"><span data-stu-id="c040d-146">Period</span></span>

<span data-ttu-id="c040d-147">To filter on a specific accounting period, in a date field enter the letter `p`, or the word `period`, followed by a number that identifies the accounting period, like `p2` or `period4`.</span><span class="sxs-lookup"><span data-stu-id="c040d-147">To filter on a specific accounting period, in a date field enter the letter `p`, or the word `period`, followed by a number that identifies the accounting period, like `p2` or `period4`.</span></span> <span data-ttu-id="c040d-148">The accounting period is relative to the fiscal year of the current work date that set in your Role Centre.</span><span class="sxs-lookup"><span data-stu-id="c040d-148">The accounting period is relative to the fiscal year of the current work date that set in your Role Center.</span></span> <span data-ttu-id="c040d-149">For example, if the work date is **03/21/20**, then `p1`, or just `p`, filters on the first accounting period of the fiscal year 2020 (such as `01/01/20..01/31/20`).</span><span class="sxs-lookup"><span data-stu-id="c040d-149">For example, if the work date is **03/21/20**, then `p1`, or just `p`, filters on the first accounting period of the fiscal year 2020 (such as `01/01/20..01/31/20`).</span></span> <span data-ttu-id="c040d-150">`p15` filters on the fifteenth accounting period from the start of fiscal year 2020 (such as `03/01/21..03/31/21`).</span><span class="sxs-lookup"><span data-stu-id="c040d-150">`p15` filters on the fifteenth accounting period from the start of fiscal year 2020 (such as `03/01/21..03/31/21`).</span></span> 

<span data-ttu-id="c040d-151">The accounting periods are defined on the **Accounting Periods** page.</span><span class="sxs-lookup"><span data-stu-id="c040d-151">The accounting periods are defined on the **Accounting Periods** page.</span></span> <span data-ttu-id="c040d-152">To view or change the accounting periods, open the page [here](https://businesscentral.dynamics.com/?page=100).</span><span class="sxs-lookup"><span data-stu-id="c040d-152">To view or change the accounting periods, open the page [here](https://businesscentral.dynamics.com/?page=100).</span></span>

### <a name="current-work-date"></a><span data-ttu-id="c040d-153">Current work date</span><span class="sxs-lookup"><span data-stu-id="c040d-153">Current work date</span></span>

<span data-ttu-id="c040d-154">The work date feature allows you to record transactions using a date that is different from the current date.</span><span class="sxs-lookup"><span data-stu-id="c040d-154">The work date feature allows you to record transactions using a date that is different from the current date.</span></span>

<span data-ttu-id="c040d-155">The word for 'workdate', in the language set by **Language** setting, will set the date to the currently set work date that is specified on the [**My Settings**](https://businesscentral.dynamics.com?page=9176 "Go directly to your user settings page in Business Central") page.</span><span class="sxs-lookup"><span data-stu-id="c040d-155">The word for 'workdate', in the language set by **Language** setting, will set the date to the currently set work date that is specified on the [**My Settings**](https://businesscentral.dynamics.com?page=9176 "Go directly to your user settings page in Business Central") page.</span></span> <span data-ttu-id="c040d-156">Instead of entering the entire word, you can enter part of the word, starting from the beginning, such as 'w' or 'work'.</span><span class="sxs-lookup"><span data-stu-id="c040d-156">Instead of entering the entire word, you can enter part of the word, starting from the beginning, such as 'w' or 'work'.</span></span>

<span data-ttu-id="c040d-157">If you have not defined a work date, the current date will be used as the work date.</span><span class="sxs-lookup"><span data-stu-id="c040d-157">If you have not defined a work date, the current date will be used as the work date.</span></span> <span data-ttu-id="c040d-158">You may want to use a work date if you have many transactions with a date other than today's date.</span><span class="sxs-lookup"><span data-stu-id="c040d-158">You may want to use a work date if you have many transactions with a date other than today's date.</span></span>

<span data-ttu-id="c040d-159">See also [Changing Basic Settings, such as the Work Date](ui-change-basic-settings.md#work-date).</span><span class="sxs-lookup"><span data-stu-id="c040d-159">See also [Changing Basic Settings, such as the Work Date](ui-change-basic-settings.md#work-date).</span></span>

### <a name="closing-date"></a><span data-ttu-id="c040d-160">Closing Date</span><span class="sxs-lookup"><span data-stu-id="c040d-160">Closing Date</span></span>

<span data-ttu-id="c040d-161">When you close a fiscal year, you can use closing dates to indicate that an entry is a closing entry.</span><span class="sxs-lookup"><span data-stu-id="c040d-161">When you close a fiscal year, you can use closing dates to indicate that an entry is a closing entry.</span></span> <span data-ttu-id="c040d-162">A closing date technically is between two dates, for example between Dec 31 and Jan 1.</span><span class="sxs-lookup"><span data-stu-id="c040d-162">A closing date technically is between two dates, for example between Dec 31 and Jan 1.</span></span>

<span data-ttu-id="c040d-163">To specify that a date is a closing date, put `C` just before the date, such as `C123101`.</span><span class="sxs-lookup"><span data-stu-id="c040d-163">To specify that a date is a closing date, put `C` just before the date, such as `C123101`.</span></span> <span data-ttu-id="c040d-164">This can be used in combination with all the date patterns.</span><span class="sxs-lookup"><span data-stu-id="c040d-164">This can be used in combination with all the date patterns.</span></span>

### <a name="examples"></a><span data-ttu-id="c040d-165">Examples</span><span class="sxs-lookup"><span data-stu-id="c040d-165">Examples</span></span>

<span data-ttu-id="c040d-166">The following table contains examples of dates using all the formats.</span><span class="sxs-lookup"><span data-stu-id="c040d-166">The following table contains examples of dates using all the formats.</span></span> <span data-ttu-id="c040d-167">It assumes region settings that format dates according to: **year.month.day.**, a week starting on Monday, and the English language.</span><span class="sxs-lookup"><span data-stu-id="c040d-167">It assumes region settings that format dates according to: **year.month.day.**, a week starting on Monday, and the English language.</span></span>

|<span data-ttu-id="c040d-168">**Entry**</span><span class="sxs-lookup"><span data-stu-id="c040d-168">**Entry**</span></span>      |<span data-ttu-id="c040d-169">**Interpretation**</span><span class="sxs-lookup"><span data-stu-id="c040d-169">**Interpretation**</span></span>      |
|---------------|------------------------|
|`2018.12.31.`|<span data-ttu-id="c040d-170">2018.12.31.</span><span class="sxs-lookup"><span data-stu-id="c040d-170">2018.12.31.</span></span>|
|`181231`|<span data-ttu-id="c040d-171">2018.12.31.</span><span class="sxs-lookup"><span data-stu-id="c040d-171">2018.12.31.</span></span>|
|`18.12.31.`|<span data-ttu-id="c040d-172">2018.12.31.</span><span class="sxs-lookup"><span data-stu-id="c040d-172">2018.12.31.</span></span>|
|`18.12.31.`|<span data-ttu-id="c040d-173">2018.12.31.</span><span class="sxs-lookup"><span data-stu-id="c040d-173">2018.12.31.</span></span>|
|`20181231`|<span data-ttu-id="c040d-174">2018.12.31.</span><span class="sxs-lookup"><span data-stu-id="c040d-174">2018.12.31.</span></span>|
|`18/12,31`|<span data-ttu-id="c040d-175">2018.12.31.</span><span class="sxs-lookup"><span data-stu-id="c040d-175">2018.12.31.</span></span>|
|`11`|<span data-ttu-id="c040d-176">work date year.work date month.11.</span><span class="sxs-lookup"><span data-stu-id="c040d-176">work date year.work date month.11.</span></span>|
|`1112`|<span data-ttu-id="c040d-177">work date year.11.12.</span><span class="sxs-lookup"><span data-stu-id="c040d-177">work date year.11.12.</span></span>|
|<span data-ttu-id="c040d-178">`t` or `today`</span><span class="sxs-lookup"><span data-stu-id="c040d-178">`t` or `today`</span></span>|<span data-ttu-id="c040d-179">today's date</span><span class="sxs-lookup"><span data-stu-id="c040d-179">today's date</span></span>|
|`p4`|<span data-ttu-id="c040d-180">date range that includes the fourth accounting period, such as `04/01/20..04/30/20`</span><span class="sxs-lookup"><span data-stu-id="c040d-180">date range that includes the fourth accounting period, such as `04/01/20..04/30/20`</span></span>|
|<span data-ttu-id="c040d-181">`w` or `workdate`</span><span class="sxs-lookup"><span data-stu-id="c040d-181">`w` or `workdate`</span></span>|<span data-ttu-id="c040d-182">the working date</span><span class="sxs-lookup"><span data-stu-id="c040d-182">the working date</span></span>|
|<span data-ttu-id="c040d-183">`m` or `Monday`</span><span class="sxs-lookup"><span data-stu-id="c040d-183">`m` or `Monday`</span></span>|<span data-ttu-id="c040d-184">Monday of the work date week</span><span class="sxs-lookup"><span data-stu-id="c040d-184">Monday of the work date week</span></span>|
|<span data-ttu-id="c040d-185">`tu` or `Tuesday`</span><span class="sxs-lookup"><span data-stu-id="c040d-185">`tu` or `Tuesday`</span></span>|<span data-ttu-id="c040d-186">Tuesday of the work date week</span><span class="sxs-lookup"><span data-stu-id="c040d-186">Tuesday of the work date week</span></span>|
|<span data-ttu-id="c040d-187">`sa` or `Saturday`</span><span class="sxs-lookup"><span data-stu-id="c040d-187">`sa` or `Saturday`</span></span>|<span data-ttu-id="c040d-188">Saturday of the work date week</span><span class="sxs-lookup"><span data-stu-id="c040d-188">Saturday of the work date week</span></span>|
|<span data-ttu-id="c040d-189">`s` or `Sunday`</span><span class="sxs-lookup"><span data-stu-id="c040d-189">`s` or `Sunday`</span></span>|<span data-ttu-id="c040d-190">Sunday of the work date week</span><span class="sxs-lookup"><span data-stu-id="c040d-190">Sunday of the work date week</span></span>|
|`t23`|<span data-ttu-id="c040d-191">Tuesday of week 23 of the work date year</span><span class="sxs-lookup"><span data-stu-id="c040d-191">Tuesday of week 23 of the work date year</span></span>|
|`t 23`|<span data-ttu-id="c040d-192">Tuesday of week 23 of the work date year</span><span class="sxs-lookup"><span data-stu-id="c040d-192">Tuesday of week 23 of the work date year</span></span>|
|`t-1`|<span data-ttu-id="c040d-193">Tuesday of week 1 of the work date year</span><span class="sxs-lookup"><span data-stu-id="c040d-193">Tuesday of week 1 of the work date year</span></span>|

##  <a name="BKMK_SettingDateRanges"></a> <span data-ttu-id="c040d-194">Setting Ranges</span><span class="sxs-lookup"><span data-stu-id="c040d-194">Setting Ranges</span></span>

<span data-ttu-id="c040d-195">On lists, totals and reports, you can set filters on dates, times and datetimes containing a start value and optionally an end value to display only the data contained in that range.</span><span class="sxs-lookup"><span data-stu-id="c040d-195">On lists, totals and reports, you can set filters on dates, times and datetimes containing a start value and optionally an end value to display only the data contained in that range.</span></span> <span data-ttu-id="c040d-196">The standard rules apply to the way you set date ranges.</span><span class="sxs-lookup"><span data-stu-id="c040d-196">The standard rules apply to the way you set date ranges.</span></span>

|<span data-ttu-id="c040d-197">**Meaning**</span><span class="sxs-lookup"><span data-stu-id="c040d-197">**Meaning**</span></span>|<span data-ttu-id="c040d-198">**Sample expression (Date)**</span><span class="sxs-lookup"><span data-stu-id="c040d-198">**Sample expression (Date)**</span></span>|<span data-ttu-id="c040d-199">**Data included in the filter**</span><span class="sxs-lookup"><span data-stu-id="c040d-199">**Data included in the filter**</span></span>|
|-----------|---------------------|--------------------|
|<span data-ttu-id="c040d-200">Interval</span><span class="sxs-lookup"><span data-stu-id="c040d-200">Interval</span></span>|`12 15 00..01 15 01`<br /><br />`..12 15 00`<br /><br />`p1..p4`|<span data-ttu-id="c040d-201">Records with dates between and including 12 15 00 and 01 15 01.</span><span class="sxs-lookup"><span data-stu-id="c040d-201">Records with dates between and including 12 15 00 and 01 15 01.</span></span><br /><br /><span data-ttu-id="c040d-202">Records with dates of 12 15 00 or earlier.</span><span class="sxs-lookup"><span data-stu-id="c040d-202">Records with dates of 12 15 00 or earlier.</span></span><br /><br /><span data-ttu-id="c040d-203">Date range that includes the second, third, and fourth accounting periods, such as `01/01/20..04/30/20`.</span><span class="sxs-lookup"><span data-stu-id="c040d-203">Date range that includes the second, third, and fourth accounting periods, such as `01/01/20..04/30/20`.</span></span>|
|<span data-ttu-id="c040d-204">Either/or</span><span class="sxs-lookup"><span data-stu-id="c040d-204">Either/or</span></span>|`12 15 00|12 16 00`|<span data-ttu-id="c040d-205">Records with dates of either 12 15 00 or 12 16 00.</span><span class="sxs-lookup"><span data-stu-id="c040d-205">Records with dates of either 12 15 00 or 12 16 00.</span></span> <span data-ttu-id="c040d-206">If there are records with dates on both days, they will all be displayed.</span><span class="sxs-lookup"><span data-stu-id="c040d-206">If there are records with dates on both days, they will all be displayed.</span></span>|
|<span data-ttu-id="c040d-207">Combination</span><span class="sxs-lookup"><span data-stu-id="c040d-207">Combination</span></span>|<span data-ttu-id="c040d-208">`12 15 00|12 01 00..12 10 00`  \n`..12 14 00|12 30 00..`</span><span class="sxs-lookup"><span data-stu-id="c040d-208">`12 15 00|12 01 00..12 10 00`  \n`..12 14 00|12 30 00..`</span></span>|<span data-ttu-id="c040d-209">Records with dates of 12 15 00 or on dates between and including 12 01 00 and 12 10 00.</span><span class="sxs-lookup"><span data-stu-id="c040d-209">Records with dates of 12 15 00 or on dates between and including 12 01 00 and 12 10 00.</span></span>  <span data-ttu-id="c040d-210">\nRecords with dates of 12 14 00 or earlier, or dates of 12 30 00 or later, that is, all records except those with dates between and including 12 15 00 and 12 29 00.</span><span class="sxs-lookup"><span data-stu-id="c040d-210">\nRecords with dates of 12 14 00 or earlier, or dates of 12 30 00 or later, that is, all records except those with dates between and including 12 15 00 and 12 29 00.</span></span>|

<span data-ttu-id="c040d-211">You can use any of the valid formats in date range filters.</span><span class="sxs-lookup"><span data-stu-id="c040d-211">You can use any of the valid formats in date range filters.</span></span> <span data-ttu-id="c040d-212">For example, `mon14 3..t 4p` applied on a datetime field results in a filter from 3 AM on Monday in week 14 of the current work date year, inclusive, until today at 4PM, inclusive.</span><span class="sxs-lookup"><span data-stu-id="c040d-212">For example, `mon14 3..t 4p` applied on a datetime field results in a filter from 3 AM on Monday in week 14 of the current work date year, inclusive, until today at 4PM, inclusive.</span></span>

## <a name="using-date-formulas"></a><span data-ttu-id="c040d-213">Using Date Formulas</span><span class="sxs-lookup"><span data-stu-id="c040d-213">Using Date Formulas</span></span>
<span data-ttu-id="c040d-214">A date formula is a short, abbreviated combination of letters and numbers that specifies how to calculate dates.</span><span class="sxs-lookup"><span data-stu-id="c040d-214">A date formula is a short, abbreviated combination of letters and numbers that specifies how to calculate dates.</span></span> <span data-ttu-id="c040d-215">You can enter date formulas in various date calculation fields or filters.</span><span class="sxs-lookup"><span data-stu-id="c040d-215">You can enter date formulas in various date calculation fields or filters.</span></span>

> [!NOTE]
>  <span data-ttu-id="c040d-216">In all data formula fields, one day is automatically included to cover today as the day when the period starts.</span><span class="sxs-lookup"><span data-stu-id="c040d-216">In all data formula fields, one day is automatically included to cover today as the day when the period starts.</span></span> <span data-ttu-id="c040d-217">Accordingly, for example, if you enter `1W`, then the period is actually eight days because today is included.</span><span class="sxs-lookup"><span data-stu-id="c040d-217">Accordingly, for example, if you enter `1W`, then the period is actually eight days because today is included.</span></span> <span data-ttu-id="c040d-218">To specify a period of seven days \(one true week\) including the period starting date, then you must enter `6D` or `1W-1D`.</span><span class="sxs-lookup"><span data-stu-id="c040d-218">To specify a period of seven days \(one true week\) including the period starting date, then you must enter `6D` or `1W-1D`.</span></span>

<span data-ttu-id="c040d-219">Here are some examples of how date formulas can be used:</span><span class="sxs-lookup"><span data-stu-id="c040d-219">Here are some examples of how date formulas can be used:</span></span>

-   <span data-ttu-id="c040d-220">The date formula in the recurring frequency field in recurring journals determines how often the entry on the journal line will be posted.</span><span class="sxs-lookup"><span data-stu-id="c040d-220">The date formula in the recurring frequency field in recurring journals determines how often the entry on the journal line will be posted.</span></span>

-   <span data-ttu-id="c040d-221">The date formula in the **Grace Period** field for a specified reminder level determines the period of time that must pass from the due date \(or from the date of the previous reminder\) before a reminder will be created.</span><span class="sxs-lookup"><span data-stu-id="c040d-221">The date formula in the **Grace Period** field for a specified reminder level determines the period of time that must pass from the due date \(or from the date of the previous reminder\) before a reminder will be created.</span></span>

-   <span data-ttu-id="c040d-222">The date formula in the **Due Date Calculation** field determines how to calculate the due date on the reminder.</span><span class="sxs-lookup"><span data-stu-id="c040d-222">The date formula in the **Due Date Calculation** field determines how to calculate the due date on the reminder.</span></span>

<span data-ttu-id="c040d-223">The date formula can contain a maximum of 20 characters, both numbers and letters.</span><span class="sxs-lookup"><span data-stu-id="c040d-223">The date formula can contain a maximum of 20 characters, both numbers and letters.</span></span> <span data-ttu-id="c040d-224">You can use the following letters, which are abbreviations for calendar units.</span><span class="sxs-lookup"><span data-stu-id="c040d-224">You can use the following letters, which are abbreviations for calendar units.</span></span>

|  <span data-ttu-id="c040d-225">Letter</span><span class="sxs-lookup"><span data-stu-id="c040d-225">Letter</span></span>  |  <span data-ttu-id="c040d-226">Meaning</span><span class="sxs-lookup"><span data-stu-id="c040d-226">Meaning</span></span>  |
|----------|----------------------|
|`C`|<span data-ttu-id="c040d-227">Current</span><span class="sxs-lookup"><span data-stu-id="c040d-227">Current</span></span>|
|`D`|<span data-ttu-id="c040d-228">Day\(s\)</span><span class="sxs-lookup"><span data-stu-id="c040d-228">Day\(s\)</span></span>|
|`W`|<span data-ttu-id="c040d-229">Week\(s\)</span><span class="sxs-lookup"><span data-stu-id="c040d-229">Week\(s\)</span></span>|
|`M`|<span data-ttu-id="c040d-230">Month\(s\)</span><span class="sxs-lookup"><span data-stu-id="c040d-230">Month\(s\)</span></span>|
|`Q`|<span data-ttu-id="c040d-231">Quarter\(s\)</span><span class="sxs-lookup"><span data-stu-id="c040d-231">Quarter\(s\)</span></span>|
|`Y`|<span data-ttu-id="c040d-232">Year\(s\)</span><span class="sxs-lookup"><span data-stu-id="c040d-232">Year\(s\)</span></span>|

<span data-ttu-id="c040d-233">You can construct a date formula in three ways.</span><span class="sxs-lookup"><span data-stu-id="c040d-233">You can construct a date formula in three ways.</span></span>

<span data-ttu-id="c040d-234">The following example shows how to use `C`, for current, and a time unit.</span><span class="sxs-lookup"><span data-stu-id="c040d-234">The following example shows how to use `C`, for current, and a time unit.</span></span>

|  <span data-ttu-id="c040d-235">Expression</span><span class="sxs-lookup"><span data-stu-id="c040d-235">Expression</span></span>  |  <span data-ttu-id="c040d-236">Meaning</span><span class="sxs-lookup"><span data-stu-id="c040d-236">Meaning</span></span>  |
|--------------|-----------|
|`CW`|<span data-ttu-id="c040d-237">Current week</span><span class="sxs-lookup"><span data-stu-id="c040d-237">Current week</span></span>|
|`CM`|<span data-ttu-id="c040d-238">Current month</span><span class="sxs-lookup"><span data-stu-id="c040d-238">Current month</span></span>|

<span data-ttu-id="c040d-239">The following example shows how to use a number and a time unit.</span><span class="sxs-lookup"><span data-stu-id="c040d-239">The following example shows how to use a number and a time unit.</span></span> <span data-ttu-id="c040d-240">A number cannot be larger than 9999.</span><span class="sxs-lookup"><span data-stu-id="c040d-240">A number cannot be larger than 9999.</span></span>

|  <span data-ttu-id="c040d-241">Expression</span><span class="sxs-lookup"><span data-stu-id="c040d-241">Expression</span></span>  |  <span data-ttu-id="c040d-242">Meaning</span><span class="sxs-lookup"><span data-stu-id="c040d-242">Meaning</span></span>  |
|--------------|-----------|
|`10D`|<span data-ttu-id="c040d-243">10 days from today</span><span class="sxs-lookup"><span data-stu-id="c040d-243">10 days from today</span></span>|
|`2W`|<span data-ttu-id="c040d-244">2 weeks from today</span><span class="sxs-lookup"><span data-stu-id="c040d-244">2 weeks from today</span></span>|

<span data-ttu-id="c040d-245">The following example shows how to use a time unit and a number.</span><span class="sxs-lookup"><span data-stu-id="c040d-245">The following example shows how to use a time unit and a number.</span></span>

|  <span data-ttu-id="c040d-246">Expression</span><span class="sxs-lookup"><span data-stu-id="c040d-246">Expression</span></span>  |  <span data-ttu-id="c040d-247">Meaning</span><span class="sxs-lookup"><span data-stu-id="c040d-247">Meaning</span></span>  |
|--------------|-----------|
|`D10`|<span data-ttu-id="c040d-248">The next 10th day of a month</span><span class="sxs-lookup"><span data-stu-id="c040d-248">The next 10th day of a month</span></span>|
|`WD4`|<span data-ttu-id="c040d-249">The next 4th day of a week \(Thursday\)</span><span class="sxs-lookup"><span data-stu-id="c040d-249">The next 4th day of a week \(Thursday\)</span></span>|

<span data-ttu-id="c040d-250">The following example shows how you can combine these three forms as needed.</span><span class="sxs-lookup"><span data-stu-id="c040d-250">The following example shows how you can combine these three forms as needed.</span></span>

|  <span data-ttu-id="c040d-251">Expression</span><span class="sxs-lookup"><span data-stu-id="c040d-251">Expression</span></span>  |  <span data-ttu-id="c040d-252">Meaning</span><span class="sxs-lookup"><span data-stu-id="c040d-252">Meaning</span></span>  |
|--------------|-----------|
|`CM+10D`|<span data-ttu-id="c040d-253">Current month \+ 10 days</span><span class="sxs-lookup"><span data-stu-id="c040d-253">Current month \+ 10 days</span></span>|

<span data-ttu-id="c040d-254">The following example shows how you can use a minus sign to indicate a date in the past.</span><span class="sxs-lookup"><span data-stu-id="c040d-254">The following example shows how you can use a minus sign to indicate a date in the past.</span></span>

|  <span data-ttu-id="c040d-255">Expression</span><span class="sxs-lookup"><span data-stu-id="c040d-255">Expression</span></span>  |  <span data-ttu-id="c040d-256">Meaning</span><span class="sxs-lookup"><span data-stu-id="c040d-256">Meaning</span></span>  |
|--------------|-----------|
|`-1Y`|<span data-ttu-id="c040d-257">1 year ago from today</span><span class="sxs-lookup"><span data-stu-id="c040d-257">1 year ago from today</span></span>|

> [!IMPORTANT]
>  <span data-ttu-id="c040d-258">If the location uses a base calendar, then the date formula that you enter in, for example, the **Shipping Time** field is interpreted according to the calendar working days.</span><span class="sxs-lookup"><span data-stu-id="c040d-258">If the location uses a base calendar, then the date formula that you enter in, for example, the **Shipping Time** field is interpreted according to the calendar working days.</span></span> <span data-ttu-id="c040d-259">For example, `1W`  means seven working days.</span><span class="sxs-lookup"><span data-stu-id="c040d-259">For example, `1W`  means seven working days.</span></span>
<!--
# Entering Date Ranges
You can set filters containing a start date and an end date to display only the data contained in that date range or time interval. Special rules apply to the way you set date ranges. Let's take the **Customer Top 10** as an example:

![Setting a date range in the request page for the Customer Top 10 list](./media/ui-enter-date-ranges/customer-top10-list.png)

Here you can limit the report to a date range such as the past 2 weeks, or a total of 6 weeks, or whatever range you want. To set date ranges, you enter dates and then use either **..** or **|** to set the range. In our example, to show the top 10 customers for the first two weeks of May, you would set the date filter to *05 01 17..05 14 17*.
Here are a couple of other examples:

| Meaning | Example | Entries included |
|---|---|---|
|Equal to| 12 15 16 |Only those posted on December 15 2016.|
|Interval| 12 15 16..01 15 17<br /><br />..12 15 16|Those posted on dates between and including December 15 2016 and January 15 2017.<br /><br />Those posted on December 15 2016 or earlier.|
|Either/or|12 15 16&#124;12 16 16|Those posted on either December 15 or December 16 2016. If there are entries posted on both days, they will all be displayed.|

You can also combine the various format types.

| Example | Entries included |
|---|---|
|12 15 16&#124;12 01 16..05 31 17 | Entries posted either on December 15 2016 or on dates between and including December 01 2016 and May 31 2017. |
|..12 14 16&#124;12 30 16.. | Entries posted on December 14 or earlier, or entries posted on December 30 or later - that is, all entries except those posted on dates between and including December 15 and 29. |

Note that we have used the US date format MMDDYY here. As [!INCLUDE[d365fin](includes/d365fin_md.md)] becomes available in other markets, you'll be able to use the formats that you are used to.

## Using Date Formulas
A date formula is a short, abbreviated combination of letters and numbers that specifies how to calculate dates. You can enter date formulas in various date calculation fields and in recurring frequency fields in recurring journals.

> [!NOTE]
>  In all data formula fields, one day is automatically included to cover today as the day when the period starts. Accordingly, for example, if you enter **1W**, then the period is actually eight days because today is included. To specify a period of seven days (one true week) including the period starting date, then you must enter **6D** or **1W\-1D**.

Here are some examples of how date formulas can be used:

-   The date formula in the recurring frequency field in recurring journals determines how often the entry on the journal line will be posted.

-   The date formula in the **Grace Period** field for a specified reminder level determines the period of time that must pass from the due date (or from the due date of the previous reminder) before a reminder will be created.

-   The date formula in the **Due Date Calculation** field determines how to calculate the due date on the reminder.

The date calculation formula can contain a maximum of 20 characters, both numbers and letters. You can use the following letters, which are abbreviations for time specifications.

|  Letter  |  Time specification  |
|----------|----------------------|
|C|Current|
|D|Day\(s\)|
|W|Week\(s\)|
|M|Month\(s\)|
|Q|Quarter\(s\)|
|Y|Year\(s\)|

You can construct a date formula in three ways.

The following example shows how to use **C**, for current, and a time unit.

|  Expression  |  Meaning  |
|--------------|-----------|
|CW|Current week|
|CM|Current month|

The following example shows how to use a number and a time unit. A number cannot be larger than 9999.

|  Expression  |  Meaning  |
|--------------|-----------|
|10D|10 days from today|
|2W|2 weeks from today|

The following example shows how to use a time unit and a number.

|  Expression  |  Meaning  |
|--------------|-----------|
|D10|The next 10th day of a month|
|WD4|The next 4th day of a week \(Thursday\)|

The following example shows how you can combine these three forms as needed.

|  Expression  |  Meaning  |
|--------------|-----------|
|CM\+10D|Current month \+ 10 days|

The following example shows how you can use a minus sign to indicate a date in the past.

|  Expression  |  Meaning  |
|--------------|-----------|
|-1Y|1 year ago from today|

> [!IMPORTANT]
>  If the location uses a base calendar, then the date formula that you enter in, for example, the **Shipping Time** field is interpreted according to the calendar working days. For example, **1W**  means seven working days.

-->

## <a name="entering-times"></a><span data-ttu-id="c040d-260">Entering Times</span><span class="sxs-lookup"><span data-stu-id="c040d-260">Entering Times</span></span>
<span data-ttu-id="c040d-261">When you enter times, you can insert any non-space separators that you want between the units, but if you use double digits for each unit up to milliseconds, then it is not required.</span><span class="sxs-lookup"><span data-stu-id="c040d-261">When you enter times, you can insert any non-space separators that you want between the units, but if you use double digits for each unit up to milliseconds, then it is not required.</span></span>

<span data-ttu-id="c040d-262">You only have to write the largest units that you require; the rest will be set to zero.</span><span class="sxs-lookup"><span data-stu-id="c040d-262">You only have to write the largest units that you require; the rest will be set to zero.</span></span> <span data-ttu-id="c040d-263">You can also leave out any AM/PM indicator.</span><span class="sxs-lookup"><span data-stu-id="c040d-263">You can also leave out any AM/PM indicator.</span></span>

<span data-ttu-id="c040d-264">The following table lists the various ways in which times can be entered and how they are interpreted.</span><span class="sxs-lookup"><span data-stu-id="c040d-264">The following table lists the various ways in which times can be entered and how they are interpreted.</span></span> <span data-ttu-id="c040d-265">It assumes region settings that format times according to: **Hours:Minutes:Seconds.Milliseconds.**</span><span class="sxs-lookup"><span data-stu-id="c040d-265">It assumes region settings that format times according to: **Hours:Minutes:Seconds.Milliseconds.**</span></span> <span data-ttu-id="c040d-266">and use the AM and PM indicators of 'AM' and 'PM', respectively.</span><span class="sxs-lookup"><span data-stu-id="c040d-266">and use the AM and PM indicators of 'AM' and 'PM', respectively.</span></span>

|<span data-ttu-id="c040d-267">**Entry**</span><span class="sxs-lookup"><span data-stu-id="c040d-267">**Entry**</span></span>      |<span data-ttu-id="c040d-268">**Interpretation**</span><span class="sxs-lookup"><span data-stu-id="c040d-268">**Interpretation**</span></span>      |
|---------------|------------------------|
|`05:23:17`|<span data-ttu-id="c040d-269">05:23:17</span><span class="sxs-lookup"><span data-stu-id="c040d-269">05:23:17</span></span>|
|`5`|<span data-ttu-id="c040d-270">05:00:00</span><span class="sxs-lookup"><span data-stu-id="c040d-270">05:00:00</span></span>|
|`5AM`|<span data-ttu-id="c040d-271">05:00:00</span><span class="sxs-lookup"><span data-stu-id="c040d-271">05:00:00</span></span>|
|`5P`|<span data-ttu-id="c040d-272">17:00:00</span><span class="sxs-lookup"><span data-stu-id="c040d-272">17:00:00</span></span>|
|`12`|<span data-ttu-id="c040d-273">12:00:00</span><span class="sxs-lookup"><span data-stu-id="c040d-273">12:00:00</span></span>|
|`12A`|<span data-ttu-id="c040d-274">00:00:00</span><span class="sxs-lookup"><span data-stu-id="c040d-274">00:00:00</span></span>|
|`12P`|<span data-ttu-id="c040d-275">12:00:00</span><span class="sxs-lookup"><span data-stu-id="c040d-275">12:00:00</span></span>|
|`17`|<span data-ttu-id="c040d-276">17:00:00</span><span class="sxs-lookup"><span data-stu-id="c040d-276">17:00:00</span></span>|
|`5:30`|<span data-ttu-id="c040d-277">05:30:00</span><span class="sxs-lookup"><span data-stu-id="c040d-277">05:30:00</span></span>|
|`0530`|<span data-ttu-id="c040d-278">05:30:00</span><span class="sxs-lookup"><span data-stu-id="c040d-278">05:30:00</span></span>|
|`5:30:5`|<span data-ttu-id="c040d-279">05:30:05</span><span class="sxs-lookup"><span data-stu-id="c040d-279">05:30:05</span></span>|
|`053005`|<span data-ttu-id="c040d-280">05:30:05</span><span class="sxs-lookup"><span data-stu-id="c040d-280">05:30:05</span></span>|
|`5:30:5,50`|<span data-ttu-id="c040d-281">05:30:05.5</span><span class="sxs-lookup"><span data-stu-id="c040d-281">05:30:05.5</span></span>|
|`053005050`|<span data-ttu-id="c040d-282">05:30:05.05</span><span class="sxs-lookup"><span data-stu-id="c040d-282">05:30:05.05</span></span>|

<span data-ttu-id="c040d-283">You should be aware that milliseconds are interpreted as decimal notation.</span><span class="sxs-lookup"><span data-stu-id="c040d-283">You should be aware that milliseconds are interpreted as decimal notation.</span></span> <span data-ttu-id="c040d-284">So, for example, `3`, `30`, and `300` all mean 300 milliseconds, while `03` means `30` and `003` means 3 milliseconds.</span><span class="sxs-lookup"><span data-stu-id="c040d-284">So, for example, `3`, `30`, and `300` all mean 300 milliseconds, while `03` means `30` and `003` means 3 milliseconds.</span></span>

<span data-ttu-id="c040d-285">You cannot use `24:00` to mean midnight, or use any value greater than 24:00.</span><span class="sxs-lookup"><span data-stu-id="c040d-285">You cannot use `24:00` to mean midnight, or use any value greater than 24:00.</span></span>

<span data-ttu-id="c040d-286">The word for 'time' in the language used by [!INCLUDE[d365fin](includes/d365fin_long_md.md)] will be evaluated to the current time on your computer or mobile device.</span><span class="sxs-lookup"><span data-stu-id="c040d-286">The word for 'time' in the language used by [!INCLUDE[d365fin](includes/d365fin_long_md.md)] will be evaluated to the current time on your computer or mobile device.</span></span> <span data-ttu-id="c040d-287">You can enter any part of the word, starting from the beginning, such as `t` or `TIM`.</span><span class="sxs-lookup"><span data-stu-id="c040d-287">You can enter any part of the word, starting from the beginning, such as `t` or `TIM`.</span></span>

## <a name="entering-combined-dates-and-times"></a><span data-ttu-id="c040d-288">Entering combined Dates and Times</span><span class="sxs-lookup"><span data-stu-id="c040d-288">Entering combined Dates and Times</span></span>
<span data-ttu-id="c040d-289">When you enter datetimes, which are a date and time combined into one field, you must enter a space between the date and the time.</span><span class="sxs-lookup"><span data-stu-id="c040d-289">When you enter datetimes, which are a date and time combined into one field, you must enter a space between the date and the time.</span></span> <span data-ttu-id="c040d-290">The date part can only contain spaces in the form of the official date separator of your region settings.</span><span class="sxs-lookup"><span data-stu-id="c040d-290">The date part can only contain spaces in the form of the official date separator of your region settings.</span></span> <span data-ttu-id="c040d-291">The time can contain spaces around the AM/PM indicator.</span><span class="sxs-lookup"><span data-stu-id="c040d-291">The time can contain spaces around the AM/PM indicator.</span></span>

<span data-ttu-id="c040d-292">It is also possible to enter only a date in a datetime field, but it is not possible to enter only a time.</span><span class="sxs-lookup"><span data-stu-id="c040d-292">It is also possible to enter only a date in a datetime field, but it is not possible to enter only a time.</span></span>

<span data-ttu-id="c040d-293">The following table lists some examples of date/time combinations.</span><span class="sxs-lookup"><span data-stu-id="c040d-293">The following table lists some examples of date/time combinations.</span></span> <span data-ttu-id="c040d-294">The region settings in the examples displays dates in the day\-month\-year format, using AM/PM designators, English language, and Sunday as the start of the week.</span><span class="sxs-lookup"><span data-stu-id="c040d-294">The region settings in the examples displays dates in the day\-month\-year format, using AM/PM designators, English language, and Sunday as the start of the week.</span></span>

|<span data-ttu-id="c040d-295">**Entry**</span><span class="sxs-lookup"><span data-stu-id="c040d-295">**Entry**</span></span>      |<span data-ttu-id="c040d-296">**Interpretation**</span><span class="sxs-lookup"><span data-stu-id="c040d-296">**Interpretation**</span></span>      |
|---------------|------------------------|
|`08-01-2016 05:48:12 PM`|<span data-ttu-id="c040d-297">08\-01\-2016 05:48:12 PM</span><span class="sxs-lookup"><span data-stu-id="c040d-297">08\-01\-2016 05:48:12 PM</span></span>|
|`131202 132455`|<span data-ttu-id="c040d-298">13\-12\-2002 13:24:55</span><span class="sxs-lookup"><span data-stu-id="c040d-298">13\-12\-2002 13:24:55</span></span>|
|`1-12-02 10`|<span data-ttu-id="c040d-299">01\-12\-2002 10:00:00</span><span class="sxs-lookup"><span data-stu-id="c040d-299">01\-12\-2002 10:00:00</span></span>|
|`1.12.02 5`|<span data-ttu-id="c040d-300">01\-12\-2002 05:00:00</span><span class="sxs-lookup"><span data-stu-id="c040d-300">01\-12\-2002 05:00:00</span></span>|
|`1.12.02`|<span data-ttu-id="c040d-301">01\-12\-2002 00:00:00</span><span class="sxs-lookup"><span data-stu-id="c040d-301">01\-12\-2002 00:00:00</span></span>|
|`11 12`|<span data-ttu-id="c040d-302">11\-work date month\-work date year 12:00:00</span><span class="sxs-lookup"><span data-stu-id="c040d-302">11\-work date month\-work date year 12:00:00</span></span>|
|`1112 12`|<span data-ttu-id="c040d-303">11\-12\-work date year 12:00:00</span><span class="sxs-lookup"><span data-stu-id="c040d-303">11\-12\-work date year 12:00:00</span></span>|
|<span data-ttu-id="c040d-304">`t` or `today`</span><span class="sxs-lookup"><span data-stu-id="c040d-304">`t` or `today`</span></span>|<span data-ttu-id="c040d-305">today's date 00:00:00</span><span class="sxs-lookup"><span data-stu-id="c040d-305">today's date 00:00:00</span></span>|
|`t 10:30`|<span data-ttu-id="c040d-306">today's date 10:30:00</span><span class="sxs-lookup"><span data-stu-id="c040d-306">today's date 10:30:00</span></span>|
|`t 3:3:3`|<span data-ttu-id="c040d-307">today's date 03:03:03</span><span class="sxs-lookup"><span data-stu-id="c040d-307">today's date 03:03:03</span></span>|
|<span data-ttu-id="c040d-308">`w` or `workdate`</span><span class="sxs-lookup"><span data-stu-id="c040d-308">`w` or `workdate`</span></span>|<span data-ttu-id="c040d-309">the working date 00:00:00</span><span class="sxs-lookup"><span data-stu-id="c040d-309">the working date 00:00:00</span></span>|
|<span data-ttu-id="c040d-310">`m` or `Monday`</span><span class="sxs-lookup"><span data-stu-id="c040d-310">`m` or `Monday`</span></span>|<span data-ttu-id="c040d-311">Monday of the work date week 00:00:00</span><span class="sxs-lookup"><span data-stu-id="c040d-311">Monday of the work date week 00:00:00</span></span>|
|<span data-ttu-id="c040d-312">`tu` or `Tuesday`</span><span class="sxs-lookup"><span data-stu-id="c040d-312">`tu` or `Tuesday`</span></span>|<span data-ttu-id="c040d-313">Tuesday of the work date week 00:00:00</span><span class="sxs-lookup"><span data-stu-id="c040d-313">Tuesday of the work date week 00:00:00</span></span>|
|<span data-ttu-id="c040d-314">`sa` or `Saturday`</span><span class="sxs-lookup"><span data-stu-id="c040d-314">`sa` or `Saturday`</span></span>|<span data-ttu-id="c040d-315">Saturday of the work date week 00:00:00</span><span class="sxs-lookup"><span data-stu-id="c040d-315">Saturday of the work date week 00:00:00</span></span>|
|<span data-ttu-id="c040d-316">`s` or `Sunday`</span><span class="sxs-lookup"><span data-stu-id="c040d-316">`s` or `Sunday`</span></span>|<span data-ttu-id="c040d-317">Sunday of the work date week 00:00:00</span><span class="sxs-lookup"><span data-stu-id="c040d-317">Sunday of the work date week 00:00:00</span></span>|
|`tu 10:30`|<span data-ttu-id="c040d-318">Tuesday of the work date week 10:30:00</span><span class="sxs-lookup"><span data-stu-id="c040d-318">Tuesday of the work date week 10:30:00</span></span>|
|`tu 3:3:3`|<span data-ttu-id="c040d-319">Tuesday of the work date week 03:03:03</span><span class="sxs-lookup"><span data-stu-id="c040d-319">Tuesday of the work date week 03:03:03</span></span>|
|`t23 t`|<span data-ttu-id="c040d-320">Tuesday of week 23 of the work date year, current time of day</span><span class="sxs-lookup"><span data-stu-id="c040d-320">Tuesday of week 23 of the work date year, current time of day</span></span>|
|`t23`|<span data-ttu-id="c040d-321">Tuesday of week 23 of the work date year</span><span class="sxs-lookup"><span data-stu-id="c040d-321">Tuesday of week 23 of the work date year</span></span>|
|`t 23`|<span data-ttu-id="c040d-322">Today 23:00:00</span><span class="sxs-lookup"><span data-stu-id="c040d-322">Today 23:00:00</span></span>|
|`t-1`|<span data-ttu-id="c040d-323">Tuesday of week 1 of the work date year</span><span class="sxs-lookup"><span data-stu-id="c040d-323">Tuesday of week 1 of the work date year</span></span>|

## <a name="entering-duration"></a><span data-ttu-id="c040d-324">Entering Duration</span><span class="sxs-lookup"><span data-stu-id="c040d-324">Entering Duration</span></span>
<span data-ttu-id="c040d-325">Some fields in the application represent a duration, or amount of elapsed time, instead of a specific date or time.</span><span class="sxs-lookup"><span data-stu-id="c040d-325">Some fields in the application represent a duration, or amount of elapsed time, instead of a specific date or time.</span></span> <span data-ttu-id="c040d-326">You enter a duration as a number followed by its unit of measure.</span><span class="sxs-lookup"><span data-stu-id="c040d-326">You enter a duration as a number followed by its unit of measure.</span></span>

<span data-ttu-id="c040d-327">Here are some examples.</span><span class="sxs-lookup"><span data-stu-id="c040d-327">Here are some examples.</span></span>

|<span data-ttu-id="c040d-328">**Duration**</span><span class="sxs-lookup"><span data-stu-id="c040d-328">**Duration**</span></span>|<span data-ttu-id="c040d-329">**Unit of measure**</span><span class="sxs-lookup"><span data-stu-id="c040d-329">**Unit of measure**</span></span>|
|------------|-------------------|
|`2h`|<span data-ttu-id="c040d-330">2 hrs</span><span class="sxs-lookup"><span data-stu-id="c040d-330">2 hrs</span></span>|
|`6h 30 m`|<span data-ttu-id="c040d-331">6 hrs 30 mins</span><span class="sxs-lookup"><span data-stu-id="c040d-331">6 hrs 30 mins</span></span>|
|`6.5h`|<span data-ttu-id="c040d-332">6 hrs 30 mins</span><span class="sxs-lookup"><span data-stu-id="c040d-332">6 hrs 30 mins</span></span>|
|`90m`|<span data-ttu-id="c040d-333">1 hr 30 mins</span><span class="sxs-lookup"><span data-stu-id="c040d-333">1 hr 30 mins</span></span>|
|`2d 6h 30m`|<span data-ttu-id="c040d-334">2 days 6 hrs 30 mins</span><span class="sxs-lookup"><span data-stu-id="c040d-334">2 days 6 hrs 30 mins</span></span>|
|`2d 6h 30m 56s 600ms`|<span data-ttu-id="c040d-335">2 days 6 hrs 30 mins 56 secs 600 msecs</span><span class="sxs-lookup"><span data-stu-id="c040d-335">2 days 6 hrs 30 mins 56 secs 600 msecs</span></span>|

<span data-ttu-id="c040d-336">You can also enter a number, which will be automatically converted to a duration.</span><span class="sxs-lookup"><span data-stu-id="c040d-336">You can also enter a number, which will be automatically converted to a duration.</span></span> <span data-ttu-id="c040d-337">The number you enter is converted according to the default unit of measure that has been specified for the duration field.</span><span class="sxs-lookup"><span data-stu-id="c040d-337">The number you enter is converted according to the default unit of measure that has been specified for the duration field.</span></span>

<span data-ttu-id="c040d-338">To see what unit of measure is being used in a duration field, enter a number and see which unit of measure it is converted to.</span><span class="sxs-lookup"><span data-stu-id="c040d-338">To see what unit of measure is being used in a duration field, enter a number and see which unit of measure it is converted to.</span></span>

<span data-ttu-id="c040d-339">For example, if the unit of measure is hours, the number `5` is converted to 5 hrs.</span><span class="sxs-lookup"><span data-stu-id="c040d-339">For example, if the unit of measure is hours, the number `5` is converted to 5 hrs.</span></span>


## <a name="see-also"></a><span data-ttu-id="c040d-340">See Also</span><span class="sxs-lookup"><span data-stu-id="c040d-340">See Also</span></span>
<span data-ttu-id="c040d-341">[Working with [!INCLUDE[d365fin](includes/d365fin_long_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="c040d-341">[Working with [!INCLUDE[d365fin](includes/d365fin_long_md.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="c040d-342">Date Calculation for Purchases</span><span class="sxs-lookup"><span data-stu-id="c040d-342">Date Calculation for Purchases</span></span>](purchasing-date-calculation-for-purchases.md)  
[<span data-ttu-id="c040d-343">Entering Criteria in Filters</span><span class="sxs-lookup"><span data-stu-id="c040d-343">Entering Criteria in Filters </span></span>](ui-enter-criteria-filters.md)  
