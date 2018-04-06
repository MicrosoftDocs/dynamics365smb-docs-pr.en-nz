---
title: Prepare Customer Data Migration | Microsoft Docs
description: "After you import and apply setup data in the new database, you can start migrating the customer’s existing master data, such as item and customer numbers and names. To make sure that this data is created quickly and accurately in the new company, you should use templates to structure the data."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 03/07/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 3cfc53c1ea3c8d30f65b2d475a8dab052519e81e
ms.contentlocale: en-nz
ms.lasthandoff: 03/22/2018

---
# <a name="prepare-to-migrate-customer-data"></a><span data-ttu-id="e3b32-104">Prepare to Migrate Customer Data</span><span class="sxs-lookup"><span data-stu-id="e3b32-104">Prepare to Migrate Customer Data</span></span>
<span data-ttu-id="e3b32-105">After you import and apply setup data in the new database, you can start migrating the customer’s existing master data, such as item and customer numbers and names.</span><span class="sxs-lookup"><span data-stu-id="e3b32-105">After you import and apply setup data in the new database, you can start migrating the customer’s existing master data, such as item and customer numbers and names.</span></span> <span data-ttu-id="e3b32-106">To make sure that this data is created quickly and accurately in the new company, you should use templates to structure the data.</span><span class="sxs-lookup"><span data-stu-id="e3b32-106">To make sure that this data is created quickly and accurately in the new company, you should use templates to structure the data.</span></span>  

<span data-ttu-id="e3b32-107">Typically, you create data templates for the following master data tables:</span><span class="sxs-lookup"><span data-stu-id="e3b32-107">Typically, you create data templates for the following master data tables:</span></span>  

-   <span data-ttu-id="e3b32-108">**Contact**</span><span class="sxs-lookup"><span data-stu-id="e3b32-108">**Contact**</span></span>  
-   <span data-ttu-id="e3b32-109">**Customer**</span><span class="sxs-lookup"><span data-stu-id="e3b32-109">**Customer**</span></span>  
-   <span data-ttu-id="e3b32-110">**Item**</span><span class="sxs-lookup"><span data-stu-id="e3b32-110">**Item**</span></span>  
-   <span data-ttu-id="e3b32-111">**Vendor**</span><span class="sxs-lookup"><span data-stu-id="e3b32-111">**Vendor**</span></span>  

<span data-ttu-id="e3b32-112">However, you can create a template structure for and apply it to any table in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="e3b32-112">However, you can create a template structure for and apply it to any table in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  

> [!TIP]  
>  <span data-ttu-id="e3b32-113">You can also use data templates for daily operations to create new records that are based on templates.</span><span class="sxs-lookup"><span data-stu-id="e3b32-113">You can also use data templates for daily operations to create new records that are based on templates.</span></span> <span data-ttu-id="e3b32-114">These data templates only work for the supported master data tables.</span><span class="sxs-lookup"><span data-stu-id="e3b32-114">These data templates only work for the supported master data tables.</span></span> <span data-ttu-id="e3b32-115">For more information, see, for example, [Register New Items](inventory-how-register-new-items.md).</span><span class="sxs-lookup"><span data-stu-id="e3b32-115">For more information, see, for example, [Register New Items](inventory-how-register-new-items.md).</span></span>  

<span data-ttu-id="e3b32-116">When you import customer data, such as for items, from a file, the mandatory field data that you have specified is taken from the linked data template.</span><span class="sxs-lookup"><span data-stu-id="e3b32-116">When you import customer data, such as for items, from a file, the mandatory field data that you have specified is taken from the linked data template.</span></span> <span data-ttu-id="e3b32-117">When you create a new item, you only enter general information such as item name, description, and price and then collect the rest of the mandatory field data from a selected data template.</span><span class="sxs-lookup"><span data-stu-id="e3b32-117">When you create a new item, you only enter general information such as item name, description, and price and then collect the rest of the mandatory field data from a selected data template.</span></span>  

<span data-ttu-id="e3b32-118">When you create a new master data record, such as a customer card, some fields are mandatory and must be filled in.</span><span class="sxs-lookup"><span data-stu-id="e3b32-118">When you create a new master data record, such as a customer card, some fields are mandatory and must be filled in.</span></span> <span data-ttu-id="e3b32-119">You can group most mandatory fields, such as posting groups and payment terms, to make creating master data records easier and more stable.</span><span class="sxs-lookup"><span data-stu-id="e3b32-119">You can group most mandatory fields, such as posting groups and payment terms, to make creating master data records easier and more stable.</span></span> <span data-ttu-id="e3b32-120">For example, you can group mandatory fields for table 18, **Customer**, as **Domestic**, **Foreign**, or **Export** types.</span><span class="sxs-lookup"><span data-stu-id="e3b32-120">For example, you can group mandatory fields for table 18, **Customer**, as **Domestic**, **Foreign**, or **Export** types.</span></span>

