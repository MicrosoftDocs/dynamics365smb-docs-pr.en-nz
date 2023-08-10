---
title: Analyse data in list pages using data analysis mode
description: Learn how to use the data analysis mode in Business central to analyse data.
author: jswymer
ms.author: jswymer
ms.reviewer: jswymer
ms.topic: how-to
ms.date: 03/30/2023
ms.custom: bap-template
ms.service: dynamics365-business-central
ms.search.form: '456, 457, 458, 459, 460, 461, 16, 22, 25, 26, 27, 31, 143, 144, 9300, 9301, 9303, 9304, 9305, 9306, 9307, 9309, 9310, 9311'
---
# <a name="analyze-list-data-using-data-analysis-mode"></a>Analyse list data using data analysis mode

In this article, you learn how to analyse data from list pages using the *data analysis mode*. The data analysis mode enables you to analyse data directly from the page, without having to run a report or switch another application like Excel. It provides an interactive and versatile way to calculate, summarise, and examine data. Instead of running reports using different options and filters, you can add multiple tabs that represent different tasks or views on the data. Examples could be "My customers", "Follow up items", "Recently added vendors", "Sales statistics", or any other view you can imagine.

> [!TIP]
> A good thing about the data analysis mode is that it doesn't change any of the underlying data of list page or the layout of the page when it's not in data analysis mode. So the best way to learn about what you can do in the data analysis mode is to try things out.

## <a name="prerequisite"></a>Prerequisite

The data analysis mode is currently in preview, which means that an administrator must turn it on before you can use it. If you're an administrator, and you want to turn on the data analysis mode, go to the **Feature Management** page and enable **Feature Update: Analysis mode, quickly analyse data directly in Business Central**. For more information about turning features on and off, go to [Feature Management](/dynamics365/business-central/dev-itpro/administration/feature-management).

## <a name="get-started"></a>Get started

1. Open the list page.

   For example, to work with **Customer Ledger Entries**, select the ![Magnifying glass that opens the Tell Me feature.](media/ui-search/search_small.png) icon (<kbd>Alt</kbd>+<kbd>Q</kbd>), enter *customer ledger entries*, and then choose the related link.  
