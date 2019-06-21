---
title: Keyboard Shortcuts
description: The complete list of keyboard shortcut combinations to work efficiently with your data.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: accessibility, shortcuts, keyboarding, keys
ms.date: 04/01/2019
ms.author: jswymer
ms.openlocfilehash: 11d63e2745ce35067d87e66c6077d51276f90075
ms.sourcegitcommit: 04581558f6c5488c705a7ac392cf297be10b5f4f
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 06/06/2019
ms.locfileid: "1621222"
---
# <a name="keyboard-shortcuts"></a>Keyboard Shortcuts
This article provides an overview of some of the shortcut key combinations that you can use when you are working with [!INCLUDE[prodshort](includes/prodshort.md)].

> [!TIP]
> For a quick, print-friendly overview of the most popular shortcuts, [see the reference article here](keyboard-shortcuts-cheatsheet.md) or click the following image:
>
>[ ![To download for printing, right-click and select Save Picture As](media/bckeyboardmap-inline.png) ](media/bckeyboardmap.png#lightbox)

## <a name="overview"></a>Overview
The keyboard shortcuts aide accessibility and can make it easier and more efficient to navigate to different areas and elements on a page.

The keyboard shortcuts are supported by most web browsers; however, the behaviour may vary slightly.

The keyboard shortcuts described here refer to the U.S. keyboard layout. The layout of the keys on other keyboards may not correspond exactly to the keys on a U.S. keyboard.

Most of the shortcuts are the same no matter whether the operating system is Windows or macOS; however, there are some shortcuts that differ for macOS. These are indicated in parentheses in the tables in the sections that follow.

##  <a name="Keyboard"></a> General Keyboard Shortcuts
The following table describes keyboard shortcuts for navigating and accessing different elements of a page, such as actions, drop-down lists, lookups, and more. For details about keyboard shortcuts for navigating records once you get inside a list, see the next section.

|Press these keys<br />(in macOS)|To do this|
|----------------|-----------|
|Alt+Down Arrow|Open a drop-down list or look up a value for a field.|    
|Alt+Right Arrow|See the transactions that resulted in a calculated value in a field.|  
|Alt+F2|Show and hide the FactBox pane.|
|Alt+Q<br />(Ctrl+Alt+Q)|Open **Tell me what you want to do** box that can help you find a page, a report, an action on the current page, or an article in the documentation.|
|Alt+T|Open the **My Settings** page.|
|Alt+Up Arrow|Show tooltip for a field or a column header of a table. If the field has validation errors, press "Alt+Up Arrow" to show the validation error. Press "Esc" or "Alt+Up Arrow" to close the tooltip.|
|Ctrl+Alt+F1|Open and close the page inspection pane. The page inspection pane shows information about the page, like its source table, fields, filters, extensions, and more.<br /><br />For more information, see [Inspecting Pages](across-inspect-page.md).|
|Ctrl+C |Copy the value of field. If the field is in focus, and you have not selected any text in the field, this will copy the entire value. If you have selected any text in the field, then it will copy the selected text only.|
|Ctrl+F1|Open the Business Central help for the page.|
|Ctrl+F5|Reload the [!INCLUDE[prodshort](includes/prodshort.md)] application.<br/><br />This is similar to selecting refresh/reload in the browser.|
|F5|Refresh the data on the current page.<br /><br />Use this to ensure that the data on the page is up-to-date with any changes that others have made while you are working.|
|Ctrl+F12|Switch between wide and narrow layout view.|
|Enter|Enable or access the element or control that is in focus.|
|Esc|Close the current page or drop-down.|
|Tab|Move focus to the next control or element on a page, such as actions, buttons, fields, or list headings.|
|Shift+Tab|Move focus to the previous control or element on a page, such as actions, buttons, fields, or list headings.|

## <a name="keyboard-shortcuts-in-lists"></a>Keyboard Shortcuts in Lists

The following table describes the keyboard shortcuts that you can use in a list page. The shortcut action is slightly different depending on whether the page is shown in the list view or tile view.
<!--
> [!Note]
> In the table that follows, the term *actionable field* refers to a field on which you can do something, like change a value or link to another page. In general, the shortcuts will skip over fields that display information that you cannot change from the list (in other words, fields that are read-only).
-->
### <a name="general"></a>General

|Press these keys<br />(in macOS)|To do this in a list view|To do this in a tile view |
|-----------------|-------|-------|
|Alt+F7 |Sort the selected column in ascending or descending order.|Not applicable.|
|Shift+F10 |Open a menu of options that are available for selected row.|Not applicable.|
|Alt+N |Open a page for creating a new record; the same way as selecting the **New** action. |Same.|

### <a name="navigateshortcuts"></a>Navigating Between Rows and Columns

|Press these keys<br />(in macOS)|To do this in a list view |To do this in a tile view |
|-----------------|-------|-------|
|Ctrl+Home<br />(Fn+Ctrl+Left Arrow)|Select the first row in the list; focus remains in the same column.|Move to the first tile in first row. |
|Ctrl+End<br />(Fn+Ctrl+Right Arrow)|Select the last row in the list; focus remains in the same column.|Move to the last tile in last row.|
|Home<br />(Fn+Left Arrow)|Move to the first field in the row.|Move to the first tile in the row.|
|End<br />(Fn+right Arrow)|Move to the last field in the row.|Move to the last tile in the row.|
|Enter|Open the record that is associated with the field.<br /><br />Only relevant if a card page is associated with the record.|Opens the record.<br /><br />Only relevant if a card page is associated with the record.|
|Ctrl+Enter|Move focus to the next element outside the list.|Move focus to the next element outside the list.|
|Down Arrow|Move in the same column to the field in the row below. |Move in the same column to the tile in the row below. |
|Up Arrow|Move in the same column to the field in the row above.| Move in the same column to the tile in the row above.  |
|Right Arrow|In a view-only list, move in the same row to the next field to the right.<br /><br />In an editable list, move to the right within the current field.| Move in the same row to the next tile to the right. |
|Left Arrow|In a view-only list, move in the same row to the previous field to the left. <br /><br />In an editable list, move to the left within the current field.| Move in the same row to the previous tile to the left. |
|Page Up<br />(Fn+up Arrow)|Scroll to display the set rows above the current rows in view. |Scrolls to display the set of tiles above the current tiles in view. |
|Page Down<br />(Fn+down Arrow)|Scroll to display the set rows below the current rows in view.|Scroll to display the set of tiles below the current tiles in view.|
|Tab|In editable list, move in the same row to the next field to the right.|Not applicable.||
|Shift+Tab|In editable list, move in the same row to the previous field to the left. | Not applicable. |

### <a name="CopyRows"></a>Selecting, Copying, and Pasting

|Press these keys<br />(in macOS)|To do this in a list view |To do this in a tile view |
|-----------------|-------|-------|
|Ctrl+Click<br />(Cmd+Click)|Extend the selection of rows to include the row that you click.|Not applicable.|
|Shift+Click|Extend the selection of rows to include the row that you click and all the rows in between.<br /><br />You can use this after using Ctrl+Up Arrow or Ctrl+Up Down to expand your selection.|Not applicable.|
|Ctrl+Up Arrow<br />(Ctrl+Cmd+Up Arrow)|Move focus to the row above and keep the current row selected.|Not applicable.|
|Ctrl+Down Arrow<br />(Ctrl+Cmd+Down Arrow)|Move focus to the row below and keep the current row selected.|Not applicable.|
|Ctrl+Space Bar<br />(Ctrl+Cmd+Space )|Extend the selection of rows to include the focused row.<br /><br />You can use this after using Ctrl+Up Arrow or Ctrl+Down Arrow to expand your selection.|Not applicable.|
|Ctrl+A|Select all rows.|Not applicable.|
|Shift+Up Arrow|Extend the selection of rows to include the row above.|Not applicable.|
|Shift+Down Arrow|Extend the selection of rows to include the row below.|Not applicable.|
|Shift+Page Up<br />(Shift+Fn+Up Arrow)|Extend the selection of rows to include all visible rows above the current selection of rows.|Not applicable.|
|Shift+Page Down<br />(Shift+Fn+Down Arrow)|Extend the selection of rows to include all visible rows below the current selection of rows.|Not applicable.|
|Ctrl+C<br />(Cmd+C)|Copy the selected rows to the Clipboard.|Not applicable.|
|Ctrl+V<br />(Cmd+V)|Paste the selected rows from the Clipboard into the current page or external document, like Microsoft Excel or Outlook email. You can only do this in editable lists.|Not applicable.|
|F8|Copy the field in the same column of the row above, and paste it into the current row. You can only do this in editable lists. Using this shortcut followed by a Tab lets you quickly fill out fields in line items that you want to have the same value as the row above.|Not applicable.|

### <a name="KeyboardFilter"></a>Searching and Filtering Lists

|Press these keys<br />(in macOS)|To do this|
|-----------------|-------|
|F3|Toggles the search box.<ul><li>Activate the search box, so you can start typing your search text.</li><li>If the search box is already activated, F3 returns to the list without clearing the search text.</li><ul>|
|Shift+F3|Open and close the filter pane.<ul><li> If the filter pane is not open, Shift+F3 opens it and focuses on the **+ Filter** action under **Filter list by**, which lets you just hit Enter to start adding a field filter.</li><li>If the filter pane is already open, Shift+F3 closes it but does not clear any filters that you have added.</li></ul>|
|Ctrl+Shift+F3|Open and close the filter pane.<ul><li> If the filter pane is not open, Ctrl+Shift+F3 opens it and focuses on the **+ Filter** action under **Filter total by**, which lets you just hit Enter to start adding a totals filter.</li><li>If the filter pane is already open, Ctrl+Shift+F3 closes it but does not clear any filters that you have added.</li></ul>  |
|Alt+F3|Toggle filtering to the selected value.<ul><li>Applies a column filter on the selected field value in the list. This does the same as choosing **Filter to this value** from a column heading. It opens the filter pane, sets filter to the selected value, while focus remains on cell in the list.</li><li>If the column is already filtered, Alt+F3 clears the filter on that column.</li></ul> |
|Shift+Alt+F3|Open the filter pane and add a filter on the selected column in the list. Focus is on the new filter field which lets start typing the filter criteria right away.<br /><br /> This does the same as selecting **Filter** from the column heading.<br /><br />If there is already a filter on the field, a new filter is added. |
|Ctrl+Shift+Alt+F3|Reset filters. This does the same as choosing **Reset filters** in the filter pane, and it applies to field and totals filters.<br /><br /> Filters return to the default filters for the current view. If the current view is **All**, then this is the same as returning to an unfiltered view with all records. |
|Ctrl+Enter|Change focus from the the filter pane back to the list.|

## <a name="keyboard-shortcuts-in-cards-and-documents"></a>Keyboard Shortcuts in Cards and Documents

The following shortcuts are available on card pages (like **Customer**) and document pages (like **Sales Order**) for displaying and modifying records.

|Press these keys<br />(in macOS)|To do this|
|----------------|-----------|
|Alt+F6|Collapse and expand the current FastTab.|
|Alt+N |Open a page for creating a new record; the same way as choosing the **New** action. |
|Alt+Shift+N |Close the current card page and creates a new entity; the same as selecting the back arrow and then the **New** action.|
|Ctrl+Down Arrow|Open the next record for an entity.|
|Ctrl+Up Arrow |Open the previous record for an entity.|
|Ctrl+Shift+F12 |Maximise the line items part in a document page, like a sales order or invoice. Other parts of the page are hidden, and the line items part expands to entire workspace. Press the keys again to return to the normal display.<br /><br />For more information, see [Focusing on Line Items](ui-enter-data.md#Focus).|
|F6|Move to next FastTab or part (sub-page).|
|Shift+F6|Move to previous FastTab or part (sub-page).|

## <a name="QuickEntry"></a>Quick Entry Shortcuts for Fields

The following shortcuts pertain to the Quick Entry feature on cards, documents, and list pages. On lists, the shortcuts cannot be used when the list is in the tile view. For more information about Quick Entry, see [Accelerating Data Entry Using Quick Entry](ui-enter-data.md#QuickEntry).

|Press these keys<br />(in macOS)|To do this|Remarks|
|-----------------|-------|-------|
|Enter|Confirm the value in the current field and go to the next Quick Entry field.||
|Shift+Enter|Confirm the value in the current field and go to the previous Quick Entry field.||
|Ctrl+Shift+Enter|Confirm the value in the current column and go to next Quick Entry field outside the list.<br /><br />This shortcut applies to embedded lists on a page, such as line items on a sales order. It enables you to quickly get out of the list and continue entering data in other fields on the page.|

## <a name="keyboard-shortcuts-in-worksheets"></a>Keyboard Shortcuts in Worksheets

The following shortcuts are only available on Worksheet pages, like **Item Journals**.

|Press these keys<br />(in macOS)|To do this|  
|----------------|-----------|  
|Ctrl+Delete| Delete a line item.|

## <a name="a-namecalendarshortcuts-keyboard-shortcuts-in-the-calendar-date-picker"></a><a name="calendarshortcuts"/> Keyboard Shortcuts in the Calendar (Date Picker)

When setting a date field, you can either enter the date manually or open a calendar (date picker) that lets you select the date you want. The following table describes the keyboard shortcuts for the calendar.

|Press these keys<br />(in macOS)|To do this|
|-----------------|-------|
|Ctrl+Home|Open the calendar if closed.|
|Ctrl+Home<br />(Cmd+Home)|Move to the current month, current day.|
|Ctrl+Left Arrow<br />(Cmd+Left Arrow)|Move to the previous day.|
|Ctrl+Right Arrow<br />(Cmd+Right Arrow)|Move to the next day.|
|Ctrl+Up Arrow<br />(Cmd+Up Arrow)|Move to the previous week, same day of the week.|
|Ctrl+Down Arrow<br />(Cmd+Down Arrow)|Move to the next week, same day of the week.|
|Enter|Select the focused date.|
|Ctrl+End<br />(Cmd+End)|Close the calendar and delete current the date.|
|Esc|Close the calendar without a selection, keep current date.|
|Page Down|Move to the next month.|
|Page Up|Move to the previous month.|  

## <a name="a-namereportpreviewshortcutskeyboard-shortcuts-in-the-report-preview"></a><a name="reportpreviewshortcuts"/>Keyboard Shortcuts in the Report Preview

|Press these keys<br />(in macOS)|To do this|
|-----------------|-------|
|Down Arrow|Scroll down the page.|  
|Up Arrow|Scroll up the page.|
|Ctrl+0 (zero)<br />(Cmd+0)|Fits the entire page on the page. |
|Ctrl+Home<br />(Cmd+Home)|Go to the first page of the report.|
|Ctrl+End<br />(Cmd+Home)|Go to the last page of the report.|
|Left Arrow|Scroll to the left when the page is zoomed in so that it is not entirely in view. |
|Right Arrow|Scroll to the right when the page is zoomed in so that it is not entirely in view. |
|Page Down<br />(Fn+Down Arrow)|Go to the next page of the report.|
|Page Up<br />(Fn+Up Arrow)|Go to the previous page of the report.|

## <a name="see-also"></a>See also 

[Assistive Features](ui-accessibility.md)  
[Getting Started](product-get-started.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  
[Frequently Asked Questions](across-faq.md)  
