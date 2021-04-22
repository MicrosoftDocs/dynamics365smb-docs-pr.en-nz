---
title: How to Add Fields to a Word Report Layout | Microsoft Docs
description: Describes how to add fields of a report dataset to an existing Word report layout for a report.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2021
ms.author: jswymer
ms.openlocfilehash: 52cfb4ba4ca0ba645ecca48e08d63722c2c5c5b4
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 03/31/2021
ms.locfileid: "5771126"
---
# <a name="add-fields-to-a-word-report-layout"></a><span data-ttu-id="86435-103">Add Fields to a Word Report Layout</span><span class="sxs-lookup"><span data-stu-id="86435-103">Add Fields to a Word Report Layout</span></span>
<span data-ttu-id="86435-104">A report dataset can consist of fields that display labels, data, and images.</span><span class="sxs-lookup"><span data-stu-id="86435-104">A report dataset can consist of fields that display labels, data, and images.</span></span> <span data-ttu-id="86435-105">This topic describes the procedure for adding fields of a report dataset to an existing Word report layout for a report.</span><span class="sxs-lookup"><span data-stu-id="86435-105">This topic describes the procedure for adding fields of a report dataset to an existing Word report layout for a report.</span></span> <span data-ttu-id="86435-106">You add fields by using the Word custom XML part for the report and adding content controls that map to the fields of the report dataset.</span><span class="sxs-lookup"><span data-stu-id="86435-106">You add fields by using the Word custom XML part for the report and adding content controls that map to the fields of the report dataset.</span></span> <span data-ttu-id="86435-107">Adding fields requires that you have some knowledge of the report's dataset so that you can identify the fields that you want to add to the layout.</span><span class="sxs-lookup"><span data-stu-id="86435-107">Adding fields requires that you have some knowledge of the report's dataset so that you can identify the fields that you want to add to the layout.</span></span>  
  
> [!NOTE]  
>  <span data-ttu-id="86435-108">You cannot modify built-in report layouts</span><span class="sxs-lookup"><span data-stu-id="86435-108">You cannot modify built-in report layouts</span></span><!--Onprem. Built-in layouts can only be modified by using the development environment--><span data-ttu-id="86435-109">.</span><span class="sxs-lookup"><span data-stu-id="86435-109">.</span></span>  

##  <a name="to-open-the-custom-xml-part-for-the-report-in-word"></a><a name="OpenXMLPart"></a><span data-ttu-id="86435-110">To open the Custom XML part for the Report in Word</span><span class="sxs-lookup"><span data-stu-id="86435-110">To open the Custom XML part for the Report in Word</span></span>  
  
1.  <span data-ttu-id="86435-111">If not already open, then open the Word report layout document in Word.</span><span class="sxs-lookup"><span data-stu-id="86435-111">If not already open, then open the Word report layout document in Word.</span></span>  
  
     <span data-ttu-id="86435-112">For more information, see [Create and Modify a Custom Report Layout](ui-how-create-custom-report-layout.md).</span><span class="sxs-lookup"><span data-stu-id="86435-112">For more information, see [Create and Modify a Custom Report Layout](ui-how-create-custom-report-layout.md).</span></span>  
  
2.  <span data-ttu-id="86435-113">Show the **Developer** tab in the ribbon of Microsoft Word.</span><span class="sxs-lookup"><span data-stu-id="86435-113">Show the **Developer** tab in the ribbon of Microsoft Word.</span></span>  
  
     <span data-ttu-id="86435-114">By default, the **Developer** tab is not shown in the ribbon.</span><span class="sxs-lookup"><span data-stu-id="86435-114">By default, the **Developer** tab is not shown in the ribbon.</span></span> <span data-ttu-id="86435-115">For more information, see [Show the Developer Tab on the Ribbon](/visualstudio/vsto/how-to-show-the-developer-tab-on-the-ribbon).</span><span class="sxs-lookup"><span data-stu-id="86435-115">For more information, see [Show the Developer Tab on the Ribbon](/visualstudio/vsto/how-to-show-the-developer-tab-on-the-ribbon).</span></span>  
  
