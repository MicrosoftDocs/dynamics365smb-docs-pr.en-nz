---
title: Sorting, Searching, and Filtering Lists | Microsoft Docs
description: Work efficiently in lists by searching across your data, sorting columns, and refining results using powerful filter symbols and keyboard shortcuts.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: delimit, FlowFilter, totals, limit, advanced
ms.date: 07/24/2020
ms.author: sgroespe
ms.openlocfilehash: 9bdaa604841156763739adf5411469c58a74eb1e
ms.sourcegitcommit: edad0d0b129e916c2cfdfa9c4f8d9d83513f4fd1
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 07/24/2020
ms.locfileid: "3619450"
---
# <a name="sorting-searching-and-filtering"></a><span data-ttu-id="c2941-103">Sorting, Searching, and Filtering</span><span class="sxs-lookup"><span data-stu-id="c2941-103">Sorting, Searching, and Filtering</span></span>

<span data-ttu-id="c2941-104">There are a few things that you can do that will help you scan, find, and limit records on a list or in a report or XMLport.</span><span class="sxs-lookup"><span data-stu-id="c2941-104">There are a few things that you can do that will help you scan, find, and limit records on a list or in a report or XMLport.</span></span> <span data-ttu-id="c2941-105">These include sorting, searching, and filtering.</span><span class="sxs-lookup"><span data-stu-id="c2941-105">These include sorting, searching, and filtering.</span></span> <span data-ttu-id="c2941-106">You can apply some or all of these simultaneously to quickly find or analyse your data.</span><span class="sxs-lookup"><span data-stu-id="c2941-106">You can apply some or all of these simultaneously to quickly find or analyze your data.</span></span>

<span data-ttu-id="c2941-107">For reports and XMLports, as on lists, you can set filters to delimit which data to include in the report or XMLport, but you cannot sort and search.</span><span class="sxs-lookup"><span data-stu-id="c2941-107">For reports and XMLports, as on lists, you can set filters to delimit which data to include in the report or XMLport, but you cannot sort and search.</span></span>

> [!TIP]
> <span data-ttu-id="c2941-108">When viewing your data as tiles, you can search and use basic filtering.</span><span class="sxs-lookup"><span data-stu-id="c2941-108">When viewing your data as tiles, you can search and use basic filtering.</span></span> <span data-ttu-id="c2941-109">To use the full set of powerful features for sorting, searching, and filtering, choose the ![Show as list](media/ui_show_as_list_icon.png "Show as list arrow left") icon to view the records as a list.</span><span class="sxs-lookup"><span data-stu-id="c2941-109">To use the full set of powerful features for sorting, searching, and filtering, choose the ![Show as list](media/ui_show_as_list_icon.png "Show as list arrow left") icon to view the records as a list.</span></span>

<!--
When you want to search for data, such as customer names, addresses, or product groups, you enter criteria. In search criteria, you can use all the numbers and letters that you normally use in the specific field. In addition, you can use special symbols to further filter the results. There are two ways to search: using the Quick Filter or column filters.
-->

## <a name="sorting"></a><span data-ttu-id="c2941-110">Sorting</span><span class="sxs-lookup"><span data-stu-id="c2941-110">Sorting</span></span>

<span data-ttu-id="c2941-111">Sorting makes it easy for you to get a quick overview of your data.</span><span class="sxs-lookup"><span data-stu-id="c2941-111">Sorting makes it easy for you to get a quick overview of your data.</span></span> <span data-ttu-id="c2941-112">If you have many customers, for example, you can choose to sort them by **Customer No.**, **Customer Posting Group**, **Currency Code**, **Country Region Code**, or **US Sales Tax Registration No.** to get the overview you need.</span><span class="sxs-lookup"><span data-stu-id="c2941-112">If you have many customers, for example, you can choose to sort them by **Customer No.**, **Customer Posting Group**, **Currency Code**, **Country Region Code**, or **Sales Tax Registration No.** to get the overview you need.</span></span>

<span data-ttu-id="c2941-113">To sort a list, you can either choose a column heading text to toggle between ascending and descending order, or choose the drop-down arrow in the column heading, and then choose the **Ascending** or **Descending** action.</span><span class="sxs-lookup"><span data-stu-id="c2941-113">To sort a list, you can either choose a column heading text to toggle between ascending and descending order, or choose the drop-down arrow in the column heading, and then choose the **Ascending** or **Descending** action.</span></span>  

> [!NOTE]  
> <span data-ttu-id="c2941-114">Sorting is not supported on images, BLOB fields, FlowFilters, and fields that do not belong to a table.</span><span class="sxs-lookup"><span data-stu-id="c2941-114">Sorting is not supported on images, BLOB fields, FlowFilters, and fields that do not belong to a table.</span></span>  

## <a name="searching"></a><span data-ttu-id="c2941-115">Searching</span><span class="sxs-lookup"><span data-stu-id="c2941-115">Searching</span></span>

<!--## Searching by using the Quick Filter -->
<span data-ttu-id="c2941-116">At the top of each list page, there is a ![Search list](media/ui-search/search-list.png "Search list icon") **Search** action that provides a quick and easy way to reduce the records in a list and display only those records that contain the data that you are interested in seeing.</span><span class="sxs-lookup"><span data-stu-id="c2941-116">At the top of each list page, there is a ![Search list](media/ui-search/search-list.png "Search list icon") **Search** action that provides a quick and easy way to reduce the records in a list and display only those records that contain the data that you are interested in seeing.</span></span>

<span data-ttu-id="c2941-117">To search, simply choose the **Search** action, and then in the box, type the text that you are looking for.</span><span class="sxs-lookup"><span data-stu-id="c2941-117">To search, simply choose the **Search** action, and then in the box, type the text that you are looking for.</span></span> <span data-ttu-id="c2941-118">You can enter letters, numbers, and other symbols.</span><span class="sxs-lookup"><span data-stu-id="c2941-118">You can enter letters, numbers, and other symbols.</span></span>

### <a name="fine-tuning-the-search"></a><span data-ttu-id="c2941-119">Fine-tuning the Search</span><span class="sxs-lookup"><span data-stu-id="c2941-119">Fine-tuning the Search</span></span>

<span data-ttu-id="c2941-120">In general, search will attempt to match text across all fields.</span><span class="sxs-lookup"><span data-stu-id="c2941-120">In general, search will attempt to match text across all fields.</span></span> <span data-ttu-id="c2941-121">It does not distinguish between uppercase and lowercase characters (case insensitive) and will match text placed anywhere in the field, at the beginning, end, or in the middle.</span><span class="sxs-lookup"><span data-stu-id="c2941-121">It does not distinguish between uppercase and lowercase characters (case insensitive) and will match text placed anywhere in the field, at the beginning, end, or in the middle.</span></span>