## <a name="to-select-a-data-template"></a><span data-ttu-id="e3b32-121">To select a data template</span><span class="sxs-lookup"><span data-stu-id="e3b32-121">To select a data template</span></span>
<span data-ttu-id="e3b32-122">When you select an existing data template, you must evaluate if the templates that you created for the new company are sufficient for the customer.</span><span class="sxs-lookup"><span data-stu-id="e3b32-122">When you select an existing data template, you must evaluate if the templates that you created for the new company are sufficient for the customer.</span></span> <span data-ttu-id="e3b32-123">Review the provided fields and values to determine which templates are appropriate for a new company.</span><span class="sxs-lookup"><span data-stu-id="e3b32-123">Review the provided fields and values to determine which templates are appropriate for a new company.</span></span>  

> [!TIP]  
>  <span data-ttu-id="e3b32-124">You can also use data templates to create new records quickly.</span><span class="sxs-lookup"><span data-stu-id="e3b32-124">You can also use data templates to create new records quickly.</span></span> <span data-ttu-id="e3b32-125">Use them for faster and more accurate data creation.</span><span class="sxs-lookup"><span data-stu-id="e3b32-125">Use them for faster and more accurate data creation.</span></span> <span data-ttu-id="e3b32-126">For more information, see [Register New Items](inventory-how-register-new-items.md).</span><span class="sxs-lookup"><span data-stu-id="e3b32-126">For more information, see [Register New Items](inventory-how-register-new-items.md).</span></span>

1. <span data-ttu-id="e3b32-127">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Configuration Templates**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="e3b32-127">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Configuration Templates**, and then choose the related link.</span></span>  
2. <span data-ttu-id="e3b32-128">In the **Config. Template List** window, select a data template from the list, and then choose the **Edit** action.</span><span class="sxs-lookup"><span data-stu-id="e3b32-128">In the **Config. Template List** window, select a data template from the list, and then choose the **Edit** action.</span></span>  

<span data-ttu-id="e3b32-129">If the default templates do not meet your needs, you can create new templates or add fields to an existing template.</span><span class="sxs-lookup"><span data-stu-id="e3b32-129">If the default templates do not meet your needs, you can create new templates or add fields to an existing template.</span></span> <span data-ttu-id="e3b32-130">If the default templates are sufficient, you can use them to create records based on master data templates.</span><span class="sxs-lookup"><span data-stu-id="e3b32-130">If the default templates are sufficient, you can use them to create records based on master data templates.</span></span>

## <a name="to-create-a-data-template"></a><span data-ttu-id="e3b32-131">To create a data template</span><span class="sxs-lookup"><span data-stu-id="e3b32-131">To create a data template</span></span>
<span data-ttu-id="e3b32-132">You can create a new data template if the default templates do not the needs of your new company.</span><span class="sxs-lookup"><span data-stu-id="e3b32-132">You can create a new data template if the default templates do not the needs of your new company.</span></span> <span data-ttu-id="e3b32-133">If you are creating more than one, you may find it useful to adopt a naming convention for the **Code** field.</span><span class="sxs-lookup"><span data-stu-id="e3b32-133">If you are creating more than one, you may find it useful to adopt a naming convention for the **Code** field.</span></span>

<span data-ttu-id="e3b32-134">Each template consists of a header and lines.</span><span class="sxs-lookup"><span data-stu-id="e3b32-134">Each template consists of a header and lines.</span></span> <span data-ttu-id="e3b32-135">When you create a template, you can specify which fields to always apply to data of a certain type.</span><span class="sxs-lookup"><span data-stu-id="e3b32-135">When you create a template, you can specify which fields to always apply to data of a certain type.</span></span> <span data-ttu-id="e3b32-136">For example, you can create different customer templates to apply to different customer types.</span><span class="sxs-lookup"><span data-stu-id="e3b32-136">For example, you can create different customer templates to apply to different customer types.</span></span> <span data-ttu-id="e3b32-137">When you create the customer using a template, you can use template data to prepopulate certain fields.</span><span class="sxs-lookup"><span data-stu-id="e3b32-137">When you create the customer using a template, you can use template data to prepopulate certain fields.</span></span>