3.  <span data-ttu-id="86435-116">On the **Developer** tab, choose **XML Mapping Pane**.</span><span class="sxs-lookup"><span data-stu-id="86435-116">On the **Developer** tab, choose **XML Mapping Pane**.</span></span>  
  
4.  <span data-ttu-id="86435-117">In the **XML Mapping** pane, in the **Custom XML Part** dropdown list, choose the custom XML part for ADD INCLUDE</span><span class="sxs-lookup"><span data-stu-id="86435-117">In the **XML Mapping** pane, in the **Custom XML Part** dropdown list, choose the custom XML part for ADD INCLUDE</span></span><!--[!INCLUDE[prod_short](../../includes/prod_short.md)]--> <span data-ttu-id="86435-118">report, which is typically last in the list.</span><span class="sxs-lookup"><span data-stu-id="86435-118">report, which is typically last in the list.</span></span> <span data-ttu-id="86435-119">The name of the custom XML part has the following format:</span><span class="sxs-lookup"><span data-stu-id="86435-119">The name of the custom XML part has the following format:</span></span>  
  
     <span data-ttu-id="86435-120">urn:microsoft-dynamics-nav/reports/*report_name*/*ID*</span><span class="sxs-lookup"><span data-stu-id="86435-120">urn:microsoft-dynamics-nav/reports/*report_name*/*ID*</span></span>  
  
     <span data-ttu-id="86435-121">*report_name* is the name that is assigned to the report</span><span class="sxs-lookup"><span data-stu-id="86435-121">*report_name* is the name that is assigned to the report</span></span><!--OnPrem as specified by the report's [Name Property-duplicate](../FullExperience/nav_dev_long_md.md)]--><span data-ttu-id="86435-122">.</span><span class="sxs-lookup"><span data-stu-id="86435-122">.</span></span>  
  
     <span data-ttu-id="86435-123">*ID* is the identification number of the report.</span><span class="sxs-lookup"><span data-stu-id="86435-123">*ID* is the identification number of the report.</span></span>  
  
     <span data-ttu-id="86435-124">After you select the custom XML part, the XML Mapping pane displays the labels and field controls that are available for the report.</span><span class="sxs-lookup"><span data-stu-id="86435-124">After you select the custom XML part, the XML Mapping pane displays the labels and field controls that are available for the report.</span></span>  
  
### <a name="to-add-a-label-or-data-field"></a><span data-ttu-id="86435-125">To add a label or data field</span><span class="sxs-lookup"><span data-stu-id="86435-125">To add a label or data field</span></span>  
  
1.  <span data-ttu-id="86435-126">Place your cursor in the document where you want to add the control.</span><span class="sxs-lookup"><span data-stu-id="86435-126">Place your cursor in the document where you want to add the control.</span></span>  
  
2.  <span data-ttu-id="86435-127">In the **XML Mapping** pane, right-click the control that you want to add, choose **Insert Content Control**, and then choose **Plain Text**.</span><span class="sxs-lookup"><span data-stu-id="86435-127">In the **XML Mapping** pane, right-click the control that you want to add, choose **Insert Content Control**, and then choose **Plain Text**.</span></span>  
  
    > [!NOTE]  
    >  <span data-ttu-id="86435-128">You cannot add a field by manually typing the dataset field name in the content control.</span><span class="sxs-lookup"><span data-stu-id="86435-128">You cannot add a field by manually typing the dataset field name in the content control.</span></span> <span data-ttu-id="86435-129">You must use the **XML Mapping** pane to map the fields.</span><span class="sxs-lookup"><span data-stu-id="86435-129">You must use the **XML Mapping** pane to map the fields.</span></span>  
  
### <a name="to-add-repeating-rows-of-data-fields-to-create-a-list"></a><span data-ttu-id="86435-130">To add repeating rows of data fields to create a list</span><span class="sxs-lookup"><span data-stu-id="86435-130">To add repeating rows of data fields to create a list</span></span>  
  