<span data-ttu-id="c2941-122">However, you can make a more exact search by using special characters.</span><span class="sxs-lookup"><span data-stu-id="c2941-122">However, you can make a more exact search by using special characters.</span></span>

- <span data-ttu-id="c2941-123">To find only field values that match the entire text and case exactly, place the search text between single quotes `''` (for example, `'man'`).</span><span class="sxs-lookup"><span data-stu-id="c2941-123">To find only field values that match the entire text and case exactly, place the search text between single quotes `''` (for example, `'man'`).</span></span>

- <span data-ttu-id="c2941-124">To find field values that start with a certain text and match the case, place `*` after the search text (for example `man*`).</span><span class="sxs-lookup"><span data-stu-id="c2941-124">To find field values that start with a certain text and match the case, place `*` after the search text (for example `man*`).</span></span>

- <span data-ttu-id="c2941-125">To find field values that end with a certain text and match the case, place `*` before the search text (for example `*man`).</span><span class="sxs-lookup"><span data-stu-id="c2941-125">To find field values that end with a certain text and match the case, place `*` before the search text (for example `*man`).</span></span>

- <span data-ttu-id="c2941-126">When using  `''` or `*`, the search is case sensitive.</span><span class="sxs-lookup"><span data-stu-id="c2941-126">When using  `''` or `*`, the search is case sensitive.</span></span> <span data-ttu-id="c2941-127">If you want to make the search case insensitive, place `@` before the search text (for example `@man*`).</span><span class="sxs-lookup"><span data-stu-id="c2941-127">If you want to make the search case insensitive, place `@` before the search text (for example `@man*`).</span></span>

<span data-ttu-id="c2941-128">The following table provides some examples to explain how you can use the search.</span><span class="sxs-lookup"><span data-stu-id="c2941-128">The following table provides some examples to explain how you can use the search.</span></span>

|<span data-ttu-id="c2941-129">Search Criteria</span><span class="sxs-lookup"><span data-stu-id="c2941-129">Search Criteria</span></span>|<span data-ttu-id="c2941-130">Finds...</span><span class="sxs-lookup"><span data-stu-id="c2941-130">Finds...</span></span>|
|---------------|----------|
|`man`<br /><span data-ttu-id="c2941-131">or</span><span class="sxs-lookup"><span data-stu-id="c2941-131">or</span></span> <br />`Man`|<span data-ttu-id="c2941-132">All records with fields that contain the text **man**, regardless of the case.</span><span class="sxs-lookup"><span data-stu-id="c2941-132">All records with fields that contain the text **man**, regardless of the case.</span></span> <span data-ttu-id="c2941-133">For example, **Manchester**, **manual**, or **Sportsman**.</span><span class="sxs-lookup"><span data-stu-id="c2941-133">For example, **Manchester**, **manual**, or **Sportsman**.</span></span> |
|`'Man'`|<span data-ttu-id="c2941-134">All records with fields that contain only **Man**, matching the case.</span><span class="sxs-lookup"><span data-stu-id="c2941-134">All records with fields that contain only **Man**, matching the case.</span></span>|
|`Man*`|<span data-ttu-id="c2941-135">All records with fields that start with the text <b>Man</b>, matching the case.</span><span class="sxs-lookup"><span data-stu-id="c2941-135">All records with fields that start with the text <b>Man</b>, matching the case.</span></span> <span data-ttu-id="c2941-136">For example, **Manchester** but not **manual** or **Sportsman**.</span><span class="sxs-lookup"><span data-stu-id="c2941-136">For example, **Manchester** but not **manual** or **Sportsman**.</span></span>|
|`@Man*`|<span data-ttu-id="c2941-137">All records with fields that start with **man**, regardless of the case.</span><span class="sxs-lookup"><span data-stu-id="c2941-137">All records with fields that start with **man**, regardless of the case.</span></span> <span data-ttu-id="c2941-138">For example, **Manchester** and **manual**, but not **Sportsman**.</span><span class="sxs-lookup"><span data-stu-id="c2941-138">For example, **Manchester** and **manual**, but not **Sportsman**.</span></span>|
|`@*man`|<span data-ttu-id="c2941-139">All records that end with **man**, regardless of the case.</span><span class="sxs-lookup"><span data-stu-id="c2941-139">All records that end with **man**, regardless of the case.</span></span> <span data-ttu-id="c2941-140">For example **Sportsman**, but not **Manchester** or **manual**.</span><span class="sxs-lookup"><span data-stu-id="c2941-140">For example **Sportsman**, but not **Manchester** or **manual**.</span></span>|

