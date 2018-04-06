---
title: How to Enter Data in Fields| Microsoft Docs
description: There are many general functions that help you enter data  in a quick and easy way. The general functions for entering data are described in this topic.
author: jswymer
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/19/2017
ms.author: jswymer
ms.translationtype: HT
ms.sourcegitcommit: 8b2e20e694279a8c06188e0e429ef3b4fb43aea2
ms.openlocfilehash: 5f95efb5cad24db9848752035172bc7bb76db716
ms.contentlocale: en-nz
ms.lasthandoff: 03/22/2018

---
# <a name="entering-data"></a><span data-ttu-id="6ef94-104">Entering Data</span><span class="sxs-lookup"><span data-stu-id="6ef94-104">Entering Data</span></span>
<span data-ttu-id="6ef94-105">There are many general functions that help you enter data  in a quick and easy way.</span><span class="sxs-lookup"><span data-stu-id="6ef94-105">There are many general functions that help you enter data  in a quick and easy way.</span></span> <span data-ttu-id="6ef94-106">The general functions for entering data are described in this article.</span><span class="sxs-lookup"><span data-stu-id="6ef94-106">The general functions for entering data are described in this article.</span></span>  

<span data-ttu-id="6ef94-107">The examples in this article use the demonstration data.</span><span class="sxs-lookup"><span data-stu-id="6ef94-107">The examples in this article use the demonstration data.</span></span>

## <a name="mandatory-fields"></a><span data-ttu-id="6ef94-108">Mandatory Fields</span><span class="sxs-lookup"><span data-stu-id="6ef94-108">Mandatory Fields</span></span>
<span data-ttu-id="6ef94-109">When you enter data on pages, certain fields are marked with a red asterisk.</span><span class="sxs-lookup"><span data-stu-id="6ef94-109">When you enter data on pages, certain fields are marked with a red asterisk.</span></span> <span data-ttu-id="6ef94-110">The red asterisk means that the field must be filled to complete a certain process that uses the field, such as posting a transaction that uses the value in the field.</span><span class="sxs-lookup"><span data-stu-id="6ef94-110">The red asterisk means that the field must be filled to complete a certain process that uses the field, such as posting a transaction that uses the value in the field.</span></span>  

<span data-ttu-id="6ef94-111">Even though the field contains a red asterisk, you are not forced to fill the field before you continue to other fields or close the page.</span><span class="sxs-lookup"><span data-stu-id="6ef94-111">Even though the field contains a red asterisk, you are not forced to fill the field before you continue to other fields or close the page.</span></span> <span data-ttu-id="6ef94-112">The red asterisk only serves as a reminder that you will be blocked from completing a certain process.</span><span class="sxs-lookup"><span data-stu-id="6ef94-112">The red asterisk only serves as a reminder that you will be blocked from completing a certain process.</span></span>  


## <a name="finding-data-as-you-type"></a><span data-ttu-id="6ef94-113">Finding Data As You Type</span><span class="sxs-lookup"><span data-stu-id="6ef94-113">Finding Data As You Type</span></span>  
 <span data-ttu-id="6ef94-114">When you start to type characters in a field, a drop-down list is displayed and shows possible field values.</span><span class="sxs-lookup"><span data-stu-id="6ef94-114">When you start to type characters in a field, a drop-down list is displayed and shows possible field values.</span></span> <span data-ttu-id="6ef94-115">The list changes as you type more characters, and you can select the correct value when it is displayed.</span><span class="sxs-lookup"><span data-stu-id="6ef94-115">The list changes as you type more characters, and you can select the correct value when it is displayed.</span></span>  

 <span data-ttu-id="6ef94-116">Many fields have a down arrow button that you can choose.</span><span class="sxs-lookup"><span data-stu-id="6ef94-116">Many fields have a down arrow button that you can choose.</span></span> <span data-ttu-id="6ef94-117">You choose the arrow to get a list of data that is available to enter in the field.</span><span class="sxs-lookup"><span data-stu-id="6ef94-117">You choose the arrow to get a list of data that is available to enter in the field.</span></span> <span data-ttu-id="6ef94-118">The button has two functions depending on the type of field:</span><span class="sxs-lookup"><span data-stu-id="6ef94-118">The button has two functions depending on the type of field:</span></span>  

-   <span data-ttu-id="6ef94-119">Lookup - Displays information from another table that you can enter in the field.</span><span class="sxs-lookup"><span data-stu-id="6ef94-119">Lookup - Displays information from another table that you can enter in the field.</span></span> <span data-ttu-id="6ef94-120">You can select one piece of data at a time.</span><span class="sxs-lookup"><span data-stu-id="6ef94-120">You can select one piece of data at a time.</span></span>  

-   <span data-ttu-id="6ef94-121">Drop-down - Displays the set of options that exist for the field.</span><span class="sxs-lookup"><span data-stu-id="6ef94-121">Drop-down - Displays the set of options that exist for the field.</span></span> <span data-ttu-id="6ef94-122">You can select only one of the options.</span><span class="sxs-lookup"><span data-stu-id="6ef94-122">You can select only one of the options.</span></span>  

<!--Onprem ## Copy Fields or Lines  
 Depending on the type of writable document, you can copy individual line fields or whole lines to other lines in the document. Read-only data, such as posted entries, cannot be copied.  

 Several database dependencies are used to determine if fields or lines can be copied. One way to determine these dependencies is to view the shortcut menu. The content of the shortcut menu indicates which copy functions are supported by displaying either of these functions:  

