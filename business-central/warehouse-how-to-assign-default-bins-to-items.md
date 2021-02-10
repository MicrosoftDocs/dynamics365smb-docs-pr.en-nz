---
title: How to Assign Default Bins to Items | Microsoft Docs
description: If you are using bins at a location, assigning default bins to your items can make the process of shipping, receiving, and moving your items much easier. When a default bin is assigned to an item, this bin is suggested every time you initiate a transaction for this item.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: f3374929434876cee088f046efc6d5f950671cc8
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 12/17/2020
ms.locfileid: "4756333"
---
# <a name="assign-default-bins-to-items"></a><span data-ttu-id="ad35f-104">Assign Default Bins to Items</span><span class="sxs-lookup"><span data-stu-id="ad35f-104">Assign Default Bins to Items</span></span>
<span data-ttu-id="ad35f-105">If you are using bins at a location, assigning default bins to your items can make the process of shipping, receiving, and moving your items much easier.</span><span class="sxs-lookup"><span data-stu-id="ad35f-105">If you are using bins at a location, assigning default bins to your items can make the process of shipping, receiving, and moving your items much easier.</span></span> <span data-ttu-id="ad35f-106">When a default bin is assigned to an item, this bin is suggested every time you initiate a transaction for this item.</span><span class="sxs-lookup"><span data-stu-id="ad35f-106">When a default bin is assigned to an item, this bin is suggested every time you initiate a transaction for this item.</span></span> <span data-ttu-id="ad35f-107">Default bins are defined on the **Bin Content** page.</span><span class="sxs-lookup"><span data-stu-id="ad35f-107">Default bins are defined on the **Bin Content** page.</span></span>  

## <a name="to-assign-a-default-bin-to-an-item"></a><span data-ttu-id="ad35f-108">To assign a default bin to an item</span><span class="sxs-lookup"><span data-stu-id="ad35f-108">To assign a default bin to an item</span></span>
1.  <span data-ttu-id="ad35f-109">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Bin Content Creation Worksheet**, and choose the related link.</span><span class="sxs-lookup"><span data-stu-id="ad35f-109">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Bin Content Creation Worksheet**, and choose the related link.</span></span>  
2.  <span data-ttu-id="ad35f-110">Fill in the bin code and item information for each bin that you would like to set up as a default for an item.</span><span class="sxs-lookup"><span data-stu-id="ad35f-110">Fill in the bin code and item information for each bin that you would like to set up as a default for an item.</span></span> <span data-ttu-id="ad35f-111">Make sure to select the **Default** field.</span><span class="sxs-lookup"><span data-stu-id="ad35f-111">Make sure to select the **Default** field.</span></span>  
3.  <span data-ttu-id="ad35f-112">Choose the **Create Bin Content** action.</span><span class="sxs-lookup"><span data-stu-id="ad35f-112">Choose the **Create Bin Content** action.</span></span> <span data-ttu-id="ad35f-113">Default bins are now assigned for your item.</span><span class="sxs-lookup"><span data-stu-id="ad35f-113">Default bins are now assigned for your item.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="ad35f-114">When an item is put away, if the item does not have a default bin assigned, the bin where the item is put away is assigned as the default.</span><span class="sxs-lookup"><span data-stu-id="ad35f-114">When an item is put away, if the item does not have a default bin assigned, the bin where the item is put away is assigned as the default.</span></span>  

## <a name="to-change-the-default-bin-for-an-item"></a><span data-ttu-id="ad35f-115">To change the default bin for an item</span><span class="sxs-lookup"><span data-stu-id="ad35f-115">To change the default bin for an item</span></span>  
<span data-ttu-id="ad35f-116">You may need to change the default bin assignment for an item or assign a default bin to a new item.</span><span class="sxs-lookup"><span data-stu-id="ad35f-116">You may need to change the default bin assignment for an item or assign a default bin to a new item.</span></span>    
1.  <span data-ttu-id="ad35f-117">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Bin Contents**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="ad35f-117">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Bin Contents**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="ad35f-118">In the **Location Filter** field, select the appropriate location code.</span><span class="sxs-lookup"><span data-stu-id="ad35f-118">In the **Location Filter** field, select the appropriate location code.</span></span>  
3.  <span data-ttu-id="ad35f-119">Find the current default bin content entry for the item and clear the **Default Bin** check box.</span><span class="sxs-lookup"><span data-stu-id="ad35f-119">Find the current default bin content entry for the item and clear the **Default Bin** check box.</span></span>  
4.  <span data-ttu-id="ad35f-120">Find the bin content line for the bin that you would like as the new default bin.</span><span class="sxs-lookup"><span data-stu-id="ad35f-120">Find the bin content line for the bin that you would like as the new default bin.</span></span> <span data-ttu-id="ad35f-121">Select the **Default Bin** check box.</span><span class="sxs-lookup"><span data-stu-id="ad35f-121">Select the **Default Bin** check box.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="ad35f-122">When an item is put away for the first time, and the item does not have a default bin assigned, the system will assign the bin where the item is put away as the default bin for the item.</span><span class="sxs-lookup"><span data-stu-id="ad35f-122">When an item is put away for the first time, and the item does not have a default bin assigned, the system will assign the bin where the item is put away as the default bin for the item.</span></span>  

## <a name="see-also"></a><span data-ttu-id="ad35f-123">See Also</span><span class="sxs-lookup"><span data-stu-id="ad35f-123">See Also</span></span>  
[<span data-ttu-id="ad35f-124">Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="ad35f-124">Warehouse Management</span></span>](warehouse-manage-warehouse.md)  
[<span data-ttu-id="ad35f-125">Inventory</span><span class="sxs-lookup"><span data-stu-id="ad35f-125">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="ad35f-126">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span><span class="sxs-lookup"><span data-stu-id="ad35f-126">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span></span>  
<span data-ttu-id="ad35f-127">[Assembly Management](assembly-assemble-items.md)  </span><span class="sxs-lookup"><span data-stu-id="ad35f-127">[Assembly Management](assembly-assemble-items.md)  </span></span>  
[<span data-ttu-id="ad35f-128">Design Details: Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="ad35f-128">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="ad35f-129">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="ad35f-129">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>
