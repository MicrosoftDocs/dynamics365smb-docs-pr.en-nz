---
title: Design Details - Availability in the Warehouse | Microsoft Docs
description: The system must keep a constant control of item availability in the warehouse, so that outbound orders can flow efficiently and provide optimal deliveries.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 698404dab1b3888d073eb3c23268d3b009a4f577
ms.contentlocale: en-nz
ms.lasthandoff: 03/22/2018

---
# <a name="design-details-availability-in-the-warehouse"></a><span data-ttu-id="90578-103">Design Details: Availability in the Warehouse</span><span class="sxs-lookup"><span data-stu-id="90578-103">Design Details: Availability in the Warehouse</span></span>
<span data-ttu-id="90578-104">The system must keep a constant control of item availability in the warehouse, so that outbound orders can flow efficiently and provide optimal deliveries.</span><span class="sxs-lookup"><span data-stu-id="90578-104">The system must keep a constant control of item availability in the warehouse, so that outbound orders can flow efficiently and provide optimal deliveries.</span></span>  

 <span data-ttu-id="90578-105">Availability varies depending on allocations at the bin level when warehouse activities such as picks and movements occur and when the inventory reservation system imposes restrictions to comply with.</span><span class="sxs-lookup"><span data-stu-id="90578-105">Availability varies depending on allocations at the bin level when warehouse activities such as picks and movements occur and when the inventory reservation system imposes restrictions to comply with.</span></span> <span data-ttu-id="90578-106">A rather complex algorithm verifies that all conditions are met before allocating quantities to picks for outbound flows.</span><span class="sxs-lookup"><span data-stu-id="90578-106">A rather complex algorithm verifies that all conditions are met before allocating quantities to picks for outbound flows.</span></span>  

## <a name="bin-content-and-reservations"></a><span data-ttu-id="90578-107">Bin Content and Reservations</span><span class="sxs-lookup"><span data-stu-id="90578-107">Bin Content and Reservations</span></span>  
 <span data-ttu-id="90578-108">In any installation of warehouse management, item quantities exist both as warehouse entries, in the Warehouse application area, and as item ledger entries, in the Inventory application area.</span><span class="sxs-lookup"><span data-stu-id="90578-108">In any installation of warehouse management, item quantities exist both as warehouse entries, in the Warehouse application area, and as item ledger entries, in the Inventory application area.</span></span> <span data-ttu-id="90578-109">These two entry types contain different information about where items exist and whether they are available.</span><span class="sxs-lookup"><span data-stu-id="90578-109">These two entry types contain different information about where items exist and whether they are available.</span></span> <span data-ttu-id="90578-110">Warehouse entries define an item’s availability by bin and bin type, which is called bin content.</span><span class="sxs-lookup"><span data-stu-id="90578-110">Warehouse entries define an item’s availability by bin and bin type, which is called bin content.</span></span> <span data-ttu-id="90578-111">Item ledger entries define an item’s availability by its reservation to outbound documents.</span><span class="sxs-lookup"><span data-stu-id="90578-111">Item ledger entries define an item’s availability by its reservation to outbound documents.</span></span>  

 <span data-ttu-id="90578-112">Special functionality in the picking algorithm exists to calculate the quantity that is available to pick when bin content is coupled with reservations.</span><span class="sxs-lookup"><span data-stu-id="90578-112">Special functionality in the picking algorithm exists to calculate the quantity that is available to pick when bin content is coupled with reservations.</span></span>  

