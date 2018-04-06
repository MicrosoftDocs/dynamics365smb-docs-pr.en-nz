---
title: Maintain Fixed Assets| Microsoft Docs
description: You keep a maintenance record of any repairs and service on a fixed asset.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: repair, service
ms.date: 06/02/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: ce4dcfdd9b68bc5725538337b7883ba5f140cd1c
ms.contentlocale: en-nz
ms.lasthandoff: 03/22/2018

---
# <a name="maintain-fixed-assets"></a><span data-ttu-id="ec719-103">Maintain Fixed Assets</span><span class="sxs-lookup"><span data-stu-id="ec719-103">Maintain Fixed Assets</span></span>
<span data-ttu-id="ec719-104">Maintenance expenses are routine periodic costs undertaken to preserve the value of fixed assets.</span><span class="sxs-lookup"><span data-stu-id="ec719-104">Maintenance expenses are routine periodic costs undertaken to preserve the value of fixed assets.</span></span> <span data-ttu-id="ec719-105">Unlike capital improvements, they do not increase values.</span><span class="sxs-lookup"><span data-stu-id="ec719-105">Unlike capital improvements, they do not increase values.</span></span>

<span data-ttu-id="ec719-106">You can record and maintain an up-to-date file on maintenance and service of your fixed assets to have complete maintenance records on a fixed asset easily accessible.</span><span class="sxs-lookup"><span data-stu-id="ec719-106">You can record and maintain an up-to-date file on maintenance and service of your fixed assets to have complete maintenance records on a fixed asset easily accessible.</span></span> <span data-ttu-id="ec719-107">Each time a fixed asset is sent to service, you record all relevant information such as date of service, vendor number and service agent's phone number.</span><span class="sxs-lookup"><span data-stu-id="ec719-107">Each time a fixed asset is sent to service, you record all relevant information such as date of service, vendor number and service agent's phone number.</span></span> <span data-ttu-id="ec719-108">Maintenance registration is recorded for each fixed asset from the relevant fixed asset card.</span><span class="sxs-lookup"><span data-stu-id="ec719-108">Maintenance registration is recorded for each fixed asset from the relevant fixed asset card.</span></span>

<span data-ttu-id="ec719-109">Indexation is used to adjust values for general price-level changes.</span><span class="sxs-lookup"><span data-stu-id="ec719-109">Indexation is used to adjust values for general price-level changes.</span></span> <span data-ttu-id="ec719-110">The **Index Fixed Assets** batch job can be used to recalculate the maintenance costs.</span><span class="sxs-lookup"><span data-stu-id="ec719-110">The **Index Fixed Assets** batch job can be used to recalculate the maintenance costs.</span></span>

## <a name="to-record-maintenance-work-on-a-fixed-asset"></a><span data-ttu-id="ec719-111">To record maintenance work on a fixed asset</span><span class="sxs-lookup"><span data-stu-id="ec719-111">To record maintenance work on a fixed asset</span></span>
<span data-ttu-id="ec719-112">Every time maintenance has been performed, such as a service visit, you can record it for the relevant fixed asset in the **Maintenance Registrations** window.</span><span class="sxs-lookup"><span data-stu-id="ec719-112">Every time maintenance has been performed, such as a service visit, you can record it for the relevant fixed asset in the **Maintenance Registrations** window.</span></span>  

1. <span data-ttu-id="ec719-113">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Fixed Assets**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="ec719-113">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Fixed Assets**, and then choose the related link.</span></span>  
2. <span data-ttu-id="ec719-114">Select the fixed asset that you want to record maintenance for, and then choose the **Maintenance Registration** action.</span><span class="sxs-lookup"><span data-stu-id="ec719-114">Select the fixed asset that you want to record maintenance for, and then choose the **Maintenance Registration** action.</span></span>
3. <span data-ttu-id="ec719-115">In the **Maintenance Registration** window, fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="ec719-115">In the **Maintenance Registration** window, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