-   Copy Cell  

-   Copy Rows  

-   Paste Rows  

 For example, database records, such as lines on a sales order, and master data, such as cards in the **Items** window, cannot be duplicated. For this kind of data, the shortcut menu typically has the **Copy Cell** or **Copy Rows**  functions. If the **Paste** function is not available this indicates that you can only paste the data into external documents. Single fields on a sales line, however, can be copied to the same column in other sales lines.  

 Journal lines are very flexible and can be copied freely in the same journal, indicated by the presence of **Paste** on the shortcut menu.  

> [!NOTE]  
>   If you copy a journal line or document line, the fields that are not in your view are not copied to the new line.

#### To copy previous field  

-   To enter the value of the field immediately above the active field, select **Copy Previous** from the shortcut menu.-->

## <a name="entering-quantities-by-calculation"></a><span data-ttu-id="6ef94-123">Entering Quantities by Calculation</span><span class="sxs-lookup"><span data-stu-id="6ef94-123">Entering Quantities by Calculation</span></span>  
 <span data-ttu-id="6ef94-124">When entering numbers into quantity fields, such as the **Quantity** field on an item journal line, you can enter the formula instead of the sum quantity.</span><span class="sxs-lookup"><span data-stu-id="6ef94-124">When entering numbers into quantity fields, such as the **Quantity** field on an item journal line, you can enter the formula instead of the sum quantity.</span></span>  

## <a name="examples"></a><span data-ttu-id="6ef94-125">Examples</span><span class="sxs-lookup"><span data-stu-id="6ef94-125">Examples</span></span>  

-   <span data-ttu-id="6ef94-126">If you enter 19+19, the field is calculated to 38.</span><span class="sxs-lookup"><span data-stu-id="6ef94-126">If you enter 19+19, the field is calculated to 38.</span></span>  

-   <span data-ttu-id="6ef94-127">If you enter 41-9, the field is calculated to 32.</span><span class="sxs-lookup"><span data-stu-id="6ef94-127">If you enter 41-9, the field is calculated to 32.</span></span>  

-   <span data-ttu-id="6ef94-128">If you enter 12\*4, the field is calculated to 48.</span><span class="sxs-lookup"><span data-stu-id="6ef94-128">If you enter 12\*4, the field is calculated to 48.</span></span>  

-   <span data-ttu-id="6ef94-129">If you enter 12/4, the field is calculated to 3.</span><span class="sxs-lookup"><span data-stu-id="6ef94-129">If you enter 12/4, the field is calculated to 3.</span></span>  

# <a name="entering-negative-numbers"></a><span data-ttu-id="6ef94-130">Entering Negative Numbers</span><span class="sxs-lookup"><span data-stu-id="6ef94-130">Entering Negative Numbers</span></span>
<span data-ttu-id="6ef94-131">You can enter negative numbers in two ways.</span><span class="sxs-lookup"><span data-stu-id="6ef94-131">You can enter negative numbers in two ways.</span></span> <span data-ttu-id="6ef94-132">The number -20.5 can be entered as:</span><span class="sxs-lookup"><span data-stu-id="6ef94-132">The number -20.5 can be entered as:</span></span>  

-   <span data-ttu-id="6ef94-133">-20.5</span><span class="sxs-lookup"><span data-stu-id="6ef94-133">-20.5</span></span>  

    <span data-ttu-id="6ef94-134">or</span><span class="sxs-lookup"><span data-stu-id="6ef94-134">or</span></span>
-   <span data-ttu-id="6ef94-135">20.5-</span><span class="sxs-lookup"><span data-stu-id="6ef94-135">20.5-</span></span>  

 <span data-ttu-id="6ef94-136">In both cases, the amount will be recorded in as -20.5.</span><span class="sxs-lookup"><span data-stu-id="6ef94-136">In both cases, the amount will be recorded in as -20.5.</span></span>  

 <span data-ttu-id="6ef94-137">If the last character of the expression is a **+** or a **-**, the entire expression will be recorded with that sign.</span><span class="sxs-lookup"><span data-stu-id="6ef94-137">If the last character of the expression is a **+** or a **-**, the entire expression will be recorded with that sign.</span></span> <span data-ttu-id="6ef94-138">An example, **10-20+** will result in 10 and not -10.</span><span class="sxs-lookup"><span data-stu-id="6ef94-138">An example, **10-20+** will result in 10 and not -10.</span></span>  

## <a name="entering-dates-and-times"></a><span data-ttu-id="6ef94-139">Entering Dates and Times</span><span class="sxs-lookup"><span data-stu-id="6ef94-139">Entering Dates and Times</span></span>
<span data-ttu-id="6ef94-140">You can enter dates and times in all the fields that are specifically assigned to dates (date fields).</span><span class="sxs-lookup"><span data-stu-id="6ef94-140">You can enter dates and times in all the fields that are specifically assigned to dates (date fields).</span></span> <span data-ttu-id="6ef94-141">You can enter dates with or without separators.</span><span class="sxs-lookup"><span data-stu-id="6ef94-141">You can enter dates with or without separators.</span></span>