## <a name="quantity-available-to-pick"></a><span data-ttu-id="90578-113">Quantity Available to Pick</span><span class="sxs-lookup"><span data-stu-id="90578-113">Quantity Available to Pick</span></span>  
 <span data-ttu-id="90578-114">If, for example, the picking algorithm does not consider item quantities that are reserved for a pending sales order shipment, then those items might be picked for another sales order that is shipped earlier, which prevents the first sales from being fulfilled.</span><span class="sxs-lookup"><span data-stu-id="90578-114">If, for example, the picking algorithm does not consider item quantities that are reserved for a pending sales order shipment, then those items might be picked for another sales order that is shipped earlier, which prevents the first sales from being fulfilled.</span></span> <span data-ttu-id="90578-115">To avoid this situation, the picking algorithm subtracts quantities that are reserved for other outbound documents, quantities on existing pick documents, and quantities that are picked but not yet shipped or consumed.</span><span class="sxs-lookup"><span data-stu-id="90578-115">To avoid this situation, the picking algorithm subtracts quantities that are reserved for other outbound documents, quantities on existing pick documents, and quantities that are picked but not yet shipped or consumed.</span></span>  

 <span data-ttu-id="90578-116">The result is displayed in the **Available Qty. to Pick** field in the **Pick Worksheet** window, where the field is calculated dynamically.</span><span class="sxs-lookup"><span data-stu-id="90578-116">The result is displayed in the **Available Qty. to Pick** field in the **Pick Worksheet** window, where the field is calculated dynamically.</span></span> <span data-ttu-id="90578-117">The value is also calculated when users create warehouse picks directly for outbound documents.</span><span class="sxs-lookup"><span data-stu-id="90578-117">The value is also calculated when users create warehouse picks directly for outbound documents.</span></span> <span data-ttu-id="90578-118">Such outbound documents could be sales orders, production consumption, or outbound transfers, where the result is reflected in the related quantity fields, such as **Qty. to Handle**.</span><span class="sxs-lookup"><span data-stu-id="90578-118">Such outbound documents could be sales orders, production consumption, or outbound transfers, where the result is reflected in the related quantity fields, such as **Qty. to Handle**.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="90578-119">Concerning the priority of reservations, the quantity to reserve is subtracted from the quantity available to pick.</span><span class="sxs-lookup"><span data-stu-id="90578-119">Concerning the priority of reservations, the quantity to reserve is subtracted from the quantity available to pick.</span></span> <span data-ttu-id="90578-120">For example, if the quantity available in pick bins is 5 units, but 100 units are in put-away bins, then when you try to reserve more than 5 units for another order, an error message is displayed because the additional quantity must be available in pick bins.</span><span class="sxs-lookup"><span data-stu-id="90578-120">For example, if the quantity available in pick bins is 5 units, but 100 units are in put-away bins, then when you try to reserve more than 5 units for another order, an error message is displayed because the additional quantity must be available in pick bins.</span></span>  

### <a name="calculating-the-quantity-available-to-pick"></a><span data-ttu-id="90578-121">Calculating the Quantity Available to Pick</span><span class="sxs-lookup"><span data-stu-id="90578-121">Calculating the Quantity Available to Pick</span></span>  
 <span data-ttu-id="90578-122">The quantity available to pick is calculated as follows:</span><span class="sxs-lookup"><span data-stu-id="90578-122">The quantity available to pick is calculated as follows:</span></span>  

 <span data-ttu-id="90578-123">quantity available to pick = quantity in pick bins - quantity on picks and movements – (reserved quantity in pick bins + reserved quantity on picks and movements)</span><span class="sxs-lookup"><span data-stu-id="90578-123">quantity available to pick = quantity in pick bins - quantity on picks and movements – (reserved quantity in pick bins + reserved quantity on picks and movements)</span></span>  

 <span data-ttu-id="90578-124">The following diagram shows the different elements of the calculation.</span><span class="sxs-lookup"><span data-stu-id="90578-124">The following diagram shows the different elements of the calculation.</span></span>  

 <span data-ttu-id="90578-125">![Available to pick, with reservation overlap](media/design_details_warehouse_management_availability_2.png "design_details_warehouse_management_availability_2")</span><span class="sxs-lookup"><span data-stu-id="90578-125">![Available to pick, with reservation overlap](media/design_details_warehouse_management_availability_2.png "design_details_warehouse_management_availability_2")</span></span>  