### <a name="to-create-a-data-template-header"></a><span data-ttu-id="e3b32-138">To create a data template header</span><span class="sxs-lookup"><span data-stu-id="e3b32-138">To create a data template header</span></span>
1. <span data-ttu-id="e3b32-139">Open the **Config. Template List** window.</span><span class="sxs-lookup"><span data-stu-id="e3b32-139">Open the **Config. Template List** window.</span></span>
2. <span data-ttu-id="e3b32-140">Choose the **New** action.</span><span class="sxs-lookup"><span data-stu-id="e3b32-140">Choose the **New** action.</span></span>
3. <span data-ttu-id="e3b32-141">In the **Table ID** field, enter the table to which this template applies.</span><span class="sxs-lookup"><span data-stu-id="e3b32-141">In the **Table ID** field, enter the table to which this template applies.</span></span> <span data-ttu-id="e3b32-142">The **Table Name** field is automatically filled in when the **Table ID** field is set.</span><span class="sxs-lookup"><span data-stu-id="e3b32-142">The **Table Name** field is automatically filled in when the **Table ID** field is set.</span></span>

### <a name="to-create-a-data-template-line"></a><span data-ttu-id="e3b32-143">To create a data template line</span><span class="sxs-lookup"><span data-stu-id="e3b32-143">To create a data template line</span></span>
1. <span data-ttu-id="e3b32-144">On the first line, select the **Field Name** field.</span><span class="sxs-lookup"><span data-stu-id="e3b32-144">On the first line, select the **Field Name** field.</span></span> <span data-ttu-id="e3b32-145">The **Field List** window displays the list of fields in the table.</span><span class="sxs-lookup"><span data-stu-id="e3b32-145">The **Field List** window displays the list of fields in the table.</span></span>
2. <span data-ttu-id="e3b32-146">Select a field, and then choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="e3b32-146">Select a field, and then choose the **OK** button.</span></span> <span data-ttu-id="e3b32-147">The **Field Caption** field is filled in with the field name.</span><span class="sxs-lookup"><span data-stu-id="e3b32-147">The **Field Caption** field is filled in with the field name.</span></span>
3. <span data-ttu-id="e3b32-148">In the **Default Value** field, enter an appropriate value.</span><span class="sxs-lookup"><span data-stu-id="e3b32-148">In the **Default Value** field, enter an appropriate value.</span></span> <span data-ttu-id="e3b32-149">In some cases, you may want to use a value that is not a value that is available in the database.</span><span class="sxs-lookup"><span data-stu-id="e3b32-149">In some cases, you may want to use a value that is not a value that is available in the database.</span></span> <span data-ttu-id="e3b32-150">In that case, you can select the **Skip Relation Check** check box, to make it possible to apply data without error.</span><span class="sxs-lookup"><span data-stu-id="e3b32-150">In that case, you can select the **Skip Relation Check** check box, to make it possible to apply data without error.</span></span>

    > [!TIP]  
    > <span data-ttu-id="e3b32-151">Since the **Default Value** field does not have a look up to the corresponding [!INCLUDE[d365fin](includes/d365fin_md.md)] field options, you copy and paste the value that you want from the related page into the template.</span><span class="sxs-lookup"><span data-stu-id="e3b32-151">Since the **Default Value** field does not have a look up to the corresponding [!INCLUDE[d365fin](includes/d365fin_md.md)] field options, you copy and paste the value that you want from the related page into the template.</span></span>

    > <span data-ttu-id="e3b32-152">Select the **Mandatory** check box.</span><span class="sxs-lookup"><span data-stu-id="e3b32-152">Select the **Mandatory** check box.</span></span> <span data-ttu-id="e3b32-153">The check box is informational only.</span><span class="sxs-lookup"><span data-stu-id="e3b32-153">The check box is informational only.</span></span> <span data-ttu-id="e3b32-154">It tells you that information must be entered in the field by the user, but no business logic is enforced.</span><span class="sxs-lookup"><span data-stu-id="e3b32-154">It tells you that information must be entered in the field by the user, but no business logic is enforced.</span></span> <span data-ttu-id="e3b32-155">For example, you cannot invoice and post an order if posting groups have not been set up.</span><span class="sxs-lookup"><span data-stu-id="e3b32-155">For example, you cannot invoice and post an order if posting groups have not been set up.</span></span> <span data-ttu-id="e3b32-156">Since posting groups are required, you can select the **Mandatory** check box for those fields.</span><span class="sxs-lookup"><span data-stu-id="e3b32-156">Since posting groups are required, you can select the **Mandatory** check box for those fields.</span></span>