> [!NOTE]  
> <span data-ttu-id="6ef94-142">How you enter dates and times depends on your **Region** settings.</span><span class="sxs-lookup"><span data-stu-id="6ef94-142">How you enter dates and times depends on your **Region** settings.</span></span> <span data-ttu-id="6ef94-143">For more information, see [Changing Basic Settings](ui-change-basic-settings.md).</span><span class="sxs-lookup"><span data-stu-id="6ef94-143">For more information, see [Changing Basic Settings](ui-change-basic-settings.md).</span></span>  

### <a name="entering-dates"></a><span data-ttu-id="6ef94-144">Entering Dates</span><span class="sxs-lookup"><span data-stu-id="6ef94-144">Entering Dates</span></span>  
 <span data-ttu-id="6ef94-145">In a date field you can enter two, four, six, or eight digits:</span><span class="sxs-lookup"><span data-stu-id="6ef94-145">In a date field you can enter two, four, six, or eight digits:</span></span>  

-   <span data-ttu-id="6ef94-146">If you enter only two digits, this is interpreted as the day, and it will add the month and the year of the work date.</span><span class="sxs-lookup"><span data-stu-id="6ef94-146">If you enter only two digits, this is interpreted as the day, and it will add the month and the year of the work date.</span></span>  

-   <span data-ttu-id="6ef94-147">If you enter four digits, this is interpreted as the day and the month, and it will add the year of the work date.</span><span class="sxs-lookup"><span data-stu-id="6ef94-147">If you enter four digits, this is interpreted as the day and the month, and it will add the year of the work date.</span></span>  

-   <span data-ttu-id="6ef94-148">If the date you want to enter is in the range 01/01/1930 through 12/31/2029, you can enter the year with two digits; otherwise, enter the year with four digits.</span><span class="sxs-lookup"><span data-stu-id="6ef94-148">If the date you want to enter is in the range 01/01/1930 through 12/31/2029, you can enter the year with two digits; otherwise, enter the year with four digits.</span></span>  

 <span data-ttu-id="6ef94-149">You can also enter a date as a weekday followed by a week number and, optionally, a year (for example, Mon25 or mon25 means Monday in week 25).</span><span class="sxs-lookup"><span data-stu-id="6ef94-149">You can also enter a date as a weekday followed by a week number and, optionally, a year (for example, Mon25 or mon25 means Monday in week 25).</span></span>  

 <span data-ttu-id="6ef94-150">Instead of entering a specific date, you can enter one of two codes.</span><span class="sxs-lookup"><span data-stu-id="6ef94-150">Instead of entering a specific date, you can enter one of two codes.</span></span>  

|<span data-ttu-id="6ef94-151">Code</span><span class="sxs-lookup"><span data-stu-id="6ef94-151">Code</span></span>|<span data-ttu-id="6ef94-152">Result</span><span class="sxs-lookup"><span data-stu-id="6ef94-152">Result</span></span>|  
|--------------|----------------|  
|<span data-ttu-id="6ef94-153">t</span><span class="sxs-lookup"><span data-stu-id="6ef94-153">t</span></span>|<span data-ttu-id="6ef94-154">This is today's date (the system date for the computer).</span><span class="sxs-lookup"><span data-stu-id="6ef94-154">This is today's date (the system date for the computer).</span></span>|  
|<span data-ttu-id="6ef94-155">w</span><span class="sxs-lookup"><span data-stu-id="6ef94-155">w</span></span>|<span data-ttu-id="6ef94-156">This is the work date that is setup in the application.</span><span class="sxs-lookup"><span data-stu-id="6ef94-156">This is the work date that is setup in the application.</span></span> <span data-ttu-id="6ef94-157">To change the work date, see [Changing Basic Settings](ui-change-basic-settings.md).</span><span class="sxs-lookup"><span data-stu-id="6ef94-157">To change the work date, see [Changing Basic Settings](ui-change-basic-settings.md).</span></span> <span data-ttu-id="6ef94-158">You may want to use a work date if you have many transactions with a date other than today's date.</span><span class="sxs-lookup"><span data-stu-id="6ef94-158">You may want to use a work date if you have many transactions with a date other than today's date.</span></span>|  

<!--Onprem ## Closing Date  
 When you close a fiscal year, you can use closing dates to indicate that an entry is a closing entry. A closing date technically is between two dates, for example between Dec 31 and Jan 1.  

 To specify that a date is a closing date, put C just before the date: C123101. -->

## <a name="entering-times"></a><span data-ttu-id="6ef94-159">Entering Times</span><span class="sxs-lookup"><span data-stu-id="6ef94-159">Entering Times</span></span>  
 <span data-ttu-id="6ef94-160">When you enter times, you can insert any separator sign that you want between the units, but it is not required.</span><span class="sxs-lookup"><span data-stu-id="6ef94-160">When you enter times, you can insert any separator sign that you want between the units, but it is not required.</span></span> <span data-ttu-id="6ef94-161">You do not have to write minutes, seconds, or AM/PM.</span><span class="sxs-lookup"><span data-stu-id="6ef94-161">You do not have to write minutes, seconds, or AM/PM.</span></span>  

 <span data-ttu-id="6ef94-162">The following table lists the various ways in which times can be entered and how they are interpreted.</span><span class="sxs-lookup"><span data-stu-id="6ef94-162">The following table lists the various ways in which times can be entered and how they are interpreted.</span></span>  

