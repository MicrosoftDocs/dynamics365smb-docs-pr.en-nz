---
title: Sorting, Searching, and Filtering Lists | Microsoft Docs
description: Work efficiently in lists by searching across your data, sorting columns, and refining results using filter symbols and keyboard shortcuts.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: delimit, FlowFilter, totals, limit, advanced
ms.date: 04/01/2021
ms.author: jswymer
ms.openlocfilehash: a27556350851de61bd31504d0c29ef60df6d890a
ms.sourcegitcommit: 921f0c4043dcda2fb8fc35df1b64310bf32270d7
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 05/11/2021
ms.locfileid: "6017190"
---
# <a name="sorting-searching-and-filtering"></a><span data-ttu-id="bf200-103">Sorting, Searching, and Filtering</span><span class="sxs-lookup"><span data-stu-id="bf200-103">Sorting, Searching, and Filtering</span></span>

<span data-ttu-id="bf200-104">There are a few things that you can do that will help you scan, find, and limit records on a list or in a report or XMLport.</span><span class="sxs-lookup"><span data-stu-id="bf200-104">There are a few things that you can do that will help you scan, find, and limit records on a list or in a report or XMLport.</span></span> <span data-ttu-id="bf200-105">These include sorting, searching, and filtering.</span><span class="sxs-lookup"><span data-stu-id="bf200-105">These include sorting, searching, and filtering.</span></span> <span data-ttu-id="bf200-106">You can apply some or all of these simultaneously to quickly find or analyse your data.</span><span class="sxs-lookup"><span data-stu-id="bf200-106">You can apply some or all of these simultaneously to quickly find or analyze your data.</span></span>

<span data-ttu-id="bf200-107">For reports and XMLports, as on lists, you can set filters to delimit which data to include in the report or XMLport, but you can't sort and search.</span><span class="sxs-lookup"><span data-stu-id="bf200-107">For reports and XMLports, as on lists, you can set filters to delimit which data to include in the report or XMLport, but you can't sort and search.</span></span>

> [!TIP]
> <span data-ttu-id="bf200-108">When viewing your data as tiles, you can search and use filtering.</span><span class="sxs-lookup"><span data-stu-id="bf200-108">When viewing your data as tiles, you can search and use filtering.</span></span> <span data-ttu-id="bf200-109">To use the full set of powerful features for sorting, searching, and filtering, choose the ![Show as list](media/ui_show_as_list_icon.png "Show as list arrow left") icon to view the records as a list.</span><span class="sxs-lookup"><span data-stu-id="bf200-109">To use the full set of powerful features for sorting, searching, and filtering, choose the ![Show as list](media/ui_show_as_list_icon.png "Show as list arrow left") icon to view the records as a list.</span></span>

<!--
When you want to search for data, such as customer names, addresses, or product groups, you enter criteria. In search criteria, you can use all the numbers and letters that you normally use in the specific field. In addition, you can use special symbols to further filter the results. There are two ways to search: using the Quick Filter or column filters.
-->

## <a name="sorting"></a><span data-ttu-id="bf200-110">Sorting</span><span class="sxs-lookup"><span data-stu-id="bf200-110">Sorting</span></span>

<span data-ttu-id="bf200-111">Sorting makes it easy for you to get a quick overview of your data.</span><span class="sxs-lookup"><span data-stu-id="bf200-111">Sorting makes it easy for you to get a quick overview of your data.</span></span> <span data-ttu-id="bf200-112">For example, if you have many customers,  you could sort them by **Customer No.**, **Currency Code**, or **Country Region Code** to get the overview you need.</span><span class="sxs-lookup"><span data-stu-id="bf200-112">For example, if you have many customers,  you could sort them by **Customer No.**, **Currency Code**, or **Country Region Code** to get the overview you need.</span></span>

<span data-ttu-id="bf200-113">To sort a list, you can either:</span><span class="sxs-lookup"><span data-stu-id="bf200-113">To sort a list, you can either:</span></span>

- <span data-ttu-id="bf200-114">Choose a column heading text to toggle between ascending and descending order, or</span><span class="sxs-lookup"><span data-stu-id="bf200-114">Choose a column heading text to toggle between ascending and descending order, or</span></span>
- <span data-ttu-id="bf200-115">Choose the drop-down arrow in the column heading, then choose the **Ascending** or **Descending** action.</span><span class="sxs-lookup"><span data-stu-id="bf200-115">Choose the drop-down arrow in the column heading, then choose the **Ascending** or **Descending** action.</span></span>  

> [!NOTE]  
> <span data-ttu-id="bf200-116">Sorting isn't supported on images, BLOB fields, FlowFilters, and fields that do not belong to a table.</span><span class="sxs-lookup"><span data-stu-id="bf200-116">Sorting isn't supported on images, BLOB fields, FlowFilters, and fields that do not belong to a table.</span></span>  

## <a name="searching"></a><span data-ttu-id="bf200-117">Searching</span><span class="sxs-lookup"><span data-stu-id="bf200-117">Searching</span></span>

<!--## Searching by using the Quick Filter -->
<span data-ttu-id="bf200-118">At the top of each list page, there's a ![Search list](media/ui-search/search-list.png "Search list icon") **Search** action that provides a quick and easy way to reduce the records in a list and display only those records that contain the data that you're interested in seeing.</span><span class="sxs-lookup"><span data-stu-id="bf200-118">At the top of each list page, there's a ![Search list](media/ui-search/search-list.png "Search list icon") **Search** action that provides a quick and easy way to reduce the records in a list and display only those records that contain the data that you're interested in seeing.</span></span>

<span data-ttu-id="bf200-119">To search, just choose the **Search** action, and then in the box, type the text that you're looking for.</span><span class="sxs-lookup"><span data-stu-id="bf200-119">To search, just choose the **Search** action, and then in the box, type the text that you're looking for.</span></span> <span data-ttu-id="bf200-120">You can enter letters, numbers, and other symbols.</span><span class="sxs-lookup"><span data-stu-id="bf200-120">You can enter letters, numbers, and other symbols.</span></span>

<span data-ttu-id="bf200-121">In general, search will attempt to match text across all fields.</span><span class="sxs-lookup"><span data-stu-id="bf200-121">In general, search will attempt to match text across all fields.</span></span> <span data-ttu-id="bf200-122">It doesn't distinguish between uppercase and lowercase characters (case insensitive) and will match text placed anywhere in the field, at the beginning, end, or in the middle.</span><span class="sxs-lookup"><span data-stu-id="bf200-122">It doesn't distinguish between uppercase and lowercase characters (case insensitive) and will match text placed anywhere in the field, at the beginning, end, or in the middle.</span></span>

