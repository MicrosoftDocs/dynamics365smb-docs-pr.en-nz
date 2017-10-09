---
title: Use Excel to import data into Financials| Microsoft Docs
description: Use the default configuration package to add customer data in Excel and import the data back into Dynamics 365 for Financials.
author: edupont04
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: migration, Excel
ms.date: 07/05/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 2a38dc36cb9ff609c5582acd489841b20013d4bc
ms.openlocfilehash: 8cf36afea60b089afac8f1c27d126cd19b88ce94
ms.contentlocale: en-nz
ms.lasthandoff: 09/22/2017

---
# <a name="importing-data-from-legacy-accounting-software-using-a-configuration-package"></a><span data-ttu-id="b9924-103">Importing Data from Legacy Accounting Software using a Configuration Package</span><span class="sxs-lookup"><span data-stu-id="b9924-103">Importing Data from Legacy Accounting Software using a Configuration Package</span></span>
<span data-ttu-id="b9924-104">You can import master data and some transactional data from other finance systems based on the default configuration package in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="b9924-104">You can import master data and some transactional data from other finance systems based on the default configuration package in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="b9924-105">In the **Configuration Packages** window, you can work with the package to import and validate the data before you apply the package.</span><span class="sxs-lookup"><span data-stu-id="b9924-105">In the **Configuration Packages** window, you can work with the package to import and validate the data before you apply the package.</span></span>  