1.  <span data-ttu-id="86435-131">In a table, add a table row that includes a column for each field that you want repeated.</span><span class="sxs-lookup"><span data-stu-id="86435-131">In a table, add a table row that includes a column for each field that you want repeated.</span></span>  
  
     <span data-ttu-id="86435-132">This row will act as a placeholder for the repeating fields.</span><span class="sxs-lookup"><span data-stu-id="86435-132">This row will act as a placeholder for the repeating fields.</span></span>  
  
2.  <span data-ttu-id="86435-133">Select the entire row.</span><span class="sxs-lookup"><span data-stu-id="86435-133">Select the entire row.</span></span>  
  
3.  <span data-ttu-id="86435-134">In the **XML Mapping** pane, right-click the control that corresponds to the report data item that contains the fields that you want repeated, choose **Insert Content Control**, and then choose **Repeating**.</span><span class="sxs-lookup"><span data-stu-id="86435-134">In the **XML Mapping** pane, right-click the control that corresponds to the report data item that contains the fields that you want repeated, choose **Insert Content Control**, and then choose **Repeating**.</span></span>  
  
4.  <span data-ttu-id="86435-135">Add the repeating fields to the row as follows:</span><span class="sxs-lookup"><span data-stu-id="86435-135">Add the repeating fields to the row as follows:</span></span>  
  
    1.  <span data-ttu-id="86435-136">Place your pointer in a column.</span><span class="sxs-lookup"><span data-stu-id="86435-136">Place your pointer in a column.</span></span>  
  
    2.  <span data-ttu-id="86435-137">In the **XML Mapping** pane, right-click the control that you want to add, choose **Insert Content Control**, and then choose **Plain Text**.</span><span class="sxs-lookup"><span data-stu-id="86435-137">In the **XML Mapping** pane, right-click the control that you want to add, choose **Insert Content Control**, and then choose **Plain Text**.</span></span>  
  
    3.  <span data-ttu-id="86435-138">For each field, repeat steps a and b.</span><span class="sxs-lookup"><span data-stu-id="86435-138">For each field, repeat steps a and b.</span></span>  
  
## <a name="adding-image-fields"></a><span data-ttu-id="86435-139">Adding Image Fields</span><span class="sxs-lookup"><span data-stu-id="86435-139">Adding Image Fields</span></span>  
 <span data-ttu-id="86435-140">A report dataset can include a field that contains an image, such as a company logo or a picture of an item.</span><span class="sxs-lookup"><span data-stu-id="86435-140">A report dataset can include a field that contains an image, such as a company logo or a picture of an item.</span></span> <span data-ttu-id="86435-141">To add an image from the report dataset, you insert a **Picture** content control.</span><span class="sxs-lookup"><span data-stu-id="86435-141">To add an image from the report dataset, you insert a **Picture** content control.</span></span>  
  
 <span data-ttu-id="86435-142">Images align in the top-left corner of the content control and resize automatically in proportion to fit the boundary of the content control.</span><span class="sxs-lookup"><span data-stu-id="86435-142">Images align in the top-left corner of the content control and resize automatically in proportion to fit the boundary of the content control.</span></span>  
  
> [!IMPORTANT]  
>  <span data-ttu-id="86435-143">You can only add images that have a format that is supported by Word, such as .bmp, .jpeg, and .png file types.</span><span class="sxs-lookup"><span data-stu-id="86435-143">You can only add images that have a format that is supported by Word, such as .bmp, .jpeg, and .png file types.</span></span> <span data-ttu-id="86435-144">If you add an image that has a format that is not supported by Word, you will get an error when you run the report from the ADD INCLUDE</span><span class="sxs-lookup"><span data-stu-id="86435-144">If you add an image that has a format that is not supported by Word, you will get an error when you run the report from the ADD INCLUDE</span></span><!--[!INCLUDE[prod_short](../../includes/prod_short.md)]--> <span data-ttu-id="86435-145">client.</span><span class="sxs-lookup"><span data-stu-id="86435-145">client.</span></span>  
  
#### <a name="to-add-an-image"></a><span data-ttu-id="86435-146">To add an image</span><span class="sxs-lookup"><span data-stu-id="86435-146">To add an image</span></span>  
  
