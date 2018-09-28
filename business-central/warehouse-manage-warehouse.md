---
title: Warehouse Activities | Microsoft Docs
description: After goods are received and before goods are shipped, a series of internal warehouse activities take place to ensure an effective flow through the warehouse and to organise and maintain company inventories.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: de9f4a202579f347e8f0ebb3196d9b812a979ca3
ms.contentlocale: en-nz
ms.lasthandoff: 09/28/2018

---
# <a name="warehouse-management"></a><span data-ttu-id="5924a-103">Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="5924a-103">Warehouse Management</span></span>
<span data-ttu-id="5924a-104">After goods are received and before goods are shipped, a series of internal warehouse activities take place to ensure an effective flow through the warehouse and to organise and maintain company inventories.</span><span class="sxs-lookup"><span data-stu-id="5924a-104">After goods are received and before goods are shipped, a series of internal warehouse activities take place to ensure an effective flow through the warehouse and to organize and maintain company inventories.</span></span>

<span data-ttu-id="5924a-105">Typical warehouse activities include putting items away, moving items inside or between warehouses, and picking items for assembly, production, or shipment.</span><span class="sxs-lookup"><span data-stu-id="5924a-105">Typical warehouse activities include putting items away, moving items inside or between warehouses, and picking items for assembly, production, or shipment.</span></span> <span data-ttu-id="5924a-106">Assembling items for sale or inventory may also be considered warehouse activities, but these are covered elsewhere.</span><span class="sxs-lookup"><span data-stu-id="5924a-106">Assembling items for sale or inventory may also be considered warehouse activities, but these are covered elsewhere.</span></span> <span data-ttu-id="5924a-107">For more information, see [Assembly Management](assembly-assemble-items.md).</span><span class="sxs-lookup"><span data-stu-id="5924a-107">For more information, see [Assembly Management](assembly-assemble-items.md).</span></span>  

<span data-ttu-id="5924a-108">In large warehouses, these different handling tasks can be separated by departments and the integration managed by a directed workflow.</span><span class="sxs-lookup"><span data-stu-id="5924a-108">In large warehouses, these different handling tasks can be separated by departments and the integration managed by a directed workflow.</span></span> <span data-ttu-id="5924a-109">In simpler installations, the flow is less formalised and the warehouse activities are performed with so-called inventory put-aways and inventory picks.</span><span class="sxs-lookup"><span data-stu-id="5924a-109">In simpler installations, the flow is less formalized and the warehouse activities are performed with so-called inventory put-aways and inventory picks.</span></span> <span data-ttu-id="5924a-110">For more information about basic versus advanced warehouse configurations, see [Design Details: Warehouse Overview](design-details-warehouse-overview.md).</span><span class="sxs-lookup"><span data-stu-id="5924a-110">For more information about basic versus advanced warehouse configurations, see [Design Details: Warehouse Overview](design-details-warehouse-overview.md).</span></span>

<span data-ttu-id="5924a-111">Before you can perform warehouse activities, you must set the system up for the relevant complexity of warehouse processing.</span><span class="sxs-lookup"><span data-stu-id="5924a-111">Before you can perform warehouse activities, you must set the system up for the relevant complexity of warehouse processing.</span></span> <span data-ttu-id="5924a-112">For more information, see [Setting Up Warehouse Management](warehouse-setup-warehouse.md).</span><span class="sxs-lookup"><span data-stu-id="5924a-112">For more information, see [Setting Up Warehouse Management](warehouse-setup-warehouse.md).</span></span>

 <span data-ttu-id="5924a-113">The following table describes a sequence of tasks, with links to the topics that describe them.</span><span class="sxs-lookup"><span data-stu-id="5924a-113">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>   