## <a name="to-post-maintenance-costs-from-a-fixed-asset-gl-journal"></a><span data-ttu-id="ec719-116">To post maintenance costs from a fixed asset G/L journal</span><span class="sxs-lookup"><span data-stu-id="ec719-116">To post maintenance costs from a fixed asset G/L journal</span></span>
1. <span data-ttu-id="ec719-117">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Depreciation Book List**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="ec719-117">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Depreciation Book List**, and then choose the related link.</span></span>  
2. <span data-ttu-id="ec719-118">Select the depreciation book that is assigned to the fixed asset, and then choose the **Edit** action.</span><span class="sxs-lookup"><span data-stu-id="ec719-118">Select the depreciation book that is assigned to the fixed asset, and then choose the **Edit** action.</span></span>
3. <span data-ttu-id="ec719-119">In the **Depreciation Book Card** window, make sure the **Maintenance** check box is not selected.</span><span class="sxs-lookup"><span data-stu-id="ec719-119">In the **Depreciation Book Card** window, make sure the **Maintenance** check box is not selected.</span></span> <span data-ttu-id="ec719-120">This ensures that maintenance costs are not posted to the general ledger.</span><span class="sxs-lookup"><span data-stu-id="ec719-120">This ensures that maintenance costs are not posted to the general ledger.</span></span>
4. <span data-ttu-id="ec719-121">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **FA G/L Journals**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="ec719-121">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **FA G/L Journals**, and then choose the related link.</span></span>  
5. <span data-ttu-id="ec719-122">Create an initial journal line and fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="ec719-122">Create an initial journal line and fill in the fields as necessary.</span></span>
6. <span data-ttu-id="ec719-123">In the **FA Posting Type** field, select **Maintenance**.</span><span class="sxs-lookup"><span data-stu-id="ec719-123">In the **FA Posting Type** field, select **Maintenance**.</span></span>
7. <span data-ttu-id="ec719-124">Choose the **Insert FA Bal. Account** action.</span><span class="sxs-lookup"><span data-stu-id="ec719-124">Choose the **Insert FA Bal. Account** action.</span></span> <span data-ttu-id="ec719-125">A second journal line is created for the balancing account that is set up for maintenance posting.</span><span class="sxs-lookup"><span data-stu-id="ec719-125">A second journal line is created for the balancing account that is set up for maintenance posting.</span></span>

    > [!NOTE]  
>   <span data-ttu-id="ec719-126">Step 7 only works if you have set up the following: In the **FA Posting Group Card** window for the posting group of the fixed asset, the **Maintenance Account** field contains the general ledger debit account and the **Maintenance Bal. Account** field contains the general ledger account to which you want to post balancing entries for appreciation.</span><span class="sxs-lookup"><span data-stu-id="ec719-126">Step 7 only works if you have set up the following: In the **FA Posting Group Card** window for the posting group of the fixed asset, the **Maintenance Account** field contains the general ledger debit account and the **Maintenance Bal. Account** field contains the general ledger account to which you want to post balancing entries for appreciation.</span></span> <span data-ttu-id="ec719-127">For more information, see the "To set up fixed asset posting groups" section in [Set Up General Fixed Asset Information](fa-how-setup-general.md).</span><span class="sxs-lookup"><span data-stu-id="ec719-127">For more information, see the "To set up fixed asset posting groups" section in [Set Up General Fixed Asset Information](fa-how-setup-general.md).</span></span>
8. <span data-ttu-id="ec719-128">Choose the **Post** action.</span><span class="sxs-lookup"><span data-stu-id="ec719-128">Choose the **Post** action.</span></span>

