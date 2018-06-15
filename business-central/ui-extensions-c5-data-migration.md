---
title: Using the C5 Data Migration Extension | Microsoft Docs
description: Use this extension to migrate customers, vendors, items, and general ledger accounts from Microsoft Dynamics C5 2012 to Business Central.
services: project-madeira
documentationcenter: 
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: extension, migrate, data, C5, import
ms.date: 04/09/208
ms.author: bholtorf
ms.translationtype: HT
ms.sourcegitcommit: fa6779ee8fb2bbb453014e32cb7f3cf8dcfa18da
ms.openlocfilehash: 698bde6949c6053501881d07135586810fc81bdd
ms.contentlocale: en-nz
ms.lasthandoff: 04/11/2018

---

# <a name="the-c5-data-migration-extension-for-business-central"></a><span data-ttu-id="d40a7-103">The C5 Data Migration Extension for Business Central</span><span class="sxs-lookup"><span data-stu-id="d40a7-103">The C5 Data Migration Extension for Business Central</span></span>
<span data-ttu-id="d40a7-104">This extension makes it easy to migrate customers, vendors, items, and your general ledger accounts from Microsoft Dynamcis C5 2012 to [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="d40a7-104">This extension makes it easy to migrate customers, vendors, items, and your general ledger accounts from Microsoft Dynamcis C5 2012 to [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="d40a7-105">You can also migrate historical entries for general ledger accounts.</span><span class="sxs-lookup"><span data-stu-id="d40a7-105">You can also migrate historical entries for general ledger accounts.</span></span>

> [!Note]
> <span data-ttu-id="d40a7-106">The company in [!INCLUDE[d365fin](includes/d365fin_md.md)] must not contain any data.</span><span class="sxs-lookup"><span data-stu-id="d40a7-106">The company in [!INCLUDE[d365fin](includes/d365fin_md.md)] must not contain any data.</span></span> <span data-ttu-id="d40a7-107">Additionally, after you start a migration, do not create customers, vendors, items, or accounts until the migration finishes.</span><span class="sxs-lookup"><span data-stu-id="d40a7-107">Additionally, after you start a migration, do not create customers, vendors, items, or accounts until the migration finishes.</span></span>

## <a name="what-data-is-migrated"></a><span data-ttu-id="d40a7-108">What Data is Migrated?</span><span class="sxs-lookup"><span data-stu-id="d40a7-108">What Data is Migrated?</span></span>
<span data-ttu-id="d40a7-109">The following data is migrated for each entity:</span><span class="sxs-lookup"><span data-stu-id="d40a7-109">The following data is migrated for each entity:</span></span>

<span data-ttu-id="d40a7-110">**Customers**</span><span class="sxs-lookup"><span data-stu-id="d40a7-110">**Customers**</span></span>
* <span data-ttu-id="d40a7-111">Location</span><span class="sxs-lookup"><span data-stu-id="d40a7-111">Location</span></span>
* <span data-ttu-id="d40a7-112">Country</span><span class="sxs-lookup"><span data-stu-id="d40a7-112">Country</span></span>
* <span data-ttu-id="d40a7-113">Customer dimensions (department, centre, purpose)</span><span class="sxs-lookup"><span data-stu-id="d40a7-113">Customer dimensions (department, center, purpose)</span></span>
* <span data-ttu-id="d40a7-114">Shipment method</span><span class="sxs-lookup"><span data-stu-id="d40a7-114">Shipment method</span></span>
* <span data-ttu-id="d40a7-115">Sales Person</span><span class="sxs-lookup"><span data-stu-id="d40a7-115">Sales Person</span></span>
* <span data-ttu-id="d40a7-116">Payment terms</span><span class="sxs-lookup"><span data-stu-id="d40a7-116">Payment terms</span></span>
* <span data-ttu-id="d40a7-117">Payment method</span><span class="sxs-lookup"><span data-stu-id="d40a7-117">Payment method</span></span>
* <span data-ttu-id="d40a7-118">Customer price group</span><span class="sxs-lookup"><span data-stu-id="d40a7-118">Customer price group</span></span>
* <span data-ttu-id="d40a7-119">Customer invoice discount</span><span class="sxs-lookup"><span data-stu-id="d40a7-119">Customer invoice discount</span></span>

<span data-ttu-id="d40a7-120">If you migrate accounts, the following data is also migrated:</span><span class="sxs-lookup"><span data-stu-id="d40a7-120">If you migrate accounts, the following data is also migrated:</span></span>

* <span data-ttu-id="d40a7-121">Customer posting setup</span><span class="sxs-lookup"><span data-stu-id="d40a7-121">Customer posting setup</span></span>
* <span data-ttu-id="d40a7-122">General journal batch</span><span class="sxs-lookup"><span data-stu-id="d40a7-122">General journal batch</span></span>
* <span data-ttu-id="d40a7-123">Open transactions (customer ledger entries)</span><span class="sxs-lookup"><span data-stu-id="d40a7-123">Open transactions (customer ledger entries)</span></span>

<span data-ttu-id="d40a7-124">**Vendors**</span><span class="sxs-lookup"><span data-stu-id="d40a7-124">**Vendors**</span></span>
* <span data-ttu-id="d40a7-125">Location</span><span class="sxs-lookup"><span data-stu-id="d40a7-125">Location</span></span>
* <span data-ttu-id="d40a7-126">Country</span><span class="sxs-lookup"><span data-stu-id="d40a7-126">Country</span></span>
* <span data-ttu-id="d40a7-127">Vendor dimensions (department, centre, purpose)</span><span class="sxs-lookup"><span data-stu-id="d40a7-127">Vendor dimensions (department, center, purpose)</span></span>
* <span data-ttu-id="d40a7-128">Invoice discount</span><span class="sxs-lookup"><span data-stu-id="d40a7-128">Invoice discount</span></span>
* <span data-ttu-id="d40a7-129">Shipment method</span><span class="sxs-lookup"><span data-stu-id="d40a7-129">Shipment method</span></span>
* <span data-ttu-id="d40a7-130">Purchaser</span><span class="sxs-lookup"><span data-stu-id="d40a7-130">Purchaser</span></span>
* <span data-ttu-id="d40a7-131">Payment terms</span><span class="sxs-lookup"><span data-stu-id="d40a7-131">Payment terms</span></span>
* <span data-ttu-id="d40a7-132">Payment method</span><span class="sxs-lookup"><span data-stu-id="d40a7-132">Payment method</span></span>
* <span data-ttu-id="d40a7-133">Vendor invoice discount</span><span class="sxs-lookup"><span data-stu-id="d40a7-133">Vendor invoice discount</span></span>

<span data-ttu-id="d40a7-134">If you migrate accounts, the following data is also migrated:</span><span class="sxs-lookup"><span data-stu-id="d40a7-134">If you migrate accounts, the following data is also migrated:</span></span>

* <span data-ttu-id="d40a7-135">Vendor posting setup</span><span class="sxs-lookup"><span data-stu-id="d40a7-135">Vendor posting setup</span></span>
* <span data-ttu-id="d40a7-136">General journal batch</span><span class="sxs-lookup"><span data-stu-id="d40a7-136">General journal batch</span></span>
* <span data-ttu-id="d40a7-137">Open transactions (vendor ledger entries)</span><span class="sxs-lookup"><span data-stu-id="d40a7-137">Open transactions (vendor ledger entries)</span></span>

<span data-ttu-id="d40a7-138">**Items**</span><span class="sxs-lookup"><span data-stu-id="d40a7-138">**Items**</span></span>
* <span data-ttu-id="d40a7-139">Location</span><span class="sxs-lookup"><span data-stu-id="d40a7-139">Location</span></span>
* <span data-ttu-id="d40a7-140">Country</span><span class="sxs-lookup"><span data-stu-id="d40a7-140">Country</span></span>
* <span data-ttu-id="d40a7-141">Item dimensions (department, centre, purpose)</span><span class="sxs-lookup"><span data-stu-id="d40a7-141">Item dimensions (department, center, purpose)</span></span>
* <span data-ttu-id="d40a7-142">Sales line discounts</span><span class="sxs-lookup"><span data-stu-id="d40a7-142">Sales line discounts</span></span>
* <span data-ttu-id="d40a7-143">Customer discount groups</span><span class="sxs-lookup"><span data-stu-id="d40a7-143">Customer discount groups</span></span>
* <span data-ttu-id="d40a7-144">Item discount groups</span><span class="sxs-lookup"><span data-stu-id="d40a7-144">Item discount groups</span></span>
* <span data-ttu-id="d40a7-145">Sales price</span><span class="sxs-lookup"><span data-stu-id="d40a7-145">Sales price</span></span>
* <span data-ttu-id="d40a7-146">Tariff number</span><span class="sxs-lookup"><span data-stu-id="d40a7-146">Tariff number</span></span>
* <span data-ttu-id="d40a7-147">Units of measure</span><span class="sxs-lookup"><span data-stu-id="d40a7-147">Units of measure</span></span>
* <span data-ttu-id="d40a7-148">Item tracking code</span><span class="sxs-lookup"><span data-stu-id="d40a7-148">Item tracking code</span></span>
* <span data-ttu-id="d40a7-149">Customer price group</span><span class="sxs-lookup"><span data-stu-id="d40a7-149">Customer price group</span></span>

<span data-ttu-id="d40a7-150">If you migrate accounts, the following data is also migrated:</span><span class="sxs-lookup"><span data-stu-id="d40a7-150">If you migrate accounts, the following data is also migrated:</span></span>

* <span data-ttu-id="d40a7-151">Inventory posting setup</span><span class="sxs-lookup"><span data-stu-id="d40a7-151">Inventory posting setup</span></span>
* <span data-ttu-id="d40a7-152">General posting setup</span><span class="sxs-lookup"><span data-stu-id="d40a7-152">General posting setup</span></span>
* <span data-ttu-id="d40a7-153">Item journal batch</span><span class="sxs-lookup"><span data-stu-id="d40a7-153">Item journal batch</span></span>
* <span data-ttu-id="d40a7-154">Open transactions (item ledger entries)</span><span class="sxs-lookup"><span data-stu-id="d40a7-154">Open transactions (item ledger entries)</span></span>

> [!Note]
> <span data-ttu-id="d40a7-155">If there are open transactions that use foreign currencies, the exchange rates for those currencies are also migrated.</span><span class="sxs-lookup"><span data-stu-id="d40a7-155">If there are open transactions that use foreign currencies, the exchange rates for those currencies are also migrated.</span></span> <span data-ttu-id="d40a7-156">Other exchange rates are not migrated.</span><span class="sxs-lookup"><span data-stu-id="d40a7-156">Other exchange rates are not migrated.</span></span>

<span data-ttu-id="d40a7-157">**Chart of Accounts**</span><span class="sxs-lookup"><span data-stu-id="d40a7-157">**Chart of Accounts**</span></span>  
* <span data-ttu-id="d40a7-158">Standard dimensions: Department, Cost Centre, Purpose</span><span class="sxs-lookup"><span data-stu-id="d40a7-158">Standard dimensions: Department, Cost Center, Purpose</span></span>  
* <span data-ttu-id="d40a7-159">Historical G/L transactions</span><span class="sxs-lookup"><span data-stu-id="d40a7-159">Historical G/L transactions</span></span>  

> [!Note]
> <span data-ttu-id="d40a7-160">Historical G/L transactions are treated a little differently.</span><span class="sxs-lookup"><span data-stu-id="d40a7-160">Historical G/L transactions are treated a little differently.</span></span> <span data-ttu-id="d40a7-161">When you migrate data you set a **Current Period** parameter.</span><span class="sxs-lookup"><span data-stu-id="d40a7-161">When you migrate data you set a **Current Period** parameter.</span></span> <span data-ttu-id="d40a7-162">This parameter specifies how to process G/L transactions.</span><span class="sxs-lookup"><span data-stu-id="d40a7-162">This parameter specifies how to process G/L transactions.</span></span> <span data-ttu-id="d40a7-163">Transactions after this date are migrated individually.</span><span class="sxs-lookup"><span data-stu-id="d40a7-163">Transactions after this date are migrated individually.</span></span> <span data-ttu-id="d40a7-164">Transactions before this date are aggregated per account and migrated as a single amount.</span><span class="sxs-lookup"><span data-stu-id="d40a7-164">Transactions before this date are aggregated per account and migrated as a single amount.</span></span> <span data-ttu-id="d40a7-165">For example, let's say there are transactions in 2015, 2016, 2017, 2018, and you specify January 01, 2017 in the Current Period field.</span><span class="sxs-lookup"><span data-stu-id="d40a7-165">For example, let's say there are transactions in 2015, 2016, 2017, 2018, and you specify January 01, 2017 in the Current Period field.</span></span> <span data-ttu-id="d40a7-166">For each account, amounts for transactions on or before December 31, 2106, will be aggregated in a single general journal line for each G/L account.</span><span class="sxs-lookup"><span data-stu-id="d40a7-166">For each account, amounts for transactions on or before December 31, 2106, will be aggregated in a single general journal line for each G/L account.</span></span> <span data-ttu-id="d40a7-167">All trascations after this date will be migrated individually.</span><span class="sxs-lookup"><span data-stu-id="d40a7-167">All trascations after this date will be migrated individually.</span></span>

## <a name="to-migrate-data"></a><span data-ttu-id="d40a7-168">To migrate data</span><span class="sxs-lookup"><span data-stu-id="d40a7-168">To migrate data</span></span>
<span data-ttu-id="d40a7-169">There are just a few steps to export data from C5, and import it in [!INCLUDE[d365fin](includes/d365fin_md.md)]:</span><span class="sxs-lookup"><span data-stu-id="d40a7-169">There are just a few steps to export data from C5, and import it in [!INCLUDE[d365fin](includes/d365fin_md.md)]:</span></span>  

1. <span data-ttu-id="d40a7-170">In C5, use the **Export Database** feature to export the data.</span><span class="sxs-lookup"><span data-stu-id="d40a7-170">In C5, use the **Export Database** feature to export the data.</span></span> <span data-ttu-id="d40a7-171">Then send the export folder to a compressed (zipped) folder.</span><span class="sxs-lookup"><span data-stu-id="d40a7-171">Then send the export folder to a compressed (zipped) folder.</span></span>  
2. <span data-ttu-id="d40a7-172">In [!INCLUDE[d365fin](includes/d365fin_md.md)], choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Data Migration**, and then choose **Data Migration**.</span><span class="sxs-lookup"><span data-stu-id="d40a7-172">In [!INCLUDE[d365fin](includes/d365fin_md.md)], choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Data Migration**, and then choose **Data Migration**.</span></span>  
3. <span data-ttu-id="d40a7-173">Complete the steps in the assisted setup guide.</span><span class="sxs-lookup"><span data-stu-id="d40a7-173">Complete the steps in the assisted setup guide.</span></span> <span data-ttu-id="d40a7-174">Make sure to choose **Import from Microsoft Dynamcis C5 2012** as the data source.</span><span class="sxs-lookup"><span data-stu-id="d40a7-174">Make sure to choose **Import from Microsoft Dynamcis C5 2012** as the data source.</span></span>  

> [!Note]
> <span data-ttu-id="d40a7-175">Companies often add fields to customise C5 for their specific line of business.</span><span class="sxs-lookup"><span data-stu-id="d40a7-175">Companies often add fields to customize C5 for their specific line of business.</span></span> [!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="d40a7-176"> does not migrate data from custom fields.</span><span class="sxs-lookup"><span data-stu-id="d40a7-176"> does not migrate data from custom fields.</span></span> <span data-ttu-id="d40a7-177">Also, migration will fail if you have more than 10 custom fields.</span><span class="sxs-lookup"><span data-stu-id="d40a7-177">Also, migration will fail if you have more than 10 custom fields.</span></span>

## <a name="viewing-the-status-of-the-migration"></a><span data-ttu-id="d40a7-178">Viewing the Status of the Migration</span><span class="sxs-lookup"><span data-stu-id="d40a7-178">Viewing the Status of the Migration</span></span>
<span data-ttu-id="d40a7-179">Use the **Data Migration Overview** page to monitor the success of the migration.</span><span class="sxs-lookup"><span data-stu-id="d40a7-179">Use the **Data Migration Overview** page to monitor the success of the migration.</span></span> <span data-ttu-id="d40a7-180">The page shows information such as the number of entities that the migration will include, the status of the migration, and the number of items that have been migrated and whether they were successfull.</span><span class="sxs-lookup"><span data-stu-id="d40a7-180">The page shows information such as the number of entities that the migration will include, the status of the migration, and the number of items that have been migrated and whether they were successfull.</span></span> <span data-ttu-id="d40a7-181">It also shows the number of errors, lets you investigate what went wrong and, when possible, makes it easy to go to the entity to fix the issues.</span><span class="sxs-lookup"><span data-stu-id="d40a7-181">It also shows the number of errors, lets you investigate what went wrong and, when possible, makes it easy to go to the entity to fix the issues.</span></span> <span data-ttu-id="d40a7-182">For more information, see the next section in this topic.</span><span class="sxs-lookup"><span data-stu-id="d40a7-182">For more information, see the next section in this topic.</span></span>  

> [!Note]
> <span data-ttu-id="d40a7-183">While you are waiting for the results of the migration, you must refresh the page to display the results.</span><span class="sxs-lookup"><span data-stu-id="d40a7-183">While you are waiting for the results of the migration, you must refresh the page to display the results.</span></span>

## <a name="how-to-avoid-double-posting"></a><span data-ttu-id="d40a7-184">How to Avoid Double-Posting</span><span class="sxs-lookup"><span data-stu-id="d40a7-184">How to Avoid Double-Posting</span></span>
<span data-ttu-id="d40a7-185">To help avoid double-posting to the general ledger, the following balance accounts are used for open transactions:</span><span class="sxs-lookup"><span data-stu-id="d40a7-185">To help avoid double-posting to the general ledger, the following balance accounts are used for open transactions:</span></span>  
  
* <span data-ttu-id="d40a7-186">For vendors, we use the A/P account from the vendor posting group.</span><span class="sxs-lookup"><span data-stu-id="d40a7-186">For vendors, we use the A/P account from the vendor posting group.</span></span>  
* <span data-ttu-id="d40a7-187">For customers, we use the A/R account from the customer posting group.</span><span class="sxs-lookup"><span data-stu-id="d40a7-187">For customers, we use the A/R account from the customer posting group.</span></span>  
* <span data-ttu-id="d40a7-188">For items, we create a general posting setup where the adjustment account is the account specified as the inventory account on the inventory posting setup.</span><span class="sxs-lookup"><span data-stu-id="d40a7-188">For items, we create a general posting setup where the adjustment account is the account specified as the inventory account on the inventory posting setup.</span></span>  

## <a name="correcting-errors"></a><span data-ttu-id="d40a7-189">Correcting Errors</span><span class="sxs-lookup"><span data-stu-id="d40a7-189">Correcting Errors</span></span>
<span data-ttu-id="d40a7-190">If something goes wrong and an error occurs, the **Status** field will show **Completed with Errors**, and the **Error Count** field will show how many.</span><span class="sxs-lookup"><span data-stu-id="d40a7-190">If something goes wrong and an error occurs, the **Status** field will show **Completed with Errors**, and the **Error Count** field will show how many.</span></span> <span data-ttu-id="d40a7-191">To view a list of the errors, you can open the **Data Migration Errors** page by choosing:</span><span class="sxs-lookup"><span data-stu-id="d40a7-191">To view a list of the errors, you can open the **Data Migration Errors** page by choosing:</span></span>  

* <span data-ttu-id="d40a7-192">The number in the **Error Count** field for the entity.</span><span class="sxs-lookup"><span data-stu-id="d40a7-192">The number in the **Error Count** field for the entity.</span></span>  
* <span data-ttu-id="d40a7-193">The entity, and then the **Show Errors** action.</span><span class="sxs-lookup"><span data-stu-id="d40a7-193">The entity, and then the **Show Errors** action.</span></span>  

<span data-ttu-id="d40a7-194">On the **Data Migration Errors** page, to fix an error you can choose an error message, then choose **Edit Record** to open a page that shows the migrated data for the entity.</span><span class="sxs-lookup"><span data-stu-id="d40a7-194">On the **Data Migration Errors** page, to fix an error you can choose an error message, then choose **Edit Record** to open a page that shows the migrated data for the entity.</span></span> <span data-ttu-id="d40a7-195">After you fix one or more errors, you can choose **Migrate** to migrate only the entities you fixed, without having to completely restart the migration.</span><span class="sxs-lookup"><span data-stu-id="d40a7-195">After you fix one or more errors, you can choose **Migrate** to migrate only the entities you fixed, without having to completely restart the migration.</span></span>  

> [!Tip]
> <span data-ttu-id="d40a7-196">If you have fixed more than one error, you can use the **Select More** feature to select multiple lines to migrate.</span><span class="sxs-lookup"><span data-stu-id="d40a7-196">If you have fixed more than one error, you can use the **Select More** feature to select multiple lines to migrate.</span></span> <span data-ttu-id="d40a7-197">Alternatively, if there are errors that are not important to fix, you can choose them and then choose **Skip Selections**.</span><span class="sxs-lookup"><span data-stu-id="d40a7-197">Alternatively, if there are errors that are not important to fix, you can choose them and then choose **Skip Selections**.</span></span>

> [!Note]
> <span data-ttu-id="d40a7-198">If you have items that are included in a BOM, you might need to migrate more than once if the original item is not created before the variants that reference it.</span><span class="sxs-lookup"><span data-stu-id="d40a7-198">If you have items that are included in a BOM, you might need to migrate more than once if the original item is not created before the variants that reference it.</span></span> <span data-ttu-id="d40a7-199">If an item variant is created first, the reference to the original item can cause an error message.</span><span class="sxs-lookup"><span data-stu-id="d40a7-199">If an item variant is created first, the reference to the original item can cause an error message.</span></span>  

## <a name="verifying-data-after-migrating"></a><span data-ttu-id="d40a7-200">Verifying Data After Migrating</span><span class="sxs-lookup"><span data-stu-id="d40a7-200">Verifying Data After Migrating</span></span>
<span data-ttu-id="d40a7-201">One way to verify that your data migrated correctly is to look at the following pages in C5 and [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="d40a7-201">One way to verify that your data migrated correctly is to look at the following pages in C5 and [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>

|<span data-ttu-id="d40a7-202">Microsoft Dynamcis C5 2012</span><span class="sxs-lookup"><span data-stu-id="d40a7-202">Microsoft Dynamcis C5 2012</span></span> | [!INCLUDE[d365fin](includes/d365fin_md.md)]| <span data-ttu-id="d40a7-203">Batch Job to Use</span><span class="sxs-lookup"><span data-stu-id="d40a7-203">Batch Job to Use</span></span> |
|-----|-----|-----|
|<span data-ttu-id="d40a7-204">Customer Entries</span><span class="sxs-lookup"><span data-stu-id="d40a7-204">Customer Entries</span></span>| <span data-ttu-id="d40a7-205">General Journals</span><span class="sxs-lookup"><span data-stu-id="d40a7-205">General Journals</span></span>| <span data-ttu-id="d40a7-206">CUSTMIGR</span><span class="sxs-lookup"><span data-stu-id="d40a7-206">CUSTMIGR</span></span> |
|<span data-ttu-id="d40a7-207">Vendor Entries</span><span class="sxs-lookup"><span data-stu-id="d40a7-207">Vendor Entries</span></span>| <span data-ttu-id="d40a7-208">General Journals</span><span class="sxs-lookup"><span data-stu-id="d40a7-208">General Journals</span></span>| <span data-ttu-id="d40a7-209">VENDMIGR</span><span class="sxs-lookup"><span data-stu-id="d40a7-209">VENDMIGR</span></span>|
|<span data-ttu-id="d40a7-210">Item Entries</span><span class="sxs-lookup"><span data-stu-id="d40a7-210">Item Entries</span></span>| <span data-ttu-id="d40a7-211">Item Journals</span><span class="sxs-lookup"><span data-stu-id="d40a7-211">Item Journals</span></span>| <span data-ttu-id="d40a7-212">ITEMMIGR</span><span class="sxs-lookup"><span data-stu-id="d40a7-212">ITEMMIGR</span></span> |
|<span data-ttu-id="d40a7-213">G/L Entries</span><span class="sxs-lookup"><span data-stu-id="d40a7-213">G/L Entries</span></span>| <span data-ttu-id="d40a7-214">General Journals</span><span class="sxs-lookup"><span data-stu-id="d40a7-214">General Journals</span></span>| <span data-ttu-id="d40a7-215">GLACMIGR</span><span class="sxs-lookup"><span data-stu-id="d40a7-215">GLACMIGR</span></span> |

## <a name="stopping-data-migration"></a><span data-ttu-id="d40a7-216">Stopping Data Migration</span><span class="sxs-lookup"><span data-stu-id="d40a7-216">Stopping Data Migration</span></span>
<span data-ttu-id="d40a7-217">You can stop migrating data by choosing **Stop All Migrations**.</span><span class="sxs-lookup"><span data-stu-id="d40a7-217">You can stop migrating data by choosing **Stop All Migrations**.</span></span> <span data-ttu-id="d40a7-218">If you do, all pending migrations are also stopped.</span><span class="sxs-lookup"><span data-stu-id="d40a7-218">If you do, all pending migrations are also stopped.</span></span>

## <a name="see-also"></a><span data-ttu-id="d40a7-219">See Also</span><span class="sxs-lookup"><span data-stu-id="d40a7-219">See Also</span></span>
<span data-ttu-id="d40a7-220">[Customising [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions](ui-extensions.md)</span><span class="sxs-lookup"><span data-stu-id="d40a7-220">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions](ui-extensions.md)</span></span>  
[<span data-ttu-id="d40a7-221">Getting Started</span><span class="sxs-lookup"><span data-stu-id="d40a7-221">Getting Started</span></span>](product-get-started.md) 

