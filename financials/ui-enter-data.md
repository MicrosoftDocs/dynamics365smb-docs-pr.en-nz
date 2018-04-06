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
# <a name="entering-data"></a>Entering Data
There are many general functions that help you enter data  in a quick and easy way. The general functions for entering data are described in this article.  

The examples in this article use the demonstration data.

## <a name="mandatory-fields"></a>Mandatory Fields
When you enter data on pages, certain fields are marked with a red asterisk. The red asterisk means that the field must be filled to complete a certain process that uses the field, such as posting a transaction that uses the value in the field.  

Even though the field contains a red asterisk, you are not forced to fill the field before you continue to other fields or close the page. The red asterisk only serves as a reminder that you will be blocked from completing a certain process.  


## <a name="finding-data-as-you-type"></a>Finding Data As You Type  
 When you start to type characters in a field, a drop-down list is displayed and shows possible field values. The list changes as you type more characters, and you can select the correct value when it is displayed.  

 Many fields have a down arrow button that you can choose. You choose the arrow to get a list of data that is available to enter in the field. The button has two functions depending on the type of field:  

-   Lookup - Displays information from another table that you can enter in the field. You can select one piece of data at a time.  

-   Drop-down - Displays the set of options that exist for the field. You can select only one of the options.  

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

## <a name="entering-quantities-by-calculation"></a>Entering Quantities by Calculation  
 When entering numbers into quantity fields, such as the **Quantity** field on an item journal line, you can enter the formula instead of the sum quantity.  

## <a name="examples"></a>Examples  

-   If you enter 19+19, the field is calculated to 38.  

-   If you enter 41-9, the field is calculated to 32.  

-   If you enter 12*4, the field is calculated to 48.  

-   If you enter 12/4, the field is calculated to 3.  

# <a name="entering-negative-numbers"></a>Entering Negative Numbers
You can enter negative numbers in two ways. The number -20.5 can be entered as:  

-   -20.5  

    or
-   20.5-  

 In both cases, the amount will be recorded in as -20.5.  

 If the last character of the expression is a **+** or a **-**, the entire expression will be recorded with that sign. An example, **10-20+** will result in 10 and not -10.  

## <a name="entering-dates-and-times"></a>Entering Dates and Times
You can enter dates and times in all the fields that are specifically assigned to dates (date fields). You can enter dates with or without separators.

> [!NOTE]  
> How you enter dates and times depends on your **Region** settings. For more information, see [Changing Basic Settings](ui-change-basic-settings.md).  

### <a name="entering-dates"></a>Entering Dates  
 In a date field you can enter two, four, six, or eight digits:  

-   If you enter only two digits, this is interpreted as the day, and it will add the month and the year of the work date.  

-   If you enter four digits, this is interpreted as the day and the month, and it will add the year of the work date.  

-   If the date you want to enter is in the range 01/01/1930 through 12/31/2029, you can enter the year with two digits; otherwise, enter the year with four digits.  

 You can also enter a date as a weekday followed by a week number and, optionally, a year (for example, Mon25 or mon25 means Monday in week 25).  

 Instead of entering a specific date, you can enter one of two codes.  

|Code|Result|  
|--------------|----------------|  
|t|This is today's date (the system date for the computer).|  
|w|This is the work date that is setup in the application. To change the work date, see [Changing Basic Settings](ui-change-basic-settings.md). You may want to use a work date if you have many transactions with a date other than today's date.|  

<!--Onprem ## Closing Date  
 When you close a fiscal year, you can use closing dates to indicate that an entry is a closing entry. A closing date technically is between two dates, for example between Dec 31 and Jan 1.  

 To specify that a date is a closing date, put C just before the date: C123101. -->

## <a name="entering-times"></a>Entering Times  
 When you enter times, you can insert any separator sign that you want between the units, but it is not required. You do not have to write minutes, seconds, or AM/PM.  

 The following table lists the various ways in which times can be entered and how they are interpreted.  

|Entry|Interpretation|  
|---------------|------------------------|  
|5|05:00:00|  
|5:30|05:30:00|  
|0530|05:30:00|  
|5:30:5|05:30:05|  
|053005|05:30:05|  
|5:30:5,50|05:30:05.5|  
|053005050|05:30:05.05|  

 You must enter two digits for each unit of time if you do not enter a separator.  

## <a name="entering-datetimes"></a>Entering Datetimes  
 When you enter datetimes you must enter a space between the date and the time.  

 The following table lists the various ways in which you can enter datetimes and how they are interpreted.  