|<span data-ttu-id="6ef94-163">Entry</span><span class="sxs-lookup"><span data-stu-id="6ef94-163">Entry</span></span>|<span data-ttu-id="6ef94-164">Interpretation</span><span class="sxs-lookup"><span data-stu-id="6ef94-164">Interpretation</span></span>|  
|---------------|------------------------|  
|<span data-ttu-id="6ef94-165">5</span><span class="sxs-lookup"><span data-stu-id="6ef94-165">5</span></span>|<span data-ttu-id="6ef94-166">05:00:00</span><span class="sxs-lookup"><span data-stu-id="6ef94-166">05:00:00</span></span>|  
|<span data-ttu-id="6ef94-167">5:30</span><span class="sxs-lookup"><span data-stu-id="6ef94-167">5:30</span></span>|<span data-ttu-id="6ef94-168">05:30:00</span><span class="sxs-lookup"><span data-stu-id="6ef94-168">05:30:00</span></span>|  
|<span data-ttu-id="6ef94-169">0530</span><span class="sxs-lookup"><span data-stu-id="6ef94-169">0530</span></span>|<span data-ttu-id="6ef94-170">05:30:00</span><span class="sxs-lookup"><span data-stu-id="6ef94-170">05:30:00</span></span>|  
|<span data-ttu-id="6ef94-171">5:30:5</span><span class="sxs-lookup"><span data-stu-id="6ef94-171">5:30:5</span></span>|<span data-ttu-id="6ef94-172">05:30:05</span><span class="sxs-lookup"><span data-stu-id="6ef94-172">05:30:05</span></span>|  
|<span data-ttu-id="6ef94-173">053005</span><span class="sxs-lookup"><span data-stu-id="6ef94-173">053005</span></span>|<span data-ttu-id="6ef94-174">05:30:05</span><span class="sxs-lookup"><span data-stu-id="6ef94-174">05:30:05</span></span>|  
|<span data-ttu-id="6ef94-175">5:30:5,50</span><span class="sxs-lookup"><span data-stu-id="6ef94-175">5:30:5,50</span></span>|<span data-ttu-id="6ef94-176">05:30:05.5</span><span class="sxs-lookup"><span data-stu-id="6ef94-176">05:30:05.5</span></span>|  
|<span data-ttu-id="6ef94-177">053005050</span><span class="sxs-lookup"><span data-stu-id="6ef94-177">053005050</span></span>|<span data-ttu-id="6ef94-178">05:30:05.05</span><span class="sxs-lookup"><span data-stu-id="6ef94-178">05:30:05.05</span></span>|  

 <span data-ttu-id="6ef94-179">You must enter two digits for each unit of time if you do not enter a separator.</span><span class="sxs-lookup"><span data-stu-id="6ef94-179">You must enter two digits for each unit of time if you do not enter a separator.</span></span>  

## <a name="entering-datetimes"></a><span data-ttu-id="6ef94-180">Entering Datetimes</span><span class="sxs-lookup"><span data-stu-id="6ef94-180">Entering Datetimes</span></span>  
 <span data-ttu-id="6ef94-181">When you enter datetimes you must enter a space between the date and the time.</span><span class="sxs-lookup"><span data-stu-id="6ef94-181">When you enter datetimes you must enter a space between the date and the time.</span></span>  

 <span data-ttu-id="6ef94-182">The following table lists the various ways in which you can enter datetimes and how they are interpreted.</span><span class="sxs-lookup"><span data-stu-id="6ef94-182">The following table lists the various ways in which you can enter datetimes and how they are interpreted.</span></span>  