## <a name="quantity-available-to-reserve"></a><span data-ttu-id="90578-126">Quantity Available to Reserve</span><span class="sxs-lookup"><span data-stu-id="90578-126">Quantity Available to Reserve</span></span>  
 <span data-ttu-id="90578-127">Because the concepts of bin content and reservation co-exist, the quantity of items that are available to reserve must be aligned with allocations to outbound warehouse documents.</span><span class="sxs-lookup"><span data-stu-id="90578-127">Because the concepts of bin content and reservation co-exist, the quantity of items that are available to reserve must be aligned with allocations to outbound warehouse documents.</span></span>  

 <span data-ttu-id="90578-128">It should be possible to reserve all items in inventory, except those that have started outbound processing.</span><span class="sxs-lookup"><span data-stu-id="90578-128">It should be possible to reserve all items in inventory, except those that have started outbound processing.</span></span> <span data-ttu-id="90578-129">Accordingly, the quantity that is available to reserve is defined as the quantity on all documents and all bin types, except the following outbound quantities:</span><span class="sxs-lookup"><span data-stu-id="90578-129">Accordingly, the quantity that is available to reserve is defined as the quantity on all documents and all bin types, except the following outbound quantities:</span></span>  

-   <span data-ttu-id="90578-130">Quantity on unregistered pick documents</span><span class="sxs-lookup"><span data-stu-id="90578-130">Quantity on unregistered pick documents</span></span>  
-   <span data-ttu-id="90578-131">Quantity in shipment bins</span><span class="sxs-lookup"><span data-stu-id="90578-131">Quantity in shipment bins</span></span>  
-   <span data-ttu-id="90578-132">Quantity in to-production bins</span><span class="sxs-lookup"><span data-stu-id="90578-132">Quantity in to-production bins</span></span>  
-   <span data-ttu-id="90578-133">Quantity in open shop floor bins</span><span class="sxs-lookup"><span data-stu-id="90578-133">Quantity in open shop floor bins</span></span>  
-   <span data-ttu-id="90578-134">Quantity in to-assembly bins</span><span class="sxs-lookup"><span data-stu-id="90578-134">Quantity in to-assembly bins</span></span>  
-   <span data-ttu-id="90578-135">Quantity in adjustment bins</span><span class="sxs-lookup"><span data-stu-id="90578-135">Quantity in adjustment bins</span></span>  

 <span data-ttu-id="90578-136">The result is displayed in the **Total Available Quantity** field in the **Reservation** window.</span><span class="sxs-lookup"><span data-stu-id="90578-136">The result is displayed in the **Total Available Quantity** field in the **Reservation** window.</span></span>  

 <span data-ttu-id="90578-137">On a reservation line, the quantity that cannot be reserved, because it is allocated in the warehouse, is displayed in the **Qty. Allocated in Warehouse** field in the **Reservation** window.</span><span class="sxs-lookup"><span data-stu-id="90578-137">On a reservation line, the quantity that cannot be reserved, because it is allocated in the warehouse, is displayed in the **Qty. Allocated in Warehouse** field in the **Reservation** window.</span></span>  

### <a name="calculating-the-quantity-available-to-reserve"></a><span data-ttu-id="90578-138">Calculating the Quantity Available to Reserve</span><span class="sxs-lookup"><span data-stu-id="90578-138">Calculating the Quantity Available to Reserve</span></span>  
 <span data-ttu-id="90578-139">The quantity available to reserve is calculated as follows:</span><span class="sxs-lookup"><span data-stu-id="90578-139">The quantity available to reserve is calculated as follows:</span></span>  

 <span data-ttu-id="90578-140">quantity available to reserve = total quantity in inventory - quantity on picks and movements for source documents - reserved quantity - quantity in outbound bins</span><span class="sxs-lookup"><span data-stu-id="90578-140">quantity available to reserve = total quantity in inventory - quantity on picks and movements for source documents - reserved quantity - quantity in outbound bins</span></span>  

 <span data-ttu-id="90578-141">The following diagram shows the different elements of the calculation.</span><span class="sxs-lookup"><span data-stu-id="90578-141">The following diagram shows the different elements of the calculation.</span></span>  

 <span data-ttu-id="90578-142">![Avaliable to reserve, per warehouse allocations](media/design_details_warehouse_management_availability_3.png "design_details_warehouse_management_availability_3")</span><span class="sxs-lookup"><span data-stu-id="90578-142">![Avaliable to reserve, per warehouse allocations](media/design_details_warehouse_management_availability_3.png "design_details_warehouse_management_availability_3")</span></span>  

## <a name="see-also"></a><span data-ttu-id="90578-143">See Also</span><span class="sxs-lookup"><span data-stu-id="90578-143">See Also</span></span>  
 [<span data-ttu-id="90578-144">Design Details: Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="90578-144">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)
