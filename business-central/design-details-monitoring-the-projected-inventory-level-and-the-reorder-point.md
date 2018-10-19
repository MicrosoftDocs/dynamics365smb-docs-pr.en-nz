---
title: Design Details - Monitoring the Projected Inventory Level and the Reorder Point | Microsoft Docs
description: Learn how inventory planning distinguishes between projected inventory and projected available inventory levels.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: design, supply, inventory, planning
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: 336b5c300cf3640d7356313d2d627f6b4008c7b4
ms.contentlocale: en-nz
ms.lasthandoff: 09/28/2018

---
# <a name="design-details-monitoring-the-projected-inventory-level-and-the-reorder-point"></a><span data-ttu-id="afcc4-103">Design Details: Monitoring the Projected Inventory Level and the Reorder Point</span><span class="sxs-lookup"><span data-stu-id="afcc4-103">Design Details: Monitoring the Projected Inventory Level and the Reorder Point</span></span>
<span data-ttu-id="afcc4-104">Inventory is a type of supply, but for inventory planning, the planning system distinguishes between two inventory levels:</span><span class="sxs-lookup"><span data-stu-id="afcc4-104">Inventory is a type of supply, but for inventory planning, the planning system distinguishes between two inventory levels:</span></span>  

* <span data-ttu-id="afcc4-105">Projected inventory</span><span class="sxs-lookup"><span data-stu-id="afcc4-105">Projected inventory</span></span>  
* <span data-ttu-id="afcc4-106">Projected available inventory</span><span class="sxs-lookup"><span data-stu-id="afcc4-106">Projected available inventory</span></span>  

## <a name="projected-inventory"></a><span data-ttu-id="afcc4-107">Projected Inventory</span><span class="sxs-lookup"><span data-stu-id="afcc4-107">Projected Inventory</span></span>  
<span data-ttu-id="afcc4-108">Initially, projected inventory is the quantity of gross inventory, including supply and demand in the past even if not posted, when starting the planning process.</span><span class="sxs-lookup"><span data-stu-id="afcc4-108">Initially, projected inventory is the quantity of gross inventory, including supply and demand in the past even if not posted, when starting the planning process.</span></span> <span data-ttu-id="afcc4-109">In the future, this becomes a moving projected inventory level that is maintained by gross quantities from future supply and demand because those are introduced along the time line (whether reserved or in other ways allocated).</span><span class="sxs-lookup"><span data-stu-id="afcc4-109">In the future, this becomes a moving projected inventory level that is maintained by gross quantities from future supply and demand because those are introduced along the time line (whether reserved or in other ways allocated).</span></span>  

<span data-ttu-id="afcc4-110">The projected inventory is used by the planning system to monitor the reorder point and to determine the reorder quantity when using the Maximum Qty. reordering policy.</span><span class="sxs-lookup"><span data-stu-id="afcc4-110">The projected inventory is used by the planning system to monitor the reorder point and to determine the reorder quantity when using the Maximum Qty. reordering policy.</span></span>  

## <a name="projected-available-inventory"></a><span data-ttu-id="afcc4-111">Projected Available Inventory</span><span class="sxs-lookup"><span data-stu-id="afcc4-111">Projected Available Inventory</span></span>  
<span data-ttu-id="afcc4-112">The projected available inventory is the part of the projected inventory that at a given point in time is available to fulfill demand.</span><span class="sxs-lookup"><span data-stu-id="afcc4-112">The projected available inventory is the part of the projected inventory that at a given point in time is available to fulfill demand.</span></span> <span data-ttu-id="afcc4-113">The projected available inventory is used by the planning engine when monitoring the safety stock level.</span><span class="sxs-lookup"><span data-stu-id="afcc4-113">The projected available inventory is used by the planning engine when monitoring the safety stock level.</span></span>  

<span data-ttu-id="afcc4-114">The projected available inventory is used by the planning system to monitor the safety stock level, since the safety stock must always be available to serve unexpected demand.</span><span class="sxs-lookup"><span data-stu-id="afcc4-114">The projected available inventory is used by the planning system to monitor the safety stock level, since the safety stock must always be available to serve unexpected demand.</span></span>  

## <a name="time-buckets"></a><span data-ttu-id="afcc4-115">Time Buckets</span><span class="sxs-lookup"><span data-stu-id="afcc4-115">Time Buckets</span></span>  
<span data-ttu-id="afcc4-116">Having a tight control of the projected inventory is crucial to detect when the reorder point is reached or crossed and to calculate the right order quantity when using the Maximum Qty. reordering policy.</span><span class="sxs-lookup"><span data-stu-id="afcc4-116">Having a tight control of the projected inventory is crucial to detect when the reorder point is reached or crossed and to calculate the right order quantity when using the Maximum Qty. reordering policy.</span></span>  