1.  <span data-ttu-id="86435-147">Place your pointer in the document where you want to add the control.</span><span class="sxs-lookup"><span data-stu-id="86435-147">Place your pointer in the document where you want to add the control.</span></span>  
  
2.  <span data-ttu-id="86435-148">In the **XML Mapping** pane, right-click the control that you want to add, choose **Insert Content Control**, and then choose **Picture**.</span><span class="sxs-lookup"><span data-stu-id="86435-148">In the **XML Mapping** pane, right-click the control that you want to add, choose **Insert Content Control**, and then choose **Picture**.</span></span>  
  
3.  <span data-ttu-id="86435-149">To increase or decrease the image size, drag a sizing handle away from or towards the centre of the content control.</span><span class="sxs-lookup"><span data-stu-id="86435-149">To increase or decrease the image size, drag a sizing handle away from or towards the center of the content control.</span></span>  

## <a name="custom-xml-part-overview"></a><span data-ttu-id="86435-150">Custom XML Part Overview</span><span class="sxs-lookup"><span data-stu-id="86435-150">Custom XML Part Overview</span></span>
<span data-ttu-id="86435-151">Word report layouts are built on *custom XML parts*.</span><span class="sxs-lookup"><span data-stu-id="86435-151">Word report layouts are built on *custom XML parts*.</span></span> <span data-ttu-id="86435-152">A custom XML part for a report consists of elements that correspond to the data items, columns, and labels that comprise the report's dataset.</span><span class="sxs-lookup"><span data-stu-id="86435-152">A custom XML part for a report consists of elements that correspond to the data items, columns, and labels that comprise the report's dataset.</span></span> <!--OnPrem The data as defined in the Report Dataset Designer in Microsoft Dynamics NAV Development Environment. --><span data-ttu-id="86435-153">The custom XML part is used to map the data into a report when the report is run.</span><span class="sxs-lookup"><span data-stu-id="86435-153">The custom XML part is used to map the data into a report when the report is run.</span></span>

  
### <a name="xml-structure-of-custom-xml-part"></a><span data-ttu-id="86435-154">XML Structure of Custom XML Part</span><span class="sxs-lookup"><span data-stu-id="86435-154">XML Structure of Custom XML Part</span></span>  
<span data-ttu-id="86435-155">The following table provides a simplified overview of the XML of a custom XML part.</span><span class="sxs-lookup"><span data-stu-id="86435-155">The following table provides a simplified overview of the XML of a custom XML part.</span></span>  
  