2. In the action bar at the top of the page, turn on the **Analyse** toggle switch.

    Data analysis mode opens the data in an experience that's optimised for data analysis.  While in data analysis mode, the normal action bar is replaced with a special data analysis mode bar. The following figure illustrates the different areas of a page in the data analysis mode.

   [![Shows an overview of a page on the data analysis mode](media/analysis-mode-overview-2.png)](media/analysis-mode-overview-2.png#lightbox)

   Each area is explained in the sections that follow.

3. Use the different areas to manipulate, summarise and analyse data. See the sections that follow for details.

4. When you want to exit the analyse mode, turn off the **Analyse** toggle switch.

   The analysis tabs that you've added remain until you delete them. So if you return to the data analysis mode again, you'll see them exactly as you left them.

> [!NOTE]
> The data shown in analysis mode is controlled by the filters or views set on the list page. This allows you to pre-filter data before entering analysis mode.

## <a name="work-with-data-analysis-mode"></a>Work with data analysis mode

In the data analysis mode, the page is divided into two areas:

- The main area, which consists of the data area (1), summary bar (2), and tabs bar (5)
- The data manipulation area, which consists of two panes: columns (3) and analysis filters (4).

### <a name="data-area-1"></a>Data area (1)

The data area is where the rows and columns of the list page are shown and data is summarised. The data area provides a versatile way to control of the layout of columns and a quick way to get a summary of the data. For columns that contain numeric values, the sum of all values in the column is shown in a last row, unless you've defined row groups. In this case, the sums appear as a subtotal for the groups.  

![Shows an overview of a data area on a page in the data analysis mode](media/analysis-mode-data-area.png)

- To move a column, select it and drag it to where they make the most sense in your analysis.
- Right-click the column or hover over it and select the menu icon ![Shows the icon on a column in data analysis mode that opens a menu of actions](media/analysis-mode-column-menu-icon.png) to access several actions that you can do on columns. For example:

  - To pin a column to the left or right of the data area so that it doesn't move off the screen when you scroll, select ![Shows the icon on a column in data analysis mode that opens a menu of actions](media/analysis-mode-column-menu-icon.png) > **Pin column** > **Pin left** the column part.
  - Define data filters directly on the column definition instead of going to the **Analysis Filters** panes. You can still peek in on details about related data and for each line, and open the card to learn more about a given entity.
- Use the data area to interact with the data. For columns that contain numeric, summable values, you can get descriptive statistics on a set of fields by marking them. The statistics appear in the status bar (2) along the bottom of the page.
- Export data in Excel or csv format. Simply right-click on the data area or a selection of cells to export.

### <a name="summary-bar-2"></a>Summary bar (2)

The summary bar is along the bottom of the page and displays statistics about the data in the list. As you interact with columns whose values can be summed, like selecting multiple rows in a column that displays amounts, the data will update.

![Shows an overview of a summary bar on the data analysis mode](media/analysis-mode-totals-row.png)

The following table describes the different numbers that are shown in the totals area:

|Number|Description|
|-|-|
|Rows|The number of selected rows as a part of the total number of available rows. |
|Total rows|The numbers of rows in the unfiltered list.|
|Filtered|The number of rows displayed as a result of the filters applied to the list.|
|Average|The average value in all the selected summable fields.|
|Count|The number of selected rows.|
|Min|The minimum value in all the selected summable fields.|
|Max|The maximum value in all the selected summable fields.|
|Sum|The sum total of all the values in the selected summable fields.|

### <a name="columns-3"></a>Columns (3)

The **Columns** is one of two panes that work together to define your analysis. The other area is the **Analysis filters** pane. The **Columns** pane is used to summarise the data. Use the **Columns** pane to define which columns should be included in the analysis.

![Shows an overview of the columns pane in the data analysis mode](media/analysis-mode-columns-2.png)

|Areas|Description|
|-|-|
|Search/check or clear all boxes|Search for columns. Select the check box to select/clear all columns.|
|Check boxes|This area includes a check box for each field in the list's source table. Use this area to change what columns are shown in the list. Select a check box to show column for the field on the page; clear the check box to hide the column. |
|Row groups|Use this area to group and sum data by one or more fields. You can only include non-numeric fields, like text, date and time fields. Row groups are used often in pivot mode.|
|Values|Use this area to specify fields that you want a sum total for. You can only include fields that contain numbers that can be added together; for example, not text, date, or time fields.|

To move a field from one area to another, select grab icon ![Shows an overview of a page on the analysis mode](media/column-grab-icon.png) next to the column in the list above and drag into the target area. You're prevented from moving a field into an area where's it's not allowed.

### <a name="analysis-filters-4"></a>Analysis filters (4)

The **Analysis filters** pane lets you set further data filters on columns to limit the entries in the list. Set filters on columns to limit the entries in the list and subsequent sums to only those entries you're interested in based on a criteria you define. For example, suppose you're only interested in data for a specific customer or sales orders that exceed a specific amount. To set a filter, select the column, choose the comparison operation from the list (like **Equals** or **Starts with**), then enter the value.

![Shows an overview of the filters pane in the analysis mode](media/analysis-mode-filters.png)

> [!NOTE]
> The additional filters only apply to the current analysis tab. This allows you to define exactly the extra data filters that are needed for a specific analysis.

### <a name="tabs-5"></a>Tabs (5)

The tabs area at the top lets you create different configurations (columns and analysis filters) on separate tabs, where you can manipulate data on the tabs independently of each other. There's always at least one tab, called **Analysis 1** by default. Adding more tabs is beneficial for saving frequently used analysis configurations on a dataset. For example, you might have tabs for analysing data in the pivot mode, and other tabs that filter to a subset of rows. Some tabs might show a detailed view with many columns, and others only display a few key columns.

Here's some pointers on working with multiple analysis tabs:

- To add a new tab, select the large **+** sign next to the last analysis tab.
- Select the down arrowhead on a tab to access a list of actions you can do on a tab, like rename, duplicate, delete, and move.

   - **Delete** deletes the tab you currently have open. **Delete All** deletes all tabs that you've added, except the default **Analysis 1** tab.
- You can't completely remove the **Analysis 1**, but you can rename it by using the **Rename** action and clear the changes you've made by using **Delete** or **Delete All**.  

- The analysis tabs that you've added and configured remain until you delete them. So if you return to the data analysis mode again, you'll see them exactly as you left them.

   > [!TIP]
   > The tabs that you set up are only visible to you. Other users will only see tabs they've set up.
- You can copy analysis tabs. Copying can be useful if you want to experiment with changing a tab without changing the original, or if you want to create different variations of the same analysis.

## <a name="pivot-mode"></a>Pivot mode

You can use pivot mode to analyse large amount of numerical data, subtotaling data by categories and subcategories. The pivot mode is like [pivot tables in Microsoft Excel](https://support.microsoft.com/office/create-a-pivottable-to-analyze-worksheet-data-a9a84538-bfe9-40a9-a8e9-f99134456576).

To turn the pivot mode on and off, slide the **Pivot mode** switch in the **Columns** pane (3). When you turn on the pivot mode, the **Column labels** area appears in the pane. Use the **Column labels** area to group sum totals for rows into categories. Fields that you add to the **Column labels** area will show as columns in the data area (1).

Building out the data analysis in pivot mode involves moving fields into the three areas: **Row groups**, **Columns labels**, and **Values**. The following figure illustrates where the fields map to the data area (1), where `sum` is the calculated data, and optionally **Values**.

<table>
<tr><th></th><th>Column label</th><th></th><th>Column label</th><th></th></tr>
<tr><th>Row group</th><th>Value</th><th>Value</th><th>Value</th><th>Value</th></tr>
<tr><td>row</td><td>sum</td><td>sum</td><td>sum</td><td>sum</td></tr>
<tr><td>row</td><td>sum</td><td>sum</td><td>sum</td><td>sum</td></tr>
<tr><td>row</td><td>sum</td><td>sum</td><td>sum</td><td>sum</td></tr>
<tr><td>row</td><td>sum</td><td>sum</td><td>sum</td><td>sum</td></tr>
</table>

> [!TIP]
> Columns that only have a few possible values are the best candidates for using in column **Values**.

## <a name="limitations"></a>Limitations

The analysis view currently has a limit of 100,000 rows. If you exceed this limit, you'll get a message telling you so. To work around this limitation, the set filters on the page before you switch to data analysis mode, if it's possible.  Maybe you want to analyse a certain group of customers or maybe you want data from the current year only. You can also choose a predefined view if it would work for your analysis.

## <a name="see-also"></a>See also

[Ad-hoc Data Analysis](reports-adhoc-analysis.md)  
[View and Edit in Excel](across-work-with-excel.md)  