<span data-ttu-id="afcc4-117">As stated earlier, the projected inventory level is calculated at the start of the planning period.</span><span class="sxs-lookup"><span data-stu-id="afcc4-117">As stated earlier, the projected inventory level is calculated at the start of the planning period.</span></span> <span data-ttu-id="afcc4-118">It is a gross level that does not consider reservations and similar allocations.</span><span class="sxs-lookup"><span data-stu-id="afcc4-118">It is a gross level that does not consider reservations and similar allocations.</span></span> <span data-ttu-id="afcc4-119">To monitor this inventory level during the planning sequence, the system monitors the aggregated changes over a period of time, a time bucket.</span><span class="sxs-lookup"><span data-stu-id="afcc4-119">To monitor this inventory level during the planning sequence, the system monitors the aggregated changes over a period of time, a time bucket.</span></span> <span data-ttu-id="afcc4-120">The system ensures that the time bucket is at least one day since it is the most precise unit of time for a demand or supply event.</span><span class="sxs-lookup"><span data-stu-id="afcc4-120">The system ensures that the time bucket is at least one day since it is the most precise unit of time for a demand or supply event.</span></span>  

## <a name="determining-the-projected-inventory-level"></a><span data-ttu-id="afcc4-121">Determining the Projected Inventory Level</span><span class="sxs-lookup"><span data-stu-id="afcc4-121">Determining the Projected Inventory Level</span></span>  
<span data-ttu-id="afcc4-122">The following sequence describes how the projected inventory level is determined:</span><span class="sxs-lookup"><span data-stu-id="afcc4-122">The following sequence describes how the projected inventory level is determined:</span></span>  

* <span data-ttu-id="afcc4-123">When a supply event, such as a purchase order has been totally planned, it will increase the projected inventory on its due date.</span><span class="sxs-lookup"><span data-stu-id="afcc4-123">When a supply event, such as a purchase order has been totally planned, it will increase the projected inventory on its due date.</span></span>  
* <span data-ttu-id="afcc4-124">When a demand event has been fully satisfied, it will not decrease the projected inventory right away.</span><span class="sxs-lookup"><span data-stu-id="afcc4-124">When a demand event has been fully satisfied, it will not decrease the projected inventory right away.</span></span> <span data-ttu-id="afcc4-125">Instead, it posts a decrease reminder, which is an internal record that holds the date and quantity of the contribution to the projected inventory.</span><span class="sxs-lookup"><span data-stu-id="afcc4-125">Instead, it posts a decrease reminder, which is an internal record that holds the date and quantity of the contribution to the projected inventory.</span></span>  
* <span data-ttu-id="afcc4-126">When a subsequent supply event is planned and placed on the time line, the posted decrease reminders are investigated one by one up until the planned date of the supply while updating the projected inventory.</span><span class="sxs-lookup"><span data-stu-id="afcc4-126">When a subsequent supply event is planned and placed on the time line, the posted decrease reminders are investigated one by one up until the planned date of the supply while updating the projected inventory.</span></span> <span data-ttu-id="afcc4-127">During this process, the reorder point level of the internal increase reminder may be reached or crossed.</span><span class="sxs-lookup"><span data-stu-id="afcc4-127">During this process, the reorder point level of the internal increase reminder may be reached or crossed.</span></span>  
* <span data-ttu-id="afcc4-128">If a new supply order is introduced, the system checks if it is entered before the current supply.</span><span class="sxs-lookup"><span data-stu-id="afcc4-128">If a new supply order is introduced, the system checks if it is entered before the current supply.</span></span> <span data-ttu-id="afcc4-129">If it is, the new supply becomes current supply and the balancing procedure starts over.</span><span class="sxs-lookup"><span data-stu-id="afcc4-129">If it is, the new supply becomes current supply and the balancing procedure starts over.</span></span>  

<span data-ttu-id="afcc4-130">The following shows a graphical illustration of this principle:</span><span class="sxs-lookup"><span data-stu-id="afcc4-130">The following shows a graphical illustration of this principle:</span></span>  

<span data-ttu-id="afcc4-131">![Determining the Projected Inventory Level](media/nav_app_supply_planning_2_projected_inventory.png "Determining the Projected Inventory Level")</span><span class="sxs-lookup"><span data-stu-id="afcc4-131">![Determining the Projected Inventory Level](media/nav_app_supply_planning_2_projected_inventory.png "Determining the Projected Inventory Level")</span></span>  

