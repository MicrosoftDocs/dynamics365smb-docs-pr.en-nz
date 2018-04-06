---
title: Transfer Items Between Warehouse Locations| Microsoft Docs
description: Describes how to move inventory from one place or warehouse to another, either with the reclassification journal or with transfer orders.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: move, warehouse
ms.date: 01/25/2018
ms.author: SorenGP
ms.translationtype: HT
ms.sourcegitcommit: b34f276a764f0e828fbc1f015429df9852242a4c
ms.openlocfilehash: 8ee703865f86c0edcc5bff77d8bd04cc2bd107be
ms.contentlocale: en-nz
ms.lasthandoff: 03/22/2018

---
# <a name="transfer-inventory-between-locations"></a><span data-ttu-id="e80be-103">Transfer Inventory Between Locations</span><span class="sxs-lookup"><span data-stu-id="e80be-103">Transfer Inventory Between Locations</span></span>
<span data-ttu-id="e80be-104">You can transfer inventory items between locations by creating transfer orders.</span><span class="sxs-lookup"><span data-stu-id="e80be-104">You can transfer inventory items between locations by creating transfer orders.</span></span> <span data-ttu-id="e80be-105">Alternatively, you can use the item reclassification journal.</span><span class="sxs-lookup"><span data-stu-id="e80be-105">Alternatively, you can use the item reclassification journal.</span></span>

<span data-ttu-id="e80be-106">With transfer orders, you ship the outbound transfer from one location and receive the inbound transfer at the other location.</span><span class="sxs-lookup"><span data-stu-id="e80be-106">With transfer orders, you ship the outbound transfer from one location and receive the inbound transfer at the other location.</span></span> <span data-ttu-id="e80be-107">This allows you to manage the involved warehouse activities and provides more certainty that inventory quantities are updated correctly.</span><span class="sxs-lookup"><span data-stu-id="e80be-107">This allows you to manage the involved warehouse activities and provides more certainty that inventory quantities are updated correctly.</span></span>

<span data-ttu-id="e80be-108">With the reclassification journal, you simply fill in the **Location Code** and the **New Location Code** fields.</span><span class="sxs-lookup"><span data-stu-id="e80be-108">With the reclassification journal, you simply fill in the **Location Code** and the **New Location Code** fields.</span></span> <span data-ttu-id="e80be-109">When you post the journal, the item ledger entries are adjusted at the locations in question.</span><span class="sxs-lookup"><span data-stu-id="e80be-109">When you post the journal, the item ledger entries are adjusted at the locations in question.</span></span> <span data-ttu-id="e80be-110">With this method, warehouse activities are not managed.</span><span class="sxs-lookup"><span data-stu-id="e80be-110">With this method, warehouse activities are not managed.</span></span>

> [!NOTE]  
>   <span data-ttu-id="e80be-111">If you have items recorded in your inventory without a location code, for example from a time when you only had one warehouse, then you cannot transfer those items using transfer orders.</span><span class="sxs-lookup"><span data-stu-id="e80be-111">If you have items recorded in your inventory without a location code, for example from a time when you only had one warehouse, then you cannot transfer those items using transfer orders.</span></span> <span data-ttu-id="e80be-112">Instead, you must use the reclassification journal to reclassify the items from a blank location code to an actual location code.</span><span class="sxs-lookup"><span data-stu-id="e80be-112">Instead, you must use the reclassification journal to reclassify the items from a blank location code to an actual location code.</span></span>  <span data-ttu-id="e80be-113">For more information, see step 3 in the "To transfer items with the item reclassification journal" section.</span><span class="sxs-lookup"><span data-stu-id="e80be-113">For more information, see step 3 in the "To transfer items with the item reclassification journal" section.</span></span>

<span data-ttu-id="e80be-114">To transfer items, locations and transfer routes must be set up.</span><span class="sxs-lookup"><span data-stu-id="e80be-114">To transfer items, locations and transfer routes must be set up.</span></span> <span data-ttu-id="e80be-115">For more information, see [Set Up Locations](inventory-how-setup-locations.md).</span><span class="sxs-lookup"><span data-stu-id="e80be-115">For more information, see [Set Up Locations](inventory-how-setup-locations.md).</span></span>

## <a name="to-transfer-items-with-a-transfer-order"></a><span data-ttu-id="e80be-116">To transfer items with a transfer order</span><span class="sxs-lookup"><span data-stu-id="e80be-116">To transfer items with a transfer order</span></span>
1. <span data-ttu-id="e80be-117">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Transfer orders**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="e80be-117">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Transfer orders**, and then choose the related link.</span></span>
2. <span data-ttu-id="e80be-118">In the **Transfer Order** window, fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="e80be-118">In the **Transfer Order** window, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

    > [!NOTE]  