> [!TIP]
> <span data-ttu-id="c2941-141">You can press **F3** to activate and deactivate the search box.</span><span class="sxs-lookup"><span data-stu-id="c2941-141">You can press **F3** to activate and deactivate the search box.</span></span> <span data-ttu-id="c2941-142">For more information see [Keyboard Shortcuts](keyboard-shortcuts.md#KeyboardFilter).</span><span class="sxs-lookup"><span data-stu-id="c2941-142">For more information see [Keyboard Shortcuts](keyboard-shortcuts.md#KeyboardFilter).</span></span>

> [!NOTE]  
> <span data-ttu-id="c2941-143">Search will not match values in images, BLOB fields, FlowFilters, FlowFields, and other fields that are not part of a table.</span><span class="sxs-lookup"><span data-stu-id="c2941-143">Search will not match values in images, BLOB fields, FlowFilters, FlowFields, and other fields that are not part of a table.</span></span>

## <a name="filtering"></a><a name="filtering"></a><span data-ttu-id="c2941-144">Filtering</span><span class="sxs-lookup"><span data-stu-id="c2941-144">Filtering</span></span>

<span data-ttu-id="c2941-145">Filtering provides a more advanced and versatile way of controlling which records display on a list or include in a report or XMLport.</span><span class="sxs-lookup"><span data-stu-id="c2941-145">Filtering provides a more advanced and versatile way of controlling which records display on a list or include in a report or XMLport.</span></span> <span data-ttu-id="c2941-146">There are two major differences between searching and filtering, as described in the table below.</span><span class="sxs-lookup"><span data-stu-id="c2941-146">There are two major differences between searching and filtering, as described in the table below.</span></span>

|| <span data-ttu-id="c2941-147">**Searching**</span><span class="sxs-lookup"><span data-stu-id="c2941-147">**Searching**</span></span> | <span data-ttu-id="c2941-148">**Filtering**</span><span class="sxs-lookup"><span data-stu-id="c2941-148">**Filtering**</span></span> |
|--|----------|------------|
| <span data-ttu-id="c2941-149">**Applicable Fields**</span><span class="sxs-lookup"><span data-stu-id="c2941-149">**Applicable Fields**</span></span> | <span data-ttu-id="c2941-150">Searches across all fields that are visible on the page.</span><span class="sxs-lookup"><span data-stu-id="c2941-150">Searches across all fields that are visible on the page.</span></span> | <span data-ttu-id="c2941-151">Filters one or more fields individually, selecting from any field on the table, including fields that are not visible on the page.</span><span class="sxs-lookup"><span data-stu-id="c2941-151">Filters one or more fields individually, selecting from any field on the table, including fields that are not visible on the page.</span></span> |
| <span data-ttu-id="c2941-152">**Matching**</span><span class="sxs-lookup"><span data-stu-id="c2941-152">**Matching**</span></span> | <span data-ttu-id="c2941-153">Displays records with fields that match the search text, irrespective of casing or placement of that text.</span><span class="sxs-lookup"><span data-stu-id="c2941-153">Displays records with fields that match the search text, irrespective of casing or placement of that text.</span></span> | <span data-ttu-id="c2941-154">Displays records where the field matches the filter exactly and is case sensitive, unless special filter symbols are entered.</span><span class="sxs-lookup"><span data-stu-id="c2941-154">Displays records where the field matches the filter exactly and is case sensitive, unless special filter symbols are entered.</span></span>

<span data-ttu-id="c2941-155">Filtering enables you to display records for specific accounts or customers, dates, amounts, and other information by specifying filter criteria.</span><span class="sxs-lookup"><span data-stu-id="c2941-155">Filtering enables you to display records for specific accounts or customers, dates, amounts, and other information by specifying filter criteria.</span></span> <span data-ttu-id="c2941-156">Only records that match the criteria are displayed on the list or included in the report, batch job, or XMLport.</span><span class="sxs-lookup"><span data-stu-id="c2941-156">Only records that match the criteria are displayed on the list or included in the report, batch job, or XMLport.</span></span> <span data-ttu-id="c2941-157">If you specify criteria for multiple fields, then only records that match all criteria will be displayed.</span><span class="sxs-lookup"><span data-stu-id="c2941-157">If you specify criteria for multiple fields, then only records that match all criteria will be displayed.</span></span>

<span data-ttu-id="c2941-158">For lists, the filters are displayed on a filter pane that appears to the left of the list when you activate it.</span><span class="sxs-lookup"><span data-stu-id="c2941-158">For lists, the filters are displayed on a filter pane that appears to the left of the list when you activate it.</span></span> <span data-ttu-id="c2941-159">For reports, batch jobs, and XMLports, the filters are visible directly on the request page.</span><span class="sxs-lookup"><span data-stu-id="c2941-159">For reports, batch jobs, and XMLports, the filters are visible directly on the request page.</span></span>

### <a name="filtering-with-option-fields"></a><span data-ttu-id="c2941-160">Filtering with Option Fields</span><span class="sxs-lookup"><span data-stu-id="c2941-160">Filtering with Option Fields</span></span>

<span data-ttu-id="c2941-161">For "ordinary" fields that hold data, setup date or business data, you can set filters both by selecting data and by typing filter values, and you can use symbols to define advanced filter criteria.</span><span class="sxs-lookup"><span data-stu-id="c2941-161">For "ordinary" fields that hold data, setup date or business data, you can set filters both by selecting data and by typing filter values, and you can use symbols to define advanced filter criteria.</span></span> <span data-ttu-id="c2941-162">For more information, see [Entering Filter Criteria](ui-enter-criteria-filters.md#entering-filter-criteria).</span><span class="sxs-lookup"><span data-stu-id="c2941-162">For more information, see [Entering Filter Criteria](ui-enter-criteria-filters.md#entering-filter-criteria).</span></span>

<span data-ttu-id="c2941-163">For fields of type **Option**, however, you can only set a filter by selecting one or more options from a drop-down list of the available options.</span><span class="sxs-lookup"><span data-stu-id="c2941-163">For fields of type **Option**, however, you can only set a filter by selecting one or more options from a drop-down list of the available options.</span></span> <span data-ttu-id="c2941-164">An example of an option field is the **Status** field on the **Sales Orders** page.</span><span class="sxs-lookup"><span data-stu-id="c2941-164">An example of an option field is the **Status** field on the **Sales Orders** page.</span></span>

> [!NOTE]
> <span data-ttu-id="c2941-165">When you select multiple options as a filter value, the relationship between the options is defined as *OR*.</span><span class="sxs-lookup"><span data-stu-id="c2941-165">When you select multiple options as a filter value, the relationship between the options is defined as *OR*.</span></span> <span data-ttu-id="c2941-166">For example, if you select both the **Open** and the **Released** check box in the **Status** filter field on the **Sales Orders** page, it means that sales orders that are either open or released are displayed.</span><span class="sxs-lookup"><span data-stu-id="c2941-166">For example, if you select both the **Open** and the **Released** check box in the **Status** filter field on the **Sales Orders** page, it means that sales orders that are either open or released are displayed.</span></span>

### <a name="setting-filters-on-lists"></a><span data-ttu-id="c2941-167">Setting Filters on Lists</span><span class="sxs-lookup"><span data-stu-id="c2941-167">Setting Filters on Lists</span></span>

<span data-ttu-id="c2941-168">On lists, you set filters by using the filter pane.</span><span class="sxs-lookup"><span data-stu-id="c2941-168">On lists, you set filters by using the filter pane.</span></span> <span data-ttu-id="c2941-169">To display the filter pane for a list, choose the drop-down arrow next to the name of the page, and then choose the **Show filter pane** action.</span><span class="sxs-lookup"><span data-stu-id="c2941-169">To display the filter pane for a list, choose the drop-down arrow next to the name of the page, and then choose the **Show filter pane** action.</span></span> <span data-ttu-id="c2941-170">Alternatively, press **Shift+F3**.</span><span class="sxs-lookup"><span data-stu-id="c2941-170">Alternatively, press **Shift+F3**.</span></span>

<span data-ttu-id="c2941-171">To display the filter pane for a column on a list, choose the drop-down arrow, and then choose the **Filter** action.</span><span class="sxs-lookup"><span data-stu-id="c2941-171">To display the filter pane for a column on a list, choose the drop-down arrow, and then choose the **Filter** action.</span></span> <span data-ttu-id="c2941-172">Alternatively, press **Shift+F3**.</span><span class="sxs-lookup"><span data-stu-id="c2941-172">Alternatively, press **Shift+F3**.</span></span> <span data-ttu-id="c2941-173">The filter pane opens with the selected column shown as a filter field in the **Filter list by** section.</span><span class="sxs-lookup"><span data-stu-id="c2941-173">The filter pane opens with the selected column shown as a filter field in the **Filter list by** section.</span></span>

<span data-ttu-id="c2941-174">The filter pane displays the current filters for a list, and enables you to set your own custom filters on one or more fields by choosing the **+ Filter** action.</span><span class="sxs-lookup"><span data-stu-id="c2941-174">The filter pane displays the current filters for a list, and enables you to set your own custom filters on one or more fields by choosing the **+ Filter** action.</span></span>

 <span data-ttu-id="c2941-175">A filter pane is divided in three sections: **Views**, **Filter list by**, and **Filter totals by**:</span><span class="sxs-lookup"><span data-stu-id="c2941-175">A filter pane is divided in three sections: **Views**, **Filter list by**, and **Filter totals by**:</span></span>

- <span data-ttu-id="c2941-176">**Views**</span><span class="sxs-lookup"><span data-stu-id="c2941-176">**Views**</span></span>

  <span data-ttu-id="c2941-177">Some lists include the **Views** section.</span><span class="sxs-lookup"><span data-stu-id="c2941-177">Some lists include the **Views** section.</span></span> <span data-ttu-id="c2941-178">Views are variations of the list that have been preconfigured with filters.</span><span class="sxs-lookup"><span data-stu-id="c2941-178">Views are variations of the list that have been preconfigured with filters.</span></span> <span data-ttu-id="c2941-179">You can define and save as many views as you want per list, and the views will be available to you on any device you sign into.</span><span class="sxs-lookup"><span data-stu-id="c2941-179">You can define and save as many views as you want per list, and the views will be available to you on any device you sign into.</span></span> <span data-ttu-id="c2941-180">For more information, see [Save and Personalise List Views](ui-views.md).</span><span class="sxs-lookup"><span data-stu-id="c2941-180">For more information, see [Save and Personalize List Views](ui-views.md).</span></span>

- <span data-ttu-id="c2941-181">**Filter list by**</span><span class="sxs-lookup"><span data-stu-id="c2941-181">**Filter list by**</span></span>

  <span data-ttu-id="c2941-182">This is where you add filters on specific fields to reduce the number of displayed records.</span><span class="sxs-lookup"><span data-stu-id="c2941-182">This is where you add filters on specific fields to reduce the number of displayed records.</span></span> <span data-ttu-id="c2941-183">To add a filter, choose the **+ Filter** action, type the name of the field that you want to filter the list by, or pick a field from the drop-down list.</span><span class="sxs-lookup"><span data-stu-id="c2941-183">To add a filter, choose the **+ Filter** action, type the name of the field that you want to filter the list by, or pick a field from the drop-down list.</span></span>

- <span data-ttu-id="c2941-184">**Filter totals by**</span><span class="sxs-lookup"><span data-stu-id="c2941-184">**Filter totals by**</span></span>

  <span data-ttu-id="c2941-185">Some lists that display calculated fields, such as amounts and quantities, will include the **Filter totals by** section where you can adjust various dimensions that influence calculations.</span><span class="sxs-lookup"><span data-stu-id="c2941-185">Some lists that display calculated fields, such as amounts and quantities, will include the **Filter totals by** section where you can adjust various dimensions that influence calculations.</span></span> <span data-ttu-id="c2941-186">To add a filter, choose the **+ Filter** action, type the name of the field that you want to filter the list by, or pick a field from the drop-down list.</span><span class="sxs-lookup"><span data-stu-id="c2941-186">To add a filter, choose the **+ Filter** action, type the name of the field that you want to filter the list by, or pick a field from the drop-down list.</span></span>

  > [!NOTE]
  > <span data-ttu-id="c2941-187">Filters in the **Filter totals by** section are controlled by FlowFilters on the page design.</span><span class="sxs-lookup"><span data-stu-id="c2941-187">Filters in the **Filter totals by** section are controlled by FlowFilters on the page design.</span></span> <span data-ttu-id="c2941-188">For technical information, see [FlowFilters](/dynamics365/business-central/dev-itpro/developer/devenv-flowfilter-overview).</span><span class="sxs-lookup"><span data-stu-id="c2941-188">For technical information, see [FlowFilters](/dynamics365/business-central/dev-itpro/developer/devenv-flowfilter-overview).</span></span>

<span data-ttu-id="c2941-189">You can set a simple filter directly on a list within using the filter pane, namely a filter that displays only records with the same value as in the selected cell.</span><span class="sxs-lookup"><span data-stu-id="c2941-189">You can set a simple filter directly on a list within using the filter pane, namely a filter that displays only records with the same value as in the selected cell.</span></span> <span data-ttu-id="c2941-190">Select a cell on the list, choose the drop-down arrow, and then choose the **Filter to This Value** action.</span><span class="sxs-lookup"><span data-stu-id="c2941-190">Select a cell on the list, choose the drop-down arrow, and then choose the **Filter to This Value** action.</span></span> <span data-ttu-id="c2941-191">Alternatively, press **Alt+F3**.</span><span class="sxs-lookup"><span data-stu-id="c2941-191">Alternatively, press **Alt+F3**.</span></span>

### <a name="setting-filters-in-reports-batch-jobs-and-xmlports"></a><span data-ttu-id="c2941-192">Setting Filters in Reports, Batch Jobs, and XMLports</span><span class="sxs-lookup"><span data-stu-id="c2941-192">Setting Filters in Reports, Batch Jobs, and XMLports</span></span>

<span data-ttu-id="c2941-193">For reports and XMLports, the filters are visible directly on the request page.</span><span class="sxs-lookup"><span data-stu-id="c2941-193">For reports and XMLports, the filters are visible directly on the request page.</span></span> <span data-ttu-id="c2941-194">The request page displays the last used filters according to your selection in the **Use default values from** field.</span><span class="sxs-lookup"><span data-stu-id="c2941-194">The request page displays the last used filters according to your selection in the **Use default values from** field.</span></span> <span data-ttu-id="c2941-195">For more information, see [Using Saved Settings](ui-work-report.md#SavedSettings).</span><span class="sxs-lookup"><span data-stu-id="c2941-195">For more information, see [Using Saved Settings](ui-work-report.md#SavedSettings).</span></span>

<span data-ttu-id="c2941-196">The main **Filter** section shows the default filter fields that you use to delimit which records to include in the report or XMLport.</span><span class="sxs-lookup"><span data-stu-id="c2941-196">The main **Filter** section shows the default filter fields that you use to delimit which records to include in the report or XMLport.</span></span> <span data-ttu-id="c2941-197">To add a filter, choose the **+ Filter** action, type the name of the field that you want to filter by, or pick a field from the drop-down list.</span><span class="sxs-lookup"><span data-stu-id="c2941-197">To add a filter, choose the **+ Filter** action, type the name of the field that you want to filter by, or pick a field from the drop-down list.</span></span>

<span data-ttu-id="c2941-198">In the **Filter totals by** section, you can adjust various dimensions that influence calculations in the report or XMLport.</span><span class="sxs-lookup"><span data-stu-id="c2941-198">In the **Filter totals by** section, you can adjust various dimensions that influence calculations in the report or XMLport.</span></span> <span data-ttu-id="c2941-199">To add a filter, choose the **+ Filter** action, type the name of the field that you want to filter by, or pick a field from the drop-down list.</span><span class="sxs-lookup"><span data-stu-id="c2941-199">To add a filter, choose the **+ Filter** action, type the name of the field that you want to filter by, or pick a field from the drop-down list.</span></span>

## <a name="entering-filter-criteria"></a><span data-ttu-id="c2941-200">Entering Filter Criteria</span><span class="sxs-lookup"><span data-stu-id="c2941-200">Entering Filter Criteria</span></span>

<span data-ttu-id="c2941-201">Both in the filter pane and on a request page, you enter your filter criteria in the box under the filter field.</span><span class="sxs-lookup"><span data-stu-id="c2941-201">Both in the filter pane and on a request page, you enter your filter criteria in the box under the filter field.</span></span>

<span data-ttu-id="c2941-202">The type of the filter field determines which criteria you can enter.</span><span class="sxs-lookup"><span data-stu-id="c2941-202">The type of the filter field determines which criteria you can enter.</span></span> <span data-ttu-id="c2941-203">For example, filtering a field that has fixed values will only let you choose from those values.</span><span class="sxs-lookup"><span data-stu-id="c2941-203">For example, filtering a field that has fixed values will only let you choose from those values.</span></span> <span data-ttu-id="c2941-204">For more information about special filter symbols, see [Filter criteria](#FilterCriteria) and [Filter tokens](#FilterTokens).</span><span class="sxs-lookup"><span data-stu-id="c2941-204">For more information about special filter symbols, see [Filter criteria](#FilterCriteria) and [Filter tokens](#FilterTokens).</span></span>

<span data-ttu-id="c2941-205">Columns that already have filters are indicated by the ![Filter icon](media/ui-search/filter-icon.png "Filter icon") icon in the column heading.</span><span class="sxs-lookup"><span data-stu-id="c2941-205">Columns that already have filters are indicated by the ![Filter icon](media/ui-search/filter-icon.png "Filter icon") icon in the column heading.</span></span> <span data-ttu-id="c2941-206">To remove a filter, choose the drop-down arrow, and then choose the **Clear Filter** action.</span><span class="sxs-lookup"><span data-stu-id="c2941-206">To remove a filter, choose the drop-down arrow, and then choose the **Clear Filter** action.</span></span>

> [!TIP]
> <span data-ttu-id="c2941-207">Accelerate finding and analysing your data by using combinations of keyboard shortcuts.</span><span class="sxs-lookup"><span data-stu-id="c2941-207">Accelerate finding and analyzing your data by using combinations of keyboard shortcuts.</span></span> <span data-ttu-id="c2941-208">For example, select a field, use **Shift+Alt+F3** to add that field to the filter pane, type the filter criteria, use **Ctrl+Enter** to return to the rows, select another field, and use **Alt+F3** to filter to that value.</span><span class="sxs-lookup"><span data-stu-id="c2941-208">For example, select a field, use **Shift+Alt+F3** to add that field to the filter pane, type the filter criteria, use **Ctrl+Enter** to return to the rows, select another field, and use **Alt+F3** to filter to that value.</span></span> <span data-ttu-id="c2941-209">For more information see [Keyboard Shortcuts](keyboard-shortcuts.md#KeyboardFilter).</span><span class="sxs-lookup"><span data-stu-id="c2941-209">For more information see [Keyboard Shortcuts](keyboard-shortcuts.md#KeyboardFilter).</span></span>

### <a name="filter-criteria-and-symbols"></a><span data-ttu-id="c2941-210"><a name="FilterCriteria"> </a>Filter Criteria and Symbols</span><span class="sxs-lookup"><span data-stu-id="c2941-210"><a name="FilterCriteria"> </a>Filter Criteria and Symbols</span></span>

<span data-ttu-id="c2941-211">When you enter criteria, you can use all the numbers and letters that you can normally use in the field.</span><span class="sxs-lookup"><span data-stu-id="c2941-211">When you enter criteria, you can use all the numbers and letters that you can normally use in the field.</span></span> <span data-ttu-id="c2941-212">In addition, you can use special symbols (or operators) to further filter the results.</span><span class="sxs-lookup"><span data-stu-id="c2941-212">In addition, you can use special symbols (or operators) to further filter the results.</span></span> <span data-ttu-id="c2941-213">The following tables show the symbols that can be used in filters.</span><span class="sxs-lookup"><span data-stu-id="c2941-213">The following tables show the symbols that can be used in filters.</span></span> <span data-ttu-id="c2941-214">For dates and times, you can also refer to [Working with Calendar Dates and Times](ui-enter-date-ranges.md) for more detailed information.</span><span class="sxs-lookup"><span data-stu-id="c2941-214">For dates and times, you can also refer to [Working with Calendar Dates and Times](ui-enter-date-ranges.md) for more detailed information.</span></span>

> [!IMPORTANT]  
> <span data-ttu-id="c2941-215">There may be instances where field values contain these symbols and you want to filter on them.</span><span class="sxs-lookup"><span data-stu-id="c2941-215">There may be instances where field values contain these symbols and you want to filter on them.</span></span> <span data-ttu-id="c2941-216">To do this, you must include the filter expression that contains the symbol in quotation marks ('').</span><span class="sxs-lookup"><span data-stu-id="c2941-216">To do this, you must include the filter expression that contains the symbol in quotation marks ('').</span></span> <span data-ttu-id="c2941-217">For example, if you want to filter on records that start with the text *S&R*, the filter expression is `'S&R*'`.</span><span class="sxs-lookup"><span data-stu-id="c2941-217">For example, if you want to filter on records that start with the text *S&R*, the filter expression is `'S&R*'`.</span></span>

<span data-ttu-id="c2941-218">The following sections describe how to use the different operators.</span><span class="sxs-lookup"><span data-stu-id="c2941-218">The following sections describe how to use the different operators.</span></span>

> [!NOTE]
> <span data-ttu-id="c2941-219">If there are more than 200 operators in a single filter, the system will automatically group some expressions in parentheses `()` for the purpose of processing.</span><span class="sxs-lookup"><span data-stu-id="c2941-219">If there are more than 200 operators in a single filter, the system will automatically group some expressions in parentheses `()` for the purpose of processing.</span></span> <span data-ttu-id="c2941-220">This has no effect on the filter or the results.</span><span class="sxs-lookup"><span data-stu-id="c2941-220">This has no effect on the filter or the results.</span></span>  

#### <a name="-interval"></a><span data-ttu-id="c2941-221">(..) Interval</span><span class="sxs-lookup"><span data-stu-id="c2941-221">(..) Interval</span></span>

|<span data-ttu-id="c2941-222">Sample Expression</span><span class="sxs-lookup"><span data-stu-id="c2941-222">Sample Expression</span></span>|<span data-ttu-id="c2941-223">Records Displayed</span><span class="sxs-lookup"><span data-stu-id="c2941-223">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`1100..2100`|<span data-ttu-id="c2941-224">Numbers 1100 through 2100</span><span class="sxs-lookup"><span data-stu-id="c2941-224">Numbers 1100 through 2100</span></span>|  
|`..2500`|<span data-ttu-id="c2941-225">Up to and including 2500</span><span class="sxs-lookup"><span data-stu-id="c2941-225">Up to and including 2500</span></span>|  
|`..12 31 00`|<span data-ttu-id="c2941-226">Dates up to and including 12 31 00</span><span class="sxs-lookup"><span data-stu-id="c2941-226">Dates up to and including 12 31 00</span></span>|  
|`P8..`|<span data-ttu-id="c2941-227">Information for accounting period 8 and thereafter</span><span class="sxs-lookup"><span data-stu-id="c2941-227">Information for accounting period 8 and thereafter</span></span>|  
|`..23`|<span data-ttu-id="c2941-228">From the beginning date until 23-current month-current year 23:59:59</span><span class="sxs-lookup"><span data-stu-id="c2941-228">From the beginning date until 23-current month-current year 23:59:59</span></span>|  
|`23..`|<span data-ttu-id="c2941-229">From 23-current month-current year 0:00:00 until the end of time</span><span class="sxs-lookup"><span data-stu-id="c2941-229">From 23-current month-current year 0:00:00 until the end of time</span></span>|  
|`22..23`|<span data-ttu-id="c2941-230">From 22-current month-current year 0:00:00 until 23-current month-current year 23:59:59</span><span class="sxs-lookup"><span data-stu-id="c2941-230">From 22-current month-current year 0:00:00 until 23-current month-current year 23:59:59</span></span>|  

#### <a name="124-eitheror"></a><span data-ttu-id="c2941-231">(&#124;) Either/or</span><span class="sxs-lookup"><span data-stu-id="c2941-231">(&#124;) Either/or</span></span>

|<span data-ttu-id="c2941-232">Sample Expression</span><span class="sxs-lookup"><span data-stu-id="c2941-232">Sample Expression</span></span>|<span data-ttu-id="c2941-233">Records Displayed</span><span class="sxs-lookup"><span data-stu-id="c2941-233">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`1200|1300`|<span data-ttu-id="c2941-234">Numbers with 1200 or 1300</span><span class="sxs-lookup"><span data-stu-id="c2941-234">Numbers with 1200 or 1300</span></span>|  

#### <a name="-not-equal-to"></a><span data-ttu-id="c2941-235">(<>) Not equal to</span><span class="sxs-lookup"><span data-stu-id="c2941-235">(<>) Not equal to</span></span>  

|<span data-ttu-id="c2941-236">Sample Expression</span><span class="sxs-lookup"><span data-stu-id="c2941-236">Sample Expression</span></span>|<span data-ttu-id="c2941-237">Records Displayed</span><span class="sxs-lookup"><span data-stu-id="c2941-237">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`<>0`|<span data-ttu-id="c2941-238">All numbers except 0</span><span class="sxs-lookup"><span data-stu-id="c2941-238">All numbers except 0</span></span><br /><br /> <span data-ttu-id="c2941-239">The SQL Server Option allows you to combine this symbol with a wild card expression.</span><span class="sxs-lookup"><span data-stu-id="c2941-239">The SQL Server Option allows you to combine this symbol with a wild card expression.</span></span> <span data-ttu-id="c2941-240">For example, <>A\* meaning not equal to any text that starts with A.</span><span class="sxs-lookup"><span data-stu-id="c2941-240">For example, <>A\* meaning not equal to any text that starts with A.</span></span>|  

#### <a name="-greater-than"></a><span data-ttu-id="c2941-241">(>) Greater than</span><span class="sxs-lookup"><span data-stu-id="c2941-241">(>) Greater than</span></span>  

|<span data-ttu-id="c2941-242">Sample Expression</span><span class="sxs-lookup"><span data-stu-id="c2941-242">Sample Expression</span></span>|<span data-ttu-id="c2941-243">Records Displayed</span><span class="sxs-lookup"><span data-stu-id="c2941-243">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`>1200`|<span data-ttu-id="c2941-244">Numbers greater than 1200</span><span class="sxs-lookup"><span data-stu-id="c2941-244">Numbers greater than 1200</span></span>|  

#### <a name="-greater-than-or-equal-to"></a><span data-ttu-id="c2941-245">(>=) Greater than or equal to</span><span class="sxs-lookup"><span data-stu-id="c2941-245">(>=) Greater than or equal to</span></span>  

|<span data-ttu-id="c2941-246">Sample Expression</span><span class="sxs-lookup"><span data-stu-id="c2941-246">Sample Expression</span></span>|<span data-ttu-id="c2941-247">Records Displayed</span><span class="sxs-lookup"><span data-stu-id="c2941-247">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`>=1200`|<span data-ttu-id="c2941-248">Numbers greater than or equal to 1200</span><span class="sxs-lookup"><span data-stu-id="c2941-248">Numbers greater than or equal to 1200</span></span>|  

#### <a name="-less-than"></a><span data-ttu-id="c2941-249">(<) Less than</span><span class="sxs-lookup"><span data-stu-id="c2941-249">(<) Less than</span></span>  

|<span data-ttu-id="c2941-250">Sample Expression</span><span class="sxs-lookup"><span data-stu-id="c2941-250">Sample Expression</span></span>|<span data-ttu-id="c2941-251">Records Displayed</span><span class="sxs-lookup"><span data-stu-id="c2941-251">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`<1200`|<span data-ttu-id="c2941-252">Numbers less than 1200</span><span class="sxs-lookup"><span data-stu-id="c2941-252">Numbers less than 1200</span></span>|  

#### <a name="-less-than-or-equal-to"></a><span data-ttu-id="c2941-253">(<=) Less than or equal to</span><span class="sxs-lookup"><span data-stu-id="c2941-253">(<=) Less than or equal to</span></span>  

|<span data-ttu-id="c2941-254">Sample Expression</span><span class="sxs-lookup"><span data-stu-id="c2941-254">Sample Expression</span></span>|<span data-ttu-id="c2941-255">Records Displayed</span><span class="sxs-lookup"><span data-stu-id="c2941-255">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`<=1200`|<span data-ttu-id="c2941-256">Numbers less than or equal to 1200</span><span class="sxs-lookup"><span data-stu-id="c2941-256">Numbers less than or equal to 1200</span></span>|  

#### <a name="-and"></a><span data-ttu-id="c2941-257">(&) And</span><span class="sxs-lookup"><span data-stu-id="c2941-257">(&) And</span></span>  

|<span data-ttu-id="c2941-258">Sample Expression</span><span class="sxs-lookup"><span data-stu-id="c2941-258">Sample Expression</span></span>|<span data-ttu-id="c2941-259">Records Displayed</span><span class="sxs-lookup"><span data-stu-id="c2941-259">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`>200&<1200`|<span data-ttu-id="c2941-260">Numbers greater than 200 and less than 1200</span><span class="sxs-lookup"><span data-stu-id="c2941-260">Numbers greater than 200 and less than 1200</span></span>|  

#### <a name="-an-exact-character-match"></a><span data-ttu-id="c2941-261">('') An exact character match</span><span class="sxs-lookup"><span data-stu-id="c2941-261">('') An exact character match</span></span>  

|<span data-ttu-id="c2941-262">Sample Expression</span><span class="sxs-lookup"><span data-stu-id="c2941-262">Sample Expression</span></span>|<span data-ttu-id="c2941-263">Records Displayed</span><span class="sxs-lookup"><span data-stu-id="c2941-263">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`'man'`|<span data-ttu-id="c2941-264">Text that matches man exactly and is case sensitive.</span><span class="sxs-lookup"><span data-stu-id="c2941-264">Text that matches man exactly and is case sensitive.</span></span>|  

#### <a name="-case-insensitive"></a><span data-ttu-id="c2941-265">(@) Case insensitive</span><span class="sxs-lookup"><span data-stu-id="c2941-265">(@) Case insensitive</span></span>  

|<span data-ttu-id="c2941-266">Sample Expression</span><span class="sxs-lookup"><span data-stu-id="c2941-266">Sample Expression</span></span>|<span data-ttu-id="c2941-267">Records Displayed</span><span class="sxs-lookup"><span data-stu-id="c2941-267">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`@man*`|<span data-ttu-id="c2941-268">Text that starts with man and is case insensitive.</span><span class="sxs-lookup"><span data-stu-id="c2941-268">Text that starts with man and is case insensitive.</span></span>|  

#### <a name="-an-indefinite-number-of-unknown-characters"></a><span data-ttu-id="c2941-269">(\*) An indefinite number of unknown characters</span><span class="sxs-lookup"><span data-stu-id="c2941-269">(\*) An indefinite number of unknown characters</span></span>

|<span data-ttu-id="c2941-270">Sample Expression</span><span class="sxs-lookup"><span data-stu-id="c2941-270">Sample Expression</span></span>|<span data-ttu-id="c2941-271">Records Displayed</span><span class="sxs-lookup"><span data-stu-id="c2941-271">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`*Co*`|<span data-ttu-id="c2941-272">Text that contains "Co" and is case sensitive.</span><span class="sxs-lookup"><span data-stu-id="c2941-272">Text that contains "Co" and is case sensitive.</span></span>|  
|`*Co`|<span data-ttu-id="c2941-273">Text that ends with "Co" and is case sensitive.</span><span class="sxs-lookup"><span data-stu-id="c2941-273">Text that ends with "Co" and is case sensitive.</span></span>|  
|`Co*`|<span data-ttu-id="c2941-274">Text that begins with "Co" and is case sensitive.</span><span class="sxs-lookup"><span data-stu-id="c2941-274">Text that begins with "Co" and is case sensitive.</span></span>|  

#### <a name="-one-unknown-character"></a><span data-ttu-id="c2941-275">(?) One unknown character</span><span class="sxs-lookup"><span data-stu-id="c2941-275">(?) One unknown character</span></span>  

|<span data-ttu-id="c2941-276">Sample Expression</span><span class="sxs-lookup"><span data-stu-id="c2941-276">Sample Expression</span></span>|<span data-ttu-id="c2941-277">Records Displayed</span><span class="sxs-lookup"><span data-stu-id="c2941-277">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`Hans?n`|<span data-ttu-id="c2941-278">Text such as Hansen or Hanson</span><span class="sxs-lookup"><span data-stu-id="c2941-278">Text such as Hansen or Hanson</span></span>|  

#### <a name="combined-format-expressions"></a><span data-ttu-id="c2941-279">Combined Format Expressions</span><span class="sxs-lookup"><span data-stu-id="c2941-279">Combined Format Expressions</span></span>  

|<span data-ttu-id="c2941-280">Sample Expression</span><span class="sxs-lookup"><span data-stu-id="c2941-280">Sample Expression</span></span>|<span data-ttu-id="c2941-281">Records Displayed</span><span class="sxs-lookup"><span data-stu-id="c2941-281">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`5999|8100..8490`|<span data-ttu-id="c2941-282">Include any records with the number 5999 or a number from the interval 8100 through 8490.</span><span class="sxs-lookup"><span data-stu-id="c2941-282">Include any records with the number 5999 or a number from the interval 8100 through 8490.</span></span>|  
|`..1299|1400..`|<span data-ttu-id="c2941-283">Include records with a number less than or equal to 1299 or a number equal to 1400 or greater (all numbers except 1300 through 1399).</span><span class="sxs-lookup"><span data-stu-id="c2941-283">Include records with a number less than or equal to 1299 or a number equal to 1400 or greater (all numbers except 1300 through 1399).</span></span>|  
|`>50&<100`|<span data-ttu-id="c2941-284">Include records with numbers that are greater than 50 and less than 100 (numbers 51 through 99).</span><span class="sxs-lookup"><span data-stu-id="c2941-284">Include records with numbers that are greater than 50 and less than 100 (numbers 51 through 99).</span></span>|  

### <a name="filter-tokens"></a><span data-ttu-id="c2941-285"><a name="FilterTokens"> </a>Filter Tokens</span><span class="sxs-lookup"><span data-stu-id="c2941-285"><a name="FilterTokens"> </a>Filter Tokens</span></span>
<span data-ttu-id="c2941-286">When entering filter criteria, you can also type words that have special meaning, called filter tokens.</span><span class="sxs-lookup"><span data-stu-id="c2941-286">When entering filter criteria, you can also type words that have special meaning, called filter tokens.</span></span> <span data-ttu-id="c2941-287">After entering the token word, the word is replaced by the value or values that it represents.</span><span class="sxs-lookup"><span data-stu-id="c2941-287">After entering the token word, the word is replaced by the value or values that it represents.</span></span> <span data-ttu-id="c2941-288">This makes filtering easier by reducing the need to navigate to other pages to look up values you want to add to your filter.</span><span class="sxs-lookup"><span data-stu-id="c2941-288">This makes filtering easier by reducing the need to navigate to other pages to look up values you want to add to your filter.</span></span> <span data-ttu-id="c2941-289">The tables below describe some of the tokens you can type as filter criteria.</span><span class="sxs-lookup"><span data-stu-id="c2941-289">The tables below describe some of the tokens you can type as filter criteria.</span></span>

> [!TIP]
> <span data-ttu-id="c2941-290">Your organisation may use custom tokens.</span><span class="sxs-lookup"><span data-stu-id="c2941-290">Your organization may use custom tokens.</span></span> <span data-ttu-id="c2941-291">To learn about the complete set of tokens available to you or to add more custom tokens, talk to your administrator.</span><span class="sxs-lookup"><span data-stu-id="c2941-291">To learn about the complete set of tokens available to you or to add more custom tokens, talk to your administrator.</span></span> <span data-ttu-id="c2941-292">For technical information see [Adding Filter Tokens](/dynamics365/business-central/dev-itpro/developer/devenv-adding-filter-tokens).</span><span class="sxs-lookup"><span data-stu-id="c2941-292">For technical information see [Adding Filter Tokens](/dynamics365/business-central/dev-itpro/developer/devenv-adding-filter-tokens).</span></span>

#### <a name="me-or-userid-records-assigned-to-you"></a><span data-ttu-id="c2941-293">(%me or %userid) Records Assigned to You</span><span class="sxs-lookup"><span data-stu-id="c2941-293">(%me or %userid) Records Assigned to You</span></span>

<span data-ttu-id="c2941-294">Use `%me` or `%userid` when filtering fields that contain the user ID, such as **Assigned to User ID** field, to display all records that are assigned to you.</span><span class="sxs-lookup"><span data-stu-id="c2941-294">Use `%me` or `%userid` when filtering fields that contain the user ID, such as **Assigned to User ID** field, to display all records that are assigned to you.</span></span>

|<span data-ttu-id="c2941-295">Sample Expression</span><span class="sxs-lookup"><span data-stu-id="c2941-295">Sample Expression</span></span>|<span data-ttu-id="c2941-296">Records Displayed</span><span class="sxs-lookup"><span data-stu-id="c2941-296">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`%me`<br /><span data-ttu-id="c2941-297">or</span><span class="sxs-lookup"><span data-stu-id="c2941-297">or</span></span><br />`%userid`|<span data-ttu-id="c2941-298">Records that are assigned to your user account.</span><span class="sxs-lookup"><span data-stu-id="c2941-298">Records that are assigned to your user account.</span></span> |  

#### <a name="mycustomers-customers-in-my-customers"></a><span data-ttu-id="c2941-299">(%mycustomers) Customers in My Customers</span><span class="sxs-lookup"><span data-stu-id="c2941-299">(%mycustomers) Customers in My Customers</span></span>

<span data-ttu-id="c2941-300">Use `%mycustomers` in the customer **No** field to display all records for customers that are included in the **My Customers** list on your Role Centre.</span><span class="sxs-lookup"><span data-stu-id="c2941-300">Use `%mycustomers` in the customer **No** field to display all records for customers that are included in the **My Customers** list on your Role Center.</span></span>

|<span data-ttu-id="c2941-301">Sample Expression</span><span class="sxs-lookup"><span data-stu-id="c2941-301">Sample Expression</span></span>|<span data-ttu-id="c2941-302">Records Displayed</span><span class="sxs-lookup"><span data-stu-id="c2941-302">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`%mycustomers`|<span data-ttu-id="c2941-303">Customers in the **My Customers** on your Role Centre.</span><span class="sxs-lookup"><span data-stu-id="c2941-303">Customers in the **My Customers** on your Role Center.</span></span> |  

#### <a name="myitems-items-in-my-items"></a><span data-ttu-id="c2941-304">(%myitems) Items in My Items</span><span class="sxs-lookup"><span data-stu-id="c2941-304">(%myitems) Items in My Items</span></span>

<span data-ttu-id="c2941-305">Use `%myitems` in the item **No** field to display all records for items that are included in the **My Items** list on your Role Centre.</span><span class="sxs-lookup"><span data-stu-id="c2941-305">Use `%myitems` in the item **No** field to display all records for items that are included in the **My Items** list on your Role Center.</span></span>

|<span data-ttu-id="c2941-306">Sample Expression</span><span class="sxs-lookup"><span data-stu-id="c2941-306">Sample Expression</span></span>|<span data-ttu-id="c2941-307">Records Displayed</span><span class="sxs-lookup"><span data-stu-id="c2941-307">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`%myitems`|<span data-ttu-id="c2941-308">Items in the **My Items** on your Role Centre.</span><span class="sxs-lookup"><span data-stu-id="c2941-308">Items in the **My Items** on your Role Center.</span></span> |  

#### <a name="myvendors-vendors-in-my-vendors"></a><span data-ttu-id="c2941-309">(%myvendors) Vendors in My Vendors</span><span class="sxs-lookup"><span data-stu-id="c2941-309">(%myvendors) Vendors in My Vendors</span></span>

<span data-ttu-id="c2941-310">Use `%myvendors` in the vendor **No** field to display all records for vendors that are included in the **My Vendors** list on your Role Centre.</span><span class="sxs-lookup"><span data-stu-id="c2941-310">Use `%myvendors` in the vendor **No** field to display all records for vendors that are included in the **My Vendors** list on your Role Center.</span></span>

|<span data-ttu-id="c2941-311">Sample Expression</span><span class="sxs-lookup"><span data-stu-id="c2941-311">Sample Expression</span></span>|<span data-ttu-id="c2941-312">Records Displayed</span><span class="sxs-lookup"><span data-stu-id="c2941-312">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`%myvendors`|<span data-ttu-id="c2941-313">Vendors in the **My Vendors** on your Role Centre.</span><span class="sxs-lookup"><span data-stu-id="c2941-313">Vendors in the **My Vendors** on your Role Center.</span></span> |  

## <a name="see-also"></a><span data-ttu-id="c2941-314">See Also</span><span class="sxs-lookup"><span data-stu-id="c2941-314">See Also</span></span>

[<span data-ttu-id="c2941-315">Searching and Filtering FAQ</span><span class="sxs-lookup"><span data-stu-id="c2941-315">Searching and Filtering FAQ</span></span>](ui-search-filter-faq.md)  
[<span data-ttu-id="c2941-316">Save and Personalise List Views</span><span class="sxs-lookup"><span data-stu-id="c2941-316">Save and Personalize List Views</span></span>](ui-views.md)  
<span data-ttu-id="c2941-317">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="c2941-317">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