1. <span data-ttu-id="afcc4-132">Supply **Sa** of 4 (fixed) closes Demand **Da** of -3.</span><span class="sxs-lookup"><span data-stu-id="afcc4-132">Supply **Sa** of 4 (fixed) closes Demand **Da** of -3.</span></span>  
2. <span data-ttu-id="afcc4-133">CloseDemand: Create a decrease reminder of -3 (not shown).</span><span class="sxs-lookup"><span data-stu-id="afcc4-133">CloseDemand: Create a decrease reminder of -3 (not shown).</span></span>  
3. <span data-ttu-id="afcc4-134">Supply **Sa** is closed with a surplus of 1 (no more demand exists).</span><span class="sxs-lookup"><span data-stu-id="afcc4-134">Supply **Sa** is closed with a surplus of 1 (no more demand exists).</span></span>  

     <span data-ttu-id="afcc4-135">This increases the projected inventory level to +4, while the projected **available** inventory becomes -1.</span><span class="sxs-lookup"><span data-stu-id="afcc4-135">This increases the projected inventory level to +4, while the projected **available** inventory becomes -1.</span></span>  

4. <span data-ttu-id="afcc4-136">The next supply **Sb** of 2 (another order) has already been placed on the timeline.</span><span class="sxs-lookup"><span data-stu-id="afcc4-136">The next supply **Sb** of 2 (another order) has already been placed on the timeline.</span></span>  
5. <span data-ttu-id="afcc4-137">System checks if there is any decrease reminder preceding **Sb** (there is not, so no action is taken).</span><span class="sxs-lookup"><span data-stu-id="afcc4-137">System checks if there is any decrease reminder preceding **Sb** (there is not, so no action is taken).</span></span>  
6. <span data-ttu-id="afcc4-138">System closes supply **Sb** (no more demand exists)—either A: by reducing it to 0 (cancel) or B: by leaving as is.</span><span class="sxs-lookup"><span data-stu-id="afcc4-138">System closes supply **Sb** (no more demand exists)—either A: by reducing it to 0 (cancel) or B: by leaving as is.</span></span>  

     <span data-ttu-id="afcc4-139">This increases the projected inventory level (A: +0 => +4 or B: +2 = +6).</span><span class="sxs-lookup"><span data-stu-id="afcc4-139">This increases the projected inventory level (A: +0 => +4 or B: +2 = +6).</span></span>  

7. <span data-ttu-id="afcc4-140">System makes a final check: Is there any decrease reminder?</span><span class="sxs-lookup"><span data-stu-id="afcc4-140">System makes a final check: Is there any decrease reminder?</span></span> <span data-ttu-id="afcc4-141">Yes, there is one on the date of **Da**.</span><span class="sxs-lookup"><span data-stu-id="afcc4-141">Yes, there is one on the date of **Da**.</span></span>  
8. <span data-ttu-id="afcc4-142">System adds the decrease reminder of -3 reminder to the projected inventory level, either A: +4 -3 = 1 or B: +6 -3 = +3.</span><span class="sxs-lookup"><span data-stu-id="afcc4-142">System adds the decrease reminder of -3 reminder to the projected inventory level, either A: +4 -3 = 1 or B: +6 -3 = +3.</span></span>  
9. <span data-ttu-id="afcc4-143">In case of A, the system creates a forward-scheduled order starting on date **Da**.</span><span class="sxs-lookup"><span data-stu-id="afcc4-143">In case of A, the system creates a forward-scheduled order starting on date **Da**.</span></span>  

     <span data-ttu-id="afcc4-144">In case of B, the reorder point is reached and a new order is created.</span><span class="sxs-lookup"><span data-stu-id="afcc4-144">In case of B, the reorder point is reached and a new order is created.</span></span>  

## <a name="see-also"></a><span data-ttu-id="afcc4-145">See Also</span><span class="sxs-lookup"><span data-stu-id="afcc4-145">See Also</span></span>  
<span data-ttu-id="afcc4-146">[Design Details: Reordering Policies](design-details-reordering-policies.md) </span><span class="sxs-lookup"><span data-stu-id="afcc4-146">[Design Details: Reordering Policies](design-details-reordering-policies.md) </span></span>  
<span data-ttu-id="afcc4-147">[Design Details: Planning Parameters](design-details-planning-parameters.md) </span><span class="sxs-lookup"><span data-stu-id="afcc4-147">[Design Details: Planning Parameters](design-details-planning-parameters.md) </span></span>  
<span data-ttu-id="afcc4-148">[Design Details: Handling Reordering Policies](design-details-handling-reordering-policies.md) </span><span class="sxs-lookup"><span data-stu-id="afcc4-148">[Design Details: Handling Reordering Policies](design-details-handling-reordering-policies.md) </span></span>  
[<span data-ttu-id="afcc4-149">Design Details: Supply Planning</span><span class="sxs-lookup"><span data-stu-id="afcc4-149">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)

