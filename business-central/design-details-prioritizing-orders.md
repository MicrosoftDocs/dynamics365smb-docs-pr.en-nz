---
title: Design Details - Prioritising Orders | Microsoft Docs
description: Read about how to prioritise to meet both demand and supply requirements.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: design, priority, prioritize, order, sku, demand, supply
ms.date: 10/01/2019
ms.author: sgroespe
redirect_url: design-details-balancing-demand-and-supply
ms.openlocfilehash: 0a14b00b1172d616642495e3963097ddef48c54c
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 10/01/2019
ms.locfileid: "2306932"
---
# <a name="design-details-prioritizing-orders"></a><span data-ttu-id="f7b69-103">Design Details: Prioritising Orders</span><span class="sxs-lookup"><span data-stu-id="f7b69-103">Design Details: Prioritizing Orders</span></span>
<span data-ttu-id="f7b69-104">Within a given SKU, the requested or available date represents the highest priority; the demand of today should be dealt with before the demand of next week.</span><span class="sxs-lookup"><span data-stu-id="f7b69-104">Within a given SKU, the requested or available date represents the highest priority; the demand of today should be dealt with before the demand of next week.</span></span> <span data-ttu-id="f7b69-105">But in addition to this overall priority, the planning system will also suggest which type of demand should be fulfilled before fulfilling another demand.</span><span class="sxs-lookup"><span data-stu-id="f7b69-105">But in addition to this overall priority, the planning system will also suggest which type of demand should be fulfilled before fulfilling another demand.</span></span> <span data-ttu-id="f7b69-106">Likewise, it will suggest what source of supply should be applied before applying other sources of supply.</span><span class="sxs-lookup"><span data-stu-id="f7b69-106">Likewise, it will suggest what source of supply should be applied before applying other sources of supply.</span></span> <span data-ttu-id="f7b69-107">This is done according to order priorities.</span><span class="sxs-lookup"><span data-stu-id="f7b69-107">This is done according to order priorities.</span></span>  

<span data-ttu-id="f7b69-108">Loaded demand and supply contribute to a profile for the projected inventory according to the following priorities:</span><span class="sxs-lookup"><span data-stu-id="f7b69-108">Loaded demand and supply contribute to a profile for the projected inventory according to the following priorities:</span></span>  

## <a name="priorities-on-the-demand-side"></a><span data-ttu-id="f7b69-109">Priorities on the Demand Side</span><span class="sxs-lookup"><span data-stu-id="f7b69-109">Priorities on the Demand Side</span></span>  
1. <span data-ttu-id="f7b69-110">Already shipped: Item Ledger Entry</span><span class="sxs-lookup"><span data-stu-id="f7b69-110">Already shipped: Item Ledger Entry</span></span>  
2. <span data-ttu-id="f7b69-111">Purchase Return Order</span><span class="sxs-lookup"><span data-stu-id="f7b69-111">Purchase Return Order</span></span>  
3. <span data-ttu-id="f7b69-112">Sales Order</span><span class="sxs-lookup"><span data-stu-id="f7b69-112">Sales Order</span></span>  
4. <span data-ttu-id="f7b69-113">Service Order</span><span class="sxs-lookup"><span data-stu-id="f7b69-113">Service Order</span></span>  
5. <span data-ttu-id="f7b69-114">Production Component Need</span><span class="sxs-lookup"><span data-stu-id="f7b69-114">Production Component Need</span></span>  
6. <span data-ttu-id="f7b69-115">Assembly Order Line</span><span class="sxs-lookup"><span data-stu-id="f7b69-115">Assembly Order Line</span></span>  
7. <span data-ttu-id="f7b69-116">Outbound Transfer Order</span><span class="sxs-lookup"><span data-stu-id="f7b69-116">Outbound Transfer Order</span></span>  
8. <span data-ttu-id="f7b69-117">Blanket Order (that has not already been consumed by related sales orders)</span><span class="sxs-lookup"><span data-stu-id="f7b69-117">Blanket Order (that has not already been consumed by related sales orders)</span></span>  
9. <span data-ttu-id="f7b69-118">Forecast (that has not already been consumed by other sales orders)</span><span class="sxs-lookup"><span data-stu-id="f7b69-118">Forecast (that has not already been consumed by other sales orders)</span></span>  

> [!NOTE]  
>  <span data-ttu-id="f7b69-119">Purchase returns are usually not involved in supply planning; they should always be reserved from the lot that is going to be returned.</span><span class="sxs-lookup"><span data-stu-id="f7b69-119">Purchase returns are usually not involved in supply planning; they should always be reserved from the lot that is going to be returned.</span></span> <span data-ttu-id="f7b69-120">If not reserved, purchase returns play a role in the availability and are highly prioritised to avoid that the planning system suggests a supply order just to serve a purchase return.</span><span class="sxs-lookup"><span data-stu-id="f7b69-120">If not reserved, purchase returns play a role in the availability and are highly prioritized to avoid that the planning system suggests a supply order just to serve a purchase return.</span></span>  