|<span data-ttu-id="6ef94-183">Entry</span><span class="sxs-lookup"><span data-stu-id="6ef94-183">Entry</span></span>|<span data-ttu-id="6ef94-184">Interpretation</span><span class="sxs-lookup"><span data-stu-id="6ef94-184">Interpretation</span></span>|  
|---------------|------------------------|  
|<span data-ttu-id="6ef94-185">131202 132455</span><span class="sxs-lookup"><span data-stu-id="6ef94-185">131202 132455</span></span>|<span data-ttu-id="6ef94-186">13-12-02 13:24:55</span><span class="sxs-lookup"><span data-stu-id="6ef94-186">13-12-02 13:24:55</span></span>|  
|<span data-ttu-id="6ef94-187">1-12-02 10</span><span class="sxs-lookup"><span data-stu-id="6ef94-187">1-12-02 10</span></span>|<span data-ttu-id="6ef94-188">01-12-02 10:00:00</span><span class="sxs-lookup"><span data-stu-id="6ef94-188">01-12-02 10:00:00</span></span>|  
|<span data-ttu-id="6ef94-189">1.12.02 5</span><span class="sxs-lookup"><span data-stu-id="6ef94-189">1.12.02 5</span></span>|<span data-ttu-id="6ef94-190">01-12-02 05:00:00</span><span class="sxs-lookup"><span data-stu-id="6ef94-190">01-12-02 05:00:00</span></span>|  
|<span data-ttu-id="6ef94-191">1.12.02</span><span class="sxs-lookup"><span data-stu-id="6ef94-191">1.12.02</span></span>|<span data-ttu-id="6ef94-192">01-12-02 00:00:00</span><span class="sxs-lookup"><span data-stu-id="6ef94-192">01-12-02 00:00:00</span></span>|  
|<span data-ttu-id="6ef94-193">11 12</span><span class="sxs-lookup"><span data-stu-id="6ef94-193">11 12</span></span>|<span data-ttu-id="6ef94-194">11-current month-current year 12:00:00</span><span class="sxs-lookup"><span data-stu-id="6ef94-194">11-current month-current year 12:00:00</span></span>|  
|<span data-ttu-id="6ef94-195">1112 12</span><span class="sxs-lookup"><span data-stu-id="6ef94-195">1112 12</span></span>|<span data-ttu-id="6ef94-196">11-12-current year 12:00:00</span><span class="sxs-lookup"><span data-stu-id="6ef94-196">11-12-current year 12:00:00</span></span>|  
|<span data-ttu-id="6ef94-197">t or today</span><span class="sxs-lookup"><span data-stu-id="6ef94-197">t or today</span></span>|<span data-ttu-id="6ef94-198">today's date 00:00:00</span><span class="sxs-lookup"><span data-stu-id="6ef94-198">today's date 00:00:00</span></span>|  
|<span data-ttu-id="6ef94-199">t time</span><span class="sxs-lookup"><span data-stu-id="6ef94-199">t time</span></span>|<span data-ttu-id="6ef94-200">today's date actual time</span><span class="sxs-lookup"><span data-stu-id="6ef94-200">today's date actual time</span></span>|  
|<span data-ttu-id="6ef94-201">t 10:30</span><span class="sxs-lookup"><span data-stu-id="6ef94-201">t 10:30</span></span>|<span data-ttu-id="6ef94-202">today's date 10:30:00</span><span class="sxs-lookup"><span data-stu-id="6ef94-202">today's date 10:30:00</span></span>|  
|<span data-ttu-id="6ef94-203">t 3:3:3</span><span class="sxs-lookup"><span data-stu-id="6ef94-203">t 3:3:3</span></span>|<span data-ttu-id="6ef94-204">today's date 03:03:03</span><span class="sxs-lookup"><span data-stu-id="6ef94-204">today's date 03:03:03</span></span>|  
|<span data-ttu-id="6ef94-205">w or workdate</span><span class="sxs-lookup"><span data-stu-id="6ef94-205">w or workdate</span></span>|<span data-ttu-id="6ef94-206">the working date 00:00:00</span><span class="sxs-lookup"><span data-stu-id="6ef94-206">the working date 00:00:00</span></span>|  
|<span data-ttu-id="6ef94-207">m or Monday</span><span class="sxs-lookup"><span data-stu-id="6ef94-207">m or Monday</span></span>|<span data-ttu-id="6ef94-208">Monday of the current week 00:00:00</span><span class="sxs-lookup"><span data-stu-id="6ef94-208">Monday of the current week 00:00:00</span></span>|  
|<span data-ttu-id="6ef94-209">tu or Tuesday</span><span class="sxs-lookup"><span data-stu-id="6ef94-209">tu or Tuesday</span></span>|<span data-ttu-id="6ef94-210">Tuesday of the current week 00:00:00</span><span class="sxs-lookup"><span data-stu-id="6ef94-210">Tuesday of the current week 00:00:00</span></span>|  
|<span data-ttu-id="6ef94-211">we or Wednesday</span><span class="sxs-lookup"><span data-stu-id="6ef94-211">we or Wednesday</span></span>|<span data-ttu-id="6ef94-212">Wednesday of the current week 00:00:00</span><span class="sxs-lookup"><span data-stu-id="6ef94-212">Wednesday of the current week 00:00:00</span></span>|  
|<span data-ttu-id="6ef94-213">th or Thursday</span><span class="sxs-lookup"><span data-stu-id="6ef94-213">th or Thursday</span></span>|<span data-ttu-id="6ef94-214">Thursday of the current week 00:00:00</span><span class="sxs-lookup"><span data-stu-id="6ef94-214">Thursday of the current week 00:00:00</span></span>|  
|<span data-ttu-id="6ef94-215">f or Friday</span><span class="sxs-lookup"><span data-stu-id="6ef94-215">f or Friday</span></span>|<span data-ttu-id="6ef94-216">Friday of the current week 00:00:00</span><span class="sxs-lookup"><span data-stu-id="6ef94-216">Friday of the current week 00:00:00</span></span>|  
|<span data-ttu-id="6ef94-217">s or Saturday</span><span class="sxs-lookup"><span data-stu-id="6ef94-217">s or Saturday</span></span>|<span data-ttu-id="6ef94-218">Saturday of the current week 00:00:00</span><span class="sxs-lookup"><span data-stu-id="6ef94-218">Saturday of the current week 00:00:00</span></span>|  
|<span data-ttu-id="6ef94-219">su or Sunday</span><span class="sxs-lookup"><span data-stu-id="6ef94-219">su or Sunday</span></span>|<span data-ttu-id="6ef94-220">Sunday of the current week 00:00:00</span><span class="sxs-lookup"><span data-stu-id="6ef94-220">Sunday of the current week 00:00:00</span></span>|  
|<span data-ttu-id="6ef94-221">tu 10:30</span><span class="sxs-lookup"><span data-stu-id="6ef94-221">tu 10:30</span></span>|<span data-ttu-id="6ef94-222">Tuesday of the current week 10:30:00</span><span class="sxs-lookup"><span data-stu-id="6ef94-222">Tuesday of the current week 10:30:00</span></span>|  
|<span data-ttu-id="6ef94-223">tu 3:3:3</span><span class="sxs-lookup"><span data-stu-id="6ef94-223">tu 3:3:3</span></span>|<span data-ttu-id="6ef94-224">Tuesday of the current week 03:03:03</span><span class="sxs-lookup"><span data-stu-id="6ef94-224">Tuesday of the current week 03:03:03</span></span>|  