|Entry|Interpretation|  
|---------------|------------------------|  
|131202 132455|13-12-02 13:24:55|  
|1-12-02 10|01-12-02 10:00:00|  
|1.12.02 5|01-12-02 05:00:00|  
|1.12.02|01-12-02 00:00:00|  
|11 12|11-current month-current year 12:00:00|  
|1112 12|11-12-current year 12:00:00|  
|t or today|today's date 00:00:00|  
|t time|today's date actual time|  
|t 10:30|today's date 10:30:00|  
|t 3:3:3|today's date 03:03:03|  
|w or workdate|the working date 00:00:00|  
|m or Monday|Monday of the current week 00:00:00|  
|tu or Tuesday|Tuesday of the current week 00:00:00|  
|we or Wednesday|Wednesday of the current week 00:00:00|  
|th or Thursday|Thursday of the current week 00:00:00|  
|f or Friday|Friday of the current week 00:00:00|  
|s or Saturday|Saturday of the current week 00:00:00|  
|su or Sunday|Sunday of the current week 00:00:00|  
|tu 10:30|Tuesday of the current week 10:30:00|  
|tu 3:3:3|Tuesday of the current week 03:03:03|  

## <a name="entering-duration"></a>Entering Duration  
 You enter a duration as a number followed by its unit of measure.  

 Here are some examples.  

|Duration|Unit of measure**|  
|------------------|-------------------------|  
|2h|2 hrs|  
|6h 30 m|6 hrs 30 mins|  
|6.5h|6 hrs 30 mins|  
|90m|1 hr 30 mins|  
|2d 6h 30m|2 days 6 hrs 30 mins|  
|2d 6h 30m 56s 600ms|2 days 6 hrs 30 mins 56 secs 600 msecs|  

 You can also enter a number and it is automatically converted to a duration. The number you enter is converted according to the default unit of measure that has been specified for the duration field.  

 To see what unit of measure is being used in a duration field, enter a number and see which unit of measure it is converted to.  

 The number 5 is converted to 5 hrs, if the unit of measure is hours.  

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

## <a name="using-date-formulas"></a>Using Date Formulas  
 A date formula is a short, abbreviated combination of letters and numbers that specifies how to calculate dates. You can enter date formulas in various date calculation fields and in recurring frequency fields in recurring journals.  

> [!NOTE]  
>  In all data formula fields, one day is automatically included to cover today as the day when the period starts. Accordingly, if you enter 1W, for example, then the period is actually eight days because today is included. To specify a period of seven days (one true week) including the period starting date, then you must enter 6D or 1W-1D.  

 Here are some examples of how date formulas can be used:  

-   The date formula in the recurring frequency field in recurring journals determines how often the entry on the journal line will be posted.  

-   The date formula in the Grace Period field for a specified reminder level determines the period of time that must pass from the due date (or from the date of the previous reminder) before a reminder will be created.  

-   The date formula in the Due Date Calculation field determines how to calculate the due date on the reminder.  

 The date calculation formula can contain a maximum of 20 characters, both numbers and letters. You can use the following letters, which are abbreviations for time specifications.  

|||  
|-|-|  
|C|Current|  
|D|Day(s)|  
|W|Week(s)|  
|M|Month(s)|  
|Q|Quarter(s)|  
|Y|Year(s)|  

 You can construct a date formula in three ways.  

 The following example shows how current plus a time unit.  

|||  
|-|-|  
|CW|Current week|  
|CM|Current month|  

 The following example shows how a number and a time unit. A number cannot be larger than 9999.  

|||  
|-|-|  
|10D|10 days from today|  
|2W|2 weeks from today|  

 The following example shows how a time unit and a number.  

|||  
|-|-|  
|D10|The next 10th day of a month|  
|WD4|The next 4th day of a week (Thursday)|  

 The following example shows how you can combine these three forms as needed.  

|||  
|-|-|  
|CM+10D|Current month + 10 days|  

 The following example shows how you can use a minus sign to indicate a date in the past.  

|||  
|-|-|  
|-1Y|1 year ago from today|  

<!--OnPrem > [!CAUTION]  
>  If the location uses a base calendar, then the date formula that you enter in, for example, the **Shipping Time** field is interpreted according to the calendar working days. For example, a 1W means seven working days. For more information, see Base Calendar Card.-->  
## <a name="see-also"></a>See Also  
 [Searching, Filtering, and Sorting Data](ui-enter-criteria-filters.md)  
 [Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