|<span data-ttu-id="86435-156">XML Elements</span><span class="sxs-lookup"><span data-stu-id="86435-156">XML Elements</span></span>|<span data-ttu-id="86435-157">Description</span><span class="sxs-lookup"><span data-stu-id="86435-157">Description</span></span>|  
|------------------|-----------------|  
|`<?xml version="1.0" encoding="utf-16"?>`|<span data-ttu-id="86435-158">Header</span><span class="sxs-lookup"><span data-stu-id="86435-158">Header</span></span>|  
|`<WordReportXmlPart xmlns="urn:microsoft-dynamics-365/report/<reportname>/<id>/"`|<span data-ttu-id="86435-159">XML namespace specification.</span><span class="sxs-lookup"><span data-stu-id="86435-159">XML namespace specification.</span></span> <span data-ttu-id="86435-160">`<reportname>` is the name that is assigned to the report.</span><span class="sxs-lookup"><span data-stu-id="86435-160">`<reportname>` is the name that is assigned to the report.</span></span> <span data-ttu-id="86435-161">`<id>` is the ID that is assigned to the report.</span><span class="sxs-lookup"><span data-stu-id="86435-161">`<id>` is the ID that is assigned to the report.</span></span>|  
|`..<Labels>`<br /><br /> `....<ColumnNameCaption>ColumnNameCaption</ColumnNameCaption>`<br /><br /> `....<LabelName>LabelCaption</LabelName>`<br /><br /> `..</Labels>`|<span data-ttu-id="86435-162">Contains all the labels for the report.</span><span class="sxs-lookup"><span data-stu-id="86435-162">Contains all the labels for the report.</span></span><!--OnPren The element includes labels that are related to columns that have the IncludeCaption Property.--><br /><span data-ttu-id="86435-163">-   Label elements that are related to columns have the format `<ColumnNameCaption>ColumnNameCaption</ColumnNameCaption>`</span><span class="sxs-lookup"><span data-stu-id="86435-163">-   Label elements that are related to columns have the format `<ColumnNameCaption>ColumnNameCaption</ColumnNameCaption>`</span></span><!--OnPrem where `ColumnName` is determined by the column's Name Property.--><span data-ttu-id="86435-164">.</span><span class="sxs-lookup"><span data-stu-id="86435-164">.</span></span><br /><span data-ttu-id="86435-165">-  Label elements have the format `<LabelName>LabelName</LabelName`</span><span class="sxs-lookup"><span data-stu-id="86435-165">-  Label elements have the format `<LabelName>LabelName</LabelName`</span></span><!--OnPrem where LabelName is determined by the label's Name Property.--><span data-ttu-id="86435-166">.</span><span class="sxs-lookup"><span data-stu-id="86435-166">.</span></span><br /><span data-ttu-id="86435-167">-   Labels are listed in alphabetical order.</span><span class="sxs-lookup"><span data-stu-id="86435-167">-   Labels are listed in alphabetical order.</span></span>|  
|`..<DataItem1>`<br /><br /> `....<DataItem1Column1>DataItem1Column1</DataItem1Column1>`|<span data-ttu-id="86435-168">Top-level data item and columns.</span><span class="sxs-lookup"><span data-stu-id="86435-168">Top-level data item and columns.</span></span> <span data-ttu-id="86435-169">Columns are listed in alphabetical order.</span><span class="sxs-lookup"><span data-stu-id="86435-169">Columns are listed in alphabetical order.</span></span><!--OnPrem <br /><br /> The element names and values are determined by the Name Property of the data item or column.-->|  
|`....<DataItem2>`<br /><br /> `......<DataItem2Column1>DataItem2Column1</DataItem2Column1>`<br /><br /> `....</DataItem2>`<br /><br /> `....<DataItem3>`<br /><br /> `......<DataItem3Column1>DataItem3Column1</DataItem3Column1>`<br /><br /> `....</DataItem3>`|<span data-ttu-id="86435-170">Data items and columns that are nested in the top-level data item.</span><span class="sxs-lookup"><span data-stu-id="86435-170">Data items and columns that are nested in the top-level data item.</span></span> <span data-ttu-id="86435-171">Columns are listed in alphabetical order under the respective data item.</span><span class="sxs-lookup"><span data-stu-id="86435-171">Columns are listed in alphabetical order under the respective data item.</span></span>|  
|`..</DataItem1>`<br /><br /> `</WordReportXmlPart>`|<span data-ttu-id="86435-172">Closing element.</span><span class="sxs-lookup"><span data-stu-id="86435-172">Closing element.</span></span>|  
  