## <a name="entering-duration"></a><span data-ttu-id="6ef94-225">Entering Duration</span><span class="sxs-lookup"><span data-stu-id="6ef94-225">Entering Duration</span></span>  
 <span data-ttu-id="6ef94-226">You enter a duration as a number followed by its unit of measure.</span><span class="sxs-lookup"><span data-stu-id="6ef94-226">You enter a duration as a number followed by its unit of measure.</span></span>  

 <span data-ttu-id="6ef94-227">Here are some examples.</span><span class="sxs-lookup"><span data-stu-id="6ef94-227">Here are some examples.</span></span>  

|<span data-ttu-id="6ef94-228">Duration</span><span class="sxs-lookup"><span data-stu-id="6ef94-228">Duration</span></span>|<span data-ttu-id="6ef94-229">Unit of measure**</span><span class="sxs-lookup"><span data-stu-id="6ef94-229">Unit of measure**</span></span>|  
|------------------|-------------------------|  
|<span data-ttu-id="6ef94-230">2h</span><span class="sxs-lookup"><span data-stu-id="6ef94-230">2h</span></span>|<span data-ttu-id="6ef94-231">2 hrs</span><span class="sxs-lookup"><span data-stu-id="6ef94-231">2 hrs</span></span>|  
|<span data-ttu-id="6ef94-232">6h 30 m</span><span class="sxs-lookup"><span data-stu-id="6ef94-232">6h 30 m</span></span>|<span data-ttu-id="6ef94-233">6 hrs 30 mins</span><span class="sxs-lookup"><span data-stu-id="6ef94-233">6 hrs 30 mins</span></span>|  
|<span data-ttu-id="6ef94-234">6.5h</span><span class="sxs-lookup"><span data-stu-id="6ef94-234">6.5h</span></span>|<span data-ttu-id="6ef94-235">6 hrs 30 mins</span><span class="sxs-lookup"><span data-stu-id="6ef94-235">6 hrs 30 mins</span></span>|  
|<span data-ttu-id="6ef94-236">90m</span><span class="sxs-lookup"><span data-stu-id="6ef94-236">90m</span></span>|<span data-ttu-id="6ef94-237">1 hr 30 mins</span><span class="sxs-lookup"><span data-stu-id="6ef94-237">1 hr 30 mins</span></span>|  
|<span data-ttu-id="6ef94-238">2d 6h 30m</span><span class="sxs-lookup"><span data-stu-id="6ef94-238">2d 6h 30m</span></span>|<span data-ttu-id="6ef94-239">2 days 6 hrs 30 mins</span><span class="sxs-lookup"><span data-stu-id="6ef94-239">2 days 6 hrs 30 mins</span></span>|  
|<span data-ttu-id="6ef94-240">2d 6h 30m 56s 600ms</span><span class="sxs-lookup"><span data-stu-id="6ef94-240">2d 6h 30m 56s 600ms</span></span>|<span data-ttu-id="6ef94-241">2 days 6 hrs 30 mins 56 secs 600 msecs</span><span class="sxs-lookup"><span data-stu-id="6ef94-241">2 days 6 hrs 30 mins 56 secs 600 msecs</span></span>|  

 <span data-ttu-id="6ef94-242">You can also enter a number and it is automatically converted to a duration.</span><span class="sxs-lookup"><span data-stu-id="6ef94-242">You can also enter a number and it is automatically converted to a duration.</span></span> <span data-ttu-id="6ef94-243">The number you enter is converted according to the default unit of measure that has been specified for the duration field.</span><span class="sxs-lookup"><span data-stu-id="6ef94-243">The number you enter is converted according to the default unit of measure that has been specified for the duration field.</span></span>  

 <span data-ttu-id="6ef94-244">To see what unit of measure is being used in a duration field, enter a number and see which unit of measure it is converted to.</span><span class="sxs-lookup"><span data-stu-id="6ef94-244">To see what unit of measure is being used in a duration field, enter a number and see which unit of measure it is converted to.</span></span>  

 <span data-ttu-id="6ef94-245">The number 5 is converted to 5 hrs, if the unit of measure is hours.</span><span class="sxs-lookup"><span data-stu-id="6ef94-245">The number 5 is converted to 5 hrs, if the unit of measure is hours.</span></span>  

<!--OnPrem  ##  <a name="BKMK_SettingDateRanges"></a> Setting Date Ranges  
 You can set filters containing a start date and an end date to display only the data contained in that date range or time interval. Special rules apply to the way you set date ranges.  

|**Meaning**|**Sample expression**|**Entries included**|  
|-----------------|---------------------------|--------------------------|  
|**Equal to**|12 15 00|Only those posted on 12 15 00.|  
|**Interval**|12 15 00..01 15 01<br /><br /> ..12 15 00|Those posted on dates between and including 12 15 00 and 01 15 01.<br /><br /> Those posted on 12 15 00 or earlier.|  
|**Either/or**|12 15 00&#124;12 16 00|Those posted on either 12 15 00 or 12 16 00. If there are entries posted on both days, they will all be displayed.|  

 You can also combine the various format types.  

