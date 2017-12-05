---
title: Using the C5 Data Migration Extension | Microsoft Docs
description: Use this extension to migrate customers, vendors, items, and general ledger accounts from Microsoft Dynamics C5 2012 to Financials.
services: project-madeira
documentationcenter: 
author: bholtorf
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: extension, migrate, data, C5, import
ms.date: 09/26/2017
ms.author: bholtorf
ms.translationtype: HT
ms.sourcegitcommit: ba26b354d235981bd7291f9ac6402779f554ac7a
ms.openlocfilehash: 2d7d533662936116ffa40ded07b68e845fed810b
ms.contentlocale: en-nz
ms.lasthandoff: 11/10/2017

---

# <a name="the-c5-data-migration-extension-for-dynamics-365-for-finance-and-operations-business-edition"></a><span data-ttu-id="96a58-103">The C5 Data Migration Extension for Dynamics 365 for Finance and Operations, Business Edition</span><span class="sxs-lookup"><span data-stu-id="96a58-103">The C5 Data Migration Extension for Dynamics 365 for Finance and Operations, Business Edition</span></span>
<span data-ttu-id="96a58-104">This extension makes it easy to migrate customers, vendors, items, and your general ledger accounts from Microsoft Dynamcis C5 2012 to [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="96a58-104">This extension makes it easy to migrate customers, vendors, items, and your general ledger accounts from Microsoft Dynamcis C5 2012 to [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  
  
> [!Note] 
> <span data-ttu-id="96a58-105">The company in [!INCLUDE[d365fin](includes/d365fin_md.md)] must not contain any data.</span><span class="sxs-lookup"><span data-stu-id="96a58-105">The company in [!INCLUDE[d365fin](includes/d365fin_md.md)] must not contain any data.</span></span> <span data-ttu-id="96a58-106">Additionally, after you start a migration, do not create customers, vendors, items, or accounts until the migration finishes.</span><span class="sxs-lookup"><span data-stu-id="96a58-106">Additionally, after you start a migration, do not create customers, vendors, items, or accounts until the migration finishes.</span></span>

## <a name="to-migrate-data"></a><span data-ttu-id="96a58-107">To migrate data</span><span class="sxs-lookup"><span data-stu-id="96a58-107">To migrate data</span></span>
<span data-ttu-id="96a58-108">There are just a few steps to export data from C5, and import it in [!INCLUDE[d365fin](includes/d365fin_md.md)]:</span><span class="sxs-lookup"><span data-stu-id="96a58-108">There are just a few steps to export data from C5, and import it in [!INCLUDE[d365fin](includes/d365fin_md.md)]:</span></span>  
  
1. <span data-ttu-id="96a58-109">In C5, use the **Export Database** feature to export the data.</span><span class="sxs-lookup"><span data-stu-id="96a58-109">In C5, use the **Export Database** feature to export the data.</span></span> <span data-ttu-id="96a58-110">Then send the export folder to a compressed (zipped) folder.</span><span class="sxs-lookup"><span data-stu-id="96a58-110">Then send the export folder to a compressed (zipped) folder.</span></span>  
2. <span data-ttu-id="96a58-111">In [!INCLUDE[d365fin](includes/d365fin_md.md)], choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Data Migration**, and then choose **Data Migration**.</span><span class="sxs-lookup"><span data-stu-id="96a58-111">In [!INCLUDE[d365fin](includes/d365fin_md.md)], choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Data Migration**, and then choose **Data Migration**.</span></span>  
3. <span data-ttu-id="96a58-112">Complete the steps in the assisted setup guide.</span><span class="sxs-lookup"><span data-stu-id="96a58-112">Complete the steps in the assisted setup guide.</span></span> <span data-ttu-id="96a58-113">Make sure to choose **Import from Microsoft Dynamcis C5 2012** as the data source.</span><span class="sxs-lookup"><span data-stu-id="96a58-113">Make sure to choose **Import from Microsoft Dynamcis C5 2012** as the data source.</span></span>  

> [!Note] 
> <span data-ttu-id="96a58-114">Companies often add fields to customise C5 for their specific line of business.</span><span class="sxs-lookup"><span data-stu-id="96a58-114">Companies often add fields to customize C5 for their specific line of business.</span></span> [!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="96a58-115"> does not migrate data from custom fields.</span><span class="sxs-lookup"><span data-stu-id="96a58-115"> does not migrate data from custom fields.</span></span> <span data-ttu-id="96a58-116">Also, migration will fail if you have more than 10 custom fields.</span><span class="sxs-lookup"><span data-stu-id="96a58-116">Also, migration will fail if you have more than 10 custom fields.</span></span> 

## <a name="viewing-the-status-of-the-migration"></a><span data-ttu-id="96a58-117">Viewing the Status of the Migration</span><span class="sxs-lookup"><span data-stu-id="96a58-117">Viewing the Status of the Migration</span></span>
<span data-ttu-id="96a58-118">Use the **Data Migration Overview** page to monitor the success of the migration.</span><span class="sxs-lookup"><span data-stu-id="96a58-118">Use the **Data Migration Overview** page to monitor the success of the migration.</span></span> <span data-ttu-id="96a58-119">The page shows information such as the number of entities that the migration will include, the status of the migration, and the number of items that have been migrated and whether they were successfull.</span><span class="sxs-lookup"><span data-stu-id="96a58-119">The page shows information such as the number of entities that the migration will include, the status of the migration, and the number of items that have been migrated and whether they were successfull.</span></span> <span data-ttu-id="96a58-120">It also shows the number of errors, lets you investigate what went wrong and, when possible, makes it easy to go to the entity to fix the issues.</span><span class="sxs-lookup"><span data-stu-id="96a58-120">It also shows the number of errors, lets you investigate what went wrong and, when possible, makes it easy to go to the entity to fix the issues.</span></span> <span data-ttu-id="96a58-121">For more information, see the next section in this topic.</span><span class="sxs-lookup"><span data-stu-id="96a58-121">For more information, see the next section in this topic.</span></span> 

> [!Note] 
> <span data-ttu-id="96a58-122">While you are waiting for the results of the migration, you must refresh the page to display the results.</span><span class="sxs-lookup"><span data-stu-id="96a58-122">While you are waiting for the results of the migration, you must refresh the page to display the results.</span></span>

## <a name="correcting-errors"></a><span data-ttu-id="96a58-123">Correcting Errors</span><span class="sxs-lookup"><span data-stu-id="96a58-123">Correcting Errors</span></span>
<span data-ttu-id="96a58-124">If something goes wrong and an error occurs, the **Status** field will show **Completed with Errors**, and the **Error Count** field will show how many.</span><span class="sxs-lookup"><span data-stu-id="96a58-124">If something goes wrong and an error occurs, the **Status** field will show **Completed with Errors**, and the **Error Count** field will show how many.</span></span> <span data-ttu-id="96a58-125">To view a list of the errors, you can open the **Data Migration Errors** page by choosing:</span><span class="sxs-lookup"><span data-stu-id="96a58-125">To view a list of the errors, you can open the **Data Migration Errors** page by choosing:</span></span>

* <span data-ttu-id="96a58-126">The number in the **Error Count** field for the entity.</span><span class="sxs-lookup"><span data-stu-id="96a58-126">The number in the **Error Count** field for the entity.</span></span> 
* <span data-ttu-id="96a58-127">The entity, and then the **Show Errors** action.</span><span class="sxs-lookup"><span data-stu-id="96a58-127">The entity, and then the **Show Errors** action.</span></span> 

<span data-ttu-id="96a58-128">On the **Data Migration Errors** page, to fix an error you can choose an error message, then choose **Edit Record** to open a page that shows the migrated data for the entity.</span><span class="sxs-lookup"><span data-stu-id="96a58-128">On the **Data Migration Errors** page, to fix an error you can choose an error message, then choose **Edit Record** to open a page that shows the migrated data for the entity.</span></span> <span data-ttu-id="96a58-129">After you fix one or more errors, you can choose **Migrate** to migrate only the entities you fixed, without having to completely restart the migration.</span><span class="sxs-lookup"><span data-stu-id="96a58-129">After you fix one or more errors, you can choose **Migrate** to migrate only the entities you fixed, without having to completely restart the migration.</span></span>  

> [!Tip]
> <span data-ttu-id="96a58-130">If you have fixed more than one error, you can use the **Select More** feature to select multiple lines to migrate.</span><span class="sxs-lookup"><span data-stu-id="96a58-130">If you have fixed more than one error, you can use the **Select More** feature to select multiple lines to migrate.</span></span> <span data-ttu-id="96a58-131">Alternatively, if there are errors that are not important to fix, you can choose them and then choose **Skip Selections**.</span><span class="sxs-lookup"><span data-stu-id="96a58-131">Alternatively, if there are errors that are not important to fix, you can choose them and then choose **Skip Selections**.</span></span>

> [!Note]
> <span data-ttu-id="96a58-132">If you have items that are included in a BOM, you might need to migrate more than once if the original item is not created before the variants that reference it.</span><span class="sxs-lookup"><span data-stu-id="96a58-132">If you have items that are included in a BOM, you might need to migrate more than once if the original item is not created before the variants that reference it.</span></span> <span data-ttu-id="96a58-133">If an item variant is created first, the reference to the original item can cause an error message.</span><span class="sxs-lookup"><span data-stu-id="96a58-133">If an item variant is created first, the reference to the original item can cause an error message.</span></span>  

## <a name="verifying-data-after-migrating"></a><span data-ttu-id="96a58-134">Verifying Data After Migrating</span><span class="sxs-lookup"><span data-stu-id="96a58-134">Verifying Data After Migrating</span></span> 
<span data-ttu-id="96a58-135">If you want to verify that your data migrated correctly, you can look at the following pages in C5 and [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="96a58-135">If you want to verify that your data migrated correctly, you can look at the following pages in C5 and [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>

|<span data-ttu-id="96a58-136">Microsoft Dynamcis C5 2012</span><span class="sxs-lookup"><span data-stu-id="96a58-136">Microsoft Dynamcis C5 2012</span></span> | [!INCLUDE[d365fin](includes/d365fin_md.md)]|
|-----|-----|
|<span data-ttu-id="96a58-137">Customer Entries</span><span class="sxs-lookup"><span data-stu-id="96a58-137">Customer Entries</span></span>| <span data-ttu-id="96a58-138">General Journals</span><span class="sxs-lookup"><span data-stu-id="96a58-138">General Journals</span></span>|
|<span data-ttu-id="96a58-139">Vendor Entries</span><span class="sxs-lookup"><span data-stu-id="96a58-139">Vendor Entries</span></span>| <span data-ttu-id="96a58-140">General Journals</span><span class="sxs-lookup"><span data-stu-id="96a58-140">General Journals</span></span>|
|<span data-ttu-id="96a58-141">Item Entries</span><span class="sxs-lookup"><span data-stu-id="96a58-141">Item Entries</span></span>| <span data-ttu-id="96a58-142">Item Journals</span><span class="sxs-lookup"><span data-stu-id="96a58-142">Item Journals</span></span>|

<span data-ttu-id="96a58-143">In [!INCLUDE[d365fin](includes/d365fin_md.md)], the batch for the migrated data is named **C5MIGRATE**.</span><span class="sxs-lookup"><span data-stu-id="96a58-143">In [!INCLUDE[d365fin](includes/d365fin_md.md)], the batch for the migrated data is named **C5MIGRATE**.</span></span> 

## <a name="stopping-data-migration"></a><span data-ttu-id="96a58-144">Stopping Data Migration</span><span class="sxs-lookup"><span data-stu-id="96a58-144">Stopping Data Migration</span></span>
<span data-ttu-id="96a58-145">You can stop migrating data by choosing **Stop All Migrations**.</span><span class="sxs-lookup"><span data-stu-id="96a58-145">You can stop migrating data by choosing **Stop All Migrations**.</span></span> <span data-ttu-id="96a58-146">If you do, all pending migrations are also stopped.</span><span class="sxs-lookup"><span data-stu-id="96a58-146">If you do, all pending migrations are also stopped.</span></span>

## <a name="see-also"></a><span data-ttu-id="96a58-147">See Also</span><span class="sxs-lookup"><span data-stu-id="96a58-147">See Also</span></span>
<span data-ttu-id="96a58-148">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions](ui-extensions.md)</span><span class="sxs-lookup"><span data-stu-id="96a58-148">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions](ui-extensions.md)</span></span>  
<span data-ttu-id="96a58-149">[Welcome to [!INCLUDE[d365fin](includes/d365fin_md.md)]](index.md)</span><span class="sxs-lookup"><span data-stu-id="96a58-149">[Welcome to [!INCLUDE[d365fin](includes/d365fin_md.md)]](index.md)</span></span>  