## <a name="to-follow-up-on-fixed-assets-service-visits"></a><span data-ttu-id="ec719-129">To follow up on fixed assets service visits</span><span class="sxs-lookup"><span data-stu-id="ec719-129">To follow up on fixed assets service visits</span></span>
<span data-ttu-id="ec719-130">You can print the **Maintenance - Next Service** report to see which assets you have scheduled a service visit for.</span><span class="sxs-lookup"><span data-stu-id="ec719-130">You can print the **Maintenance - Next Service** report to see which assets you have scheduled a service visit for.</span></span> <span data-ttu-id="ec719-131">You can also use this report when you are updating the **Next Service Date** field on fixed asset cards.</span><span class="sxs-lookup"><span data-stu-id="ec719-131">You can also use this report when you are updating the **Next Service Date** field on fixed asset cards.</span></span>  

1. <span data-ttu-id="ec719-132">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Maintenance Next Service**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="ec719-132">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Maintenance Next Service**, and then choose the related link.</span></span>  
2. <span data-ttu-id="ec719-133">Fill in the **Starting Date** and **Ending Date** fields.</span><span class="sxs-lookup"><span data-stu-id="ec719-133">Fill in the **Starting Date** and **Ending Date** fields.</span></span>  
3. <span data-ttu-id="ec719-134">Choose the **Print** or **Preview** button.</span><span class="sxs-lookup"><span data-stu-id="ec719-134">Choose the **Print** or **Preview** button.</span></span>

## <a name="to-monitor-maintenance-costs"></a><span data-ttu-id="ec719-135">To monitor maintenance costs</span><span class="sxs-lookup"><span data-stu-id="ec719-135">To monitor maintenance costs</span></span>
<span data-ttu-id="ec719-136">You can view the maintenance costs when you look at the statistics of a fixed asset.</span><span class="sxs-lookup"><span data-stu-id="ec719-136">You can view the maintenance costs when you look at the statistics of a fixed asset.</span></span>  

1. <span data-ttu-id="ec719-137">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Fixed Assets**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="ec719-137">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Fixed Assets**, and then choose the related link.</span></span>
2. <span data-ttu-id="ec719-138">Select the fixed asset you want to view maintenance costs for, and then choose the **Depreciation Books** action.</span><span class="sxs-lookup"><span data-stu-id="ec719-138">Select the fixed asset you want to view maintenance costs for, and then choose the **Depreciation Books** action.</span></span>
3. <span data-ttu-id="ec719-139">In the **FA Depreciation Books** window, select the relevant fixed asset depreciation book, and then choose the **Statistics** action.</span><span class="sxs-lookup"><span data-stu-id="ec719-139">In the **FA Depreciation Books** window, select the relevant fixed asset depreciation book, and then choose the **Statistics** action.</span></span>
4. <span data-ttu-id="ec719-140">In the **Fixed Asset Statistics** window, choose the **Maintenance** field.</span><span class="sxs-lookup"><span data-stu-id="ec719-140">In the **Fixed Asset Statistics** window, choose the **Maintenance** field.</span></span>

<span data-ttu-id="ec719-141">The **Maintenance Ledger Entries** window opens showing the entries that make up the amount in the **Maintenance** field.</span><span class="sxs-lookup"><span data-stu-id="ec719-141">The **Maintenance Ledger Entries** window opens showing the entries that make up the amount in the **Maintenance** field.</span></span>

## <a name="to-view-or-print-maintenance-costs-for-multiple-fixed-assets"></a><span data-ttu-id="ec719-142">To view or print maintenance costs for multiple fixed assets</span><span class="sxs-lookup"><span data-stu-id="ec719-142">To view or print maintenance costs for multiple fixed assets</span></span>
<span data-ttu-id="ec719-143">In the **Maintenance - Analysis** report, you can select to see maintenance based on one, two, or three maintenance codes for a specified date or period.</span><span class="sxs-lookup"><span data-stu-id="ec719-143">In the **Maintenance - Analysis** report, you can select to see maintenance based on one, two, or three maintenance codes for a specified date or period.</span></span> <span data-ttu-id="ec719-144">You can see the total of all selected assets or a total for each asset.</span><span class="sxs-lookup"><span data-stu-id="ec719-144">You can see the total of all selected assets or a total for each asset.</span></span>