3. <span data-ttu-id="e3b32-157">In the **Reference** field, enter information about the field as needed.</span><span class="sxs-lookup"><span data-stu-id="e3b32-157">In the **Reference** field, enter information about the field as needed.</span></span>
4. <span data-ttu-id="e3b32-158">Choose the **OK** button</span><span class="sxs-lookup"><span data-stu-id="e3b32-158">Choose the **OK** button</span></span>

## <a name="to-export-to-a-template-in-excel"></a><span data-ttu-id="e3b32-159">To export to a template in Excel</span><span class="sxs-lookup"><span data-stu-id="e3b32-159">To export to a template in Excel</span></span>
<span data-ttu-id="e3b32-160">You can create an Excel workbook to serve as a template that is based on the structure of an existing database table quickly.</span><span class="sxs-lookup"><span data-stu-id="e3b32-160">You can create an Excel workbook to serve as a template that is based on the structure of an existing database table quickly.</span></span> <span data-ttu-id="e3b32-161">You can then use the template to gather together customer data in a consistent format for later import into [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="e3b32-161">You can then use the template to gather together customer data in a consistent format for later import into [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>

1. <span data-ttu-id="e3b32-162">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Configuration Worksheet**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="e3b32-162">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Configuration Worksheet**, and then choose the related link.</span></span>
2. <span data-ttu-id="e3b32-163">Add a table to the list, or select an existing table.</span><span class="sxs-lookup"><span data-stu-id="e3b32-163">Add a table to the list, or select an existing table.</span></span> <span data-ttu-id="e3b32-164">For more information, see [Manage Company Configuration in a Worksheet](admin-how-to-manage-company-configuration-in-a-worksheet.md).</span><span class="sxs-lookup"><span data-stu-id="e3b32-164">For more information, see [Manage Company Configuration in a Worksheet](admin-how-to-manage-company-configuration-in-a-worksheet.md).</span></span>
3. <span data-ttu-id="e3b32-165">Define the fields from the table that you want to include in the template.</span><span class="sxs-lookup"><span data-stu-id="e3b32-165">Define the fields from the table that you want to include in the template.</span></span>
4. <span data-ttu-id="e3b32-166">Choose the **Export to Template** action.</span><span class="sxs-lookup"><span data-stu-id="e3b32-166">Choose the **Export to Template** action.</span></span>
5. <span data-ttu-id="e3b32-167">Name and save the Excel file.</span><span class="sxs-lookup"><span data-stu-id="e3b32-167">Name and save the Excel file.</span></span> <span data-ttu-id="e3b32-168">The Excel workbook is automatically opened.</span><span class="sxs-lookup"><span data-stu-id="e3b32-168">The Excel workbook is automatically opened.</span></span>

<span data-ttu-id="e3b32-169">You can now enter customer data in the Excel worksheet.</span><span class="sxs-lookup"><span data-stu-id="e3b32-169">You can now enter customer data in the Excel worksheet.</span></span> <span data-ttu-id="e3b32-170">If you have exported multiple tables, each table will be on its own worksheet.</span><span class="sxs-lookup"><span data-stu-id="e3b32-170">If you have exported multiple tables, each table will be on its own worksheet.</span></span> <span data-ttu-id="e3b32-171">Save the workbook before you continue with the next procedure.</span><span class="sxs-lookup"><span data-stu-id="e3b32-171">Save the workbook before you continue with the next procedure.</span></span>

> [!NOTE]  
> <span data-ttu-id="e3b32-172">You may encounter the following error when you run an English version of Excel, but have your regional settings configured for a non-English language: "Old format or invalid type library."</span><span class="sxs-lookup"><span data-stu-id="e3b32-172">You may encounter the following error when you run an English version of Excel, but have your regional settings configured for a non-English language: "Old format or invalid type library."</span></span> <span data-ttu-id="e3b32-173">To fix this error, make sure that the language pack for the non-English language is installed.</span><span class="sxs-lookup"><span data-stu-id="e3b32-173">To fix this error, make sure that the language pack for the non-English language is installed.</span></span>

## <a name="to-import-from-a-template-in-excel"></a><span data-ttu-id="e3b32-174">To import from a template in Excel</span><span class="sxs-lookup"><span data-stu-id="e3b32-174">To import from a template in Excel</span></span>
1. <span data-ttu-id="e3b32-175">In the **Config. Worksheet** window, choose the **Import from Template** action.</span><span class="sxs-lookup"><span data-stu-id="e3b32-175">In the **Config. Worksheet** window, choose the **Import from Template** action.</span></span>
3. <span data-ttu-id="e3b32-176">Navigate to the template worksheet that you have created, and then choose the **Open** action.</span><span class="sxs-lookup"><span data-stu-id="e3b32-176">Navigate to the template worksheet that you have created, and then choose the **Open** action.</span></span>
4. <span data-ttu-id="e3b32-177">To add the collected customer data to the database, choose the **Apply Data** action.</span><span class="sxs-lookup"><span data-stu-id="e3b32-177">To add the collected customer data to the database, choose the **Apply Data** action.</span></span>

<span data-ttu-id="e3b32-178">When you apply data from a template in Excel to a table that also has a configuration template linked to it in the configuration package, the default field values from the configuration template are also applied.</span><span class="sxs-lookup"><span data-stu-id="e3b32-178">When you apply data from a template in Excel to a table that also has a configuration template linked to it in the configuration package, the default field values from the configuration template are also applied.</span></span>

<span data-ttu-id="e3b32-179">Any record whose data is applied in this manner is complete, because it consists of data entered by a user in Excel, plus the default values specified by the configuration template.</span><span class="sxs-lookup"><span data-stu-id="e3b32-179">Any record whose data is applied in this manner is complete, because it consists of data entered by a user in Excel, plus the default values specified by the configuration template.</span></span>

## <a name="to-create-a-record-from-a-configuration-template"></a><span data-ttu-id="e3b32-180">To create a record from a configuration template</span><span class="sxs-lookup"><span data-stu-id="e3b32-180">To create a record from a configuration template</span></span>
<span data-ttu-id="e3b32-181">You can use the structure of data that is contained in the data templates to convert your information into records in the database, one-by-one.</span><span class="sxs-lookup"><span data-stu-id="e3b32-181">You can use the structure of data that is contained in the data templates to convert your information into records in the database, one-by-one.</span></span> <span data-ttu-id="e3b32-182">To do so, you use the **Create Instance** function.</span><span class="sxs-lookup"><span data-stu-id="e3b32-182">To do so, you use the **Create Instance** function.</span></span> <span data-ttu-id="e3b32-183">This is a miniature version of the data migration process and can be useful for prototyping or treating smaller data creation tasks.</span><span class="sxs-lookup"><span data-stu-id="e3b32-183">This is a miniature version of the data migration process and can be useful for prototyping or treating smaller data creation tasks.</span></span>  

<span data-ttu-id="e3b32-184">The following steps illustrate how to create an item card from an item data template.</span><span class="sxs-lookup"><span data-stu-id="e3b32-184">The following steps illustrate how to create an item card from an item data template.</span></span> <span data-ttu-id="e3b32-185">You can create a record from any data template using the same procedure.</span><span class="sxs-lookup"><span data-stu-id="e3b32-185">You can create a record from any data template using the same procedure.</span></span>  

1. <span data-ttu-id="e3b32-186">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Configuration Templates**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="e3b32-186">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Configuration Templates**, and then choose the related link.</span></span>  
2. <span data-ttu-id="e3b32-187">Select the **Item** template, and then choose the **Edit** action.</span><span class="sxs-lookup"><span data-stu-id="e3b32-187">Select the **Item** template, and then choose the **Edit** action.</span></span> <span data-ttu-id="e3b32-188">For more information, see the "To create a data template" section.</span><span class="sxs-lookup"><span data-stu-id="e3b32-188">For more information, see the "To create a data template" section.</span></span>
3. <span data-ttu-id="e3b32-189">Choose the **Create Instance** action.</span><span class="sxs-lookup"><span data-stu-id="e3b32-189">Choose the **Create Instance** action.</span></span> <span data-ttu-id="e3b32-190">An item card is created.</span><span class="sxs-lookup"><span data-stu-id="e3b32-190">An item card is created.</span></span>  
4. <span data-ttu-id="e3b32-191">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="e3b32-191">Choose the **OK** button.</span></span>  
5. <span data-ttu-id="e3b32-192">To review the new item card, choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Items**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="e3b32-192">To review the new item card, choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Items**, and then choose the related link.</span></span>  
6. <span data-ttu-id="e3b32-193">Open the new item card.</span><span class="sxs-lookup"><span data-stu-id="e3b32-193">Open the new item card.</span></span>  
7. <span data-ttu-id="e3b32-194">Expand various FastTabs, and verify that the information was created correctly on them.</span><span class="sxs-lookup"><span data-stu-id="e3b32-194">Expand various FastTabs, and verify that the information was created correctly on them.</span></span>  

## <a name="to-use-a-configuration-template-on-a-record"></a><span data-ttu-id="e3b32-195">To use a configuration template on a record</span><span class="sxs-lookup"><span data-stu-id="e3b32-195">To use a configuration template on a record</span></span>
<span data-ttu-id="e3b32-196">You can apply a data template to any record that is in [!INCLUDE[d365fin](includes/d365fin_md.md)] and use this technique to change or modify a record.</span><span class="sxs-lookup"><span data-stu-id="e3b32-196">You can apply a data template to any record that is in [!INCLUDE[d365fin](includes/d365fin_md.md)] and use this technique to change or modify a record.</span></span> <span data-ttu-id="e3b32-197">However, when you do this, you overwrite existing values in the record with those of the template.</span><span class="sxs-lookup"><span data-stu-id="e3b32-197">However, when you do this, you overwrite existing values in the record with those of the template.</span></span> <span data-ttu-id="e3b32-198">Consequently, you should be careful when you apply a template to existing records.</span><span class="sxs-lookup"><span data-stu-id="e3b32-198">Consequently, you should be careful when you apply a template to existing records.</span></span>

> [!WARNING]  
>  <span data-ttu-id="e3b32-199">The **Apply Template** function overwrites existing data in a record.</span><span class="sxs-lookup"><span data-stu-id="e3b32-199">The **Apply Template** function overwrites existing data in a record.</span></span> <span data-ttu-id="e3b32-200">If this function is used in master data migration, it will overwrite the imported data when you create records.</span><span class="sxs-lookup"><span data-stu-id="e3b32-200">If this function is used in master data migration, it will overwrite the imported data when you create records.</span></span>

<span data-ttu-id="e3b32-201">The following procedure is based on a new customer card.</span><span class="sxs-lookup"><span data-stu-id="e3b32-201">The following procedure is based on a new customer card.</span></span>  

1. <span data-ttu-id="e3b32-202">Create a customer.</span><span class="sxs-lookup"><span data-stu-id="e3b32-202">Create a customer.</span></span> <span data-ttu-id="e3b32-203">For more information, see [Register New Customers](sales-how-register-new-customers.md).</span><span class="sxs-lookup"><span data-stu-id="e3b32-203">For more information, see [Register New Customers](sales-how-register-new-customers.md).</span></span>
2. <span data-ttu-id="e3b32-204">In the **Customer Card** window, choose the **Apply Template** action.</span><span class="sxs-lookup"><span data-stu-id="e3b32-204">In the **Customer Card** window, choose the **Apply Template** action.</span></span>  
3. <span data-ttu-id="e3b32-205">In the **Customer Templates** window, select one of the templates, and then choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="e3b32-205">In the **Customer Templates** window, select one of the templates, and then choose the **OK** button.</span></span>  

<span data-ttu-id="e3b32-206">The default values from the chosen customer template are inserted on the customer card.</span><span class="sxs-lookup"><span data-stu-id="e3b32-206">The default values from the chosen customer template are inserted on the customer card.</span></span>

## <a name="see-also"></a><span data-ttu-id="e3b32-207">See Also</span><span class="sxs-lookup"><span data-stu-id="e3b32-207">See Also</span></span>  
[<span data-ttu-id="e3b32-208">Setting Up a Company With RapidStart Services</span><span class="sxs-lookup"><span data-stu-id="e3b32-208">Setting Up a Company With RapidStart Services</span></span>](admin-set-up-a-company-with-rapidstart.md)  
[<span data-ttu-id="e3b32-209">Administration</span><span class="sxs-lookup"><span data-stu-id="e3b32-209">Administration</span></span>](admin-setup-and-administration.md)  
[<span data-ttu-id="e3b32-210">Register New Customers</span><span class="sxs-lookup"><span data-stu-id="e3b32-210">Register New Customers</span></span>](sales-how-register-new-customers.md)