### <a name="custom-xml-part-in-word"></a><span data-ttu-id="86435-173">Custom XML Part in Word</span><span class="sxs-lookup"><span data-stu-id="86435-173">Custom XML Part in Word</span></span>  
 <span data-ttu-id="86435-174">In Word, you open the custom XML part in the **XML Mapping** pane, and then use the pane to map elements to content controls in the Word document.</span><span class="sxs-lookup"><span data-stu-id="86435-174">In Word, you open the custom XML part in the **XML Mapping** pane, and then use the pane to map elements to content controls in the Word document.</span></span> <span data-ttu-id="86435-175">The **XML Mapping** pane is accessible from the **Developer** tab (for more information, see [Show the Developer Tab on the Ribbon](/visualstudio/vsto/how-to-show-the-developer-tab-on-the-ribbon)).</span><span class="sxs-lookup"><span data-stu-id="86435-175">The **XML Mapping** pane is accessible from the **Developer** tab (for more information, see [Show the Developer Tab on the Ribbon](/visualstudio/vsto/how-to-show-the-developer-tab-on-the-ribbon)).</span></span>  
  
 <span data-ttu-id="86435-176">The elements in the **XML Mapping** pane appear in a structure that is similar to the XML source.</span><span class="sxs-lookup"><span data-stu-id="86435-176">The elements in the **XML Mapping** pane appear in a structure that is similar to the XML source.</span></span> <span data-ttu-id="86435-177">Label fields are grouped under a common **Labels** element and data item and columns are arranged in a hierarchal structure that corresponds to the XML source, with columns listed in alphabetical order.</span><span class="sxs-lookup"><span data-stu-id="86435-177">Label fields are grouped under a common **Labels** element and data item and columns are arranged in a hierarchal structure that corresponds to the XML source, with columns listed in alphabetical order.</span></span> <span data-ttu-id="86435-178">Elements are identified by their name as defined by the Name property in Report Dataset Designer in ADD INCLUDE</span><span class="sxs-lookup"><span data-stu-id="86435-178">Elements are identified by their name as defined by the Name property in Report Dataset Designer in ADD INCLUDE</span></span><!--[!INCLUDE[nav_dev_short](../../includes/nav_dev_short_md.md)]--><span data-ttu-id="86435-179">.</span><span class="sxs-lookup"><span data-stu-id="86435-179">.</span></span>  
  
 <span data-ttu-id="86435-180">The following figure illustrates the simple custom XML part from the previous section in the **XML Mapping** pane of a Word document.</span><span class="sxs-lookup"><span data-stu-id="86435-180">The following figure illustrates the simple custom XML part from the previous section in the **XML Mapping** pane of a Word document.</span></span>  
  
 <span data-ttu-id="86435-181">![Clip of the XML Mapping pane in word](media/nav_reportlayout_xmlmappingpane.png "NAV_ReportLayout_XMLMappingPane")</span><span class="sxs-lookup"><span data-stu-id="86435-181">![Clip of the XML Mapping pane in word](media/nav_reportlayout_xmlmappingpane.png "NAV_ReportLayout_XMLMappingPane")</span></span>  
  
-   <span data-ttu-id="86435-182">To add a label or field to the layout, you insert a content control that maps to the element in the **XML Mapping** pane.</span><span class="sxs-lookup"><span data-stu-id="86435-182">To add a label or field to the layout, you insert a content control that maps to the element in the **XML Mapping** pane.</span></span>  
  
-   <span data-ttu-id="86435-183">To create repeating rows of columns, insert a **Repeating** content control for the parent data item element, and then add content control for the columns.</span><span class="sxs-lookup"><span data-stu-id="86435-183">To create repeating rows of columns, insert a **Repeating** content control for the parent data item element, and then add content control for the columns.</span></span>  
  
-   <span data-ttu-id="86435-184">For labels, the actual text that appears in the generated report is the value of the **Caption** property for the field in the data item table (if the label is related to the column in the report dataset) or a label in the Report Label Designer (if the label is not related to a column in the dataset).</span><span class="sxs-lookup"><span data-stu-id="86435-184">For labels, the actual text that appears in the generated report is the value of the **Caption** property for the field in the data item table (if the label is related to the column in the report dataset) or a label in the Report Label Designer (if the label is not related to a column in the dataset).</span></span>  
  
-   <span data-ttu-id="86435-185">The language of the label that is displayed when you run the report depends on the language setting of the report object.</span><span class="sxs-lookup"><span data-stu-id="86435-185">The language of the label that is displayed when you run the report depends on the language setting of the report object.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="86435-186">See Also</span><span class="sxs-lookup"><span data-stu-id="86435-186">See Also</span></span>  
 [<span data-ttu-id="86435-187">Create and Modify a Custom Report Layout</span><span class="sxs-lookup"><span data-stu-id="86435-187">Create and Modify a Custom Report Layout</span></span>](ui-how-create-custom-report-layout.md)   


[!INCLUDE[footer-include](includes/footer-banner.md)]