|**Sample expression**|**Entries included**|  
|---------------------------|--------------------------|  
|12 15 00&#124;12 01 00..12 10 00|Entries posted either on 12 15 00 or on dates between and including 12 01 00 and 12 10 00.|  
|..12 14 00&#124;12 30 00..|Entries posted on 12 14 00 or earlier, or entries posted on 12 30 00 or later - that is, all entries except those posted on dates between and including 12 15 00 and 12 29 00.|  -->

## <a name="using-date-formulas"></a><span data-ttu-id="6ef94-246">Using Date Formulas</span><span class="sxs-lookup"><span data-stu-id="6ef94-246">Using Date Formulas</span></span>  
 <span data-ttu-id="6ef94-247">A date formula is a short, abbreviated combination of letters and numbers that specifies how to calculate dates.</span><span class="sxs-lookup"><span data-stu-id="6ef94-247">A date formula is a short, abbreviated combination of letters and numbers that specifies how to calculate dates.</span></span> <span data-ttu-id="6ef94-248">You can enter date formulas in various date calculation fields and in recurring frequency fields in recurring journals.</span><span class="sxs-lookup"><span data-stu-id="6ef94-248">You can enter date formulas in various date calculation fields and in recurring frequency fields in recurring journals.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="6ef94-249">In all data formula fields, one day is automatically included to cover today as the day when the period starts.</span><span class="sxs-lookup"><span data-stu-id="6ef94-249">In all data formula fields, one day is automatically included to cover today as the day when the period starts.</span></span> <span data-ttu-id="6ef94-250">Accordingly, if you enter 1W, for example, then the period is actually eight days because today is included.</span><span class="sxs-lookup"><span data-stu-id="6ef94-250">Accordingly, if you enter 1W, for example, then the period is actually eight days because today is included.</span></span> <span data-ttu-id="6ef94-251">To specify a period of seven days (one true week) including the period starting date, then you must enter 6D or 1W-1D.</span><span class="sxs-lookup"><span data-stu-id="6ef94-251">To specify a period of seven days (one true week) including the period starting date, then you must enter 6D or 1W-1D.</span></span>  

 <span data-ttu-id="6ef94-252">Here are some examples of how date formulas can be used:</span><span class="sxs-lookup"><span data-stu-id="6ef94-252">Here are some examples of how date formulas can be used:</span></span>  

-   <span data-ttu-id="6ef94-253">The date formula in the recurring frequency field in recurring journals determines how often the entry on the journal line will be posted.</span><span class="sxs-lookup"><span data-stu-id="6ef94-253">The date formula in the recurring frequency field in recurring journals determines how often the entry on the journal line will be posted.</span></span>  

-   <span data-ttu-id="6ef94-254">The date formula in the Grace Period field for a specified reminder level determines the period of time that must pass from the due date (or from the date of the previous reminder) before a reminder will be created.</span><span class="sxs-lookup"><span data-stu-id="6ef94-254">The date formula in the Grace Period field for a specified reminder level determines the period of time that must pass from the due date (or from the date of the previous reminder) before a reminder will be created.</span></span>  

-   <span data-ttu-id="6ef94-255">The date formula in the Due Date Calculation field determines how to calculate the due date on the reminder.</span><span class="sxs-lookup"><span data-stu-id="6ef94-255">The date formula in the Due Date Calculation field determines how to calculate the due date on the reminder.</span></span>  

 <span data-ttu-id="6ef94-256">The date calculation formula can contain a maximum of 20 characters, both numbers and letters.</span><span class="sxs-lookup"><span data-stu-id="6ef94-256">The date calculation formula can contain a maximum of 20 characters, both numbers and letters.</span></span> <span data-ttu-id="6ef94-257">You can use the following letters, which are abbreviations for time specifications.</span><span class="sxs-lookup"><span data-stu-id="6ef94-257">You can use the following letters, which are abbreviations for time specifications.</span></span>  

|||  
|-|-|  
|<span data-ttu-id="6ef94-258">C</span><span class="sxs-lookup"><span data-stu-id="6ef94-258">C</span></span>|<span data-ttu-id="6ef94-259">Current</span><span class="sxs-lookup"><span data-stu-id="6ef94-259">Current</span></span>|  
|<span data-ttu-id="6ef94-260">D</span><span class="sxs-lookup"><span data-stu-id="6ef94-260">D</span></span>|<span data-ttu-id="6ef94-261">Day(s)</span><span class="sxs-lookup"><span data-stu-id="6ef94-261">Day(s)</span></span>|  
|<span data-ttu-id="6ef94-262">W</span><span class="sxs-lookup"><span data-stu-id="6ef94-262">W</span></span>|<span data-ttu-id="6ef94-263">Week(s)</span><span class="sxs-lookup"><span data-stu-id="6ef94-263">Week(s)</span></span>|  
|<span data-ttu-id="6ef94-264">M</span><span class="sxs-lookup"><span data-stu-id="6ef94-264">M</span></span>|<span data-ttu-id="6ef94-265">Month(s)</span><span class="sxs-lookup"><span data-stu-id="6ef94-265">Month(s)</span></span>|  
|<span data-ttu-id="6ef94-266">Q</span><span class="sxs-lookup"><span data-stu-id="6ef94-266">Q</span></span>|<span data-ttu-id="6ef94-267">Quarter(s)</span><span class="sxs-lookup"><span data-stu-id="6ef94-267">Quarter(s)</span></span>|  
|<span data-ttu-id="6ef94-268">Y</span><span class="sxs-lookup"><span data-stu-id="6ef94-268">Y</span></span>|<span data-ttu-id="6ef94-269">Year(s)</span><span class="sxs-lookup"><span data-stu-id="6ef94-269">Year(s)</span></span>|  

 <span data-ttu-id="6ef94-270">You can construct a date formula in three ways.</span><span class="sxs-lookup"><span data-stu-id="6ef94-270">You can construct a date formula in three ways.</span></span>  

 <span data-ttu-id="6ef94-271">The following example shows how current plus a time unit.</span><span class="sxs-lookup"><span data-stu-id="6ef94-271">The following example shows how current plus a time unit.</span></span>  

