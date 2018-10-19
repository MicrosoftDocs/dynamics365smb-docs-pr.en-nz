---
title: Entering dates and times in Business Central  | Microsoft Docs
description: Learn how to enter dates and times including various productivity tips such as shorthand, expressions and ranges. Filter lists or reports down to specific date or time periods.
documentationcenter: 
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: dates, reporting, filter, calendar, shorthand, range
ms.date: 10/01/2018
ms.author: jswymer
ms.translationtype: HT
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: 8717d60a8449ca300eaf9c1a5c4b137ea1a1a247
ms.contentlocale: en-nz
ms.lasthandoff: 09/28/2018

---

# <a name="working-with-calendar-dates-and-times"></a><span data-ttu-id="7ee50-104">Working with Calendar Dates and Times</span><span class="sxs-lookup"><span data-stu-id="7ee50-104">Working with Calendar Dates and Times</span></span>
[!INCLUDE[d365fin](includes/d365fin_long_md.md)] <span data-ttu-id="7ee50-105">offers multiple ways to enter dates and times, including powerful features that accelerate data entry, or help you write complex calendar expressions.</span><span class="sxs-lookup"><span data-stu-id="7ee50-105">offers multiple ways to enter dates and times, including powerful features that accelerate data entry, or help you write complex calendar expressions.</span></span> <span data-ttu-id="7ee50-106">There are various places throughout the application where you can enter dates and times in fields.</span><span class="sxs-lookup"><span data-stu-id="7ee50-106">There are various places throughout the application where you can enter dates and times in fields.</span></span> <span data-ttu-id="7ee50-107">For example, on a sales order, you can set the shipment date.</span><span class="sxs-lookup"><span data-stu-id="7ee50-107">For example, on a sales order, you can set the shipment date.</span></span> <span data-ttu-id="7ee50-108">When filtering lists or report data, you can enter dates and times to pinpoint only the data that you are interested in.</span><span class="sxs-lookup"><span data-stu-id="7ee50-108">When filtering lists or report data, you can enter dates and times to pinpoint only the data that you are interested in.</span></span>