|<span data-ttu-id="5924a-114">**To**</span><span class="sxs-lookup"><span data-stu-id="5924a-114">**To**</span></span>|<span data-ttu-id="5924a-115">**See**</span><span class="sxs-lookup"><span data-stu-id="5924a-115">**See**</span></span>|  
|------------|-------------|  
|<span data-ttu-id="5924a-116">Record the receipt of items at warehouse locations, either with a purchase order only, in simple location setups, or with a warehouse receipt, in case of semi or fully automated warehouse processing at the location.</span><span class="sxs-lookup"><span data-stu-id="5924a-116">Record the receipt of items at warehouse locations, either with a purchase order only, in simple location setups, or with a warehouse receipt, in case of semi or fully automated warehouse processing at the location.</span></span>|[<span data-ttu-id="5924a-117">Receive Items</span><span class="sxs-lookup"><span data-stu-id="5924a-117">Receive Items</span></span>](warehouse-how-receive-items.md)|
|<span data-ttu-id="5924a-118">Bypass the put-away and pick processes to expedite an item straight from receiving or production to shipping.</span><span class="sxs-lookup"><span data-stu-id="5924a-118">Bypass the put-away and pick processes to expedite an item straight from receiving or production to shipping.</span></span>|[<span data-ttu-id="5924a-119">Cross-Dock Items</span><span class="sxs-lookup"><span data-stu-id="5924a-119">Cross-Dock Items</span></span>](warehouse-how-to-cross-dock-items.md)|    
|<span data-ttu-id="5924a-120">Put away items received from purchases, sales returns, transfers, or production output according to the configured warehouse process.</span><span class="sxs-lookup"><span data-stu-id="5924a-120">Put away items received from purchases, sales returns, transfers, or production output according to the configured warehouse process.</span></span>|[<span data-ttu-id="5924a-121">Putting Items Away</span><span class="sxs-lookup"><span data-stu-id="5924a-121">Putting Items Away</span></span>](warehouse-put-away-items.md)|
|<span data-ttu-id="5924a-122">Move items between bins in the warehouse.</span><span class="sxs-lookup"><span data-stu-id="5924a-122">Move items between bins in the warehouse.</span></span>|[<span data-ttu-id="5924a-123">Moving Items</span><span class="sxs-lookup"><span data-stu-id="5924a-123">Moving Items</span></span>](warehouse-move-items.md)|
|<span data-ttu-id="5924a-124">Pick items to be shipped, transferred, or consumed in assembly or production, according to the configured warehouse process.</span><span class="sxs-lookup"><span data-stu-id="5924a-124">Pick items to be shipped, transferred, or consumed in assembly or production, according to the configured warehouse process.</span></span>|[<span data-ttu-id="5924a-125">Picking Items</span><span class="sxs-lookup"><span data-stu-id="5924a-125">Picking Items</span></span>](warehouse-pick-items.md)|
|<span data-ttu-id="5924a-126">Record the shipment of items from warehouse locations, either with a sales order only, in simple location setups, or with a warehouse shipment, in case of semi or fully automated warehouse processes at the location.</span><span class="sxs-lookup"><span data-stu-id="5924a-126">Record the shipment of items from warehouse locations, either with a sales order only, in simple location setups, or with a warehouse shipment, in case of semi or fully automated warehouse processes at the location.</span></span>|[<span data-ttu-id="5924a-127">Ship Items</span><span class="sxs-lookup"><span data-stu-id="5924a-127">Ship Items</span></span>](warehouse-how-ship-items.md)|  

## <a name="see-also"></a><span data-ttu-id="5924a-128">See Also</span><span class="sxs-lookup"><span data-stu-id="5924a-128">See Also</span></span>  
[<span data-ttu-id="5924a-129">Inventory</span><span class="sxs-lookup"><span data-stu-id="5924a-129">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="5924a-130">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span><span class="sxs-lookup"><span data-stu-id="5924a-130">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span></span>  
<span data-ttu-id="5924a-131">[Assembly Management](assembly-assemble-items.md)  </span><span class="sxs-lookup"><span data-stu-id="5924a-131">[Assembly Management](assembly-assemble-items.md)  </span></span>  
[<span data-ttu-id="5924a-132">Design Details: Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="5924a-132">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="5924a-133">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="5924a-133">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  

## [!INCLUDE[d365fin](includes/free_trial_md.md)]  
 