|||  
|-|-|  
|<span data-ttu-id="6ef94-272">CW</span><span class="sxs-lookup"><span data-stu-id="6ef94-272">CW</span></span>|<span data-ttu-id="6ef94-273">Current week</span><span class="sxs-lookup"><span data-stu-id="6ef94-273">Current week</span></span>|  
|<span data-ttu-id="6ef94-274">CM</span><span class="sxs-lookup"><span data-stu-id="6ef94-274">CM</span></span>|<span data-ttu-id="6ef94-275">Current month</span><span class="sxs-lookup"><span data-stu-id="6ef94-275">Current month</span></span>|  

 <span data-ttu-id="6ef94-276">The following example shows how a number and a time unit.</span><span class="sxs-lookup"><span data-stu-id="6ef94-276">The following example shows how a number and a time unit.</span></span> <span data-ttu-id="6ef94-277">A number cannot be larger than 9999.</span><span class="sxs-lookup"><span data-stu-id="6ef94-277">A number cannot be larger than 9999.</span></span>  

|||  
|-|-|  
|<span data-ttu-id="6ef94-278">10D</span><span class="sxs-lookup"><span data-stu-id="6ef94-278">10D</span></span>|<span data-ttu-id="6ef94-279">10 days from today</span><span class="sxs-lookup"><span data-stu-id="6ef94-279">10 days from today</span></span>|  
|<span data-ttu-id="6ef94-280">2W</span><span class="sxs-lookup"><span data-stu-id="6ef94-280">2W</span></span>|<span data-ttu-id="6ef94-281">2 weeks from today</span><span class="sxs-lookup"><span data-stu-id="6ef94-281">2 weeks from today</span></span>|  

 <span data-ttu-id="6ef94-282">The following example shows how a time unit and a number.</span><span class="sxs-lookup"><span data-stu-id="6ef94-282">The following example shows how a time unit and a number.</span></span>  

|||  
|-|-|  
|<span data-ttu-id="6ef94-283">D10</span><span class="sxs-lookup"><span data-stu-id="6ef94-283">D10</span></span>|<span data-ttu-id="6ef94-284">The next 10th day of a month</span><span class="sxs-lookup"><span data-stu-id="6ef94-284">The next 10th day of a month</span></span>|  
|<span data-ttu-id="6ef94-285">WD4</span><span class="sxs-lookup"><span data-stu-id="6ef94-285">WD4</span></span>|<span data-ttu-id="6ef94-286">The next 4th day of a week (Thursday)</span><span class="sxs-lookup"><span data-stu-id="6ef94-286">The next 4th day of a week (Thursday)</span></span>|  

 <span data-ttu-id="6ef94-287">The following example shows how you can combine these three forms as needed.</span><span class="sxs-lookup"><span data-stu-id="6ef94-287">The following example shows how you can combine these three forms as needed.</span></span>  

|||  
|-|-|  
|<span data-ttu-id="6ef94-288">CM+10D</span><span class="sxs-lookup"><span data-stu-id="6ef94-288">CM+10D</span></span>|<span data-ttu-id="6ef94-289">Current month + 10 days</span><span class="sxs-lookup"><span data-stu-id="6ef94-289">Current month + 10 days</span></span>|  

 <span data-ttu-id="6ef94-290">The following example shows how you can use a minus sign to indicate a date in the past.</span><span class="sxs-lookup"><span data-stu-id="6ef94-290">The following example shows how you can use a minus sign to indicate a date in the past.</span></span>  

|||  
|-|-|  
|<span data-ttu-id="6ef94-291">-1Y</span><span class="sxs-lookup"><span data-stu-id="6ef94-291">-1Y</span></span>|<span data-ttu-id="6ef94-292">1 year ago from today</span><span class="sxs-lookup"><span data-stu-id="6ef94-292">1 year ago from today</span></span>|  

<!--OnPrem > [!CAUTION]  
>  If the location uses a base calendar, then the date formula that you enter in, for example, the **Shipping Time** field is interpreted according to the calendar working days. For example, a 1W means seven working days. For more information, see Base Calendar Card.-->  
## <a name="see-also"></a><span data-ttu-id="6ef94-293">See Also</span><span class="sxs-lookup"><span data-stu-id="6ef94-293">See Also</span></span>  
 [<span data-ttu-id="6ef94-294">Searching, Filtering, and Sorting Data</span><span class="sxs-lookup"><span data-stu-id="6ef94-294">Searching, Filtering, and Sorting Data</span></span>](ui-enter-criteria-filters.md)  
 <span data-ttu-id="6ef94-295">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="6ef94-295">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

