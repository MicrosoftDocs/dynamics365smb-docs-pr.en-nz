---
title: Warehouse Activities | Microsoft Docs
description: After goods are received and before goods are shipped, a series of internal warehouse activities take place to ensure an effective flow through the warehouse and to organise and maintain company inventories.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/15/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: c1ea1c4a5ea4b917243d60981ec35050895f82a7
ms.contentlocale: en-nz
ms.lasthandoff: 09/22/2017

---
# <a name="warehouse-management"></a><span data-ttu-id="5b443-103">Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="5b443-103">Warehouse Management</span></span>
<span data-ttu-id="5b443-104">After goods are received and before goods are shipped, a series of internal warehouse activities take place to ensure an effective flow through the warehouse and to organise and maintain company inventories.</span><span class="sxs-lookup"><span data-stu-id="5b443-104">After goods are received and before goods are shipped, a series of internal warehouse activities take place to ensure an effective flow through the warehouse and to organize and maintain company inventories.</span></span>

<span data-ttu-id="5b443-105">Typical warehouse activities include putting items away, moving items inside or between warehouses, and picking items for assembly, production, or shipment.</span><span class="sxs-lookup"><span data-stu-id="5b443-105">Typical warehouse activities include putting items away, moving items inside or between warehouses, and picking items for assembly, production, or shipment.</span></span> <span data-ttu-id="5b443-106">Assembling items for sale or inventory may also be considered warehouse activities, but these are covered elsewhere.</span><span class="sxs-lookup"><span data-stu-id="5b443-106">Assembling items for sale or inventory may also be considered warehouse activities, but these are covered elsewhere.</span></span> <span data-ttu-id="5b443-107">For more information, see [Assembly Management](assembly-assemble-items.md).</span><span class="sxs-lookup"><span data-stu-id="5b443-107">For more information, see [Assembly Management](assembly-assemble-items.md).</span></span>  

<span data-ttu-id="5b443-108">In large warehouses, these different handling tasks can be separated by departments and the integration managed by a directed workflow.</span><span class="sxs-lookup"><span data-stu-id="5b443-108">In large warehouses, these different handling tasks can be separated by departments and the integration managed by a directed workflow.</span></span> <span data-ttu-id="5b443-109">In simpler installations, the flow is less formalised and the warehouse activities are performed with so-called inventory put-aways and inventory picks.</span><span class="sxs-lookup"><span data-stu-id="5b443-109">In simpler installations, the flow is less formalized and the warehouse activities are performed with so-called inventory put-aways and inventory picks.</span></span> <span data-ttu-id="5b443-110">For more information about basic versus advanced warehouse configurations, see [Design Details: Warehouse Overview](design-details-warehouse-overview.md).</span><span class="sxs-lookup"><span data-stu-id="5b443-110">For more information about basic versus advanced warehouse configurations, see [Design Details: Warehouse Overview](design-details-warehouse-overview.md).</span></span>

<span data-ttu-id="5b443-111">Before you can perform warehouse activities, you must set the system up for the relevant complexity of warehouse processing.</span><span class="sxs-lookup"><span data-stu-id="5b443-111">Before you can perform warehouse activities, you must set the system up for the relevant complexity of warehouse processing.</span></span> <span data-ttu-id="5b443-112">For more information, see [Setting Up Warehouse Management](warehouse-setup-warehouse.md).</span><span class="sxs-lookup"><span data-stu-id="5b443-112">For more information, see [Setting Up Warehouse Management](warehouse-setup-warehouse.md).</span></span>

 <span data-ttu-id="5b443-113">The following table describes a sequence of tasks, with links to the topics that describe them.</span><span class="sxs-lookup"><span data-stu-id="5b443-113">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>   