## <a name="priorities-on-the-supply-side"></a><span data-ttu-id="f7b69-121">Priorities on the Supply Side</span><span class="sxs-lookup"><span data-stu-id="f7b69-121">Priorities on the Supply Side</span></span>  
1. <span data-ttu-id="f7b69-122">Already in inventory: Item Ledger Entry (Planning Flexibility = None)</span><span class="sxs-lookup"><span data-stu-id="f7b69-122">Already in inventory: Item Ledger Entry (Planning Flexibility = None)</span></span>  
2. <span data-ttu-id="f7b69-123">Sales Return Order (Planning Flexibility = None)</span><span class="sxs-lookup"><span data-stu-id="f7b69-123">Sales Return Order (Planning Flexibility = None)</span></span>  
3. <span data-ttu-id="f7b69-124">Inbound Transfer Order</span><span class="sxs-lookup"><span data-stu-id="f7b69-124">Inbound Transfer Order</span></span>  
4. <span data-ttu-id="f7b69-125">Production Order</span><span class="sxs-lookup"><span data-stu-id="f7b69-125">Production Order</span></span>  
5. <span data-ttu-id="f7b69-126">Assembly Order</span><span class="sxs-lookup"><span data-stu-id="f7b69-126">Assembly Order</span></span>  
6. <span data-ttu-id="f7b69-127">Purchase Order</span><span class="sxs-lookup"><span data-stu-id="f7b69-127">Purchase Order</span></span>  

## <a name="priority-related-to-the-state-of-demand-and-supply"></a><span data-ttu-id="f7b69-128">Priority Related to the State of Demand and Supply</span><span class="sxs-lookup"><span data-stu-id="f7b69-128">Priority Related to the State of Demand and Supply</span></span>  
<span data-ttu-id="f7b69-129">Apart from priorities given by the type of demand and supply, the present state of the orders in the execution process also defines a priority.</span><span class="sxs-lookup"><span data-stu-id="f7b69-129">Apart from priorities given by the type of demand and supply, the present state of the orders in the execution process also defines a priority.</span></span> <span data-ttu-id="f7b69-130">For example, warehouse activities have an impact, and the status of sales, purchase, transfer, assembly, and production orders is taken into account:</span><span class="sxs-lookup"><span data-stu-id="f7b69-130">For example, warehouse activities have an impact, and the status of sales, purchase, transfer, assembly, and production orders is taken into account:</span></span>  

1. <span data-ttu-id="f7b69-131">Partly handled (Planning Flexibility = None)</span><span class="sxs-lookup"><span data-stu-id="f7b69-131">Partly handled (Planning Flexibility = None)</span></span>  
2. <span data-ttu-id="f7b69-132">Already in process in the warehouse (Planning Flexibility = None)</span><span class="sxs-lookup"><span data-stu-id="f7b69-132">Already in process in the warehouse (Planning Flexibility = None)</span></span>  
3. <span data-ttu-id="f7b69-133">Released – all order types (Planning Flexibility = Unlimited)</span><span class="sxs-lookup"><span data-stu-id="f7b69-133">Released – all order types (Planning Flexibility = Unlimited)</span></span>  
4. <span data-ttu-id="f7b69-134">Firm Planned Production Order (Planning Flexibility = Unlimited)</span><span class="sxs-lookup"><span data-stu-id="f7b69-134">Firm Planned Production Order (Planning Flexibility = Unlimited)</span></span>  
5. <span data-ttu-id="f7b69-135">Planned/Open – all order types (Planning Flexibility = Unlimited)</span><span class="sxs-lookup"><span data-stu-id="f7b69-135">Planned/Open – all order types (Planning Flexibility = Unlimited)</span></span>  

## <a name="see-also"></a><span data-ttu-id="f7b69-136">See Also</span><span class="sxs-lookup"><span data-stu-id="f7b69-136">See Also</span></span>  
<span data-ttu-id="f7b69-137">[Design Details: Balancing Demand and Supply](design-details-balancing-demand-and-supply.md) </span><span class="sxs-lookup"><span data-stu-id="f7b69-137">[Design Details: Balancing Demand and Supply](design-details-balancing-demand-and-supply.md) </span></span>  
<span data-ttu-id="f7b69-138">[Design Details: Central Concepts of the Planning System](design-details-central-concepts-of-the-planning-system.md) </span><span class="sxs-lookup"><span data-stu-id="f7b69-138">[Design Details: Central Concepts of the Planning System](design-details-central-concepts-of-the-planning-system.md) </span></span>  
[<span data-ttu-id="f7b69-139">Design Details: Supply Planning</span><span class="sxs-lookup"><span data-stu-id="f7b69-139">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)
