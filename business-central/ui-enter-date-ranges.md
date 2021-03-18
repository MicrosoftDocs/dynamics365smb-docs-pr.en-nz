---
title: Entering dates and times in Business Central  | Microsoft Docs
description: Learn how to enter dates and times including various productivity tips such as shorthand, expressions and ranges. Filter lists or reports down to specific date or time periods.
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: dates, reporting, filter, calendar, shorthand, range
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 3a48863231c06742e5cc1b2f13d554e65cb8ae91
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "5381231"
---
# <a name="working-with-calendar-dates-and-times"></a><span data-ttu-id="ebe65-104">Working with Calendar Dates and Times</span><span class="sxs-lookup"><span data-stu-id="ebe65-104">Working with Calendar Dates and Times</span></span>

[!INCLUDE[prod_short](includes/prod_long.md)] <span data-ttu-id="ebe65-105">offers multiple ways to enter dates and times, including powerful features that accelerate data entry, or help you write complex calendar expressions.</span><span class="sxs-lookup"><span data-stu-id="ebe65-105">offers multiple ways to enter dates and times, including powerful features that accelerate data entry, or help you write complex calendar expressions.</span></span> <span data-ttu-id="ebe65-106">There are various places throughout the application where you can enter dates and times in fields.</span><span class="sxs-lookup"><span data-stu-id="ebe65-106">There are various places throughout the application where you can enter dates and times in fields.</span></span> <span data-ttu-id="ebe65-107">For example, on a sales order, you can set the shipment date.</span><span class="sxs-lookup"><span data-stu-id="ebe65-107">For example, on a sales order, you can set the shipment date.</span></span> <span data-ttu-id="ebe65-108">When filtering lists or report data, you can enter dates and times to pinpoint only the data that you are interested in.</span><span class="sxs-lookup"><span data-stu-id="ebe65-108">When filtering lists or report data, you can enter dates and times to pinpoint only the data that you are interested in.</span></span>

## <a name="check-your-region-and-language-settings"></a><span data-ttu-id="ebe65-109">Check your region and language settings</span><span class="sxs-lookup"><span data-stu-id="ebe65-109">Check your region and language settings</span></span>
<span data-ttu-id="ebe65-110">The **My Settings** page specifies the **Region** and **Language** that you are using in the application.</span><span class="sxs-lookup"><span data-stu-id="ebe65-110">The **My Settings** page specifies the **Region** and **Language** that you are using in the application.</span></span> <span data-ttu-id="ebe65-111">These settings influence how you enter dates and times.</span><span class="sxs-lookup"><span data-stu-id="ebe65-111">These settings influence how you enter dates and times.</span></span>

-   <span data-ttu-id="ebe65-112">The **Region** setting determines how dates, times, numbers, and currencies are shown or formatted.</span><span class="sxs-lookup"><span data-stu-id="ebe65-112">The **Region** setting determines how dates, times, numbers, and currencies are shown or formatted.</span></span>

-   <span data-ttu-id="ebe65-113">For date patterns that involve words, the language of the words that you use must correspond to the **Language** setting.</span><span class="sxs-lookup"><span data-stu-id="ebe65-113">For date patterns that involve words, the language of the words that you use must correspond to the **Language** setting.</span></span>

> [!NOTE]
> [!INCLUDE[prod_short](includes/prod_long.md)] <span data-ttu-id="ebe65-114">uses the Gregorian calendar system.</span><span class="sxs-lookup"><span data-stu-id="ebe65-114">uses the Gregorian calendar system.</span></span>

<!--
The following sections describe how you can enter dates, times, datetimes, durations, date ranges, and how you use date formulas.
-->

## <a name="entering-dates"></a><span data-ttu-id="ebe65-115">Entering Dates</span><span class="sxs-lookup"><span data-stu-id="ebe65-115">Entering Dates</span></span>

<span data-ttu-id="ebe65-116">In a date field, you can enter a date using the standard format for your region setting.</span><span class="sxs-lookup"><span data-stu-id="ebe65-116">In a date field, you can enter a date using the standard format for your region setting.</span></span> <span data-ttu-id="ebe65-117">Different regions can use different separators between the days, months and years.</span><span class="sxs-lookup"><span data-stu-id="ebe65-117">Different regions can use different separators between the days, months and years.</span></span> <span data-ttu-id="ebe65-118">For example, some regions use dashes (mm-dd-yyyy) and others use forward slashes (mm/dd/yyyy).</span><span class="sxs-lookup"><span data-stu-id="ebe65-118">For example, some regions use dashes (mm-dd-yyyy) and others use forward slashes (mm/dd/yyyy).</span></span> <span data-ttu-id="ebe65-119">However, you can use any separators, even a space, and the date will automatically be changed to use separators that match your region.</span><span class="sxs-lookup"><span data-stu-id="ebe65-119">However, you can use any separators, even a space, and the date will automatically be changed to use separators that match your region.</span></span>

<span data-ttu-id="ebe65-120">Note that the format in which dates are displayed on printed reports or emailed documents is not influenced by your personal choice of region setting.</span><span class="sxs-lookup"><span data-stu-id="ebe65-120">Note that the format in which dates are displayed on printed reports or emailed documents is not influenced by your personal choice of region setting.</span></span>

<span data-ttu-id="ebe65-121">To work more productively with dates and times, you can use any of the methods or formats that are described in the following sections.</span><span class="sxs-lookup"><span data-stu-id="ebe65-121">To work more productively with dates and times, you can use any of the methods or formats that are described in the following sections.</span></span>

### <a name="picking-dates-from-the-calendar"></a><span data-ttu-id="ebe65-122">Picking dates from the calendar</span><span class="sxs-lookup"><span data-stu-id="ebe65-122">Picking dates from the calendar</span></span>

<span data-ttu-id="ebe65-123">Any field displaying a calendar icon can be set using the calendar date picker.</span><span class="sxs-lookup"><span data-stu-id="ebe65-123">Any field displaying a calendar icon can be set using the calendar date picker.</span></span> <span data-ttu-id="ebe65-124">To display the calendar date picker, activate the calendar icon or press the Ctrl + Home keyboard shortcut in the field.</span><span class="sxs-lookup"><span data-stu-id="ebe65-124">To display the calendar date picker, activate the calendar icon or press the Ctrl + Home keyboard shortcut in the field.</span></span>

<span data-ttu-id="ebe65-125">![Date fields](media/ui-date-field.png "Example of a date field")</span><span class="sxs-lookup"><span data-stu-id="ebe65-125">![Date fields](media/ui-date-field.png "Example of a date field")</span></span>