1. <span data-ttu-id="ec719-145">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Maintenance Analysis**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="ec719-145">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Maintenance Analysis**, and then choose the related link.</span></span>
2. <span data-ttu-id="ec719-146">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="ec719-146">Fill in the fields as necessary.</span></span>
3. <span data-ttu-id="ec719-147">Choose the **Print** or **Preview** button.</span><span class="sxs-lookup"><span data-stu-id="ec719-147">Choose the **Print** or **Preview** button.</span></span>

## <a name="to-view-maintenance-ledger-entries"></a><span data-ttu-id="ec719-148">To view maintenance ledger entries</span><span class="sxs-lookup"><span data-stu-id="ec719-148">To view maintenance ledger entries</span></span>
<span data-ttu-id="ec719-149">You can also study maintenance costs by viewing the maintenance ledger entries.</span><span class="sxs-lookup"><span data-stu-id="ec719-149">You can also study maintenance costs by viewing the maintenance ledger entries.</span></span>  

1. <span data-ttu-id="ec719-150">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Fixed Assets**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="ec719-150">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Fixed Assets**, and then choose the related link.</span></span>
2. <span data-ttu-id="ec719-151">Select the fixed asset that you want to view ledger entries for, and then choose the **Depreciation Books** action.</span><span class="sxs-lookup"><span data-stu-id="ec719-151">Select the fixed asset that you want to view ledger entries for, and then choose the **Depreciation Books** action.</span></span>
3. <span data-ttu-id="ec719-152">In the **FA Depreciation Books** window, select the relevant fixed asset depreciation book, and then choose the **Maintenance Ledger Entries** action.</span><span class="sxs-lookup"><span data-stu-id="ec719-152">In the **FA Depreciation Books** window, select the relevant fixed asset depreciation book, and then choose the **Maintenance Ledger Entries** action.</span></span>

## <a name="to-view-or-print-maintenance-ledger-entries-for-multiple-fixed-assets"></a><span data-ttu-id="ec719-153">To view or print maintenance ledger entries for multiple fixed assets</span><span class="sxs-lookup"><span data-stu-id="ec719-153">To view or print maintenance ledger entries for multiple fixed assets</span></span>
<span data-ttu-id="ec719-154">In the **Maintenance - Details** report, you can view or print maintenance ledger entries for one or many fixed assets.</span><span class="sxs-lookup"><span data-stu-id="ec719-154">In the **Maintenance - Details** report, you can view or print maintenance ledger entries for one or many fixed assets.</span></span>  

1. <span data-ttu-id="ec719-155">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Maintenance Details**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="ec719-155">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Maintenance Details**, and then choose the related link.</span></span>
2. <span data-ttu-id="ec719-156">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="ec719-156">Fill in the fields as necessary.</span></span>
3. <span data-ttu-id="ec719-157">Choose the **Print** or **Preview** button.</span><span class="sxs-lookup"><span data-stu-id="ec719-157">Choose the **Print** or **Preview** button.</span></span>

## <a name="see-also"></a><span data-ttu-id="ec719-158">See Also</span><span class="sxs-lookup"><span data-stu-id="ec719-158">See Also</span></span>
[<span data-ttu-id="ec719-159">Fixed Assets</span><span class="sxs-lookup"><span data-stu-id="ec719-159">Fixed Assets</span></span>](fa-manage.md)  
[<span data-ttu-id="ec719-160">Setting Up Fixed Assets</span><span class="sxs-lookup"><span data-stu-id="ec719-160">Setting Up Fixed Assets</span></span>](fa-setup.md)  
[<span data-ttu-id="ec719-161">Finance</span><span class="sxs-lookup"><span data-stu-id="ec719-161">Finance</span></span>](finance.md)  
<span data-ttu-id="ec719-162">[Welcome to [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)</span><span class="sxs-lookup"><span data-stu-id="ec719-162">[Welcome to [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)</span></span>  
<span data-ttu-id="ec719-163">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="ec719-163">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