|<span data-ttu-id="5b443-114">**To**</span><span class="sxs-lookup"><span data-stu-id="5b443-114">**To**</span></span>|<span data-ttu-id="5b443-115">**See**</span><span class="sxs-lookup"><span data-stu-id="5b443-115">**See**</span></span>|  
|------------|-------------|  
|<span data-ttu-id="5b443-116">Record the receipt of items at warehouse locations, either with a purchase order only, in simple location setups, or with a warehouse receipt, in case of semi or fully automated warehouse processing at the location.</span><span class="sxs-lookup"><span data-stu-id="5b443-116">Record the receipt of items at warehouse locations, either with a purchase order only, in simple location setups, or with a warehouse receipt, in case of semi or fully automated warehouse processing at the location.</span></span>|[<span data-ttu-id="5b443-117">How to: Receive Items</span><span class="sxs-lookup"><span data-stu-id="5b443-117">How to: Receive Items</span></span>](warehouse-how-receive-items.md)|
|<span data-ttu-id="5b443-118">Bypass the put-away and pick processes to expedite an item straight from receiving or production to shipping.</span><span class="sxs-lookup"><span data-stu-id="5b443-118">Bypass the put-away and pick processes to expedite an item straight from receiving or production to shipping.</span></span>|[<span data-ttu-id="5b443-119">How to: Cross-Dock Items</span><span class="sxs-lookup"><span data-stu-id="5b443-119">How to: Cross-Dock Items</span></span>](warehouse-how-to-cross-dock-items.md)|    
|<span data-ttu-id="5b443-120">Put away items received from purchases, sales returns, transfers, or production output according to the configured warehouse process.</span><span class="sxs-lookup"><span data-stu-id="5b443-120">Put away items received from purchases, sales returns, transfers, or production output according to the configured warehouse process.</span></span>|[<span data-ttu-id="5b443-121">Putting Items Away</span><span class="sxs-lookup"><span data-stu-id="5b443-121">Putting Items Away</span></span>](warehouse-put-away-items.md)|
|<span data-ttu-id="5b443-122">Move items between bins in the warehouse.</span><span class="sxs-lookup"><span data-stu-id="5b443-122">Move items between bins in the warehouse.</span></span>|[<span data-ttu-id="5b443-123">Moving Items</span><span class="sxs-lookup"><span data-stu-id="5b443-123">Moving Items</span></span>](warehouse-move-items.md)|
|<span data-ttu-id="5b443-124">Pick items to be shipped, transferred, or consumed in assembly or production, according to the configured warehouse process.</span><span class="sxs-lookup"><span data-stu-id="5b443-124">Pick items to be shipped, transferred, or consumed in assembly or production, according to the configured warehouse process.</span></span>|[<span data-ttu-id="5b443-125">Picking Items</span><span class="sxs-lookup"><span data-stu-id="5b443-125">Picking Items</span></span>](warehouse-pick-items.md)|
|<span data-ttu-id="5b443-126">Record the shipment of items from warehouse locations, either with a sales order only, in simple location setups, or with a warehouse shipment, in case of semi or fully automated warehouse processes at the location.</span><span class="sxs-lookup"><span data-stu-id="5b443-126">Record the shipment of items from warehouse locations, either with a sales order only, in simple location setups, or with a warehouse shipment, in case of semi or fully automated warehouse processes at the location.</span></span>|[<span data-ttu-id="5b443-127">How to: Ship Items</span><span class="sxs-lookup"><span data-stu-id="5b443-127">How to: Ship Items</span></span>](warehouse-how-ship-items.md)|  

## <a name="see-also"></a><span data-ttu-id="5b443-128">See Also</span><span class="sxs-lookup"><span data-stu-id="5b443-128">See Also</span></span>  
 [<span data-ttu-id="5b443-129">Inventory</span><span class="sxs-lookup"><span data-stu-id="5b443-129">Inventory</span></span>](inventory-manage-inventory.md)  
 <span data-ttu-id="5b443-130">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span><span class="sxs-lookup"><span data-stu-id="5b443-130">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span></span>  
 <span data-ttu-id="5b443-131">[Assembly Management](assembly-assemble-items.md)  </span><span class="sxs-lookup"><span data-stu-id="5b443-131">[Assembly Management](assembly-assemble-items.md)  </span></span>  
[<span data-ttu-id="5b443-132">Design Details: Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="5b443-132">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
 <span data-ttu-id="5b443-133">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="5b443-133">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  