## <a name="check-your-region-and-language-settings"></a><span data-ttu-id="7ee50-109">Check your region and language settings</span><span class="sxs-lookup"><span data-stu-id="7ee50-109">Check your region and language settings</span></span>
<span data-ttu-id="7ee50-110">The [**My Settings**](https://businesscentral.dynamics.com?page=9176 "Go directly to your user settings page in Business Central") page specifies the **Region** and **Language** that you are using in the application.</span><span class="sxs-lookup"><span data-stu-id="7ee50-110">The [**My Settings**](https://businesscentral.dynamics.com?page=9176 "Go directly to your user settings page in Business Central") page specifies the **Region** and **Language** that you are using in the application.</span></span> <span data-ttu-id="7ee50-111">These settings influence how you enter dates and times.</span><span class="sxs-lookup"><span data-stu-id="7ee50-111">These settings influence how you enter dates and times.</span></span> 

-   <span data-ttu-id="7ee50-112">The **Region** setting determines how dates, times, numbers, and currencies are shown or formatted.</span><span class="sxs-lookup"><span data-stu-id="7ee50-112">The **Region** setting determines how dates, times, numbers, and currencies are shown or formatted.</span></span>

-   <span data-ttu-id="7ee50-113">For date patterns that involve words, the language of the words that you use must correspond to the **Language** setting.</span><span class="sxs-lookup"><span data-stu-id="7ee50-113">For date patterns that involve words, the language of the words that you use must correspond to the **Language** setting.</span></span>

> [!NOTE]
> [!INCLUDE[d365fin](includes/d365fin_long_md.md)] <span data-ttu-id="7ee50-114">uses the Gregorian calendar system.</span><span class="sxs-lookup"><span data-stu-id="7ee50-114">uses the Gregorian calendar system.</span></span>

<!-- 
The following sections describe how you can enter dates, times, datetimes, durations, date ranges, and how you use date formulas.
-->
## <a name="entering-dates"></a><span data-ttu-id="7ee50-115">Entering Dates</span><span class="sxs-lookup"><span data-stu-id="7ee50-115">Entering Dates</span></span>
<span data-ttu-id="7ee50-116">In a date field, you can enter a date using the standard format for your region setting.</span><span class="sxs-lookup"><span data-stu-id="7ee50-116">In a date field, you can enter a date using the standard format for your region setting.</span></span> <span data-ttu-id="7ee50-117">Different regions can use different separators between the days, months and years.</span><span class="sxs-lookup"><span data-stu-id="7ee50-117">Different regions can use different separators between the days, months and years.</span></span> <span data-ttu-id="7ee50-118">For example, some regions use dashes (mm-dd-yyyy) and others use forward slashes (mm/dd/yyyy).</span><span class="sxs-lookup"><span data-stu-id="7ee50-118">For example, some regions use dashes (mm-dd-yyyy) and others use forward slashes (mm/dd/yyyy).</span></span> <span data-ttu-id="7ee50-119">However, you can use any separators, even a space, and the date will automatically be changed to use separators that match your region.</span><span class="sxs-lookup"><span data-stu-id="7ee50-119">However, you can use any separators, even a space, and the date will automatically be changed to use separators that match your region.</span></span>

<span data-ttu-id="7ee50-120">Note that the format in which dates are displayed on printed reports or emailed documents is not influenced by your personal choice of region setting.</span><span class="sxs-lookup"><span data-stu-id="7ee50-120">Note that the format in which dates are displayed on printed reports or emailed documents is not influenced by your personal choice of region setting.</span></span>

<span data-ttu-id="7ee50-121">To work more productively with dates and times, you can use any of the methods or formats that are described in the following sections.</span><span class="sxs-lookup"><span data-stu-id="7ee50-121">To work more productively with dates and times, you can use any of the methods or formats that are described in the following sections.</span></span> 

### <a name="picking-dates-from-the-calendar"></a><span data-ttu-id="7ee50-122">Picking dates from the calendar</span><span class="sxs-lookup"><span data-stu-id="7ee50-122">Picking dates from the calendar</span></span>
<span data-ttu-id="7ee50-123">Any field displaying a calendar icon can be set using the calendar date picker.</span><span class="sxs-lookup"><span data-stu-id="7ee50-123">Any field displaying a calendar icon can be set using the calendar date picker.</span></span> <span data-ttu-id="7ee50-124">To display the calendar date picker, activate the calendar icon or press the Ctrl + Home keyboard shortcut in the field.</span><span class="sxs-lookup"><span data-stu-id="7ee50-124">To display the calendar date picker, activate the calendar icon or press the Ctrl + Home keyboard shortcut in the field.</span></span>

<span data-ttu-id="7ee50-125">![Date fields](media/ui-date-field.png "Example of a date field")</span><span class="sxs-lookup"><span data-stu-id="7ee50-125">![Date fields](media/ui-date-field.png "Example of a date field")</span></span>

<span data-ttu-id="7ee50-126">See also [Keyboard Shortcuts in the calendar date picker](keyboard-shortcuts.md#calendarshortcuts)</span><span class="sxs-lookup"><span data-stu-id="7ee50-126">See also [Keyboard Shortcuts in the calendar date picker](keyboard-shortcuts.md#calendarshortcuts)</span></span>

### <a name="today"></a><span data-ttu-id="7ee50-127">Today</span><span class="sxs-lookup"><span data-stu-id="7ee50-127">Today</span></span>
<span data-ttu-id="7ee50-128">Enter the word for `today`, in the language set by **Language** setting, that will set the date to the current date.</span><span class="sxs-lookup"><span data-stu-id="7ee50-128">Enter the word for `today`, in the language set by **Language** setting, that will set the date to the current date.</span></span> <span data-ttu-id="7ee50-129">Instead of entering the entire word, you can enter part of the word, starting from the beginning, such as `t` or `tod`, as long as it is not also the start of another word.</span><span class="sxs-lookup"><span data-stu-id="7ee50-129">Instead of entering the entire word, you can enter part of the word, starting from the beginning, such as `t` or `tod`, as long as it is not also the start of another word.</span></span>

### <a name="day-week-year-pattern"></a><span data-ttu-id="7ee50-130">Day\-week\-year pattern</span><span class="sxs-lookup"><span data-stu-id="7ee50-130">Day\-week\-year pattern</span></span>
<span data-ttu-id="7ee50-131">You can enter a date as a weekday followed by a week number and, optionally, a year.</span><span class="sxs-lookup"><span data-stu-id="7ee50-131">You can enter a date as a weekday followed by a week number and, optionally, a year.</span></span> <span data-ttu-id="7ee50-132">For example, `Mon25` or `mon25` means Monday in week 25.</span><span class="sxs-lookup"><span data-stu-id="7ee50-132">For example, `Mon25` or `mon25` means Monday in week 25.</span></span> <span data-ttu-id="7ee50-133">If you do not enter a year, the year of the work date is used.</span><span class="sxs-lookup"><span data-stu-id="7ee50-133">If you do not enter a year, the year of the work date is used.</span></span>

<span data-ttu-id="7ee50-134">Instead of entering the entire word for the day of the week, you can enter part of the word, starting from the beginning.</span><span class="sxs-lookup"><span data-stu-id="7ee50-134">Instead of entering the entire word for the day of the week, you can enter part of the word, starting from the beginning.</span></span> <span data-ttu-id="7ee50-135">In case of conflicts (such as with `s` which could be Saturday or Sunday), the days are evaluated according to the region setting.</span><span class="sxs-lookup"><span data-stu-id="7ee50-135">In case of conflicts (such as with `s` which could be Saturday or Sunday), the days are evaluated according to the region setting.</span></span> <span data-ttu-id="7ee50-136">The input is first evaluated against `workdate` and `today` as well, so keep this in mind when abbreviating.</span><span class="sxs-lookup"><span data-stu-id="7ee50-136">The input is first evaluated against `workdate` and `today` as well, so keep this in mind when abbreviating.</span></span> <span data-ttu-id="7ee50-137">For example, `t` already means today, so it cannot mean Tuesday or Thursday.</span><span class="sxs-lookup"><span data-stu-id="7ee50-137">For example, `t` already means today, so it cannot mean Tuesday or Thursday.</span></span>

<span data-ttu-id="7ee50-138">The week number scheme is always ISO 8601, where week 1 is the week with 4 January in it, or the week with the first Thursday of the year.</span><span class="sxs-lookup"><span data-stu-id="7ee50-138">The week number scheme is always ISO 8601, where week 1 is the week with 4 January in it, or the week with the first Thursday of the year.</span></span>

### <a name="digit-patterns"></a><span data-ttu-id="7ee50-139">Digit patterns</span><span class="sxs-lookup"><span data-stu-id="7ee50-139">Digit patterns</span></span>
<span data-ttu-id="7ee50-140">In a date field you can enter two, four, six, or eight digits:</span><span class="sxs-lookup"><span data-stu-id="7ee50-140">In a date field you can enter two, four, six, or eight digits:</span></span>

-   <span data-ttu-id="7ee50-141">If you enter only two digits, this is interpreted as the day, and it will add the month and the year of the work date.</span><span class="sxs-lookup"><span data-stu-id="7ee50-141">If you enter only two digits, this is interpreted as the day, and it will add the month and the year of the work date.</span></span>

-   <span data-ttu-id="7ee50-142">If you enter four digits, this is interpreted as the day and the month, and it will add the year of the work date.</span><span class="sxs-lookup"><span data-stu-id="7ee50-142">If you enter four digits, this is interpreted as the day and the month, and it will add the year of the work date.</span></span> <span data-ttu-id="7ee50-143">The order of the day and month is determined by your region settings.</span><span class="sxs-lookup"><span data-stu-id="7ee50-143">The order of the day and month is determined by your region settings.</span></span> <span data-ttu-id="7ee50-144">Even if your region settings have the year before the day and month, four digits are interpreted as the day and month.</span><span class="sxs-lookup"><span data-stu-id="7ee50-144">Even if your region settings have the year before the day and month, four digits are interpreted as the day and month.</span></span>

-   <span data-ttu-id="7ee50-145">If the date you want to enter is in the range 01/01/1930 through 12/31/2029, you can enter the year with two digits; otherwise, enter the year with four digits.</span><span class="sxs-lookup"><span data-stu-id="7ee50-145">If the date you want to enter is in the range 01/01/1930 through 12/31/2029, you can enter the year with two digits; otherwise, enter the year with four digits.</span></span>

### <a name="current-work-date"></a><span data-ttu-id="7ee50-146">Current work date</span><span class="sxs-lookup"><span data-stu-id="7ee50-146">Current work date</span></span>
<span data-ttu-id="7ee50-147">The work date feature allows you to record transations using a date that is different from the current date.</span><span class="sxs-lookup"><span data-stu-id="7ee50-147">The work date feature allows you to record transations using a date that is different from the current date.</span></span>

<span data-ttu-id="7ee50-148">The word for 'workdate', in the language set by **Language** setting, will set the date to the currently set work date that is specified on the [**My Settings**](https://businesscentral.dynamics.com?page=9176 "Go directly to your user settings page in Business Central") page.</span><span class="sxs-lookup"><span data-stu-id="7ee50-148">The word for 'workdate', in the language set by **Language** setting, will set the date to the currently set work date that is specified on the [**My Settings**](https://businesscentral.dynamics.com?page=9176 "Go directly to your user settings page in Business Central") page.</span></span> <span data-ttu-id="7ee50-149">Instead of entering the entire word, you can enter part of the word, starting from the beginning, such as 'w' or 'work'.</span><span class="sxs-lookup"><span data-stu-id="7ee50-149">Instead of entering the entire word, you can enter part of the word, starting from the beginning, such as 'w' or 'work'.</span></span>

<span data-ttu-id="7ee50-150">If you have not defined a work date, the current date will be used as the work date.</span><span class="sxs-lookup"><span data-stu-id="7ee50-150">If you have not defined a work date, the current date will be used as the work date.</span></span> <span data-ttu-id="7ee50-151">You may want to use a work date if you have many transactions with a date other than today's date.</span><span class="sxs-lookup"><span data-stu-id="7ee50-151">You may want to use a work date if you have many transactions with a date other than today's date.</span></span>

<span data-ttu-id="7ee50-152">See also [Changing Basic Settings, such as the Work Date](ui-change-basic-settings.md#work-date)</span><span class="sxs-lookup"><span data-stu-id="7ee50-152">See also [Changing Basic Settings, such as the Work Date](ui-change-basic-settings.md#work-date)</span></span>

### <a name="closing-date"></a><span data-ttu-id="7ee50-153">Closing Date</span><span class="sxs-lookup"><span data-stu-id="7ee50-153">Closing Date</span></span>
<span data-ttu-id="7ee50-154">When you close a fiscal year, you can use closing dates to indicate that an entry is a closing entry.</span><span class="sxs-lookup"><span data-stu-id="7ee50-154">When you close a fiscal year, you can use closing dates to indicate that an entry is a closing entry.</span></span> <span data-ttu-id="7ee50-155">A closing date technically is between two dates, for example between Dec 31 and Jan 1.</span><span class="sxs-lookup"><span data-stu-id="7ee50-155">A closing date technically is between two dates, for example between Dec 31 and Jan 1.</span></span>

<span data-ttu-id="7ee50-156">To specify that a date is a closing date, put `C` just before the date, such as `C123101`.</span><span class="sxs-lookup"><span data-stu-id="7ee50-156">To specify that a date is a closing date, put `C` just before the date, such as `C123101`.</span></span> <span data-ttu-id="7ee50-157">This can be used in combination with all the date patterns.</span><span class="sxs-lookup"><span data-stu-id="7ee50-157">This can be used in combination with all the date patterns.</span></span>

### <a name="examples"></a><span data-ttu-id="7ee50-158">Examples</span><span class="sxs-lookup"><span data-stu-id="7ee50-158">Examples</span></span>
<span data-ttu-id="7ee50-159">The following table contains examples of dates using all the formats.</span><span class="sxs-lookup"><span data-stu-id="7ee50-159">The following table contains examples of dates using all the formats.</span></span> <span data-ttu-id="7ee50-160">It assumes region settings that format dates according to: **year.month.day.**, a week starting on Monday, and the English language.</span><span class="sxs-lookup"><span data-stu-id="7ee50-160">It assumes region settings that format dates according to: **year.month.day.**, a week starting on Monday, and the English language.</span></span>

|<span data-ttu-id="7ee50-161">**Entry**</span><span class="sxs-lookup"><span data-stu-id="7ee50-161">**Entry**</span></span>      |<span data-ttu-id="7ee50-162">**Interpretation**</span><span class="sxs-lookup"><span data-stu-id="7ee50-162">**Interpretation**</span></span>      |
|---------------|------------------------|
|`2018.12.31.`|<span data-ttu-id="7ee50-163">2018.12.31.</span><span class="sxs-lookup"><span data-stu-id="7ee50-163">2018.12.31.</span></span>|
|`181231`|<span data-ttu-id="7ee50-164">2018.12.31.</span><span class="sxs-lookup"><span data-stu-id="7ee50-164">2018.12.31.</span></span>|
|`18.12.31.`|<span data-ttu-id="7ee50-165">2018.12.31.</span><span class="sxs-lookup"><span data-stu-id="7ee50-165">2018.12.31.</span></span>|
|`18.12.31.`|<span data-ttu-id="7ee50-166">2018.12.31.</span><span class="sxs-lookup"><span data-stu-id="7ee50-166">2018.12.31.</span></span>|
|`20181231`|<span data-ttu-id="7ee50-167">2018.12.31.</span><span class="sxs-lookup"><span data-stu-id="7ee50-167">2018.12.31.</span></span>|
|`18/12,31`|<span data-ttu-id="7ee50-168">2018.12.31.</span><span class="sxs-lookup"><span data-stu-id="7ee50-168">2018.12.31.</span></span>|
|`11`|<span data-ttu-id="7ee50-169">work date year.work date month.11.</span><span class="sxs-lookup"><span data-stu-id="7ee50-169">work date year.work date month.11.</span></span>|
|`1112`|<span data-ttu-id="7ee50-170">work date year.11.12.</span><span class="sxs-lookup"><span data-stu-id="7ee50-170">work date year.11.12.</span></span>|
|<span data-ttu-id="7ee50-171">`t` or `today`</span><span class="sxs-lookup"><span data-stu-id="7ee50-171">`t` or `today`</span></span>|<span data-ttu-id="7ee50-172">today's date</span><span class="sxs-lookup"><span data-stu-id="7ee50-172">today's date</span></span>|
|<span data-ttu-id="7ee50-173">`w` or `workdate`</span><span class="sxs-lookup"><span data-stu-id="7ee50-173">`w` or `workdate`</span></span>|<span data-ttu-id="7ee50-174">the working date</span><span class="sxs-lookup"><span data-stu-id="7ee50-174">the working date</span></span>|
|<span data-ttu-id="7ee50-175">`m` or `Monday`</span><span class="sxs-lookup"><span data-stu-id="7ee50-175">`m` or `Monday`</span></span>|<span data-ttu-id="7ee50-176">Monday of the work date week</span><span class="sxs-lookup"><span data-stu-id="7ee50-176">Monday of the work date week</span></span>|
|<span data-ttu-id="7ee50-177">`tu` or `Tuesday`</span><span class="sxs-lookup"><span data-stu-id="7ee50-177">`tu` or `Tuesday`</span></span>|<span data-ttu-id="7ee50-178">Tuesday of the work date week</span><span class="sxs-lookup"><span data-stu-id="7ee50-178">Tuesday of the work date week</span></span>|
|<span data-ttu-id="7ee50-179">`sa` or `Saturday`</span><span class="sxs-lookup"><span data-stu-id="7ee50-179">`sa` or `Saturday`</span></span>|<span data-ttu-id="7ee50-180">Saturday of the work date week</span><span class="sxs-lookup"><span data-stu-id="7ee50-180">Saturday of the work date week</span></span>|
|<span data-ttu-id="7ee50-181">`s` or `Sunday`</span><span class="sxs-lookup"><span data-stu-id="7ee50-181">`s` or `Sunday`</span></span>|<span data-ttu-id="7ee50-182">Sunday of the work date week</span><span class="sxs-lookup"><span data-stu-id="7ee50-182">Sunday of the work date week</span></span>|
|`t23`|<span data-ttu-id="7ee50-183">Tuesday of week 23 of the work date year</span><span class="sxs-lookup"><span data-stu-id="7ee50-183">Tuesday of week 23 of the work date year</span></span>|
|`t 23`|<span data-ttu-id="7ee50-184">Tuesday of week 23 of the work date year</span><span class="sxs-lookup"><span data-stu-id="7ee50-184">Tuesday of week 23 of the work date year</span></span>|
|`t-1`|<span data-ttu-id="7ee50-185">Tuesday of week 1 of the work date year</span><span class="sxs-lookup"><span data-stu-id="7ee50-185">Tuesday of week 1 of the work date year</span></span>|

##  <a name="BKMK_SettingDateRanges"></a> <span data-ttu-id="7ee50-186">Setting Ranges</span><span class="sxs-lookup"><span data-stu-id="7ee50-186">Setting Ranges</span></span>
<span data-ttu-id="7ee50-187">On lists, totals and reports, you can set filters on dates, times and datetimes containing a start value and optionally an end value to display only the data contained in that range.</span><span class="sxs-lookup"><span data-stu-id="7ee50-187">On lists, totals and reports, you can set filters on dates, times and datetimes containing a start value and optionally an end value to display only the data contained in that range.</span></span> <span data-ttu-id="7ee50-188">The standard rules apply to the way you set date ranges.</span><span class="sxs-lookup"><span data-stu-id="7ee50-188">The standard rules apply to the way you set date ranges.</span></span>

|<span data-ttu-id="7ee50-189">**Meaning**</span><span class="sxs-lookup"><span data-stu-id="7ee50-189">**Meaning**</span></span>|<span data-ttu-id="7ee50-190">**Sample expression (Date)**</span><span class="sxs-lookup"><span data-stu-id="7ee50-190">**Sample expression (Date)**</span></span>|<span data-ttu-id="7ee50-191">**Data included in the filter**</span><span class="sxs-lookup"><span data-stu-id="7ee50-191">**Data included in the filter**</span></span>|
|-----------|---------------------|--------------------|
|<span data-ttu-id="7ee50-192">Interval</span><span class="sxs-lookup"><span data-stu-id="7ee50-192">Interval</span></span>|<span data-ttu-id="7ee50-193">`12 15 00..01 15 01`  \n`..12 15 00`</span><span class="sxs-lookup"><span data-stu-id="7ee50-193">`12 15 00..01 15 01`  \n`..12 15 00`</span></span>|<span data-ttu-id="7ee50-194">Records with dates between and including 12 15 00 and 01 15 01.</span><span class="sxs-lookup"><span data-stu-id="7ee50-194">Records with dates between and including 12 15 00 and 01 15 01.</span></span>  <span data-ttu-id="7ee50-195">\nRecords with dates of 12 15 00 or earlier.</span><span class="sxs-lookup"><span data-stu-id="7ee50-195">\nRecords with dates of 12 15 00 or earlier.</span></span>|
|<span data-ttu-id="7ee50-196">Either/or</span><span class="sxs-lookup"><span data-stu-id="7ee50-196">Either/or</span></span>|<span data-ttu-id="7ee50-197">\`12 15 00</span><span class="sxs-lookup"><span data-stu-id="7ee50-197">\`12 15 00</span></span>|<span data-ttu-id="7ee50-198">12 16 00\`</span><span class="sxs-lookup"><span data-stu-id="7ee50-198">12 16 00\`</span></span>|<span data-ttu-id="7ee50-199">Records with dates of either 12 15 00 or 12 16 00.</span><span class="sxs-lookup"><span data-stu-id="7ee50-199">Records with dates of either 12 15 00 or 12 16 00.</span></span> <span data-ttu-id="7ee50-200">If there are records with dates on both days, they will all be displayed.</span><span class="sxs-lookup"><span data-stu-id="7ee50-200">If there are records with dates on both days, they will all be displayed.</span></span>|
|<span data-ttu-id="7ee50-201">Combination</span><span class="sxs-lookup"><span data-stu-id="7ee50-201">Combination</span></span>|<span data-ttu-id="7ee50-202">\`12 15 00</span><span class="sxs-lookup"><span data-stu-id="7ee50-202">\`12 15 00</span></span>|<span data-ttu-id="7ee50-203">12 01 00..12 10 00`  \n`..12 14 00</span><span class="sxs-lookup"><span data-stu-id="7ee50-203">12 01 00..12 10 00`  \n`..12 14 00</span></span>|<span data-ttu-id="7ee50-204">12 30 00..\`</span><span class="sxs-lookup"><span data-stu-id="7ee50-204">12 30 00..\`</span></span>|<span data-ttu-id="7ee50-205">Records with dates of 12 15 00 or on dates between and including 12 01 00 and 12 10 00.</span><span class="sxs-lookup"><span data-stu-id="7ee50-205">Records with dates of 12 15 00 or on dates between and including 12 01 00 and 12 10 00.</span></span>  <span data-ttu-id="7ee50-206">\nRecords with dates of 12 14 00 or earlier, or dates of 12 30 00 or later, that is, all records except those with dates between and including 12 15 00 and 12 29 00.</span><span class="sxs-lookup"><span data-stu-id="7ee50-206">\nRecords with dates of 12 14 00 or earlier, or dates of 12 30 00 or later, that is, all records except those with dates between and including 12 15 00 and 12 29 00.</span></span>|

<span data-ttu-id="7ee50-207">You can use any of the valid formats in date range filters.</span><span class="sxs-lookup"><span data-stu-id="7ee50-207">You can use any of the valid formats in date range filters.</span></span> <span data-ttu-id="7ee50-208">For example, `mon14 3..t 4p` applied on a datetime field results in a filter from 3 AM on Monday in week 14 of the current work date year, inclusive, until today at 4PM, inclusive.</span><span class="sxs-lookup"><span data-stu-id="7ee50-208">For example, `mon14 3..t 4p` applied on a datetime field results in a filter from 3 AM on Monday in week 14 of the current work date year, inclusive, until today at 4PM, inclusive.</span></span>


## <a name="using-date-formulas"></a><span data-ttu-id="7ee50-209">Using Date Formulas</span><span class="sxs-lookup"><span data-stu-id="7ee50-209">Using Date Formulas</span></span>
<span data-ttu-id="7ee50-210">A date formula is a short, abbreviated combination of letters and numbers that specifies how to calculate dates.</span><span class="sxs-lookup"><span data-stu-id="7ee50-210">A date formula is a short, abbreviated combination of letters and numbers that specifies how to calculate dates.</span></span> <span data-ttu-id="7ee50-211">You can enter date formulas in various date calculation fields or filters.</span><span class="sxs-lookup"><span data-stu-id="7ee50-211">You can enter date formulas in various date calculation fields or filters.</span></span>

> [!NOTE]
>  <span data-ttu-id="7ee50-212">In all data formula fields, one day is automatically included to cover today as the day when the period starts.</span><span class="sxs-lookup"><span data-stu-id="7ee50-212">In all data formula fields, one day is automatically included to cover today as the day when the period starts.</span></span> <span data-ttu-id="7ee50-213">Accordingly, for example, if you enter `1W`, then the period is actually eight days because today is included.</span><span class="sxs-lookup"><span data-stu-id="7ee50-213">Accordingly, for example, if you enter `1W`, then the period is actually eight days because today is included.</span></span> <span data-ttu-id="7ee50-214">To specify a period of seven days \(one true week\) including the period starting date, then you must enter `6D` or `1W-1D`.</span><span class="sxs-lookup"><span data-stu-id="7ee50-214">To specify a period of seven days \(one true week\) including the period starting date, then you must enter `6D` or `1W-1D`.</span></span>

<span data-ttu-id="7ee50-215">Here are some examples of how date formulas can be used:</span><span class="sxs-lookup"><span data-stu-id="7ee50-215">Here are some examples of how date formulas can be used:</span></span>

-   <span data-ttu-id="7ee50-216">The date formula in the recurring frequency field in recurring journals determines how often the entry on the journal line will be posted.</span><span class="sxs-lookup"><span data-stu-id="7ee50-216">The date formula in the recurring frequency field in recurring journals determines how often the entry on the journal line will be posted.</span></span>

-   <span data-ttu-id="7ee50-217">The date formula in the **Grace Period** field for a specified reminder level determines the period of time that must pass from the due date \(or from the date of the previous reminder\) before a reminder will be created.</span><span class="sxs-lookup"><span data-stu-id="7ee50-217">The date formula in the **Grace Period** field for a specified reminder level determines the period of time that must pass from the due date \(or from the date of the previous reminder\) before a reminder will be created.</span></span>

-   <span data-ttu-id="7ee50-218">The date formula in the **Due Date Calculation** field determines how to calculate the due date on the reminder.</span><span class="sxs-lookup"><span data-stu-id="7ee50-218">The date formula in the **Due Date Calculation** field determines how to calculate the due date on the reminder.</span></span>

<span data-ttu-id="7ee50-219">The date formula can contain a maximum of 20 characters, both numbers and letters.</span><span class="sxs-lookup"><span data-stu-id="7ee50-219">The date formula can contain a maximum of 20 characters, both numbers and letters.</span></span> <span data-ttu-id="7ee50-220">You can use the following letters, which are abbreviations for calendar units.</span><span class="sxs-lookup"><span data-stu-id="7ee50-220">You can use the following letters, which are abbreviations for calendar units.</span></span>

|  <span data-ttu-id="7ee50-221">Letter</span><span class="sxs-lookup"><span data-stu-id="7ee50-221">Letter</span></span>  |  <span data-ttu-id="7ee50-222">Meaning</span><span class="sxs-lookup"><span data-stu-id="7ee50-222">Meaning</span></span>  |
|----------|----------------------|
|`C`|<span data-ttu-id="7ee50-223">Current</span><span class="sxs-lookup"><span data-stu-id="7ee50-223">Current</span></span>|
|`D`|<span data-ttu-id="7ee50-224">Day\(s\)</span><span class="sxs-lookup"><span data-stu-id="7ee50-224">Day\(s\)</span></span>|
|`W`|<span data-ttu-id="7ee50-225">Week\(s\)</span><span class="sxs-lookup"><span data-stu-id="7ee50-225">Week\(s\)</span></span>|
|`M`|<span data-ttu-id="7ee50-226">Month\(s\)</span><span class="sxs-lookup"><span data-stu-id="7ee50-226">Month\(s\)</span></span>|
|`Q`|<span data-ttu-id="7ee50-227">Quarter\(s\)</span><span class="sxs-lookup"><span data-stu-id="7ee50-227">Quarter\(s\)</span></span>|
|`Y`|<span data-ttu-id="7ee50-228">Year\(s\)</span><span class="sxs-lookup"><span data-stu-id="7ee50-228">Year\(s\)</span></span>|

<span data-ttu-id="7ee50-229">You can construct a date formula in three ways.</span><span class="sxs-lookup"><span data-stu-id="7ee50-229">You can construct a date formula in three ways.</span></span>

<span data-ttu-id="7ee50-230">The following example shows how to use `C`, for current, and a time unit.</span><span class="sxs-lookup"><span data-stu-id="7ee50-230">The following example shows how to use `C`, for current, and a time unit.</span></span>

|  <span data-ttu-id="7ee50-231">Expression</span><span class="sxs-lookup"><span data-stu-id="7ee50-231">Expression</span></span>  |  <span data-ttu-id="7ee50-232">Meaning</span><span class="sxs-lookup"><span data-stu-id="7ee50-232">Meaning</span></span>  |
|--------------|-----------|
|`CW`|<span data-ttu-id="7ee50-233">Current week</span><span class="sxs-lookup"><span data-stu-id="7ee50-233">Current week</span></span>|
|`CM`|<span data-ttu-id="7ee50-234">Current month</span><span class="sxs-lookup"><span data-stu-id="7ee50-234">Current month</span></span>|

<span data-ttu-id="7ee50-235">The following example shows how to use a number and a time unit.</span><span class="sxs-lookup"><span data-stu-id="7ee50-235">The following example shows how to use a number and a time unit.</span></span> <span data-ttu-id="7ee50-236">A number cannot be larger than 9999.</span><span class="sxs-lookup"><span data-stu-id="7ee50-236">A number cannot be larger than 9999.</span></span>

|  <span data-ttu-id="7ee50-237">Expression</span><span class="sxs-lookup"><span data-stu-id="7ee50-237">Expression</span></span>  |  <span data-ttu-id="7ee50-238">Meaning</span><span class="sxs-lookup"><span data-stu-id="7ee50-238">Meaning</span></span>  |
|--------------|-----------|
|`10D`|<span data-ttu-id="7ee50-239">10 days from today</span><span class="sxs-lookup"><span data-stu-id="7ee50-239">10 days from today</span></span>|
|`2W`|<span data-ttu-id="7ee50-240">2 weeks from today</span><span class="sxs-lookup"><span data-stu-id="7ee50-240">2 weeks from today</span></span>|

<span data-ttu-id="7ee50-241">The following example shows how to use a time unit and a number.</span><span class="sxs-lookup"><span data-stu-id="7ee50-241">The following example shows how to use a time unit and a number.</span></span>

|  <span data-ttu-id="7ee50-242">Expression</span><span class="sxs-lookup"><span data-stu-id="7ee50-242">Expression</span></span>  |  <span data-ttu-id="7ee50-243">Meaning</span><span class="sxs-lookup"><span data-stu-id="7ee50-243">Meaning</span></span>  |
|--------------|-----------|
|`D10`|<span data-ttu-id="7ee50-244">The next 10th day of a month</span><span class="sxs-lookup"><span data-stu-id="7ee50-244">The next 10th day of a month</span></span>|
|`WD4`|<span data-ttu-id="7ee50-245">The next 4th day of a week \(Thursday\)</span><span class="sxs-lookup"><span data-stu-id="7ee50-245">The next 4th day of a week \(Thursday\)</span></span>|

<span data-ttu-id="7ee50-246">The following example shows how you can combine these three forms as needed.</span><span class="sxs-lookup"><span data-stu-id="7ee50-246">The following example shows how you can combine these three forms as needed.</span></span>

|  <span data-ttu-id="7ee50-247">Expression</span><span class="sxs-lookup"><span data-stu-id="7ee50-247">Expression</span></span>  |  <span data-ttu-id="7ee50-248">Meaning</span><span class="sxs-lookup"><span data-stu-id="7ee50-248">Meaning</span></span>  |
|--------------|-----------|
|`CM+10D`|<span data-ttu-id="7ee50-249">Current month \+ 10 days</span><span class="sxs-lookup"><span data-stu-id="7ee50-249">Current month \+ 10 days</span></span>|

<span data-ttu-id="7ee50-250">The following example shows how you can use a minus sign to indicate a date in the past.</span><span class="sxs-lookup"><span data-stu-id="7ee50-250">The following example shows how you can use a minus sign to indicate a date in the past.</span></span>

|  <span data-ttu-id="7ee50-251">Expression</span><span class="sxs-lookup"><span data-stu-id="7ee50-251">Expression</span></span>  |  <span data-ttu-id="7ee50-252">Meaning</span><span class="sxs-lookup"><span data-stu-id="7ee50-252">Meaning</span></span>  |
|--------------|-----------|
|`-1Y`|<span data-ttu-id="7ee50-253">1 year ago from today</span><span class="sxs-lookup"><span data-stu-id="7ee50-253">1 year ago from today</span></span>|

> [!IMPORTANT]
>  <span data-ttu-id="7ee50-254">If the location uses a base calendar, then the date formula that you enter in, for example, the **Shipping Time** field is interpreted according to the calendar working days.</span><span class="sxs-lookup"><span data-stu-id="7ee50-254">If the location uses a base calendar, then the date formula that you enter in, for example, the **Shipping Time** field is interpreted according to the calendar working days.</span></span> <span data-ttu-id="7ee50-255">For example, `1W`  means seven working days.</span><span class="sxs-lookup"><span data-stu-id="7ee50-255">For example, `1W`  means seven working days.</span></span>
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

## <a name="entering-times"></a><span data-ttu-id="7ee50-256">Entering Times</span><span class="sxs-lookup"><span data-stu-id="7ee50-256">Entering Times</span></span>
<span data-ttu-id="7ee50-257">When you enter times, you can insert any non-space separators that you want between the units, but if you use double digits for each unit up to milliseconds, then it is not required.</span><span class="sxs-lookup"><span data-stu-id="7ee50-257">When you enter times, you can insert any non-space separators that you want between the units, but if you use double digits for each unit up to milliseconds, then it is not required.</span></span>

<span data-ttu-id="7ee50-258">You only have to write the largest units that you require; the rest will be set to zero.</span><span class="sxs-lookup"><span data-stu-id="7ee50-258">You only have to write the largest units that you require; the rest will be set to zero.</span></span> <span data-ttu-id="7ee50-259">You can also leave out any AM/PM indicator.</span><span class="sxs-lookup"><span data-stu-id="7ee50-259">You can also leave out any AM/PM indicator.</span></span>

<span data-ttu-id="7ee50-260">The following table lists the various ways in which times can be entered and how they are interpreted.</span><span class="sxs-lookup"><span data-stu-id="7ee50-260">The following table lists the various ways in which times can be entered and how they are interpreted.</span></span> <span data-ttu-id="7ee50-261">It assumes region settings that format times according to: **Hours:Minutes:Seconds.Milliseconds.**</span><span class="sxs-lookup"><span data-stu-id="7ee50-261">It assumes region settings that format times according to: **Hours:Minutes:Seconds.Milliseconds.**</span></span> <span data-ttu-id="7ee50-262">and use the AM and PM indicators of 'AM' and 'PM', respectively.</span><span class="sxs-lookup"><span data-stu-id="7ee50-262">and use the AM and PM indicators of 'AM' and 'PM', respectively.</span></span>

|<span data-ttu-id="7ee50-263">**Entry**</span><span class="sxs-lookup"><span data-stu-id="7ee50-263">**Entry**</span></span>      |<span data-ttu-id="7ee50-264">**Interpretation**</span><span class="sxs-lookup"><span data-stu-id="7ee50-264">**Interpretation**</span></span>      |
|---------------|------------------------|
|`05:23:17`|<span data-ttu-id="7ee50-265">05:23:17</span><span class="sxs-lookup"><span data-stu-id="7ee50-265">05:23:17</span></span>|
|`5`|<span data-ttu-id="7ee50-266">05:00:00</span><span class="sxs-lookup"><span data-stu-id="7ee50-266">05:00:00</span></span>|
|`5AM`|<span data-ttu-id="7ee50-267">05:00:00</span><span class="sxs-lookup"><span data-stu-id="7ee50-267">05:00:00</span></span>|
|`5P`|<span data-ttu-id="7ee50-268">17:00:00</span><span class="sxs-lookup"><span data-stu-id="7ee50-268">17:00:00</span></span>|
|`12`|<span data-ttu-id="7ee50-269">12:00:00</span><span class="sxs-lookup"><span data-stu-id="7ee50-269">12:00:00</span></span>|
|`12A`|<span data-ttu-id="7ee50-270">00:00:00</span><span class="sxs-lookup"><span data-stu-id="7ee50-270">00:00:00</span></span>|
|`12P`|<span data-ttu-id="7ee50-271">12:00:00</span><span class="sxs-lookup"><span data-stu-id="7ee50-271">12:00:00</span></span>|
|`17`|<span data-ttu-id="7ee50-272">17:00:00</span><span class="sxs-lookup"><span data-stu-id="7ee50-272">17:00:00</span></span>|
|`5:30`|<span data-ttu-id="7ee50-273">05:30:00</span><span class="sxs-lookup"><span data-stu-id="7ee50-273">05:30:00</span></span>|
|`0530`|<span data-ttu-id="7ee50-274">05:30:00</span><span class="sxs-lookup"><span data-stu-id="7ee50-274">05:30:00</span></span>|
|`5:30:5`|<span data-ttu-id="7ee50-275">05:30:05</span><span class="sxs-lookup"><span data-stu-id="7ee50-275">05:30:05</span></span>|
|`053005`|<span data-ttu-id="7ee50-276">05:30:05</span><span class="sxs-lookup"><span data-stu-id="7ee50-276">05:30:05</span></span>|
|`5:30:5,50`|<span data-ttu-id="7ee50-277">05:30:05.5</span><span class="sxs-lookup"><span data-stu-id="7ee50-277">05:30:05.5</span></span>|
|`053005050`|<span data-ttu-id="7ee50-278">05:30:05.05</span><span class="sxs-lookup"><span data-stu-id="7ee50-278">05:30:05.05</span></span>|

<span data-ttu-id="7ee50-279">You should be aware that milliseconds are interpreted as decimal notation.</span><span class="sxs-lookup"><span data-stu-id="7ee50-279">You should be aware that milliseconds are interpreted as decimal notation.</span></span> <span data-ttu-id="7ee50-280">So, for example, `3`, `30`, and `300` all mean 300 milliseconds, while `03` means `30` and `003` means 3 milliseconds.</span><span class="sxs-lookup"><span data-stu-id="7ee50-280">So, for example, `3`, `30`, and `300` all mean 300 milliseconds, while `03` means `30` and `003` means 3 milliseconds.</span></span>

<span data-ttu-id="7ee50-281">You cannot use `24:00` to mean midnight, or use any value greater than 24:00.</span><span class="sxs-lookup"><span data-stu-id="7ee50-281">You cannot use `24:00` to mean midnight, or use any value greater than 24:00.</span></span>

<span data-ttu-id="7ee50-282">The word for 'time' in the language used by [!INCLUDE[d365fin](includes/d365fin_long_md.md)] will be evaluated to the current time on your computer or mobile device.</span><span class="sxs-lookup"><span data-stu-id="7ee50-282">The word for 'time' in the language used by [!INCLUDE[d365fin](includes/d365fin_long_md.md)] will be evaluated to the current time on your computer or mobile device.</span></span> <span data-ttu-id="7ee50-283">You can enter any part of the word, starting from the beginning, such as `t` or `TIM`.</span><span class="sxs-lookup"><span data-stu-id="7ee50-283">You can enter any part of the word, starting from the beginning, such as `t` or `TIM`.</span></span>

## <a name="entering-combined-dates-and-times"></a><span data-ttu-id="7ee50-284">Entering combined Dates and Times</span><span class="sxs-lookup"><span data-stu-id="7ee50-284">Entering combined Dates and Times</span></span>
<span data-ttu-id="7ee50-285">When you enter datetimes, which are a date and time combined into one field, you must enter a space between the date and the time.</span><span class="sxs-lookup"><span data-stu-id="7ee50-285">When you enter datetimes, which are a date and time combined into one field, you must enter a space between the date and the time.</span></span> <span data-ttu-id="7ee50-286">The date part can only contain spaces in the form of the official date separator of your region settings.</span><span class="sxs-lookup"><span data-stu-id="7ee50-286">The date part can only contain spaces in the form of the official date separator of your region settings.</span></span> <span data-ttu-id="7ee50-287">The time can contain spaces around the AM/PM indicator.</span><span class="sxs-lookup"><span data-stu-id="7ee50-287">The time can contain spaces around the AM/PM indicator.</span></span>

<span data-ttu-id="7ee50-288">It is also possible to enter only a date in a datetime field, but it is not possible to enter only a time.</span><span class="sxs-lookup"><span data-stu-id="7ee50-288">It is also possible to enter only a date in a datetime field, but it is not possible to enter only a time.</span></span>

<span data-ttu-id="7ee50-289">The following table lists some examples of date/time combinations.</span><span class="sxs-lookup"><span data-stu-id="7ee50-289">The following table lists some examples of date/time combinations.</span></span> <span data-ttu-id="7ee50-290">The region settings in the examples displays dates in the day\-month\-year format, using AM/PM designators, English language, and Sunday as the start of the week.</span><span class="sxs-lookup"><span data-stu-id="7ee50-290">The region settings in the examples displays dates in the day\-month\-year format, using AM/PM designators, English language, and Sunday as the start of the week.</span></span>

|<span data-ttu-id="7ee50-291">**Entry**</span><span class="sxs-lookup"><span data-stu-id="7ee50-291">**Entry**</span></span>      |<span data-ttu-id="7ee50-292">**Interpretation**</span><span class="sxs-lookup"><span data-stu-id="7ee50-292">**Interpretation**</span></span>      |
|---------------|------------------------|
|`08-01-2016 05:48:12 PM`|<span data-ttu-id="7ee50-293">08\-01\-2016 05:48:12 PM</span><span class="sxs-lookup"><span data-stu-id="7ee50-293">08\-01\-2016 05:48:12 PM</span></span>|
|`131202 132455`|<span data-ttu-id="7ee50-294">13\-12\-2002 13:24:55</span><span class="sxs-lookup"><span data-stu-id="7ee50-294">13\-12\-2002 13:24:55</span></span>|
|`1-12-02 10`|<span data-ttu-id="7ee50-295">01\-12\-2002 10:00:00</span><span class="sxs-lookup"><span data-stu-id="7ee50-295">01\-12\-2002 10:00:00</span></span>|
|`1.12.02 5`|<span data-ttu-id="7ee50-296">01\-12\-2002 05:00:00</span><span class="sxs-lookup"><span data-stu-id="7ee50-296">01\-12\-2002 05:00:00</span></span>|
|`1.12.02`|<span data-ttu-id="7ee50-297">01\-12\-2002 00:00:00</span><span class="sxs-lookup"><span data-stu-id="7ee50-297">01\-12\-2002 00:00:00</span></span>|
|`11 12`|<span data-ttu-id="7ee50-298">11\-work date month\-work date year 12:00:00</span><span class="sxs-lookup"><span data-stu-id="7ee50-298">11\-work date month\-work date year 12:00:00</span></span>|
|`1112 12`|<span data-ttu-id="7ee50-299">11\-12\-work date year 12:00:00</span><span class="sxs-lookup"><span data-stu-id="7ee50-299">11\-12\-work date year 12:00:00</span></span>|
|<span data-ttu-id="7ee50-300">`t` or `today`</span><span class="sxs-lookup"><span data-stu-id="7ee50-300">`t` or `today`</span></span>|<span data-ttu-id="7ee50-301">today's date 00:00:00</span><span class="sxs-lookup"><span data-stu-id="7ee50-301">today's date 00:00:00</span></span>|
|`t 10:30`|<span data-ttu-id="7ee50-302">today's date 10:30:00</span><span class="sxs-lookup"><span data-stu-id="7ee50-302">today's date 10:30:00</span></span>|
|`t 3:3:3`|<span data-ttu-id="7ee50-303">today's date 03:03:03</span><span class="sxs-lookup"><span data-stu-id="7ee50-303">today's date 03:03:03</span></span>|
|<span data-ttu-id="7ee50-304">`w` or `workdate`</span><span class="sxs-lookup"><span data-stu-id="7ee50-304">`w` or `workdate`</span></span>|<span data-ttu-id="7ee50-305">the working date 00:00:00</span><span class="sxs-lookup"><span data-stu-id="7ee50-305">the working date 00:00:00</span></span>|
|<span data-ttu-id="7ee50-306">`m` or `Monday`</span><span class="sxs-lookup"><span data-stu-id="7ee50-306">`m` or `Monday`</span></span>|<span data-ttu-id="7ee50-307">Monday of the work date week 00:00:00</span><span class="sxs-lookup"><span data-stu-id="7ee50-307">Monday of the work date week 00:00:00</span></span>|
|<span data-ttu-id="7ee50-308">`tu` or `Tuesday`</span><span class="sxs-lookup"><span data-stu-id="7ee50-308">`tu` or `Tuesday`</span></span>|<span data-ttu-id="7ee50-309">Tuesday of the work date week 00:00:00</span><span class="sxs-lookup"><span data-stu-id="7ee50-309">Tuesday of the work date week 00:00:00</span></span>|
|<span data-ttu-id="7ee50-310">`sa` or `Saturday`</span><span class="sxs-lookup"><span data-stu-id="7ee50-310">`sa` or `Saturday`</span></span>|<span data-ttu-id="7ee50-311">Saturday of the work date week 00:00:00</span><span class="sxs-lookup"><span data-stu-id="7ee50-311">Saturday of the work date week 00:00:00</span></span>|
|<span data-ttu-id="7ee50-312">`s` or `Sunday`</span><span class="sxs-lookup"><span data-stu-id="7ee50-312">`s` or `Sunday`</span></span>|<span data-ttu-id="7ee50-313">Sunday of the work date week 00:00:00</span><span class="sxs-lookup"><span data-stu-id="7ee50-313">Sunday of the work date week 00:00:00</span></span>|
|`tu 10:30`|<span data-ttu-id="7ee50-314">Tuesday of the work date week 10:30:00</span><span class="sxs-lookup"><span data-stu-id="7ee50-314">Tuesday of the work date week 10:30:00</span></span>|
|`tu 3:3:3`|<span data-ttu-id="7ee50-315">Tuesday of the work date week 03:03:03</span><span class="sxs-lookup"><span data-stu-id="7ee50-315">Tuesday of the work date week 03:03:03</span></span>|
|`t23 t`|<span data-ttu-id="7ee50-316">Tuesday of week 23 of the work date year, current time of day</span><span class="sxs-lookup"><span data-stu-id="7ee50-316">Tuesday of week 23 of the work date year, current time of day</span></span>|
|`t23`|<span data-ttu-id="7ee50-317">Tuesday of week 23 of the work date year</span><span class="sxs-lookup"><span data-stu-id="7ee50-317">Tuesday of week 23 of the work date year</span></span>|
|`t 23`|<span data-ttu-id="7ee50-318">Today 23:00:00</span><span class="sxs-lookup"><span data-stu-id="7ee50-318">Today 23:00:00</span></span>|
|`t-1`|<span data-ttu-id="7ee50-319">Tuesday of week 1 of the work date year</span><span class="sxs-lookup"><span data-stu-id="7ee50-319">Tuesday of week 1 of the work date year</span></span>|

## <a name="entering-duration"></a><span data-ttu-id="7ee50-320">Entering Duration</span><span class="sxs-lookup"><span data-stu-id="7ee50-320">Entering Duration</span></span>
<span data-ttu-id="7ee50-321">Some fields in the application represent a duration, or amount of elapsed time, instead of a specific date or time.</span><span class="sxs-lookup"><span data-stu-id="7ee50-321">Some fields in the application represent a duration, or amount of elapsed time, instead of a specific date or time.</span></span> <span data-ttu-id="7ee50-322">You enter a duration as a number followed by its unit of measure.</span><span class="sxs-lookup"><span data-stu-id="7ee50-322">You enter a duration as a number followed by its unit of measure.</span></span>

<span data-ttu-id="7ee50-323">Here are some examples.</span><span class="sxs-lookup"><span data-stu-id="7ee50-323">Here are some examples.</span></span>

|<span data-ttu-id="7ee50-324">**Duration**</span><span class="sxs-lookup"><span data-stu-id="7ee50-324">**Duration**</span></span>|<span data-ttu-id="7ee50-325">**Unit of measure**</span><span class="sxs-lookup"><span data-stu-id="7ee50-325">**Unit of measure**</span></span>|
|------------|-------------------|
|`2h`|<span data-ttu-id="7ee50-326">2 hrs</span><span class="sxs-lookup"><span data-stu-id="7ee50-326">2 hrs</span></span>|
|`6h 30 m`|<span data-ttu-id="7ee50-327">6 hrs 30 mins</span><span class="sxs-lookup"><span data-stu-id="7ee50-327">6 hrs 30 mins</span></span>|
|`6.5h`|<span data-ttu-id="7ee50-328">6 hrs 30 mins</span><span class="sxs-lookup"><span data-stu-id="7ee50-328">6 hrs 30 mins</span></span>|
|`90m`|<span data-ttu-id="7ee50-329">1 hr 30 mins</span><span class="sxs-lookup"><span data-stu-id="7ee50-329">1 hr 30 mins</span></span>|
|`2d 6h 30m`|<span data-ttu-id="7ee50-330">2 days 6 hrs 30 mins</span><span class="sxs-lookup"><span data-stu-id="7ee50-330">2 days 6 hrs 30 mins</span></span>|
|`2d 6h 30m 56s 600ms`|<span data-ttu-id="7ee50-331">2 days 6 hrs 30 mins 56 secs 600 msecs</span><span class="sxs-lookup"><span data-stu-id="7ee50-331">2 days 6 hrs 30 mins 56 secs 600 msecs</span></span>|

<span data-ttu-id="7ee50-332">You can also enter a number, which will be automatically converted to a duration.</span><span class="sxs-lookup"><span data-stu-id="7ee50-332">You can also enter a number, which will be automatically converted to a duration.</span></span> <span data-ttu-id="7ee50-333">The number you enter is converted according to the default unit of measure that has been specified for the duration field.</span><span class="sxs-lookup"><span data-stu-id="7ee50-333">The number you enter is converted according to the default unit of measure that has been specified for the duration field.</span></span>

<span data-ttu-id="7ee50-334">To see what unit of measure is being used in a duration field, enter a number and see which unit of measure it is converted to.</span><span class="sxs-lookup"><span data-stu-id="7ee50-334">To see what unit of measure is being used in a duration field, enter a number and see which unit of measure it is converted to.</span></span>

<span data-ttu-id="7ee50-335">For example, if the unit of measure is hours, the number `5` is converted to 5 hrs.</span><span class="sxs-lookup"><span data-stu-id="7ee50-335">For example, if the unit of measure is hours, the number `5` is converted to 5 hrs.</span></span>


## <a name="see-also"></a><span data-ttu-id="7ee50-336">See Also</span><span class="sxs-lookup"><span data-stu-id="7ee50-336">See Also</span></span>
<span data-ttu-id="7ee50-337">[Working with [!INCLUDE[d365fin](includes/d365fin_long_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="7ee50-337">[Working with [!INCLUDE[d365fin](includes/d365fin_long_md.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="7ee50-338">Date Calculation for Purchases</span><span class="sxs-lookup"><span data-stu-id="7ee50-338">Date Calculation for Purchases</span></span>](purchasing-date-calculation-for-purchases.md)  
[<span data-ttu-id="7ee50-339">Entering Criteria in Filters</span><span class="sxs-lookup"><span data-stu-id="7ee50-339">Entering Criteria in Filters </span></span>](ui-enter-criteria-filters.md)  