<span data-ttu-id="ebe65-126">See also [Keyboard Shortcuts in the calendar date picker](keyboard-shortcuts.md#calendarshortcuts).</span><span class="sxs-lookup"><span data-stu-id="ebe65-126">See also [Keyboard Shortcuts in the calendar date picker](keyboard-shortcuts.md#calendarshortcuts).</span></span>

### <a name="day-week-year-pattern"></a><span data-ttu-id="ebe65-127">Day\-week\-year pattern</span><span class="sxs-lookup"><span data-stu-id="ebe65-127">Day\-week\-year pattern</span></span>

<span data-ttu-id="ebe65-128">You can enter a date as a weekday followed by a week number and, optionally, a year.</span><span class="sxs-lookup"><span data-stu-id="ebe65-128">You can enter a date as a weekday followed by a week number and, optionally, a year.</span></span> <span data-ttu-id="ebe65-129">For example, Mon25 or mon25 means Monday in week 25.</span><span class="sxs-lookup"><span data-stu-id="ebe65-129">For example, Mon25 or mon25 means Monday in week 25.</span></span> <span data-ttu-id="ebe65-130">If you do not enter a year, the year of the work date is used.</span><span class="sxs-lookup"><span data-stu-id="ebe65-130">If you do not enter a year, the year of the work date is used.</span></span>

<span data-ttu-id="ebe65-131">Instead of entering the entire word for the day of the week, you can enter part of the word, starting from the beginning.</span><span class="sxs-lookup"><span data-stu-id="ebe65-131">Instead of entering the entire word for the day of the week, you can enter part of the word, starting from the beginning.</span></span> <span data-ttu-id="ebe65-132">In case of conflicts (such as with s which could be Saturday or Sunday), the days are evaluated according to the region setting.</span><span class="sxs-lookup"><span data-stu-id="ebe65-132">In case of conflicts (such as with s which could be Saturday or Sunday), the days are evaluated according to the region setting.</span></span> <span data-ttu-id="ebe65-133">The input is first evaluated against workdate and today as well, so keep this in mind when abbreviating.</span><span class="sxs-lookup"><span data-stu-id="ebe65-133">The input is first evaluated against workdate and today as well, so keep this in mind when abbreviating.</span></span> <span data-ttu-id="ebe65-134">For example, t already means today, so it cannot mean Tuesday or Thursday.</span><span class="sxs-lookup"><span data-stu-id="ebe65-134">For example, t already means today, so it cannot mean Tuesday or Thursday.</span></span>

<span data-ttu-id="ebe65-135">The week number scheme is always ISO 8601, where week 1 is the week with 4 January in it, or the week with the first Thursday of the year.</span><span class="sxs-lookup"><span data-stu-id="ebe65-135">The week number scheme is always ISO 8601, where week 1 is the week with 4 January in it, or the week with the first Thursday of the year.</span></span>

### <a name="digit-patterns"></a><span data-ttu-id="ebe65-136">Digit patterns</span><span class="sxs-lookup"><span data-stu-id="ebe65-136">Digit patterns</span></span>

<span data-ttu-id="ebe65-137">In a date field you can enter two, four, six, or eight digits:</span><span class="sxs-lookup"><span data-stu-id="ebe65-137">In a date field you can enter two, four, six, or eight digits:</span></span>

-   <span data-ttu-id="ebe65-138">If you enter only two digits, this is interpreted as the day, and it will add the month and the year of the work date.</span><span class="sxs-lookup"><span data-stu-id="ebe65-138">If you enter only two digits, this is interpreted as the day, and it will add the month and the year of the work date.</span></span>

-   <span data-ttu-id="ebe65-139">If you enter four digits, this is interpreted as the day and the month, and it will add the year of the work date.</span><span class="sxs-lookup"><span data-stu-id="ebe65-139">If you enter four digits, this is interpreted as the day and the month, and it will add the year of the work date.</span></span> <span data-ttu-id="ebe65-140">The order of the day and month is determined by your region settings.</span><span class="sxs-lookup"><span data-stu-id="ebe65-140">The order of the day and month is determined by your region settings.</span></span> <span data-ttu-id="ebe65-141">Even if your region settings have the year before the day and month, four digits are interpreted as the day and month.</span><span class="sxs-lookup"><span data-stu-id="ebe65-141">Even if your region settings have the year before the day and month, four digits are interpreted as the day and month.</span></span>

-   <span data-ttu-id="ebe65-142">If the date you want to enter is in the range 01/01/1930 through 12/31/2029, you can enter the year with two digits; otherwise, enter the year with four digits.</span><span class="sxs-lookup"><span data-stu-id="ebe65-142">If the date you want to enter is in the range 01/01/1930 through 12/31/2029, you can enter the year with two digits; otherwise, enter the year with four digits.</span></span>

### <a name="today"></a><span data-ttu-id="ebe65-143">Today</span><span class="sxs-lookup"><span data-stu-id="ebe65-143">Today</span></span>

<span data-ttu-id="ebe65-144">Enter the word for today, in the language set by **Language** setting, that will set the date to the current date.</span><span class="sxs-lookup"><span data-stu-id="ebe65-144">Enter the word for today, in the language set by **Language** setting, that will set the date to the current date.</span></span> <span data-ttu-id="ebe65-145">Instead of entering the entire word, you can enter part of the word, starting from the beginning, such as t or tod, as long as it is not also the start of another word.</span><span class="sxs-lookup"><span data-stu-id="ebe65-145">Instead of entering the entire word, you can enter part of the word, starting from the beginning, such as t or tod, as long as it is not also the start of another word.</span></span>

### <a name="period"></a><span data-ttu-id="ebe65-146">Period</span><span class="sxs-lookup"><span data-stu-id="ebe65-146">Period</span></span>

<span data-ttu-id="ebe65-147">To filter on a specific accounting period, in a date field enter the letter p, or the word period, followed by a number that identifies the accounting period, like p2 or period4.</span><span class="sxs-lookup"><span data-stu-id="ebe65-147">To filter on a specific accounting period, in a date field enter the letter p, or the word period, followed by a number that identifies the accounting period, like p2 or period4.</span></span> <span data-ttu-id="ebe65-148">The accounting period is relative to the fiscal year of the current work date that set in your Role Centre.</span><span class="sxs-lookup"><span data-stu-id="ebe65-148">The accounting period is relative to the fiscal year of the current work date that set in your Role Center.</span></span> <span data-ttu-id="ebe65-149">For example, if the work date is **03/21/20**, then p1, or just p, filters on the first accounting period of the fiscal year 2020 (such as 01/01/20..01/31/20).</span><span class="sxs-lookup"><span data-stu-id="ebe65-149">For example, if the work date is **03/21/20**, then p1, or just p, filters on the first accounting period of the fiscal year 2020 (such as 01/01/20..01/31/20).</span></span> <span data-ttu-id="ebe65-150">p15 filters on the fifteenth accounting period from the start of fiscal year 2020 (such as 03/01/21..03/31/21).</span><span class="sxs-lookup"><span data-stu-id="ebe65-150">p15 filters on the fifteenth accounting period from the start of fiscal year 2020 (such as 03/01/21..03/31/21).</span></span>

<span data-ttu-id="ebe65-151">The accounting periods are defined on the **Accounting Periods** page.</span><span class="sxs-lookup"><span data-stu-id="ebe65-151">The accounting periods are defined on the **Accounting Periods** page.</span></span> <span data-ttu-id="ebe65-152">To view or change the accounting periods, open the page [here](https://businesscentral.dynamics.com/?page=100).</span><span class="sxs-lookup"><span data-stu-id="ebe65-152">To view or change the accounting periods, open the page [here](https://businesscentral.dynamics.com/?page=100).</span></span>

### <a name="current-work-date"></a><span data-ttu-id="ebe65-153">Current work date</span><span class="sxs-lookup"><span data-stu-id="ebe65-153">Current work date</span></span>

<span data-ttu-id="ebe65-154">The work date feature allows you to record transactions using a date that is different from the current date.</span><span class="sxs-lookup"><span data-stu-id="ebe65-154">The work date feature allows you to record transactions using a date that is different from the current date.</span></span>

<span data-ttu-id="ebe65-155">The word for 'workdate', in the language set by **Language** setting, will set the date to the currently set work date that is specified on the **My Settings** page.</span><span class="sxs-lookup"><span data-stu-id="ebe65-155">The word for 'workdate', in the language set by **Language** setting, will set the date to the currently set work date that is specified on the **My Settings** page.</span></span> <span data-ttu-id="ebe65-156">Instead of entering the entire word, you can enter part of the word, starting from the beginning, such as 'w' or 'work'.</span><span class="sxs-lookup"><span data-stu-id="ebe65-156">Instead of entering the entire word, you can enter part of the word, starting from the beginning, such as 'w' or 'work'.</span></span>

<span data-ttu-id="ebe65-157">If you have not defined a work date, the current date will be used as the work date.</span><span class="sxs-lookup"><span data-stu-id="ebe65-157">If you have not defined a work date, the current date will be used as the work date.</span></span> <span data-ttu-id="ebe65-158">You may want to use a work date if you have many transactions with a date other than today's date.</span><span class="sxs-lookup"><span data-stu-id="ebe65-158">You may want to use a work date if you have many transactions with a date other than today's date.</span></span>

<span data-ttu-id="ebe65-159">See also [Change Basic Settings, such as the Work Date](ui-change-basic-settings.md#work-date).</span><span class="sxs-lookup"><span data-stu-id="ebe65-159">See also [Change Basic Settings, such as the Work Date](ui-change-basic-settings.md#work-date).</span></span>

### <a name="closing-date"></a><span data-ttu-id="ebe65-160">Closing Date</span><span class="sxs-lookup"><span data-stu-id="ebe65-160">Closing Date</span></span>

<span data-ttu-id="ebe65-161">When you close a fiscal year, you can use closing dates to indicate that an entry is a closing entry.</span><span class="sxs-lookup"><span data-stu-id="ebe65-161">When you close a fiscal year, you can use closing dates to indicate that an entry is a closing entry.</span></span> <span data-ttu-id="ebe65-162">A closing date technically is between two dates, for example between Dec 31 and Jan 1.</span><span class="sxs-lookup"><span data-stu-id="ebe65-162">A closing date technically is between two dates, for example between Dec 31 and Jan 1.</span></span>

<span data-ttu-id="ebe65-163">To specify that a date is a closing date, put C just before the date, such as C123101.</span><span class="sxs-lookup"><span data-stu-id="ebe65-163">To specify that a date is a closing date, put C just before the date, such as C123101.</span></span> <span data-ttu-id="ebe65-164">This can be used in combination with all the date patterns.</span><span class="sxs-lookup"><span data-stu-id="ebe65-164">This can be used in combination with all the date patterns.</span></span>

### <a name="examples"></a><span data-ttu-id="ebe65-165">Examples</span><span class="sxs-lookup"><span data-stu-id="ebe65-165">Examples</span></span>

<span data-ttu-id="ebe65-166">The following table contains examples of dates using all the formats.</span><span class="sxs-lookup"><span data-stu-id="ebe65-166">The following table contains examples of dates using all the formats.</span></span> <span data-ttu-id="ebe65-167">It assumes region settings that format dates according to: **year.month.day.**, a week starting on Monday, and the English language.</span><span class="sxs-lookup"><span data-stu-id="ebe65-167">It assumes region settings that format dates according to: **year.month.day.**, a week starting on Monday, and the English language.</span></span>

|<span data-ttu-id="ebe65-168">**Entry**</span><span class="sxs-lookup"><span data-stu-id="ebe65-168">**Entry**</span></span>      |<span data-ttu-id="ebe65-169">**Interpretation**</span><span class="sxs-lookup"><span data-stu-id="ebe65-169">**Interpretation**</span></span>      |
|---------------|------------------------|
|<span data-ttu-id="ebe65-170">2018.12.31.</span><span class="sxs-lookup"><span data-stu-id="ebe65-170">2018.12.31.</span></span>|<span data-ttu-id="ebe65-171">2018.12.31.</span><span class="sxs-lookup"><span data-stu-id="ebe65-171">2018.12.31.</span></span>|
|<span data-ttu-id="ebe65-172">181231</span><span class="sxs-lookup"><span data-stu-id="ebe65-172">181231</span></span>|<span data-ttu-id="ebe65-173">2018.12.31.</span><span class="sxs-lookup"><span data-stu-id="ebe65-173">2018.12.31.</span></span>|
|<span data-ttu-id="ebe65-174">18.12.31.</span><span class="sxs-lookup"><span data-stu-id="ebe65-174">18.12.31.</span></span>|<span data-ttu-id="ebe65-175">2018.12.31.</span><span class="sxs-lookup"><span data-stu-id="ebe65-175">2018.12.31.</span></span>|
|<span data-ttu-id="ebe65-176">18.12.31.</span><span class="sxs-lookup"><span data-stu-id="ebe65-176">18.12.31.</span></span>|<span data-ttu-id="ebe65-177">2018.12.31.</span><span class="sxs-lookup"><span data-stu-id="ebe65-177">2018.12.31.</span></span>|
|<span data-ttu-id="ebe65-178">20181231</span><span class="sxs-lookup"><span data-stu-id="ebe65-178">20181231</span></span>|<span data-ttu-id="ebe65-179">2018.12.31.</span><span class="sxs-lookup"><span data-stu-id="ebe65-179">2018.12.31.</span></span>|
|<span data-ttu-id="ebe65-180">18/12,31</span><span class="sxs-lookup"><span data-stu-id="ebe65-180">18/12,31</span></span>|<span data-ttu-id="ebe65-181">2018.12.31.</span><span class="sxs-lookup"><span data-stu-id="ebe65-181">2018.12.31.</span></span>|
|<span data-ttu-id="ebe65-182">11</span><span class="sxs-lookup"><span data-stu-id="ebe65-182">11</span></span>|<span data-ttu-id="ebe65-183">work date year.work date month.11.</span><span class="sxs-lookup"><span data-stu-id="ebe65-183">work date year.work date month.11.</span></span>|
|<span data-ttu-id="ebe65-184">1112</span><span class="sxs-lookup"><span data-stu-id="ebe65-184">1112</span></span>|<span data-ttu-id="ebe65-185">work date year.11.12.</span><span class="sxs-lookup"><span data-stu-id="ebe65-185">work date year.11.12.</span></span>|
|<span data-ttu-id="ebe65-186">t or today</span><span class="sxs-lookup"><span data-stu-id="ebe65-186">t or today</span></span>|<span data-ttu-id="ebe65-187">today's date</span><span class="sxs-lookup"><span data-stu-id="ebe65-187">today's date</span></span>|
|<span data-ttu-id="ebe65-188">p4</span><span class="sxs-lookup"><span data-stu-id="ebe65-188">p4</span></span>|<span data-ttu-id="ebe65-189">date range that includes the fourth accounting period, such as 04/01/20..04/30/20</span><span class="sxs-lookup"><span data-stu-id="ebe65-189">date range that includes the fourth accounting period, such as 04/01/20..04/30/20</span></span>|
|<span data-ttu-id="ebe65-190">w or workdate</span><span class="sxs-lookup"><span data-stu-id="ebe65-190">w or workdate</span></span>|<span data-ttu-id="ebe65-191">the working date</span><span class="sxs-lookup"><span data-stu-id="ebe65-191">the working date</span></span>|
|<span data-ttu-id="ebe65-192">m or Monday</span><span class="sxs-lookup"><span data-stu-id="ebe65-192">m or Monday</span></span>|<span data-ttu-id="ebe65-193">Monday of the work date week</span><span class="sxs-lookup"><span data-stu-id="ebe65-193">Monday of the work date week</span></span>|
|<span data-ttu-id="ebe65-194">tu or Tuesday</span><span class="sxs-lookup"><span data-stu-id="ebe65-194">tu or Tuesday</span></span>|<span data-ttu-id="ebe65-195">Tuesday of the work date week</span><span class="sxs-lookup"><span data-stu-id="ebe65-195">Tuesday of the work date week</span></span>|
|<span data-ttu-id="ebe65-196">sa or Saturday</span><span class="sxs-lookup"><span data-stu-id="ebe65-196">sa or Saturday</span></span>|<span data-ttu-id="ebe65-197">Saturday of the work date week</span><span class="sxs-lookup"><span data-stu-id="ebe65-197">Saturday of the work date week</span></span>|
|<span data-ttu-id="ebe65-198">s or Sunday</span><span class="sxs-lookup"><span data-stu-id="ebe65-198">s or Sunday</span></span>|<span data-ttu-id="ebe65-199">Sunday of the work date week</span><span class="sxs-lookup"><span data-stu-id="ebe65-199">Sunday of the work date week</span></span>|
|<span data-ttu-id="ebe65-200">t23</span><span class="sxs-lookup"><span data-stu-id="ebe65-200">t23</span></span>|<span data-ttu-id="ebe65-201">Tuesday of week 23 of the work date year</span><span class="sxs-lookup"><span data-stu-id="ebe65-201">Tuesday of week 23 of the work date year</span></span>|
|<span data-ttu-id="ebe65-202">t 23</span><span class="sxs-lookup"><span data-stu-id="ebe65-202">t 23</span></span>|<span data-ttu-id="ebe65-203">Tuesday of week 23 of the work date year</span><span class="sxs-lookup"><span data-stu-id="ebe65-203">Tuesday of week 23 of the work date year</span></span>|
|<span data-ttu-id="ebe65-204">t-1</span><span class="sxs-lookup"><span data-stu-id="ebe65-204">t-1</span></span>|<span data-ttu-id="ebe65-205">Tuesday of week 1 of the work date year</span><span class="sxs-lookup"><span data-stu-id="ebe65-205">Tuesday of week 1 of the work date year</span></span>|

##  <a name="setting-ranges"></a><a name="BKMK_SettingDateRanges"></a> <span data-ttu-id="ebe65-206">Setting Ranges</span><span class="sxs-lookup"><span data-stu-id="ebe65-206">Setting Ranges</span></span>

<span data-ttu-id="ebe65-207">On lists, totals and reports, you can set filters on dates, times and datetimes containing a start value and optionally an end value to display only the data contained in that range.</span><span class="sxs-lookup"><span data-stu-id="ebe65-207">On lists, totals and reports, you can set filters on dates, times and datetimes containing a start value and optionally an end value to display only the data contained in that range.</span></span> <span data-ttu-id="ebe65-208">The standard rules apply to the way you set date ranges.</span><span class="sxs-lookup"><span data-stu-id="ebe65-208">The standard rules apply to the way you set date ranges.</span></span>

|<span data-ttu-id="ebe65-209">**Meaning**</span><span class="sxs-lookup"><span data-stu-id="ebe65-209">**Meaning**</span></span>|<span data-ttu-id="ebe65-210">**Sample expression (Date)**</span><span class="sxs-lookup"><span data-stu-id="ebe65-210">**Sample expression (Date)**</span></span>|<span data-ttu-id="ebe65-211">**Data included in the filter**</span><span class="sxs-lookup"><span data-stu-id="ebe65-211">**Data included in the filter**</span></span>|
|-----------|---------------------|--------------------|
|<span data-ttu-id="ebe65-212">Interval</span><span class="sxs-lookup"><span data-stu-id="ebe65-212">Interval</span></span>|<span data-ttu-id="ebe65-213">12 15 00..01 15 01</span><span class="sxs-lookup"><span data-stu-id="ebe65-213">12 15 00..01 15 01</span></span><br /><br /><span data-ttu-id="ebe65-214">..12 15 00</span><span class="sxs-lookup"><span data-stu-id="ebe65-214">..12 15 00</span></span><br /><br /><span data-ttu-id="ebe65-215">p1..p4</span><span class="sxs-lookup"><span data-stu-id="ebe65-215">p1..p4</span></span>|<span data-ttu-id="ebe65-216">Records with dates between and including 12 15 00 and 01 15 01.</span><span class="sxs-lookup"><span data-stu-id="ebe65-216">Records with dates between and including 12 15 00 and 01 15 01.</span></span><br /><br /><span data-ttu-id="ebe65-217">Records with dates of 12 15 00 or earlier.</span><span class="sxs-lookup"><span data-stu-id="ebe65-217">Records with dates of 12 15 00 or earlier.</span></span><br /><br /><span data-ttu-id="ebe65-218">Date range that includes the second, third, and fourth accounting periods, such as 01/01/20..04/30/20.</span><span class="sxs-lookup"><span data-stu-id="ebe65-218">Date range that includes the second, third, and fourth accounting periods, such as 01/01/20..04/30/20.</span></span>|
|<span data-ttu-id="ebe65-219">Either/or</span><span class="sxs-lookup"><span data-stu-id="ebe65-219">Either/or</span></span>|<span data-ttu-id="ebe65-220">12 15 00\|12 16 00</span><span class="sxs-lookup"><span data-stu-id="ebe65-220">12 15 00\|12 16 00</span></span>|<span data-ttu-id="ebe65-221">Records with dates of either 12 15 00 or 12 16 00.</span><span class="sxs-lookup"><span data-stu-id="ebe65-221">Records with dates of either 12 15 00 or 12 16 00.</span></span> <span data-ttu-id="ebe65-222">If there are records with dates on both days, they will all be displayed.</span><span class="sxs-lookup"><span data-stu-id="ebe65-222">If there are records with dates on both days, they will all be displayed.</span></span>|
|<span data-ttu-id="ebe65-223">Combination</span><span class="sxs-lookup"><span data-stu-id="ebe65-223">Combination</span></span>|<span data-ttu-id="ebe65-224">12 15 00\|12 01 00..12 10 00</span><span class="sxs-lookup"><span data-stu-id="ebe65-224">12 15 00\|12 01 00..12 10 00</span></span>  <br /><br /><span data-ttu-id="ebe65-225">..12 14 00\|12 30 00..</span><span class="sxs-lookup"><span data-stu-id="ebe65-225">..12 14 00\|12 30 00..</span></span>|<span data-ttu-id="ebe65-226">Records with dates of 12 15 00 or on dates between and including 12 01 00 and 12 10 00.</span><span class="sxs-lookup"><span data-stu-id="ebe65-226">Records with dates of 12 15 00 or on dates between and including 12 01 00 and 12 10 00.</span></span>  <br /><br /><span data-ttu-id="ebe65-227">Records with dates of 12 14 00 or earlier, or dates of 12 30 00 or later, that is, all records except those with dates between and including 12 15 00 and 12 29 00.</span><span class="sxs-lookup"><span data-stu-id="ebe65-227">Records with dates of 12 14 00 or earlier, or dates of 12 30 00 or later, that is, all records except those with dates between and including 12 15 00 and 12 29 00.</span></span>|

<span data-ttu-id="ebe65-228">You can use any of the valid formats in date range filters.</span><span class="sxs-lookup"><span data-stu-id="ebe65-228">You can use any of the valid formats in date range filters.</span></span> <span data-ttu-id="ebe65-229">For example, mon14 3..t 4p applied on a datetime field results in a filter from 3 AM on Monday in week 14 of the current work date year, inclusive, until today at 4PM, inclusive.</span><span class="sxs-lookup"><span data-stu-id="ebe65-229">For example, mon14 3..t 4p applied on a datetime field results in a filter from 3 AM on Monday in week 14 of the current work date year, inclusive, until today at 4PM, inclusive.</span></span>

## <a name="using-date-formulas"></a><span data-ttu-id="ebe65-230">Using Date Formulas</span><span class="sxs-lookup"><span data-stu-id="ebe65-230">Using Date Formulas</span></span>
<span data-ttu-id="ebe65-231">A date formula is a short, abbreviated combination of letters and numbers that specifies how to calculate dates.</span><span class="sxs-lookup"><span data-stu-id="ebe65-231">A date formula is a short, abbreviated combination of letters and numbers that specifies how to calculate dates.</span></span> <span data-ttu-id="ebe65-232">You can enter date formulas in various date calculation fields or filters.</span><span class="sxs-lookup"><span data-stu-id="ebe65-232">You can enter date formulas in various date calculation fields or filters.</span></span>

> [!NOTE]
>  <span data-ttu-id="ebe65-233">In all data formula fields, one day is automatically included to cover today as the day when the period starts.</span><span class="sxs-lookup"><span data-stu-id="ebe65-233">In all data formula fields, one day is automatically included to cover today as the day when the period starts.</span></span> <span data-ttu-id="ebe65-234">Accordingly, for example, if you enter 1W, then the period is actually eight days because today is included.</span><span class="sxs-lookup"><span data-stu-id="ebe65-234">Accordingly, for example, if you enter 1W, then the period is actually eight days because today is included.</span></span> <span data-ttu-id="ebe65-235">To specify a period of seven days \(one true week\) including the period starting date, then you must enter 6D or 1W-1D.</span><span class="sxs-lookup"><span data-stu-id="ebe65-235">To specify a period of seven days \(one true week\) including the period starting date, then you must enter 6D or 1W-1D.</span></span>

<span data-ttu-id="ebe65-236">Here are some examples of how date formulas can be used:</span><span class="sxs-lookup"><span data-stu-id="ebe65-236">Here are some examples of how date formulas can be used:</span></span>

-   <span data-ttu-id="ebe65-237">The date formula in the recurring frequency field in recurring journals determines how often the entry on the journal line will be posted.</span><span class="sxs-lookup"><span data-stu-id="ebe65-237">The date formula in the recurring frequency field in recurring journals determines how often the entry on the journal line will be posted.</span></span>

-   <span data-ttu-id="ebe65-238">The date formula in the **Grace Period** field for a specified reminder level determines the period of time that must pass from the due date \(or from the date of the previous reminder\) before a reminder will be created.</span><span class="sxs-lookup"><span data-stu-id="ebe65-238">The date formula in the **Grace Period** field for a specified reminder level determines the period of time that must pass from the due date \(or from the date of the previous reminder\) before a reminder will be created.</span></span>

-   <span data-ttu-id="ebe65-239">The date formula in the **Due Date Calculation** field determines how to calculate the due date on the reminder.</span><span class="sxs-lookup"><span data-stu-id="ebe65-239">The date formula in the **Due Date Calculation** field determines how to calculate the due date on the reminder.</span></span>

<span data-ttu-id="ebe65-240">The date formula can contain a maximum of 20 characters, both numbers and letters.</span><span class="sxs-lookup"><span data-stu-id="ebe65-240">The date formula can contain a maximum of 20 characters, both numbers and letters.</span></span> <span data-ttu-id="ebe65-241">You can use the following letters, which are abbreviations for calendar units.</span><span class="sxs-lookup"><span data-stu-id="ebe65-241">You can use the following letters, which are abbreviations for calendar units.</span></span>

|  <span data-ttu-id="ebe65-242">Letter</span><span class="sxs-lookup"><span data-stu-id="ebe65-242">Letter</span></span>  |  <span data-ttu-id="ebe65-243">Meaning</span><span class="sxs-lookup"><span data-stu-id="ebe65-243">Meaning</span></span>  |
|----------|----------------------|
|<span data-ttu-id="ebe65-244">C</span><span class="sxs-lookup"><span data-stu-id="ebe65-244">C</span></span>|<span data-ttu-id="ebe65-245">Current</span><span class="sxs-lookup"><span data-stu-id="ebe65-245">Current</span></span>|
|<span data-ttu-id="ebe65-246">D</span><span class="sxs-lookup"><span data-stu-id="ebe65-246">D</span></span>|<span data-ttu-id="ebe65-247">Day\(s\)</span><span class="sxs-lookup"><span data-stu-id="ebe65-247">Day\(s\)</span></span>|
|<span data-ttu-id="ebe65-248">W</span><span class="sxs-lookup"><span data-stu-id="ebe65-248">W</span></span>|<span data-ttu-id="ebe65-249">Week\(s\)</span><span class="sxs-lookup"><span data-stu-id="ebe65-249">Week\(s\)</span></span>|
|<span data-ttu-id="ebe65-250">M</span><span class="sxs-lookup"><span data-stu-id="ebe65-250">M</span></span>|<span data-ttu-id="ebe65-251">Month\(s\)</span><span class="sxs-lookup"><span data-stu-id="ebe65-251">Month\(s\)</span></span>|
|<span data-ttu-id="ebe65-252">Q</span><span class="sxs-lookup"><span data-stu-id="ebe65-252">Q</span></span>|<span data-ttu-id="ebe65-253">Quarter\(s\)</span><span class="sxs-lookup"><span data-stu-id="ebe65-253">Quarter\(s\)</span></span>|
|<span data-ttu-id="ebe65-254">Y</span><span class="sxs-lookup"><span data-stu-id="ebe65-254">Y</span></span>|<span data-ttu-id="ebe65-255">Year\(s\)</span><span class="sxs-lookup"><span data-stu-id="ebe65-255">Year\(s\)</span></span>|

<span data-ttu-id="ebe65-256">You can construct a date formula in three ways.</span><span class="sxs-lookup"><span data-stu-id="ebe65-256">You can construct a date formula in three ways.</span></span>

<span data-ttu-id="ebe65-257">The following example shows how to use C, for current, and a time unit.</span><span class="sxs-lookup"><span data-stu-id="ebe65-257">The following example shows how to use C, for current, and a time unit.</span></span>

|  <span data-ttu-id="ebe65-258">Expression</span><span class="sxs-lookup"><span data-stu-id="ebe65-258">Expression</span></span>  |  <span data-ttu-id="ebe65-259">Meaning</span><span class="sxs-lookup"><span data-stu-id="ebe65-259">Meaning</span></span>  |
|--------------|-----------|
|<span data-ttu-id="ebe65-260">CW</span><span class="sxs-lookup"><span data-stu-id="ebe65-260">CW</span></span>|<span data-ttu-id="ebe65-261">Current week</span><span class="sxs-lookup"><span data-stu-id="ebe65-261">Current week</span></span>|
|<span data-ttu-id="ebe65-262">CM</span><span class="sxs-lookup"><span data-stu-id="ebe65-262">CM</span></span>|<span data-ttu-id="ebe65-263">Current month</span><span class="sxs-lookup"><span data-stu-id="ebe65-263">Current month</span></span>|

<span data-ttu-id="ebe65-264">The following example shows how to use a number and a time unit.</span><span class="sxs-lookup"><span data-stu-id="ebe65-264">The following example shows how to use a number and a time unit.</span></span> <span data-ttu-id="ebe65-265">A number cannot be larger than 9999.</span><span class="sxs-lookup"><span data-stu-id="ebe65-265">A number cannot be larger than 9999.</span></span>

|  <span data-ttu-id="ebe65-266">Expression</span><span class="sxs-lookup"><span data-stu-id="ebe65-266">Expression</span></span>  |  <span data-ttu-id="ebe65-267">Meaning</span><span class="sxs-lookup"><span data-stu-id="ebe65-267">Meaning</span></span>  |
|--------------|-----------|
|<span data-ttu-id="ebe65-268">10D</span><span class="sxs-lookup"><span data-stu-id="ebe65-268">10D</span></span>|<span data-ttu-id="ebe65-269">10 days from today</span><span class="sxs-lookup"><span data-stu-id="ebe65-269">10 days from today</span></span>|
|<span data-ttu-id="ebe65-270">2W</span><span class="sxs-lookup"><span data-stu-id="ebe65-270">2W</span></span>|<span data-ttu-id="ebe65-271">2 weeks from today</span><span class="sxs-lookup"><span data-stu-id="ebe65-271">2 weeks from today</span></span>|

<span data-ttu-id="ebe65-272">The following example shows how to use a time unit and a number.</span><span class="sxs-lookup"><span data-stu-id="ebe65-272">The following example shows how to use a time unit and a number.</span></span>

|  <span data-ttu-id="ebe65-273">Expression</span><span class="sxs-lookup"><span data-stu-id="ebe65-273">Expression</span></span>  |  <span data-ttu-id="ebe65-274">Meaning</span><span class="sxs-lookup"><span data-stu-id="ebe65-274">Meaning</span></span>  |
|--------------|-----------|
|<span data-ttu-id="ebe65-275">D10</span><span class="sxs-lookup"><span data-stu-id="ebe65-275">D10</span></span>|<span data-ttu-id="ebe65-276">The next 10th day of a month</span><span class="sxs-lookup"><span data-stu-id="ebe65-276">The next 10th day of a month</span></span>|
|<span data-ttu-id="ebe65-277">WD4</span><span class="sxs-lookup"><span data-stu-id="ebe65-277">WD4</span></span>|<span data-ttu-id="ebe65-278">The next 4th day of a week \(Thursday\)</span><span class="sxs-lookup"><span data-stu-id="ebe65-278">The next 4th day of a week \(Thursday\)</span></span>|

<span data-ttu-id="ebe65-279">The following example shows how you can combine these three forms as needed.</span><span class="sxs-lookup"><span data-stu-id="ebe65-279">The following example shows how you can combine these three forms as needed.</span></span>

|  <span data-ttu-id="ebe65-280">Expression</span><span class="sxs-lookup"><span data-stu-id="ebe65-280">Expression</span></span>  |  <span data-ttu-id="ebe65-281">Meaning</span><span class="sxs-lookup"><span data-stu-id="ebe65-281">Meaning</span></span>  |
|--------------|-----------|
|<span data-ttu-id="ebe65-282">CM+10D</span><span class="sxs-lookup"><span data-stu-id="ebe65-282">CM+10D</span></span>|<span data-ttu-id="ebe65-283">Current month \+ 10 days</span><span class="sxs-lookup"><span data-stu-id="ebe65-283">Current month \+ 10 days</span></span>|

<span data-ttu-id="ebe65-284">The following example shows how you can use a minus sign to indicate a date in the past.</span><span class="sxs-lookup"><span data-stu-id="ebe65-284">The following example shows how you can use a minus sign to indicate a date in the past.</span></span>

|  <span data-ttu-id="ebe65-285">Expression</span><span class="sxs-lookup"><span data-stu-id="ebe65-285">Expression</span></span>  |  <span data-ttu-id="ebe65-286">Meaning</span><span class="sxs-lookup"><span data-stu-id="ebe65-286">Meaning</span></span>  |
|--------------|-----------|
|<span data-ttu-id="ebe65-287">-1Y</span><span class="sxs-lookup"><span data-stu-id="ebe65-287">-1Y</span></span>|<span data-ttu-id="ebe65-288">1 year ago from today</span><span class="sxs-lookup"><span data-stu-id="ebe65-288">1 year ago from today</span></span>|

> [!IMPORTANT]
>  <span data-ttu-id="ebe65-289">If the location uses a base calendar, then the date formula that you enter in, for example, the **Shipping Time** field is interpreted according to the calendar working days.</span><span class="sxs-lookup"><span data-stu-id="ebe65-289">If the location uses a base calendar, then the date formula that you enter in, for example, the **Shipping Time** field is interpreted according to the calendar working days.</span></span> <span data-ttu-id="ebe65-290">For example, 1W  means seven working days.</span><span class="sxs-lookup"><span data-stu-id="ebe65-290">For example, 1W  means seven working days.</span></span>
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

Note that we have used the US date format MMDDYY here. As [!INCLUDE[prod_short](includes/prod_short.md)] becomes available in other markets, you'll be able to use the formats that you are used to.

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

## <a name="entering-times"></a><span data-ttu-id="ebe65-291">Entering Times</span><span class="sxs-lookup"><span data-stu-id="ebe65-291">Entering Times</span></span>
<span data-ttu-id="ebe65-292">When you enter times, you can insert any non-space separators that you want between the units, but if you use double digits for each unit up to milliseconds, then it is not required.</span><span class="sxs-lookup"><span data-stu-id="ebe65-292">When you enter times, you can insert any non-space separators that you want between the units, but if you use double digits for each unit up to milliseconds, then it is not required.</span></span>

<span data-ttu-id="ebe65-293">You only have to write the largest units that you require; the rest will be set to zero.</span><span class="sxs-lookup"><span data-stu-id="ebe65-293">You only have to write the largest units that you require; the rest will be set to zero.</span></span> <span data-ttu-id="ebe65-294">You can also leave out any AM/PM indicator.</span><span class="sxs-lookup"><span data-stu-id="ebe65-294">You can also leave out any AM/PM indicator.</span></span>

<span data-ttu-id="ebe65-295">The following table lists the various ways in which times can be entered and how they are interpreted.</span><span class="sxs-lookup"><span data-stu-id="ebe65-295">The following table lists the various ways in which times can be entered and how they are interpreted.</span></span> <span data-ttu-id="ebe65-296">It assumes region settings that format times according to: **Hours:Minutes:Seconds.Milliseconds.**</span><span class="sxs-lookup"><span data-stu-id="ebe65-296">It assumes region settings that format times according to: **Hours:Minutes:Seconds.Milliseconds.**</span></span> <span data-ttu-id="ebe65-297">and use the AM and PM indicators of 'AM' and 'PM', respectively.</span><span class="sxs-lookup"><span data-stu-id="ebe65-297">and use the AM and PM indicators of 'AM' and 'PM', respectively.</span></span>

|<span data-ttu-id="ebe65-298">**Entry**</span><span class="sxs-lookup"><span data-stu-id="ebe65-298">**Entry**</span></span>      |<span data-ttu-id="ebe65-299">**Interpretation**</span><span class="sxs-lookup"><span data-stu-id="ebe65-299">**Interpretation**</span></span>      |
|---------------|------------------------|
|<span data-ttu-id="ebe65-300">05:23:17</span><span class="sxs-lookup"><span data-stu-id="ebe65-300">05:23:17</span></span>|<span data-ttu-id="ebe65-301">05:23:17</span><span class="sxs-lookup"><span data-stu-id="ebe65-301">05:23:17</span></span>|
|<span data-ttu-id="ebe65-302">5</span><span class="sxs-lookup"><span data-stu-id="ebe65-302">5</span></span>|<span data-ttu-id="ebe65-303">05:00:00</span><span class="sxs-lookup"><span data-stu-id="ebe65-303">05:00:00</span></span>|
|<span data-ttu-id="ebe65-304">5AM</span><span class="sxs-lookup"><span data-stu-id="ebe65-304">5AM</span></span>|<span data-ttu-id="ebe65-305">05:00:00</span><span class="sxs-lookup"><span data-stu-id="ebe65-305">05:00:00</span></span>|
|<span data-ttu-id="ebe65-306">5P</span><span class="sxs-lookup"><span data-stu-id="ebe65-306">5P</span></span>|<span data-ttu-id="ebe65-307">17:00:00</span><span class="sxs-lookup"><span data-stu-id="ebe65-307">17:00:00</span></span>|
|<span data-ttu-id="ebe65-308">12</span><span class="sxs-lookup"><span data-stu-id="ebe65-308">12</span></span>|<span data-ttu-id="ebe65-309">12:00:00</span><span class="sxs-lookup"><span data-stu-id="ebe65-309">12:00:00</span></span>|
|<span data-ttu-id="ebe65-310">12A</span><span class="sxs-lookup"><span data-stu-id="ebe65-310">12A</span></span>|<span data-ttu-id="ebe65-311">00:00:00</span><span class="sxs-lookup"><span data-stu-id="ebe65-311">00:00:00</span></span>|
|<span data-ttu-id="ebe65-312">12P</span><span class="sxs-lookup"><span data-stu-id="ebe65-312">12P</span></span>|<span data-ttu-id="ebe65-313">12:00:00</span><span class="sxs-lookup"><span data-stu-id="ebe65-313">12:00:00</span></span>|
|<span data-ttu-id="ebe65-314">17</span><span class="sxs-lookup"><span data-stu-id="ebe65-314">17</span></span>|<span data-ttu-id="ebe65-315">17:00:00</span><span class="sxs-lookup"><span data-stu-id="ebe65-315">17:00:00</span></span>|
|<span data-ttu-id="ebe65-316">5:30</span><span class="sxs-lookup"><span data-stu-id="ebe65-316">5:30</span></span>|<span data-ttu-id="ebe65-317">05:30:00</span><span class="sxs-lookup"><span data-stu-id="ebe65-317">05:30:00</span></span>|
|<span data-ttu-id="ebe65-318">0530</span><span class="sxs-lookup"><span data-stu-id="ebe65-318">0530</span></span>|<span data-ttu-id="ebe65-319">05:30:00</span><span class="sxs-lookup"><span data-stu-id="ebe65-319">05:30:00</span></span>|
|<span data-ttu-id="ebe65-320">5:30:5</span><span class="sxs-lookup"><span data-stu-id="ebe65-320">5:30:5</span></span>|<span data-ttu-id="ebe65-321">05:30:05</span><span class="sxs-lookup"><span data-stu-id="ebe65-321">05:30:05</span></span>|
|<span data-ttu-id="ebe65-322">053005</span><span class="sxs-lookup"><span data-stu-id="ebe65-322">053005</span></span>|<span data-ttu-id="ebe65-323">05:30:05</span><span class="sxs-lookup"><span data-stu-id="ebe65-323">05:30:05</span></span>|
|<span data-ttu-id="ebe65-324">5:30:5,50</span><span class="sxs-lookup"><span data-stu-id="ebe65-324">5:30:5,50</span></span>|<span data-ttu-id="ebe65-325">05:30:05.5</span><span class="sxs-lookup"><span data-stu-id="ebe65-325">05:30:05.5</span></span>|
|<span data-ttu-id="ebe65-326">053005050</span><span class="sxs-lookup"><span data-stu-id="ebe65-326">053005050</span></span>|<span data-ttu-id="ebe65-327">05:30:05.05</span><span class="sxs-lookup"><span data-stu-id="ebe65-327">05:30:05.05</span></span>|

<span data-ttu-id="ebe65-328">You should be aware that milliseconds are interpreted as decimal notation.</span><span class="sxs-lookup"><span data-stu-id="ebe65-328">You should be aware that milliseconds are interpreted as decimal notation.</span></span> <span data-ttu-id="ebe65-329">So, for example, 3, 30, and 300 all mean 300 milliseconds, while 03 means 30 and 003 means 3 milliseconds.</span><span class="sxs-lookup"><span data-stu-id="ebe65-329">So, for example, 3, 30, and 300 all mean 300 milliseconds, while 03 means 30 and 003 means 3 milliseconds.</span></span>

<span data-ttu-id="ebe65-330">You cannot use 24:00 to mean midnight, or use any value greater than 24:00.</span><span class="sxs-lookup"><span data-stu-id="ebe65-330">You cannot use 24:00 to mean midnight, or use any value greater than 24:00.</span></span>

<span data-ttu-id="ebe65-331">The word for 'time' in the language used by [!INCLUDE[prod_short](includes/prod_long.md)] will be evaluated to the current time on your computer or mobile device.</span><span class="sxs-lookup"><span data-stu-id="ebe65-331">The word for 'time' in the language used by [!INCLUDE[prod_short](includes/prod_long.md)] will be evaluated to the current time on your computer or mobile device.</span></span> <span data-ttu-id="ebe65-332">You can enter any part of the word, starting from the beginning, such as t or TIM.</span><span class="sxs-lookup"><span data-stu-id="ebe65-332">You can enter any part of the word, starting from the beginning, such as t or TIM.</span></span>

## <a name="entering-combined-dates-and-times"></a><span data-ttu-id="ebe65-333">Entering combined Dates and Times</span><span class="sxs-lookup"><span data-stu-id="ebe65-333">Entering combined Dates and Times</span></span>
<span data-ttu-id="ebe65-334">When you enter datetimes, which are a date and time combined into one field, you must enter a space between the date and the time.</span><span class="sxs-lookup"><span data-stu-id="ebe65-334">When you enter datetimes, which are a date and time combined into one field, you must enter a space between the date and the time.</span></span> <span data-ttu-id="ebe65-335">The date part can only contain spaces in the form of the official date separator of your region settings.</span><span class="sxs-lookup"><span data-stu-id="ebe65-335">The date part can only contain spaces in the form of the official date separator of your region settings.</span></span> <span data-ttu-id="ebe65-336">The time can contain spaces around the AM/PM indicator.</span><span class="sxs-lookup"><span data-stu-id="ebe65-336">The time can contain spaces around the AM/PM indicator.</span></span>

<span data-ttu-id="ebe65-337">It is also possible to enter only a date in a datetime field, but it is not possible to enter only a time.</span><span class="sxs-lookup"><span data-stu-id="ebe65-337">It is also possible to enter only a date in a datetime field, but it is not possible to enter only a time.</span></span>

<span data-ttu-id="ebe65-338">The following table lists some examples of date/time combinations.</span><span class="sxs-lookup"><span data-stu-id="ebe65-338">The following table lists some examples of date/time combinations.</span></span> <span data-ttu-id="ebe65-339">The region settings in the examples displays dates in the day\-month\-year format, using AM/PM designators, English language, and Sunday as the start of the week.</span><span class="sxs-lookup"><span data-stu-id="ebe65-339">The region settings in the examples displays dates in the day\-month\-year format, using AM/PM designators, English language, and Sunday as the start of the week.</span></span>

|<span data-ttu-id="ebe65-340">**Entry**</span><span class="sxs-lookup"><span data-stu-id="ebe65-340">**Entry**</span></span>      |<span data-ttu-id="ebe65-341">**Interpretation**</span><span class="sxs-lookup"><span data-stu-id="ebe65-341">**Interpretation**</span></span>      |
|---------------|------------------------|
|<span data-ttu-id="ebe65-342">08-01-2016 05:48:12 PM</span><span class="sxs-lookup"><span data-stu-id="ebe65-342">08-01-2016 05:48:12 PM</span></span>|<span data-ttu-id="ebe65-343">08\-01\-2016 05:48:12 PM</span><span class="sxs-lookup"><span data-stu-id="ebe65-343">08\-01\-2016 05:48:12 PM</span></span>|
|<span data-ttu-id="ebe65-344">131202 132455</span><span class="sxs-lookup"><span data-stu-id="ebe65-344">131202 132455</span></span>|<span data-ttu-id="ebe65-345">13\-12\-2002 13:24:55</span><span class="sxs-lookup"><span data-stu-id="ebe65-345">13\-12\-2002 13:24:55</span></span>|
|<span data-ttu-id="ebe65-346">1-12-02 10</span><span class="sxs-lookup"><span data-stu-id="ebe65-346">1-12-02 10</span></span>|<span data-ttu-id="ebe65-347">01\-12\-2002 10:00:00</span><span class="sxs-lookup"><span data-stu-id="ebe65-347">01\-12\-2002 10:00:00</span></span>|
|<span data-ttu-id="ebe65-348">1.12.02 5</span><span class="sxs-lookup"><span data-stu-id="ebe65-348">1.12.02 5</span></span>|<span data-ttu-id="ebe65-349">01\-12\-2002 05:00:00</span><span class="sxs-lookup"><span data-stu-id="ebe65-349">01\-12\-2002 05:00:00</span></span>|
|<span data-ttu-id="ebe65-350">1.12.02</span><span class="sxs-lookup"><span data-stu-id="ebe65-350">1.12.02</span></span>|<span data-ttu-id="ebe65-351">01\-12\-2002 00:00:00</span><span class="sxs-lookup"><span data-stu-id="ebe65-351">01\-12\-2002 00:00:00</span></span>|
|<span data-ttu-id="ebe65-352">11 12</span><span class="sxs-lookup"><span data-stu-id="ebe65-352">11 12</span></span>|<span data-ttu-id="ebe65-353">11\-work date month\-work date year 12:00:00</span><span class="sxs-lookup"><span data-stu-id="ebe65-353">11\-work date month\-work date year 12:00:00</span></span>|
|<span data-ttu-id="ebe65-354">1112 12</span><span class="sxs-lookup"><span data-stu-id="ebe65-354">1112 12</span></span>|<span data-ttu-id="ebe65-355">11\-12\-work date year 12:00:00</span><span class="sxs-lookup"><span data-stu-id="ebe65-355">11\-12\-work date year 12:00:00</span></span>|
|<span data-ttu-id="ebe65-356">t or today</span><span class="sxs-lookup"><span data-stu-id="ebe65-356">t or today</span></span>|<span data-ttu-id="ebe65-357">today's date 00:00:00</span><span class="sxs-lookup"><span data-stu-id="ebe65-357">today's date 00:00:00</span></span>|
|<span data-ttu-id="ebe65-358">t 10:30</span><span class="sxs-lookup"><span data-stu-id="ebe65-358">t 10:30</span></span>|<span data-ttu-id="ebe65-359">today's date 10:30:00</span><span class="sxs-lookup"><span data-stu-id="ebe65-359">today's date 10:30:00</span></span>|
|<span data-ttu-id="ebe65-360">t 3:3:3</span><span class="sxs-lookup"><span data-stu-id="ebe65-360">t 3:3:3</span></span>|<span data-ttu-id="ebe65-361">today's date 03:03:03</span><span class="sxs-lookup"><span data-stu-id="ebe65-361">today's date 03:03:03</span></span>|
|<span data-ttu-id="ebe65-362">w or workdate</span><span class="sxs-lookup"><span data-stu-id="ebe65-362">w or workdate</span></span>|<span data-ttu-id="ebe65-363">the working date 00:00:00</span><span class="sxs-lookup"><span data-stu-id="ebe65-363">the working date 00:00:00</span></span>|
|<span data-ttu-id="ebe65-364">m or Monday</span><span class="sxs-lookup"><span data-stu-id="ebe65-364">m or Monday</span></span>|<span data-ttu-id="ebe65-365">Monday of the work date week 00:00:00</span><span class="sxs-lookup"><span data-stu-id="ebe65-365">Monday of the work date week 00:00:00</span></span>|
|<span data-ttu-id="ebe65-366">tu or Tuesday</span><span class="sxs-lookup"><span data-stu-id="ebe65-366">tu or Tuesday</span></span>|<span data-ttu-id="ebe65-367">Tuesday of the work date week 00:00:00</span><span class="sxs-lookup"><span data-stu-id="ebe65-367">Tuesday of the work date week 00:00:00</span></span>|
|<span data-ttu-id="ebe65-368">sa or Saturday</span><span class="sxs-lookup"><span data-stu-id="ebe65-368">sa or Saturday</span></span>|<span data-ttu-id="ebe65-369">Saturday of the work date week 00:00:00</span><span class="sxs-lookup"><span data-stu-id="ebe65-369">Saturday of the work date week 00:00:00</span></span>|
|<span data-ttu-id="ebe65-370">s or Sunday</span><span class="sxs-lookup"><span data-stu-id="ebe65-370">s or Sunday</span></span>|<span data-ttu-id="ebe65-371">Sunday of the work date week 00:00:00</span><span class="sxs-lookup"><span data-stu-id="ebe65-371">Sunday of the work date week 00:00:00</span></span>|
|<span data-ttu-id="ebe65-372">tu 10:30</span><span class="sxs-lookup"><span data-stu-id="ebe65-372">tu 10:30</span></span>|<span data-ttu-id="ebe65-373">Tuesday of the work date week 10:30:00</span><span class="sxs-lookup"><span data-stu-id="ebe65-373">Tuesday of the work date week 10:30:00</span></span>|
|<span data-ttu-id="ebe65-374">tu 3:3:3</span><span class="sxs-lookup"><span data-stu-id="ebe65-374">tu 3:3:3</span></span>|<span data-ttu-id="ebe65-375">Tuesday of the work date week 03:03:03</span><span class="sxs-lookup"><span data-stu-id="ebe65-375">Tuesday of the work date week 03:03:03</span></span>|
|<span data-ttu-id="ebe65-376">t23 t</span><span class="sxs-lookup"><span data-stu-id="ebe65-376">t23 t</span></span>|<span data-ttu-id="ebe65-377">Tuesday of week 23 of the work date year, current time of day</span><span class="sxs-lookup"><span data-stu-id="ebe65-377">Tuesday of week 23 of the work date year, current time of day</span></span>|
|<span data-ttu-id="ebe65-378">t23</span><span class="sxs-lookup"><span data-stu-id="ebe65-378">t23</span></span>|<span data-ttu-id="ebe65-379">Tuesday of week 23 of the work date year</span><span class="sxs-lookup"><span data-stu-id="ebe65-379">Tuesday of week 23 of the work date year</span></span>|
|<span data-ttu-id="ebe65-380">t 23</span><span class="sxs-lookup"><span data-stu-id="ebe65-380">t 23</span></span>|<span data-ttu-id="ebe65-381">Today 23:00:00</span><span class="sxs-lookup"><span data-stu-id="ebe65-381">Today 23:00:00</span></span>|
|<span data-ttu-id="ebe65-382">t-1</span><span class="sxs-lookup"><span data-stu-id="ebe65-382">t-1</span></span>|<span data-ttu-id="ebe65-383">Tuesday of week 1 of the work date year</span><span class="sxs-lookup"><span data-stu-id="ebe65-383">Tuesday of week 1 of the work date year</span></span>|

## <a name="entering-duration"></a><span data-ttu-id="ebe65-384">Entering Duration</span><span class="sxs-lookup"><span data-stu-id="ebe65-384">Entering Duration</span></span>
<span data-ttu-id="ebe65-385">Some fields in the application represent a duration, or amount of elapsed time, instead of a specific date or time.</span><span class="sxs-lookup"><span data-stu-id="ebe65-385">Some fields in the application represent a duration, or amount of elapsed time, instead of a specific date or time.</span></span> <span data-ttu-id="ebe65-386">You enter a duration as a number followed by its unit of measure.</span><span class="sxs-lookup"><span data-stu-id="ebe65-386">You enter a duration as a number followed by its unit of measure.</span></span>

<span data-ttu-id="ebe65-387">Here are some examples.</span><span class="sxs-lookup"><span data-stu-id="ebe65-387">Here are some examples.</span></span>

|<span data-ttu-id="ebe65-388">**Duration**</span><span class="sxs-lookup"><span data-stu-id="ebe65-388">**Duration**</span></span>|<span data-ttu-id="ebe65-389">**Unit of measure**</span><span class="sxs-lookup"><span data-stu-id="ebe65-389">**Unit of measure**</span></span>|
|------------|-------------------|
|<span data-ttu-id="ebe65-390">2h</span><span class="sxs-lookup"><span data-stu-id="ebe65-390">2h</span></span>|<span data-ttu-id="ebe65-391">2 hrs</span><span class="sxs-lookup"><span data-stu-id="ebe65-391">2 hrs</span></span>|
|<span data-ttu-id="ebe65-392">6h 30 m</span><span class="sxs-lookup"><span data-stu-id="ebe65-392">6h 30 m</span></span>|<span data-ttu-id="ebe65-393">6 hrs 30 mins</span><span class="sxs-lookup"><span data-stu-id="ebe65-393">6 hrs 30 mins</span></span>|
|<span data-ttu-id="ebe65-394">6.5h</span><span class="sxs-lookup"><span data-stu-id="ebe65-394">6.5h</span></span>|<span data-ttu-id="ebe65-395">6 hrs 30 mins</span><span class="sxs-lookup"><span data-stu-id="ebe65-395">6 hrs 30 mins</span></span>|
|<span data-ttu-id="ebe65-396">90m</span><span class="sxs-lookup"><span data-stu-id="ebe65-396">90m</span></span>|<span data-ttu-id="ebe65-397">1 hr 30 mins</span><span class="sxs-lookup"><span data-stu-id="ebe65-397">1 hr 30 mins</span></span>|
|<span data-ttu-id="ebe65-398">2d 6h 30m</span><span class="sxs-lookup"><span data-stu-id="ebe65-398">2d 6h 30m</span></span>|<span data-ttu-id="ebe65-399">2 days 6 hrs 30 mins</span><span class="sxs-lookup"><span data-stu-id="ebe65-399">2 days 6 hrs 30 mins</span></span>|
|<span data-ttu-id="ebe65-400">2d 6h 30m 56s 600ms</span><span class="sxs-lookup"><span data-stu-id="ebe65-400">2d 6h 30m 56s 600ms</span></span>|<span data-ttu-id="ebe65-401">2 days 6 hrs 30 mins 56 secs 600 msecs</span><span class="sxs-lookup"><span data-stu-id="ebe65-401">2 days 6 hrs 30 mins 56 secs 600 msecs</span></span>|

<span data-ttu-id="ebe65-402">You can also enter a number, which will be automatically converted to a duration.</span><span class="sxs-lookup"><span data-stu-id="ebe65-402">You can also enter a number, which will be automatically converted to a duration.</span></span> <span data-ttu-id="ebe65-403">The number you enter is converted according to the default unit of measure that has been specified for the duration field.</span><span class="sxs-lookup"><span data-stu-id="ebe65-403">The number you enter is converted according to the default unit of measure that has been specified for the duration field.</span></span>

<span data-ttu-id="ebe65-404">To see what unit of measure is being used in a duration field, enter a number and see which unit of measure it is converted to.</span><span class="sxs-lookup"><span data-stu-id="ebe65-404">To see what unit of measure is being used in a duration field, enter a number and see which unit of measure it is converted to.</span></span>

<span data-ttu-id="ebe65-405">For example, if the unit of measure is hours, the number 5 is converted to 5 hrs.</span><span class="sxs-lookup"><span data-stu-id="ebe65-405">For example, if the unit of measure is hours, the number 5 is converted to 5 hrs.</span></span>

## <a name="see-also"></a><span data-ttu-id="ebe65-406">See Also</span><span class="sxs-lookup"><span data-stu-id="ebe65-406">See Also</span></span>
<span data-ttu-id="ebe65-407">[Working with [!INCLUDE[prod_short](includes/prod_long.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="ebe65-407">[Working with [!INCLUDE[prod_short](includes/prod_long.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="ebe65-408">Date Calculation for Purchases</span><span class="sxs-lookup"><span data-stu-id="ebe65-408">Date Calculation for Purchases</span></span>](purchasing-date-calculation-for-purchases.md)  
[<span data-ttu-id="ebe65-409">Entering Criteria in Filters</span><span class="sxs-lookup"><span data-stu-id="ebe65-409">Entering Criteria in Filters </span></span>](ui-enter-criteria-filters.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]