>   <span data-ttu-id="e80be-119">If you have filled in the **In-Transit Code**, **Shipping Agent Code**, and **Shipping Agent Service** fields in the **Trans. Route Spec.** window when you set up the transfer route, then the corresponding fields on the transfer order are filled in automatically.</span><span class="sxs-lookup"><span data-stu-id="e80be-119">If you have filled in the **In-Transit Code**, **Shipping Agent Code**, and **Shipping Agent Service** fields in the **Trans. Route Spec.** window when you set up the transfer route, then the corresponding fields on the transfer order are filled in automatically.</span></span>

    <span data-ttu-id="e80be-120">When you fill in the **Shipping Agent Service** field, the receipt date at the transfer-to location is calculated by adding the shipping time of the shipping agent service to the shipment date.</span><span class="sxs-lookup"><span data-stu-id="e80be-120">When you fill in the **Shipping Agent Service** field, the receipt date at the transfer-to location is calculated by adding the shipping time of the shipping agent service to the shipment date.</span></span>

    <span data-ttu-id="e80be-121">As a warehouse worker at the transfer-from location, proceed to ship the items.</span><span class="sxs-lookup"><span data-stu-id="e80be-121">As a warehouse worker at the transfer-from location, proceed to ship the items.</span></span>
3. <span data-ttu-id="e80be-122">Choose the **Post** action, choose the **Ship** option, and then choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="e80be-122">Choose the **Post** action, choose the **Ship** option, and then choose the **OK** button.</span></span>

    <span data-ttu-id="e80be-123">The items are now in transit between the specified locations, according to the specifies transfer route.</span><span class="sxs-lookup"><span data-stu-id="e80be-123">The items are now in transit between the specified locations, according to the specifies transfer route.</span></span>

    <span data-ttu-id="e80be-124">As a warehouse worker at the transfer-from location, proceed to receive the items.</span><span class="sxs-lookup"><span data-stu-id="e80be-124">As a warehouse worker at the transfer-from location, proceed to receive the items.</span></span>
4. <span data-ttu-id="e80be-125">Choose the **Post** action, choose the **Receive** option, and then choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="e80be-125">Choose the **Post** action, choose the **Receive** option, and then choose the **OK** button.</span></span>

## <a name="to-transfer-items-with-the-item-reclassification-journal"></a><span data-ttu-id="e80be-126">To transfer items with the item reclassification journal</span><span class="sxs-lookup"><span data-stu-id="e80be-126">To transfer items with the item reclassification journal</span></span>
1. <span data-ttu-id="e80be-127">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Item Reclass. Journals**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="e80be-127">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Item Reclass. Journals**, and then choose the related link.</span></span>
2. <span data-ttu-id="e80be-128">In the **Item Reclass. Journal** window, fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="e80be-128">In the **Item Reclass. Journal** window, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. <span data-ttu-id="e80be-129">In the **Location Code** field, enter the location where the items are currently stored.</span><span class="sxs-lookup"><span data-stu-id="e80be-129">In the **Location Code** field, enter the location where the items are currently stored.</span></span>

    > [!NOTE]  
>   <span data-ttu-id="e80be-130">To transfer items that have no location code, leave the **Location Code** field blank.</span><span class="sxs-lookup"><span data-stu-id="e80be-130">To transfer items that have no location code, leave the **Location Code** field blank.</span></span>
4. <span data-ttu-id="e80be-131">In the **New Location Code** field, enter the location that you want to transfer the items to.</span><span class="sxs-lookup"><span data-stu-id="e80be-131">In the **New Location Code** field, enter the location that you want to transfer the items to.</span></span>
5. <span data-ttu-id="e80be-132">Choose the **Post** action.</span><span class="sxs-lookup"><span data-stu-id="e80be-132">Choose the **Post** action.</span></span>

## <a name="see-also"></a><span data-ttu-id="e80be-133">See Also</span><span class="sxs-lookup"><span data-stu-id="e80be-133">See Also</span></span>
[<span data-ttu-id="e80be-134">Manage Inventory</span><span class="sxs-lookup"><span data-stu-id="e80be-134">Manage Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="e80be-135">Set Up Locations</span><span class="sxs-lookup"><span data-stu-id="e80be-135">Set Up Locations</span></span>](inventory-how-setup-locations.md)  

<span data-ttu-id="e80be-136">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="e80be-136">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
<span data-ttu-id="e80be-137">[Customizing Your [!INCLUDE[d365fin](includes/d365fin_md.md)] Experience](ui-experiences.md)</span><span class="sxs-lookup"><span data-stu-id="e80be-137">[Customizing Your [!INCLUDE[d365fin](includes/d365fin_md.md)] Experience](ui-experiences.md)</span></span>  
[<span data-ttu-id="e80be-138">General Business Functionality</span><span class="sxs-lookup"><span data-stu-id="e80be-138">General Business Functionality</span></span>](ui-across-business-areas.md)