<span data-ttu-id="b9924-106">If you are familiar with RapidStart Services for Microsoft Dynamics, you are also familiar with configuration packages.</span><span class="sxs-lookup"><span data-stu-id="b9924-106">If you are familiar with RapidStart Services for Microsoft Dynamics, you are also familiar with configuration packages.</span></span> <span data-ttu-id="b9924-107">The default configuration package supports the most common types of data that you want to import from a legacy system.</span><span class="sxs-lookup"><span data-stu-id="b9924-107">The default configuration package supports the most common types of data that you want to import from a legacy system.</span></span> <span data-ttu-id="b9924-108">In Excel, you can then add the data from the legacy system and set it up according to the business logic of the [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="b9924-108">In Excel, you can then add the data from the legacy system and set it up according to the business logic of the [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  

> [!TIP]  
>   <span data-ttu-id="b9924-109">Alternatively, use data migration wizards to import data from QuickBooks or Dynamics GP.</span><span class="sxs-lookup"><span data-stu-id="b9924-109">Alternatively, use data migration wizards to import data from QuickBooks or Dynamics GP.</span></span> <span data-ttu-id="b9924-110">For more information, see [QuickBooks Data Migration](ui-extensions-quickbooks-data-migration.md) or [Dynamics GP Data Migration](ui-extensions-dynamicsgp-data-migration.md).</span><span class="sxs-lookup"><span data-stu-id="b9924-110">For more information, see [QuickBooks Data Migration](ui-extensions-quickbooks-data-migration.md) or [Dynamics GP Data Migration](ui-extensions-dynamicsgp-data-migration.md).</span></span>  

## <a name="working-with-data-in-excel"></a><span data-ttu-id="b9924-111">Working with Data in Excel</span><span class="sxs-lookup"><span data-stu-id="b9924-111">Working with Data in Excel</span></span>
<span data-ttu-id="b9924-112">When you export the default configuration package to Excel, the generated workbook contains a worksheet for each table in the package.</span><span class="sxs-lookup"><span data-stu-id="b9924-112">When you export the default configuration package to Excel, the generated workbook contains a worksheet for each table in the package.</span></span> <span data-ttu-id="b9924-113">To simplify your tasks, you can take advantage of the XML manipulation tools that are built into Excel.</span><span class="sxs-lookup"><span data-stu-id="b9924-113">To simplify your tasks, you can take advantage of the XML manipulation tools that are built into Excel.</span></span> <span data-ttu-id="b9924-114">You can also use Excel built-in functions to help with data formatting and to put data in the correct cell.</span><span class="sxs-lookup"><span data-stu-id="b9924-114">You can also use Excel built-in functions to help with data formatting and to put data in the correct cell.</span></span> <span data-ttu-id="b9924-115">For example, add a blank worksheet and copy the legacy data to it.</span><span class="sxs-lookup"><span data-stu-id="b9924-115">For example, add a blank worksheet and copy the legacy data to it.</span></span> <span data-ttu-id="b9924-116">Then make an Excel formula to map data in the transformation worksheet between the fields in the exported worksheet and customer legacy data.</span><span class="sxs-lookup"><span data-stu-id="b9924-116">Then make an Excel formula to map data in the transformation worksheet between the fields in the exported worksheet and customer legacy data.</span></span> <span data-ttu-id="b9924-117">After you have mapped all of the data, copy the range of data onto the table worksheet.</span><span class="sxs-lookup"><span data-stu-id="b9924-117">After you have mapped all of the data, copy the range of data onto the table worksheet.</span></span>  

> [!IMPORTANT]  
>  <span data-ttu-id="b9924-118">Do not change the columns in the worksheets.</span><span class="sxs-lookup"><span data-stu-id="b9924-118">Do not change the columns in the worksheets.</span></span> <span data-ttu-id="b9924-119">If they are moved, changed, or deleted, the worksheet cannot be imported into [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="b9924-119">If they are moved, changed, or deleted, the worksheet cannot be imported into [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>

## <a name="tables-in-the-default-configuration-package"></a><span data-ttu-id="b9924-120">Tables in the Default Configuration Package</span><span class="sxs-lookup"><span data-stu-id="b9924-120">Tables in the Default Configuration Package</span></span>
<span data-ttu-id="b9924-121">The default configuration package supports the following tables:</span><span class="sxs-lookup"><span data-stu-id="b9924-121">The default configuration package supports the following tables:</span></span>

-   <span data-ttu-id="b9924-122">Payment Terms</span><span class="sxs-lookup"><span data-stu-id="b9924-122">Payment Terms</span></span>
-   <span data-ttu-id="b9924-123">Customer Price Group</span><span class="sxs-lookup"><span data-stu-id="b9924-123">Customer Price Group</span></span>
-   <span data-ttu-id="b9924-124">Shipment Method</span><span class="sxs-lookup"><span data-stu-id="b9924-124">Shipment Method</span></span>
-   <span data-ttu-id="b9924-125">Salesperson/Purchaser</span><span class="sxs-lookup"><span data-stu-id="b9924-125">Salesperson/Purchaser</span></span>
-   <span data-ttu-id="b9924-126">Location</span><span class="sxs-lookup"><span data-stu-id="b9924-126">Location</span></span>
-   <span data-ttu-id="b9924-127">GL Account</span><span class="sxs-lookup"><span data-stu-id="b9924-127">GL Account</span></span>
-   <span data-ttu-id="b9924-128">Customer</span><span class="sxs-lookup"><span data-stu-id="b9924-128">Customer</span></span>
-   <span data-ttu-id="b9924-129">Vendor</span><span class="sxs-lookup"><span data-stu-id="b9924-129">Vendor</span></span>
-   <span data-ttu-id="b9924-130">Item</span><span class="sxs-lookup"><span data-stu-id="b9924-130">Item</span></span>
-   <span data-ttu-id="b9924-131">Sales Header</span><span class="sxs-lookup"><span data-stu-id="b9924-131">Sales Header</span></span>
-   <span data-ttu-id="b9924-132">Sales Line</span><span class="sxs-lookup"><span data-stu-id="b9924-132">Sales Line</span></span>
-   <span data-ttu-id="b9924-133">Purchase Header</span><span class="sxs-lookup"><span data-stu-id="b9924-133">Purchase Header</span></span>
-   <span data-ttu-id="b9924-134">Purchase Line</span><span class="sxs-lookup"><span data-stu-id="b9924-134">Purchase Line</span></span>
-   <span data-ttu-id="b9924-135">Gen. Journal Line</span><span class="sxs-lookup"><span data-stu-id="b9924-135">Gen. Journal Line</span></span>
-   <span data-ttu-id="b9924-136">Item Journal Line</span><span class="sxs-lookup"><span data-stu-id="b9924-136">Item Journal Line</span></span>
-   <span data-ttu-id="b9924-137">Customer Posting Group</span><span class="sxs-lookup"><span data-stu-id="b9924-137">Customer Posting Group</span></span>
-   <span data-ttu-id="b9924-138">Vendor Posting Group</span><span class="sxs-lookup"><span data-stu-id="b9924-138">Vendor Posting Group</span></span>
-   <span data-ttu-id="b9924-139">Inventory Posting Group</span><span class="sxs-lookup"><span data-stu-id="b9924-139">Inventory Posting Group</span></span>
-   <span data-ttu-id="b9924-140">Unit of Measure</span><span class="sxs-lookup"><span data-stu-id="b9924-140">Unit of Measure</span></span>
-   <span data-ttu-id="b9924-141">Gen. Business Posting Group</span><span class="sxs-lookup"><span data-stu-id="b9924-141">Gen. Business Posting Group</span></span>
-   <span data-ttu-id="b9924-142">Gen. Product Posting Group</span><span class="sxs-lookup"><span data-stu-id="b9924-142">Gen. Product Posting Group</span></span>
-   <span data-ttu-id="b9924-143">General Posting Setup</span><span class="sxs-lookup"><span data-stu-id="b9924-143">General Posting Setup</span></span>
-   <span data-ttu-id="b9924-144">Territory</span><span class="sxs-lookup"><span data-stu-id="b9924-144">Territory</span></span>
-   <span data-ttu-id="b9924-145">Item Category</span><span class="sxs-lookup"><span data-stu-id="b9924-145">Item Category</span></span>
-   <span data-ttu-id="b9924-146">Sales Price</span><span class="sxs-lookup"><span data-stu-id="b9924-146">Sales Price</span></span>
-   <span data-ttu-id="b9924-147">Purchase Price</span><span class="sxs-lookup"><span data-stu-id="b9924-147">Purchase Price</span></span>

## <a name="importing-customer-data"></a><span data-ttu-id="b9924-148">Importing Customer Data</span><span class="sxs-lookup"><span data-stu-id="b9924-148">Importing Customer Data</span></span>
<span data-ttu-id="b9924-149">After the customer data has been entered in Excel, you import the data into [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="b9924-149">After the customer data has been entered in Excel, you import the data into [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="b9924-150">In the **Configuration Packages** window, you import the data from the Excel file, and you can validate that the data is consistent with [!INCLUDE[d365fin](includes/d365fin_md.md)] before you apply the package.</span><span class="sxs-lookup"><span data-stu-id="b9924-150">In the **Configuration Packages** window, you import the data from the Excel file, and you can validate that the data is consistent with [!INCLUDE[d365fin](includes/d365fin_md.md)] before you apply the package.</span></span>

## <a name="see-also"></a><span data-ttu-id="b9924-151">See Also</span><span class="sxs-lookup"><span data-stu-id="b9924-151">See Also</span></span>
[<span data-ttu-id="b9924-152">Importing Business Data from Other Finance Systems</span><span class="sxs-lookup"><span data-stu-id="b9924-152">Importing Business Data from Other Finance Systems</span></span>](upload-data.md)  
[<span data-ttu-id="b9924-153">QuickBooks Data Migration</span><span class="sxs-lookup"><span data-stu-id="b9924-153">QuickBooks Data Migration</span></span>](ui-extensions-quickbooks-data-migration.md)  
[<span data-ttu-id="b9924-154">Dynamics GP Data Migration</span><span class="sxs-lookup"><span data-stu-id="b9924-154">Dynamics GP Data Migration</span></span>](ui-extensions-dynamicsgp-data-migration.md)  

## [!INCLUDE[d365fin](includes/free_trial_md.md)]