> [!TIP]
> <span data-ttu-id="bf200-123">You can press **F3** to activate and deactivate the search box.</span><span class="sxs-lookup"><span data-stu-id="bf200-123">You can press **F3** to activate and deactivate the search box.</span></span> <span data-ttu-id="bf200-124">For more information, see [Keyboard Shortcuts](keyboard-shortcuts.md#KeyboardFilter).</span><span class="sxs-lookup"><span data-stu-id="bf200-124">For more information, see [Keyboard Shortcuts](keyboard-shortcuts.md#KeyboardFilter).</span></span>

> [!NOTE]  
> <span data-ttu-id="bf200-125">Search won't match values in images, BLOB fields, FlowFilters, FlowFields, and other fields that aren't part of a table.</span><span class="sxs-lookup"><span data-stu-id="bf200-125">Search won't match values in images, BLOB fields, FlowFilters, FlowFields, and other fields that aren't part of a table.</span></span>


### <a name="fine-tuning-the-search-with-filter-criteria"></a><span data-ttu-id="bf200-126">Fine-tuning the Search with Filter criteria</span><span class="sxs-lookup"><span data-stu-id="bf200-126">Fine-tuning the Search with Filter criteria</span></span>

<span data-ttu-id="bf200-127">You can make a more exact search by using filter operators, expressions, and filter tokens.</span><span class="sxs-lookup"><span data-stu-id="bf200-127">You can make a more exact search by using filter operators, expressions, and filter tokens.</span></span> <span data-ttu-id="bf200-128">Unlike filtering, these are applied across all fields when used in the search box, making them less efficient than filtering.</span><span class="sxs-lookup"><span data-stu-id="bf200-128">Unlike filtering, these are applied across all fields when used in the search box, making them less efficient than filtering.</span></span>

- <span data-ttu-id="bf200-129">To find only field values that match the entire text and case exactly, place the search text between single quotes `''` (for example, `'man'`).</span><span class="sxs-lookup"><span data-stu-id="bf200-129">To find only field values that match the entire text and case exactly, place the search text between single quotes `''` (for example, `'man'`).</span></span>

- <span data-ttu-id="bf200-130">To find field values that start with a certain text and match the case, place `*` after the search text (for example `man*`).</span><span class="sxs-lookup"><span data-stu-id="bf200-130">To find field values that start with a certain text and match the case, place `*` after the search text (for example `man*`).</span></span>

- <span data-ttu-id="bf200-131">To find field values that end with a certain text and match the case, place `*` before the search text (for example `*man`).</span><span class="sxs-lookup"><span data-stu-id="bf200-131">To find field values that end with a certain text and match the case, place `*` before the search text (for example `*man`).</span></span>

- <span data-ttu-id="bf200-132">When using  `''` or `*`, the search is case-sensitive.</span><span class="sxs-lookup"><span data-stu-id="bf200-132">When using  `''` or `*`, the search is case-sensitive.</span></span> <span data-ttu-id="bf200-133">If you want to make the search case insensitive, place `@` before the search text (for example `@man*`).</span><span class="sxs-lookup"><span data-stu-id="bf200-133">If you want to make the search case insensitive, place `@` before the search text (for example `@man*`).</span></span>

<span data-ttu-id="bf200-134">The following table provides some examples to explain how you can use the search.</span><span class="sxs-lookup"><span data-stu-id="bf200-134">The following table provides some examples to explain how you can use the search.</span></span>

|<span data-ttu-id="bf200-135">Search Criteria</span><span class="sxs-lookup"><span data-stu-id="bf200-135">Search Criteria</span></span>|<span data-ttu-id="bf200-136">Finds...</span><span class="sxs-lookup"><span data-stu-id="bf200-136">Finds...</span></span>|
|---------------|----------|
|`man`<br /><span data-ttu-id="bf200-137">or</span><span class="sxs-lookup"><span data-stu-id="bf200-137">or</span></span> <br />`Man`|<span data-ttu-id="bf200-138">All records with fields that contain the text **man**, regardless of the case.</span><span class="sxs-lookup"><span data-stu-id="bf200-138">All records with fields that contain the text **man**, regardless of the case.</span></span> <span data-ttu-id="bf200-139">For example, **Manchester**, **manual**, or **Sportsman**.</span><span class="sxs-lookup"><span data-stu-id="bf200-139">For example, **Manchester**, **manual**, or **Sportsman**.</span></span> |
|`'Man'`|<span data-ttu-id="bf200-140">All records with fields that contain only **Man**, matching the case.</span><span class="sxs-lookup"><span data-stu-id="bf200-140">All records with fields that contain only **Man**, matching the case.</span></span>|
|`Man*`|<span data-ttu-id="bf200-141">All records with fields that start with the text <b>Man</b>, matching the case.</span><span class="sxs-lookup"><span data-stu-id="bf200-141">All records with fields that start with the text <b>Man</b>, matching the case.</span></span> <span data-ttu-id="bf200-142">For example, **Manchester** but not **manual** or **Sportsman**.</span><span class="sxs-lookup"><span data-stu-id="bf200-142">For example, **Manchester** but not **manual** or **Sportsman**.</span></span>|
|`@Man*`|<span data-ttu-id="bf200-143">All records with fields that start with **man**, regardless of the case.</span><span class="sxs-lookup"><span data-stu-id="bf200-143">All records with fields that start with **man**, regardless of the case.</span></span> <span data-ttu-id="bf200-144">For example, **Manchester** and **manual**, but not **Sportsman**.</span><span class="sxs-lookup"><span data-stu-id="bf200-144">For example, **Manchester** and **manual**, but not **Sportsman**.</span></span>|
|`@*man`|<span data-ttu-id="bf200-145">All records that end with **man**, regardless of the case.</span><span class="sxs-lookup"><span data-stu-id="bf200-145">All records that end with **man**, regardless of the case.</span></span> <span data-ttu-id="bf200-146">For example **Sportsman**, but not **Manchester** or **manual**.</span><span class="sxs-lookup"><span data-stu-id="bf200-146">For example **Sportsman**, but not **Manchester** or **manual**.</span></span>|


## <a name="filtering"></a><a name="filtering"></a><span data-ttu-id="bf200-147">Filtering</span><span class="sxs-lookup"><span data-stu-id="bf200-147">Filtering</span></span>

<span data-ttu-id="bf200-148">Filtering provides a more advanced and versatile way to control which records are included in a list, report, or XMLport.</span><span class="sxs-lookup"><span data-stu-id="bf200-148">Filtering provides a more advanced and versatile way to control which records are included in a list, report, or XMLport.</span></span> <span data-ttu-id="bf200-149">There are two major differences between searching and filtering, as described in the table below.</span><span class="sxs-lookup"><span data-stu-id="bf200-149">There are two major differences between searching and filtering, as described in the table below.</span></span>

|| <span data-ttu-id="bf200-150">**Searching**</span><span class="sxs-lookup"><span data-stu-id="bf200-150">**Searching**</span></span> | <span data-ttu-id="bf200-151">**Filtering**</span><span class="sxs-lookup"><span data-stu-id="bf200-151">**Filtering**</span></span> |
|--|----------|------------|
| <span data-ttu-id="bf200-152">**Applicable Fields**</span><span class="sxs-lookup"><span data-stu-id="bf200-152">**Applicable Fields**</span></span> | <span data-ttu-id="bf200-153">Searches across all fields that are visible on the page.</span><span class="sxs-lookup"><span data-stu-id="bf200-153">Searches across all fields that are visible on the page.</span></span> | <span data-ttu-id="bf200-154">Filters one or more fields individually, selecting from any field on the table, including fields that aren't visible on the page.</span><span class="sxs-lookup"><span data-stu-id="bf200-154">Filters one or more fields individually, selecting from any field on the table, including fields that aren't visible on the page.</span></span> |
| <span data-ttu-id="bf200-155">**Matching**</span><span class="sxs-lookup"><span data-stu-id="bf200-155">**Matching**</span></span> | <span data-ttu-id="bf200-156">Displays records with fields that match the search text, no matter the text's case or placement in the field.</span><span class="sxs-lookup"><span data-stu-id="bf200-156">Displays records with fields that match the search text, no matter the text's case or placement in the field.</span></span> | <span data-ttu-id="bf200-157">Displays records where the field exactly matches the filter, including the text's case, unless special filter symbols are entered.</span><span class="sxs-lookup"><span data-stu-id="bf200-157">Displays records where the field exactly matches the filter, including the text's case, unless special filter symbols are entered.</span></span>

<span data-ttu-id="bf200-158">Filtering enables you to display records for specific accounts or customers, dates, amounts, and other information by specifying filter criteria.</span><span class="sxs-lookup"><span data-stu-id="bf200-158">Filtering enables you to display records for specific accounts or customers, dates, amounts, and other information by specifying filter criteria.</span></span> <span data-ttu-id="bf200-159">Only records that match the criteria are displayed on the list or included in the report, batch job, or XMLport.</span><span class="sxs-lookup"><span data-stu-id="bf200-159">Only records that match the criteria are displayed on the list or included in the report, batch job, or XMLport.</span></span> <span data-ttu-id="bf200-160">If you specify criteria for multiple fields, then only records that match all criteria will be displayed.</span><span class="sxs-lookup"><span data-stu-id="bf200-160">If you specify criteria for multiple fields, then only records that match all criteria will be displayed.</span></span>

<span data-ttu-id="bf200-161">For lists, the filters are displayed on a filter pane that appears to the left of the list when you activate it.</span><span class="sxs-lookup"><span data-stu-id="bf200-161">For lists, the filters are displayed on a filter pane that appears to the left of the list when you activate it.</span></span> <span data-ttu-id="bf200-162">For reports, batch jobs, and XMLports, the filters are visible directly on the request page.</span><span class="sxs-lookup"><span data-stu-id="bf200-162">For reports, batch jobs, and XMLports, the filters are visible directly on the request page.</span></span>

### <a name="filtering-with-option-fields"></a><span data-ttu-id="bf200-163">Filtering with Option Fields</span><span class="sxs-lookup"><span data-stu-id="bf200-163">Filtering with Option Fields</span></span>

<span data-ttu-id="bf200-164">For "ordinary" fields that hold data, setup date, or business data, you can set filters both by selecting data and by typing filter values, and you can use symbols to define advanced filter criteria.</span><span class="sxs-lookup"><span data-stu-id="bf200-164">For "ordinary" fields that hold data, setup date, or business data, you can set filters both by selecting data and by typing filter values, and you can use symbols to define advanced filter criteria.</span></span> <span data-ttu-id="bf200-165">For more information, see [Entering Filter Criteria](ui-enter-criteria-filters.md#entering-filter-criteria).</span><span class="sxs-lookup"><span data-stu-id="bf200-165">For more information, see [Entering Filter Criteria](ui-enter-criteria-filters.md#entering-filter-criteria).</span></span>

<span data-ttu-id="bf200-166">For fields of type **Option**, however, you can only set a filter by selecting one or more options from a drop-down list of the available options.</span><span class="sxs-lookup"><span data-stu-id="bf200-166">For fields of type **Option**, however, you can only set a filter by selecting one or more options from a drop-down list of the available options.</span></span> <span data-ttu-id="bf200-167">An example of an option field is the **Status** field on the **Sales Orders** page.</span><span class="sxs-lookup"><span data-stu-id="bf200-167">An example of an option field is the **Status** field on the **Sales Orders** page.</span></span>

> [!NOTE]
> <span data-ttu-id="bf200-168">When you select multiple options as a filter value, the relationship between the options is defined as *OR*.</span><span class="sxs-lookup"><span data-stu-id="bf200-168">When you select multiple options as a filter value, the relationship between the options is defined as *OR*.</span></span> <span data-ttu-id="bf200-169">For example, if you select both the **Open** and the **Released** check box in the **Status** filter field on the **Sales Orders** page, it means that sales orders that are either open or released are displayed.</span><span class="sxs-lookup"><span data-stu-id="bf200-169">For example, if you select both the **Open** and the **Released** check box in the **Status** filter field on the **Sales Orders** page, it means that sales orders that are either open or released are displayed.</span></span>

### <a name="setting-filters-on-lists"></a><span data-ttu-id="bf200-170">Setting Filters on Lists</span><span class="sxs-lookup"><span data-stu-id="bf200-170">Setting Filters on Lists</span></span>

<span data-ttu-id="bf200-171">On lists, you set filters by using the filter pane.</span><span class="sxs-lookup"><span data-stu-id="bf200-171">On lists, you set filters by using the filter pane.</span></span> <span data-ttu-id="bf200-172">To display the filter pane for a list, choose the drop-down arrow next to the name of the page, and then choose the **Show filter pane** action.</span><span class="sxs-lookup"><span data-stu-id="bf200-172">To display the filter pane for a list, choose the drop-down arrow next to the name of the page, and then choose the **Show filter pane** action.</span></span> <span data-ttu-id="bf200-173">Alternatively, press **Shift+F3**.</span><span class="sxs-lookup"><span data-stu-id="bf200-173">Alternatively, press **Shift+F3**.</span></span>

<span data-ttu-id="bf200-174">To display the filter pane for a column on a list, choose the drop-down arrow, and then choose the **Filter** action.</span><span class="sxs-lookup"><span data-stu-id="bf200-174">To display the filter pane for a column on a list, choose the drop-down arrow, and then choose the **Filter** action.</span></span> <span data-ttu-id="bf200-175">Alternatively, press **Shift+F3**.</span><span class="sxs-lookup"><span data-stu-id="bf200-175">Alternatively, press **Shift+F3**.</span></span> <span data-ttu-id="bf200-176">The filter pane opens with the selected column shown as a filter field in the **Filter list by** section.</span><span class="sxs-lookup"><span data-stu-id="bf200-176">The filter pane opens with the selected column shown as a filter field in the **Filter list by** section.</span></span>

<span data-ttu-id="bf200-177">The filter pane displays the current filters for a list, and enables you to set your own custom filters on one or more fields by choosing the **+ Filter** action.</span><span class="sxs-lookup"><span data-stu-id="bf200-177">The filter pane displays the current filters for a list, and enables you to set your own custom filters on one or more fields by choosing the **+ Filter** action.</span></span>

 <span data-ttu-id="bf200-178">A filter pane is divided in three sections: **Views**, **Filter list by**, and **Filter totals by**:</span><span class="sxs-lookup"><span data-stu-id="bf200-178">A filter pane is divided in three sections: **Views**, **Filter list by**, and **Filter totals by**:</span></span>

- <span data-ttu-id="bf200-179">**Views**</span><span class="sxs-lookup"><span data-stu-id="bf200-179">**Views**</span></span>

  <span data-ttu-id="bf200-180">Some lists include the **Views** section.</span><span class="sxs-lookup"><span data-stu-id="bf200-180">Some lists include the **Views** section.</span></span> <span data-ttu-id="bf200-181">Views are variations of the list that have been preconfigured with filters.</span><span class="sxs-lookup"><span data-stu-id="bf200-181">Views are variations of the list that have been preconfigured with filters.</span></span> <span data-ttu-id="bf200-182">You can define and save as many views as you want per list.</span><span class="sxs-lookup"><span data-stu-id="bf200-182">You can define and save as many views as you want per list.</span></span> <span data-ttu-id="bf200-183">The views will be available to you on any device you sign into.</span><span class="sxs-lookup"><span data-stu-id="bf200-183">The views will be available to you on any device you sign into.</span></span> <span data-ttu-id="bf200-184">For more information, see [Save and Personalise List Views](ui-views.md).</span><span class="sxs-lookup"><span data-stu-id="bf200-184">For more information, see [Save and Personalize List Views](ui-views.md).</span></span>

- <span data-ttu-id="bf200-185">**Filter list by**</span><span class="sxs-lookup"><span data-stu-id="bf200-185">**Filter list by**</span></span>

  <span data-ttu-id="bf200-186">This section is where you add filters on specific fields to reduce the number of displayed records.</span><span class="sxs-lookup"><span data-stu-id="bf200-186">This section is where you add filters on specific fields to reduce the number of displayed records.</span></span> <span data-ttu-id="bf200-187">To add a filter, choose the **+ Filter** action.</span><span class="sxs-lookup"><span data-stu-id="bf200-187">To add a filter, choose the **+ Filter** action.</span></span> <span data-ttu-id="bf200-188">Then, type the name of the field that you want to filter the list by or pick a field from the drop-down list.</span><span class="sxs-lookup"><span data-stu-id="bf200-188">Then, type the name of the field that you want to filter the list by or pick a field from the drop-down list.</span></span>

- <span data-ttu-id="bf200-189">**Filter totals by**</span><span class="sxs-lookup"><span data-stu-id="bf200-189">**Filter totals by**</span></span>

  <span data-ttu-id="bf200-190">Some lists that display calculated fields, such as amounts and quantities, will include the **Filter totals by** section where you can adjust various dimensions that influence calculations.</span><span class="sxs-lookup"><span data-stu-id="bf200-190">Some lists that display calculated fields, such as amounts and quantities, will include the **Filter totals by** section where you can adjust various dimensions that influence calculations.</span></span> <span data-ttu-id="bf200-191">To add a filter, choose the **+ Filter** action.</span><span class="sxs-lookup"><span data-stu-id="bf200-191">To add a filter, choose the **+ Filter** action.</span></span> <span data-ttu-id="bf200-192">Then, type the name of the field that you want to filter the list by or pick a field from the drop-down list.</span><span class="sxs-lookup"><span data-stu-id="bf200-192">Then, type the name of the field that you want to filter the list by or pick a field from the drop-down list.</span></span>

  > [!NOTE]
  > <span data-ttu-id="bf200-193">Filters in the **Filter totals by** section are controlled by FlowFilters on the page design.</span><span class="sxs-lookup"><span data-stu-id="bf200-193">Filters in the **Filter totals by** section are controlled by FlowFilters on the page design.</span></span> <span data-ttu-id="bf200-194">For technical information, see [FlowFilters](/dynamics365/business-central/dev-itpro/developer/devenv-flowfilter-overview).</span><span class="sxs-lookup"><span data-stu-id="bf200-194">For technical information, see [FlowFilters](/dynamics365/business-central/dev-itpro/developer/devenv-flowfilter-overview).</span></span>

<span data-ttu-id="bf200-195">You can set a simple filter directly on a list within using the filter pane, namely a filter that displays only records with the same value as in the selected cell.</span><span class="sxs-lookup"><span data-stu-id="bf200-195">You can set a simple filter directly on a list within using the filter pane, namely a filter that displays only records with the same value as in the selected cell.</span></span> <span data-ttu-id="bf200-196">Select a cell on the list, choose the drop-down arrow, and then choose the **Filter to This Value** action.</span><span class="sxs-lookup"><span data-stu-id="bf200-196">Select a cell on the list, choose the drop-down arrow, and then choose the **Filter to This Value** action.</span></span> <span data-ttu-id="bf200-197">Alternatively, press **Alt+F3**.</span><span class="sxs-lookup"><span data-stu-id="bf200-197">Alternatively, press **Alt+F3**.</span></span>

### <a name="setting-filters-in-reports-batch-jobs-and-xmlports"></a><span data-ttu-id="bf200-198">Setting Filters in Reports, Batch Jobs, and XMLports</span><span class="sxs-lookup"><span data-stu-id="bf200-198">Setting Filters in Reports, Batch Jobs, and XMLports</span></span>

<span data-ttu-id="bf200-199">For reports and XMLports, the filters are visible directly on the request page.</span><span class="sxs-lookup"><span data-stu-id="bf200-199">For reports and XMLports, the filters are visible directly on the request page.</span></span> <span data-ttu-id="bf200-200">The request page displays the last used filters according to your selection in the **Use default values from** field.</span><span class="sxs-lookup"><span data-stu-id="bf200-200">The request page displays the last used filters according to your selection in the **Use default values from** field.</span></span> <span data-ttu-id="bf200-201">For more information, see [Using Saved Settings](ui-work-report.md#SavedSettings).</span><span class="sxs-lookup"><span data-stu-id="bf200-201">For more information, see [Using Saved Settings](ui-work-report.md#SavedSettings).</span></span>

<span data-ttu-id="bf200-202">The main **Filter** section shows the default filter fields that you use to delimit which records to include in the report or XMLport.</span><span class="sxs-lookup"><span data-stu-id="bf200-202">The main **Filter** section shows the default filter fields that you use to delimit which records to include in the report or XMLport.</span></span> <span data-ttu-id="bf200-203">To add a filter, choose the **+ Filter** action.</span><span class="sxs-lookup"><span data-stu-id="bf200-203">To add a filter, choose the **+ Filter** action.</span></span> <span data-ttu-id="bf200-204">Then, type the name of the field that you want to filter by, or pick a field from the drop-down list.</span><span class="sxs-lookup"><span data-stu-id="bf200-204">Then, type the name of the field that you want to filter by, or pick a field from the drop-down list.</span></span>

<span data-ttu-id="bf200-205">In the **Filter totals by** section, you can adjust various dimensions that influence calculations in the report or XMLport.</span><span class="sxs-lookup"><span data-stu-id="bf200-205">In the **Filter totals by** section, you can adjust various dimensions that influence calculations in the report or XMLport.</span></span> <span data-ttu-id="bf200-206">To add a filter, choose the **+ Filter** action.</span><span class="sxs-lookup"><span data-stu-id="bf200-206">To add a filter, choose the **+ Filter** action.</span></span> <span data-ttu-id="bf200-207">Then, type the name of the field that you want to filter by, or pick a field from the drop-down list.</span><span class="sxs-lookup"><span data-stu-id="bf200-207">Then, type the name of the field that you want to filter by, or pick a field from the drop-down list.</span></span>

## <a name="entering-filter-criteria"></a><span data-ttu-id="bf200-208">Entering Filter Criteria</span><span class="sxs-lookup"><span data-stu-id="bf200-208">Entering Filter Criteria</span></span>

<span data-ttu-id="bf200-209">Both in the filter pane and on a request page, you enter your filter criteria in the box under the filter field.</span><span class="sxs-lookup"><span data-stu-id="bf200-209">Both in the filter pane and on a request page, you enter your filter criteria in the box under the filter field.</span></span>

<span data-ttu-id="bf200-210">The type of the filter field determines which criteria you can enter.</span><span class="sxs-lookup"><span data-stu-id="bf200-210">The type of the filter field determines which criteria you can enter.</span></span> <span data-ttu-id="bf200-211">For example, filtering a field that has fixed values will only let you choose from those values.</span><span class="sxs-lookup"><span data-stu-id="bf200-211">For example, filtering a field that has fixed values will only let you choose from those values.</span></span> <span data-ttu-id="bf200-212">For more information about special filter symbols, see [Filter criteria](#FilterCriteria) and [Filter tokens](#FilterTokens).</span><span class="sxs-lookup"><span data-stu-id="bf200-212">For more information about special filter symbols, see [Filter criteria](#FilterCriteria) and [Filter tokens](#FilterTokens).</span></span>

<span data-ttu-id="bf200-213">Columns that already have filters are indicated by the ![Filter icon](media/ui-search/filter-icon.png "Filter icon") icon in the column heading.</span><span class="sxs-lookup"><span data-stu-id="bf200-213">Columns that already have filters are indicated by the ![Filter icon](media/ui-search/filter-icon.png "Filter icon") icon in the column heading.</span></span> <span data-ttu-id="bf200-214">To remove a filter, choose the drop-down arrow, and then choose the **Clear Filter** action.</span><span class="sxs-lookup"><span data-stu-id="bf200-214">To remove a filter, choose the drop-down arrow, and then choose the **Clear Filter** action.</span></span>

> [!TIP]
> <span data-ttu-id="bf200-215">Accelerate finding and analysing your data by using combinations of keyboard shortcuts.</span><span class="sxs-lookup"><span data-stu-id="bf200-215">Accelerate finding and analyzing your data by using combinations of keyboard shortcuts.</span></span> <span data-ttu-id="bf200-216">For example, select a field, use **Shift+Alt+F3** to add that field to the filter pane, type the filter criteria, use **Ctrl+Enter** to return to the rows, select another field, and use **Alt+F3** to filter to that value.</span><span class="sxs-lookup"><span data-stu-id="bf200-216">For example, select a field, use **Shift+Alt+F3** to add that field to the filter pane, type the filter criteria, use **Ctrl+Enter** to return to the rows, select another field, and use **Alt+F3** to filter to that value.</span></span> <span data-ttu-id="bf200-217">For more information, see [Keyboard Shortcuts](keyboard-shortcuts.md#KeyboardFilter).</span><span class="sxs-lookup"><span data-stu-id="bf200-217">For more information, see [Keyboard Shortcuts](keyboard-shortcuts.md#KeyboardFilter).</span></span>

### <a name="filter-criteria-and-operators"></a><span data-ttu-id="bf200-218"><a name="FilterCriteria"> </a>Filter Criteria and Operators</span><span class="sxs-lookup"><span data-stu-id="bf200-218"><a name="FilterCriteria"> </a>Filter Criteria and Operators</span></span>

<span data-ttu-id="bf200-219">When you enter criteria, you can use all the numbers and letters that you normally use in the field.</span><span class="sxs-lookup"><span data-stu-id="bf200-219">When you enter criteria, you can use all the numbers and letters that you normally use in the field.</span></span> <span data-ttu-id="bf200-220">But there's also a set of special symbols that you can use as operators to further filter the results.</span><span class="sxs-lookup"><span data-stu-id="bf200-220">But there's also a set of special symbols that you can use as operators to further filter the results.</span></span> <span data-ttu-id="bf200-221">The following sections describe these symbols and how to use them as operators in filters.</span><span class="sxs-lookup"><span data-stu-id="bf200-221">The following sections describe these symbols and how to use them as operators in filters.</span></span>

> [!TIP]
> <span data-ttu-id="bf200-222">For more information about filtering dates and times, see [Working with Calendar Dates and Times](ui-enter-date-ranges.md).</span><span class="sxs-lookup"><span data-stu-id="bf200-222">For more information about filtering dates and times, see [Working with Calendar Dates and Times](ui-enter-date-ranges.md).</span></span>

> [!IMPORTANT]
> - <span data-ttu-id="bf200-223">There may be situations where the value that you want to filter on contains a symbol that's an operator.</span><span class="sxs-lookup"><span data-stu-id="bf200-223">There may be situations where the value that you want to filter on contains a symbol that's an operator.</span></span> <span data-ttu-id="bf200-224">For more information about handling these situtions, see [Filtering on Values That Contain Symbols](#symbols) for more instructions about handling this situation.</span><span class="sxs-lookup"><span data-stu-id="bf200-224">For more information about handling these situtions, see [Filtering on Values That Contain Symbols](#symbols) for more instructions about handling this situation.</span></span>
>
> - <span data-ttu-id="bf200-225">If there are more than 200 operators in a single filter, the system will automatically group some expressions in parentheses `()` for the purpose of processing.</span><span class="sxs-lookup"><span data-stu-id="bf200-225">If there are more than 200 operators in a single filter, the system will automatically group some expressions in parentheses `()` for the purpose of processing.</span></span> <span data-ttu-id="bf200-226">This has no effect on the filter or the results.</span><span class="sxs-lookup"><span data-stu-id="bf200-226">This has no effect on the filter or the results.</span></span>  

#### <a name="-interval"></a><span data-ttu-id="bf200-227">(..) Interval</span><span class="sxs-lookup"><span data-stu-id="bf200-227">(..) Interval</span></span>

|<span data-ttu-id="bf200-228">Sample Expression</span><span class="sxs-lookup"><span data-stu-id="bf200-228">Sample Expression</span></span>|<span data-ttu-id="bf200-229">Records Displayed</span><span class="sxs-lookup"><span data-stu-id="bf200-229">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`1100..2100`|<span data-ttu-id="bf200-230">Numbers 1100 through 2100</span><span class="sxs-lookup"><span data-stu-id="bf200-230">Numbers 1100 through 2100</span></span>|  
|`..2500`|<span data-ttu-id="bf200-231">Up to and including 2500</span><span class="sxs-lookup"><span data-stu-id="bf200-231">Up to and including 2500</span></span>|  
|`..12 31 00`|<span data-ttu-id="bf200-232">Dates up to and including 12 31 00</span><span class="sxs-lookup"><span data-stu-id="bf200-232">Dates up to and including 12 31 00</span></span>|  
|`P8..`|<span data-ttu-id="bf200-233">Information for accounting period 8 and after</span><span class="sxs-lookup"><span data-stu-id="bf200-233">Information for accounting period 8 and after</span></span>|  
|`..23`|<span data-ttu-id="bf200-234">From the beginning date until 23-current month-current year 23:59:59</span><span class="sxs-lookup"><span data-stu-id="bf200-234">From the beginning date until 23-current month-current year 23:59:59</span></span>|  
|`23..`|<span data-ttu-id="bf200-235">From 23-current month-current year 0:00:00 until the end of time</span><span class="sxs-lookup"><span data-stu-id="bf200-235">From 23-current month-current year 0:00:00 until the end of time</span></span>|  
|`22..23`|<span data-ttu-id="bf200-236">From 22-current month-current year 0:00:00 until 23-current month-current year 23:59:59</span><span class="sxs-lookup"><span data-stu-id="bf200-236">From 22-current month-current year 0:00:00 until 23-current month-current year 23:59:59</span></span>|  

#### <a name="124-eitheror"></a><span data-ttu-id="bf200-237">(&#124;) Either/or</span><span class="sxs-lookup"><span data-stu-id="bf200-237">(&#124;) Either/or</span></span>

|<span data-ttu-id="bf200-238">Sample Expression</span><span class="sxs-lookup"><span data-stu-id="bf200-238">Sample Expression</span></span>|<span data-ttu-id="bf200-239">Records Displayed</span><span class="sxs-lookup"><span data-stu-id="bf200-239">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`1200|1300`|<span data-ttu-id="bf200-240">Numbers with 1200 or 1300</span><span class="sxs-lookup"><span data-stu-id="bf200-240">Numbers with 1200 or 1300</span></span>|  

#### <a name="-not-equal-to"></a><span data-ttu-id="bf200-241">(<>) Not equal to</span><span class="sxs-lookup"><span data-stu-id="bf200-241">(<>) Not equal to</span></span>  

|<span data-ttu-id="bf200-242">Sample Expression</span><span class="sxs-lookup"><span data-stu-id="bf200-242">Sample Expression</span></span>|<span data-ttu-id="bf200-243">Records Displayed</span><span class="sxs-lookup"><span data-stu-id="bf200-243">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`<>0`|<span data-ttu-id="bf200-244">All numbers except 0</span><span class="sxs-lookup"><span data-stu-id="bf200-244">All numbers except 0</span></span><br /><br /> <span data-ttu-id="bf200-245">The SQL Server Option allows you to combine this symbol with a wild-card expression.</span><span class="sxs-lookup"><span data-stu-id="bf200-245">The SQL Server Option allows you to combine this symbol with a wild-card expression.</span></span> <span data-ttu-id="bf200-246">For example, <>A\* meaning not equal to any text that starts with A.</span><span class="sxs-lookup"><span data-stu-id="bf200-246">For example, <>A\* meaning not equal to any text that starts with A.</span></span>|  

#### <a name="-greater-than"></a><span data-ttu-id="bf200-247">(>) Greater than</span><span class="sxs-lookup"><span data-stu-id="bf200-247">(>) Greater than</span></span>  

|<span data-ttu-id="bf200-248">Sample Expression</span><span class="sxs-lookup"><span data-stu-id="bf200-248">Sample Expression</span></span>|<span data-ttu-id="bf200-249">Records Displayed</span><span class="sxs-lookup"><span data-stu-id="bf200-249">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`>1200`|<span data-ttu-id="bf200-250">Numbers greater than 1200</span><span class="sxs-lookup"><span data-stu-id="bf200-250">Numbers greater than 1200</span></span>|  

#### <a name="-greater-than-or-equal-to"></a><span data-ttu-id="bf200-251">(>=) Greater than or equal to</span><span class="sxs-lookup"><span data-stu-id="bf200-251">(>=) Greater than or equal to</span></span>  

|<span data-ttu-id="bf200-252">Sample Expression</span><span class="sxs-lookup"><span data-stu-id="bf200-252">Sample Expression</span></span>|<span data-ttu-id="bf200-253">Records Displayed</span><span class="sxs-lookup"><span data-stu-id="bf200-253">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`>=1200`|<span data-ttu-id="bf200-254">Numbers greater than or equal to 1200</span><span class="sxs-lookup"><span data-stu-id="bf200-254">Numbers greater than or equal to 1200</span></span>|  

#### <a name="-less-than"></a><span data-ttu-id="bf200-255">(<) Less than</span><span class="sxs-lookup"><span data-stu-id="bf200-255">(<) Less than</span></span>  

|<span data-ttu-id="bf200-256">Sample Expression</span><span class="sxs-lookup"><span data-stu-id="bf200-256">Sample Expression</span></span>|<span data-ttu-id="bf200-257">Records Displayed</span><span class="sxs-lookup"><span data-stu-id="bf200-257">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`<1200`|<span data-ttu-id="bf200-258">Numbers less than 1200</span><span class="sxs-lookup"><span data-stu-id="bf200-258">Numbers less than 1200</span></span>|  

#### <a name="-less-than-or-equal-to"></a><span data-ttu-id="bf200-259">(<=) Less than or equal to</span><span class="sxs-lookup"><span data-stu-id="bf200-259">(<=) Less than or equal to</span></span>  

|<span data-ttu-id="bf200-260">Sample Expression</span><span class="sxs-lookup"><span data-stu-id="bf200-260">Sample Expression</span></span>|<span data-ttu-id="bf200-261">Records Displayed</span><span class="sxs-lookup"><span data-stu-id="bf200-261">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`<=1200`|<span data-ttu-id="bf200-262">Numbers less than or equal to 1200</span><span class="sxs-lookup"><span data-stu-id="bf200-262">Numbers less than or equal to 1200</span></span>|  

#### <a name="-and"></a><span data-ttu-id="bf200-263">(&) And</span><span class="sxs-lookup"><span data-stu-id="bf200-263">(&) And</span></span>  

|<span data-ttu-id="bf200-264">Sample Expression</span><span class="sxs-lookup"><span data-stu-id="bf200-264">Sample Expression</span></span>|<span data-ttu-id="bf200-265">Records Displayed</span><span class="sxs-lookup"><span data-stu-id="bf200-265">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`>200&<1200`|<span data-ttu-id="bf200-266">Numbers greater than 200 and less than 1200</span><span class="sxs-lookup"><span data-stu-id="bf200-266">Numbers greater than 200 and less than 1200</span></span>|  

#### <a name="-an-exact-character-match"></a><span data-ttu-id="bf200-267">('') An exact character match</span><span class="sxs-lookup"><span data-stu-id="bf200-267">('') An exact character match</span></span>  

|<span data-ttu-id="bf200-268">Sample Expression</span><span class="sxs-lookup"><span data-stu-id="bf200-268">Sample Expression</span></span>|<span data-ttu-id="bf200-269">Records Displayed</span><span class="sxs-lookup"><span data-stu-id="bf200-269">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`'man'`|<span data-ttu-id="bf200-270">Text that matches **man** exactly and is case-sensitive.</span><span class="sxs-lookup"><span data-stu-id="bf200-270">Text that matches **man** exactly and is case-sensitive.</span></span>|  

#### <a name="-case-insensitive"></a><span data-ttu-id="bf200-271">(@) Case insensitive</span><span class="sxs-lookup"><span data-stu-id="bf200-271">(@) Case insensitive</span></span>  

|<span data-ttu-id="bf200-272">Sample Expression</span><span class="sxs-lookup"><span data-stu-id="bf200-272">Sample Expression</span></span>|<span data-ttu-id="bf200-273">Records Displayed</span><span class="sxs-lookup"><span data-stu-id="bf200-273">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`@man*`|<span data-ttu-id="bf200-274">Text that starts with **man** and is case insensitive.</span><span class="sxs-lookup"><span data-stu-id="bf200-274">Text that starts with **man** and is case insensitive.</span></span>|  

#### <a name="-an-indefinite-number-of-unknown-characters"></a><span data-ttu-id="bf200-275">(\*) An indefinite number of unknown characters</span><span class="sxs-lookup"><span data-stu-id="bf200-275">(\*) An indefinite number of unknown characters</span></span>

|<span data-ttu-id="bf200-276">Sample Expression</span><span class="sxs-lookup"><span data-stu-id="bf200-276">Sample Expression</span></span>|<span data-ttu-id="bf200-277">Records Displayed</span><span class="sxs-lookup"><span data-stu-id="bf200-277">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`*Co*`|<span data-ttu-id="bf200-278">Text that contains **Co** and is case-sensitive.</span><span class="sxs-lookup"><span data-stu-id="bf200-278">Text that contains **Co** and is case-sensitive.</span></span>|  
|`*Co`|<span data-ttu-id="bf200-279">Text that ends with **Co"** and is case-sensitive.</span><span class="sxs-lookup"><span data-stu-id="bf200-279">Text that ends with **Co"** and is case-sensitive.</span></span>|  
|`Co*`|<span data-ttu-id="bf200-280">Text that begins with **Co** and is case-sensitive.</span><span class="sxs-lookup"><span data-stu-id="bf200-280">Text that begins with **Co** and is case-sensitive.</span></span>|  

#### <a name="-one-unknown-character"></a><span data-ttu-id="bf200-281">(?) One unknown character</span><span class="sxs-lookup"><span data-stu-id="bf200-281">(?) One unknown character</span></span>  

|<span data-ttu-id="bf200-282">Sample Expression</span><span class="sxs-lookup"><span data-stu-id="bf200-282">Sample Expression</span></span>|<span data-ttu-id="bf200-283">Records Displayed</span><span class="sxs-lookup"><span data-stu-id="bf200-283">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`Hans?n`|<span data-ttu-id="bf200-284">Text such as **Hansen** or **Hanson**</span><span class="sxs-lookup"><span data-stu-id="bf200-284">Text such as **Hansen** or **Hanson**</span></span>|  

#### <a name="combined-format-expressions"></a><span data-ttu-id="bf200-285">Combined Format Expressions</span><span class="sxs-lookup"><span data-stu-id="bf200-285">Combined Format Expressions</span></span>  

|<span data-ttu-id="bf200-286">Sample Expression</span><span class="sxs-lookup"><span data-stu-id="bf200-286">Sample Expression</span></span>|<span data-ttu-id="bf200-287">Records Displayed</span><span class="sxs-lookup"><span data-stu-id="bf200-287">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`5999|8100..8490`|<span data-ttu-id="bf200-288">Include any records with the number 5999 or a number from the interval 8100 through 8490.</span><span class="sxs-lookup"><span data-stu-id="bf200-288">Include any records with the number 5999 or a number from the interval 8100 through 8490.</span></span>|  
|`..1299|1400..`|<span data-ttu-id="bf200-289">Include records with a number less than or equal to 1299 or a number equal to 1400 or greater (all numbers except 1300 through 1399).</span><span class="sxs-lookup"><span data-stu-id="bf200-289">Include records with a number less than or equal to 1299 or a number equal to 1400 or greater (all numbers except 1300 through 1399).</span></span>|  
|`>50&<100`|<span data-ttu-id="bf200-290">Include records with numbers that are greater than 50 and less than 100 (numbers 51 through 99).</span><span class="sxs-lookup"><span data-stu-id="bf200-290">Include records with numbers that are greater than 50 and less than 100 (numbers 51 through 99).</span></span>|  

### <a name="filtering-on-values-that-contain-symbols"></a><a name="symbols"></a><span data-ttu-id="bf200-291">Filtering on Values That Contain Symbols</span><span class="sxs-lookup"><span data-stu-id="bf200-291">Filtering on Values That Contain Symbols</span></span>

<span data-ttu-id="bf200-292">There may be cases where field values contain the one of the following symbols:</span><span class="sxs-lookup"><span data-stu-id="bf200-292">There may be cases where field values contain the one of the following symbols:</span></span>

- &
- <span data-ttu-id="bf200-293">(</span><span class="sxs-lookup"><span data-stu-id="bf200-293">(</span></span>
- <span data-ttu-id="bf200-294">)</span><span class="sxs-lookup"><span data-stu-id="bf200-294">)</span></span>
- =
- <span data-ttu-id="bf200-295">&#124;</span><span class="sxs-lookup"><span data-stu-id="bf200-295">&#124;</span></span>

<span data-ttu-id="bf200-296">If you want to filter on any of these symbols, place the filter expression in single quotes (`'<expression with symbol>'`).</span><span class="sxs-lookup"><span data-stu-id="bf200-296">If you want to filter on any of these symbols, place the filter expression in single quotes (`'<expression with symbol>'`).</span></span> <span data-ttu-id="bf200-297">For example, if you wanted to filter on records that start with the text *J & V*, the filter expression would be `'J & V*'`.</span><span class="sxs-lookup"><span data-stu-id="bf200-297">For example, if you wanted to filter on records that start with the text *J & V*, the filter expression would be `'J & V*'`.</span></span>

<span data-ttu-id="bf200-298">This requirement isn't necessary for other symbols.</span><span class="sxs-lookup"><span data-stu-id="bf200-298">This requirement isn't necessary for other symbols.</span></span>

### <a name="filter-tokens"></a><span data-ttu-id="bf200-299"><a name="FilterTokens"> </a>Filter Tokens</span><span class="sxs-lookup"><span data-stu-id="bf200-299"><a name="FilterTokens"> </a>Filter Tokens</span></span>

<span data-ttu-id="bf200-300">When entering filter criteria, you can also type words that have special meaning, called filter tokens.</span><span class="sxs-lookup"><span data-stu-id="bf200-300">When entering filter criteria, you can also type words that have special meaning, called filter tokens.</span></span> <span data-ttu-id="bf200-301">After entering the token word, the word is replaced by the value or values that it represents.</span><span class="sxs-lookup"><span data-stu-id="bf200-301">After entering the token word, the word is replaced by the value or values that it represents.</span></span> <span data-ttu-id="bf200-302">Filter tokens make filtering easier by reducing the need to navigate to other pages to look up values you want to add to your filter.</span><span class="sxs-lookup"><span data-stu-id="bf200-302">Filter tokens make filtering easier by reducing the need to navigate to other pages to look up values you want to add to your filter.</span></span> <span data-ttu-id="bf200-303">The tables below describe some of the tokens you can type as filter criteria.</span><span class="sxs-lookup"><span data-stu-id="bf200-303">The tables below describe some of the tokens you can type as filter criteria.</span></span>

> [!TIP]
> <span data-ttu-id="bf200-304">Your organisation may use custom tokens.</span><span class="sxs-lookup"><span data-stu-id="bf200-304">Your organization may use custom tokens.</span></span> <span data-ttu-id="bf200-305">To learn about the complete set of tokens available to you or to add more custom tokens, talk to your administrator.</span><span class="sxs-lookup"><span data-stu-id="bf200-305">To learn about the complete set of tokens available to you or to add more custom tokens, talk to your administrator.</span></span> <span data-ttu-id="bf200-306">For technical information see [Adding Filter Tokens](/dynamics365/business-central/dev-itpro/developer/devenv-adding-filter-tokens).</span><span class="sxs-lookup"><span data-stu-id="bf200-306">For technical information see [Adding Filter Tokens](/dynamics365/business-central/dev-itpro/developer/devenv-adding-filter-tokens).</span></span>

#### <a name="me-or-userid-records-assigned-to-you"></a><span data-ttu-id="bf200-307">(%me or %userid) Records Assigned to You</span><span class="sxs-lookup"><span data-stu-id="bf200-307">(%me or %userid) Records Assigned to You</span></span>

<span data-ttu-id="bf200-308">Use `%me` or `%userid` when filtering fields that contain the user ID, such as **Assigned to User ID** field, to display all records that are assigned to you.</span><span class="sxs-lookup"><span data-stu-id="bf200-308">Use `%me` or `%userid` when filtering fields that contain the user ID, such as **Assigned to User ID** field, to display all records that are assigned to you.</span></span>

|<span data-ttu-id="bf200-309">Sample Expression</span><span class="sxs-lookup"><span data-stu-id="bf200-309">Sample Expression</span></span>|<span data-ttu-id="bf200-310">Records Displayed</span><span class="sxs-lookup"><span data-stu-id="bf200-310">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`%me`<br /><span data-ttu-id="bf200-311">or</span><span class="sxs-lookup"><span data-stu-id="bf200-311">or</span></span><br />`%userid`|<span data-ttu-id="bf200-312">Records that are assigned to your user account.</span><span class="sxs-lookup"><span data-stu-id="bf200-312">Records that are assigned to your user account.</span></span> |  

#### <a name="mycustomers-customers-in-my-customers"></a><span data-ttu-id="bf200-313">(%mycustomers) Customers in My Customers</span><span class="sxs-lookup"><span data-stu-id="bf200-313">(%mycustomers) Customers in My Customers</span></span>

<span data-ttu-id="bf200-314">Use `%mycustomers` in the customer **No** field to display all records for customers that are included in the **My Customers** list on your Role Centre.</span><span class="sxs-lookup"><span data-stu-id="bf200-314">Use `%mycustomers` in the customer **No** field to display all records for customers that are included in the **My Customers** list on your Role Center.</span></span>

|<span data-ttu-id="bf200-315">Sample Expression</span><span class="sxs-lookup"><span data-stu-id="bf200-315">Sample Expression</span></span>|<span data-ttu-id="bf200-316">Records Displayed</span><span class="sxs-lookup"><span data-stu-id="bf200-316">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`%mycustomers`|<span data-ttu-id="bf200-317">Customers in the **My Customers** on your Role Centre.</span><span class="sxs-lookup"><span data-stu-id="bf200-317">Customers in the **My Customers** on your Role Center.</span></span> |  

#### <a name="myitems-items-in-my-items"></a><span data-ttu-id="bf200-318">(%myitems) Items in My Items</span><span class="sxs-lookup"><span data-stu-id="bf200-318">(%myitems) Items in My Items</span></span>

<span data-ttu-id="bf200-319">Use `%myitems` in the item **No** field to display all records for items that are included in the **My Items** list on your Role Centre.</span><span class="sxs-lookup"><span data-stu-id="bf200-319">Use `%myitems` in the item **No** field to display all records for items that are included in the **My Items** list on your Role Center.</span></span>

|<span data-ttu-id="bf200-320">Sample Expression</span><span class="sxs-lookup"><span data-stu-id="bf200-320">Sample Expression</span></span>|<span data-ttu-id="bf200-321">Records Displayed</span><span class="sxs-lookup"><span data-stu-id="bf200-321">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`%myitems`|<span data-ttu-id="bf200-322">Items in the **My Items** on your Role Centre.</span><span class="sxs-lookup"><span data-stu-id="bf200-322">Items in the **My Items** on your Role Center.</span></span> |  

#### <a name="myvendors-vendors-in-my-vendors"></a><span data-ttu-id="bf200-323">(%myvendors) Vendors in My Vendors</span><span class="sxs-lookup"><span data-stu-id="bf200-323">(%myvendors) Vendors in My Vendors</span></span>

<span data-ttu-id="bf200-324">Use `%myvendors` in the vendor **No** field to display all records for vendors that are included in the **My Vendors** list on your Role Centre.</span><span class="sxs-lookup"><span data-stu-id="bf200-324">Use `%myvendors` in the vendor **No** field to display all records for vendors that are included in the **My Vendors** list on your Role Center.</span></span>

|<span data-ttu-id="bf200-325">Sample Expression</span><span class="sxs-lookup"><span data-stu-id="bf200-325">Sample Expression</span></span>|<span data-ttu-id="bf200-326">Records Displayed</span><span class="sxs-lookup"><span data-stu-id="bf200-326">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`%myvendors`|<span data-ttu-id="bf200-327">Vendors in the **My Vendors** on your Role Centre.</span><span class="sxs-lookup"><span data-stu-id="bf200-327">Vendors in the **My Vendors** on your Role Center.</span></span> |  

## <a name="see-also"></a><span data-ttu-id="bf200-328">See Also</span><span class="sxs-lookup"><span data-stu-id="bf200-328">See Also</span></span>

[<span data-ttu-id="bf200-329">Searching and Filtering FAQ</span><span class="sxs-lookup"><span data-stu-id="bf200-329">Searching and Filtering FAQ</span></span>](ui-search-filter-faq.yml)  
[<span data-ttu-id="bf200-330">Save and Personalise List Views</span><span class="sxs-lookup"><span data-stu-id="bf200-330">Save and Personalize List Views</span></span>](ui-views.md)  
<span data-ttu-id="bf200-331">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="bf200-331">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>  


[!INCLUDE[footer-include](includes/footer-banner.md)]