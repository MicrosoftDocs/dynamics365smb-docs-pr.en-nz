---
title: Design Details - Inventory Valuation | Microsoft Docs
description: Inventory valuation XE "Inventory Valuation"  is the determination of the cost that is assigned to an inventory item, as expressed by the following equation.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 8276d7362fb940c70573f14ac10b8f02d3e145e4
ms.contentlocale: en-nz
ms.lasthandoff: 09/22/2017

---
# <a name="design-details-inventory-valuation"></a><span data-ttu-id="ac849-103">Design Details: Inventory Valuation</span><span class="sxs-lookup"><span data-stu-id="ac849-103">Design Details: Inventory Valuation</span></span>
<span data-ttu-id="ac849-104">Inventory valuation XE "Inventory Valuation"  is the determination of the cost that is assigned to an inventory item, as expressed by the following equation.</span><span class="sxs-lookup"><span data-stu-id="ac849-104">Inventory valuation XE "Inventory Valuation"  is the determination of the cost that is assigned to an inventory item, as expressed by the following equation.</span></span>  

<span data-ttu-id="ac849-105">Ending inventory = beginning inventory + net purchases – cost of goods sold</span><span class="sxs-lookup"><span data-stu-id="ac849-105">Ending inventory = beginning inventory + net purchases – cost of goods sold</span></span>  

<span data-ttu-id="ac849-106">The calculation of inventory valuation uses the **Cost Amount (Actual)** field of the value entries for the item.</span><span class="sxs-lookup"><span data-stu-id="ac849-106">The calculation of inventory valuation uses the **Cost Amount (Actual)** field of the value entries for the item.</span></span> <span data-ttu-id="ac849-107">The entries are classified according to the entry type XE "Entry Type"  that corresponds to the cost components, direct cost, indirect cost, variance, revaluation, and rounding.</span><span class="sxs-lookup"><span data-stu-id="ac849-107">The entries are classified according to the entry type XE "Entry Type"  that corresponds to the cost components, direct cost, indirect cost, variance, revaluation, and rounding.</span></span> <span data-ttu-id="ac849-108">For more information, see [Design Details: Cost Components](design-details-cost-components.md).</span><span class="sxs-lookup"><span data-stu-id="ac849-108">For more information, see [Design Details: Cost Components](design-details-cost-components.md).</span></span>  

<span data-ttu-id="ac849-109">Entries are applied against each other, either by the fixed application XE "Application; Fixed" , or according to the general cost-flow assumption defined by the costing method XE "Method; Costing"  XE "Costing Method" .</span><span class="sxs-lookup"><span data-stu-id="ac849-109">Entries are applied against each other, either by the fixed application XE "Application; Fixed" , or according to the general cost-flow assumption defined by the costing method XE "Method; Costing"  XE "Costing Method" .</span></span> <span data-ttu-id="ac849-110">One entry of inventory decrease can be applied to more than one increase entry with different posting dates and possibly different acquisition cost XE "Acquisition Cost" s.</span><span class="sxs-lookup"><span data-stu-id="ac849-110">One entry of inventory decrease can be applied to more than one increase entry with different posting dates and possibly different acquisition cost XE "Acquisition Cost" s.</span></span> <span data-ttu-id="ac849-111">For more information, see [Design Details: Item Application](design-details-item-application.md).</span><span class="sxs-lookup"><span data-stu-id="ac849-111">For more information, see [Design Details: Item Application](design-details-item-application.md).</span></span> <span data-ttu-id="ac849-112">Therefore, calculation of the inventory value XE "Inventory Value"  for a given date is based on summing up positive and negative value entries.</span><span class="sxs-lookup"><span data-stu-id="ac849-112">Therefore, calculation of the inventory value XE "Inventory Value"  for a given date is based on summing up positive and negative value entries.</span></span>  

## <a name="inventory-valuation-report"></a><span data-ttu-id="ac849-113">Inventory Valuation report</span><span class="sxs-lookup"><span data-stu-id="ac849-113">Inventory Valuation report</span></span>  
<span data-ttu-id="ac849-114">To calculate the inventory value in the **Inventory Valuation** report, the report begins by calculating the value of the item’s inventory at a given starting date.</span><span class="sxs-lookup"><span data-stu-id="ac849-114">To calculate the inventory value in the **Inventory Valuation** report, the report begins by calculating the value of the item’s inventory at a given starting date.</span></span> <span data-ttu-id="ac849-115">It then adds the value of inventory increases and subtracts the value of inventory decreases up to a given ending date.</span><span class="sxs-lookup"><span data-stu-id="ac849-115">It then adds the value of inventory increases and subtracts the value of inventory decreases up to a given ending date.</span></span> <span data-ttu-id="ac849-116">The end result is the inventory value on the ending date.</span><span class="sxs-lookup"><span data-stu-id="ac849-116">The end result is the inventory value on the ending date.</span></span> <span data-ttu-id="ac849-117">The report calculates these values by summing the values in the **Cost Amount (Actual)** field in the value entries, using the posting dates as filters.</span><span class="sxs-lookup"><span data-stu-id="ac849-117">The report calculates these values by summing the values in the **Cost Amount (Actual)** field in the value entries, using the posting dates as filters.</span></span>  

<span data-ttu-id="ac849-118">The printed report always shows actual amounts, that is, the cost of entries that have been posted as invoiced.</span><span class="sxs-lookup"><span data-stu-id="ac849-118">The printed report always shows actual amounts, that is, the cost of entries that have been posted as invoiced.</span></span> <span data-ttu-id="ac849-119">The report will also print the expected cost of entries that have posted as received or shipped, if you select the Include Expected Cost field on the Options FastTab.</span><span class="sxs-lookup"><span data-stu-id="ac849-119">The report will also print the expected cost of entries that have posted as received or shipped, if you select the Include Expected Cost field on the Options FastTab.</span></span>  

> [!IMPORTANT]  
>  <span data-ttu-id="ac849-120">Values in the **Inventory Valuation** report is reconciled with the Inventory account in the general ledger, meaning the value entries in question have been posted to the general ledger.</span><span class="sxs-lookup"><span data-stu-id="ac849-120">Values in the **Inventory Valuation** report is reconciled with the Inventory account in the general ledger, meaning the value entries in question have been posted to the general ledger.</span></span>  

> [!IMPORTANT]  
>  <span data-ttu-id="ac849-121">Amounts in the **Value** columns of the report are based on the posting date of transactions for an item.</span><span class="sxs-lookup"><span data-stu-id="ac849-121">Amounts in the **Value** columns of the report are based on the posting date of transactions for an item.</span></span>  

## <a name="inventory-valuation---wip-report"></a><span data-ttu-id="ac849-122">Inventory Valuation - WIP report</span><span class="sxs-lookup"><span data-stu-id="ac849-122">Inventory Valuation - WIP report</span></span>  
<span data-ttu-id="ac849-123">A manufacturing company needs to determine the value of three types of inventory:</span><span class="sxs-lookup"><span data-stu-id="ac849-123">A manufacturing company needs to determine the value of three types of inventory:</span></span>  

* <span data-ttu-id="ac849-124">Raw Materials inventory</span><span class="sxs-lookup"><span data-stu-id="ac849-124">Raw Materials inventory</span></span>  
* <span data-ttu-id="ac849-125">WIP inventory</span><span class="sxs-lookup"><span data-stu-id="ac849-125">WIP inventory</span></span>  
* <span data-ttu-id="ac849-126">Finished Goods inventory</span><span class="sxs-lookup"><span data-stu-id="ac849-126">Finished Goods inventory</span></span>  

<span data-ttu-id="ac849-127">The value of WIP inventory is determined by the following equation:</span><span class="sxs-lookup"><span data-stu-id="ac849-127">The value of WIP inventory is determined by the following equation:</span></span>  

* <span data-ttu-id="ac849-128">Ending WIP inventory = Beginning WIP inventory + manufacturing costs – cost of goods manufactured</span><span class="sxs-lookup"><span data-stu-id="ac849-128">Ending WIP inventory = Beginning WIP inventory + manufacturing costs – cost of goods manufactured</span></span>  

<span data-ttu-id="ac849-129">As for purchased inventory, the value entries provide the basis of the inventory valuation.</span><span class="sxs-lookup"><span data-stu-id="ac849-129">As for purchased inventory, the value entries provide the basis of the inventory valuation.</span></span> <span data-ttu-id="ac849-130">The calculation is made using the values in the **Cost Amount (Actual)** field of the item and capacity value entries associated with a production order.</span><span class="sxs-lookup"><span data-stu-id="ac849-130">The calculation is made using the values in the **Cost Amount (Actual)** field of the item and capacity value entries associated with a production order.</span></span>  

<span data-ttu-id="ac849-131">The purpose of WIP inventory valuation is to determine the value of the items whose manufacturing has not yet been completed on a given date.</span><span class="sxs-lookup"><span data-stu-id="ac849-131">The purpose of WIP inventory valuation is to determine the value of the items whose manufacturing has not yet been completed on a given date.</span></span> <span data-ttu-id="ac849-132">Therefore the WIP inventory value is based on the value entries related to the consumption and capacity ledger entries.</span><span class="sxs-lookup"><span data-stu-id="ac849-132">Therefore the WIP inventory value is based on the value entries related to the consumption and capacity ledger entries.</span></span> <span data-ttu-id="ac849-133">Consumption ledger entries must be completely invoiced at the date of the valuation.</span><span class="sxs-lookup"><span data-stu-id="ac849-133">Consumption ledger entries must be completely invoiced at the date of the valuation.</span></span> <span data-ttu-id="ac849-134">Therefore, the **Inventory Valuation – WIP** report shows the costs representing the WIP inventory value in two categories: consumption and capacity.</span><span class="sxs-lookup"><span data-stu-id="ac849-134">Therefore, the **Inventory Valuation – WIP** report shows the costs representing the WIP inventory value in two categories: consumption and capacity.</span></span>  

## <a name="see-also"></a><span data-ttu-id="ac849-135">See Also</span><span class="sxs-lookup"><span data-stu-id="ac849-135">See Also</span></span>  
<span data-ttu-id="ac849-136">[Design Details: Reconciliation with the General Ledger](design-details-reconciliation-with-the-general-ledger.md) </span><span class="sxs-lookup"><span data-stu-id="ac849-136">[Design Details: Reconciliation with the General Ledger](design-details-reconciliation-with-the-general-ledger.md) </span></span>  
<span data-ttu-id="ac849-137">[Design Details: Revaluation](design-details-revaluation.md) </span><span class="sxs-lookup"><span data-stu-id="ac849-137">[Design Details: Revaluation](design-details-revaluation.md) </span></span>  
<span data-ttu-id="ac849-138">[Design Details: Production Order Posting](design-details-production-order-posting.md)
[Managing Inventory Costs](finance-manage-inventory-costs.md)</span><span class="sxs-lookup"><span data-stu-id="ac849-138">[Design Details: Production Order Posting](design-details-production-order-posting.md)
[Managing Inventory Costs](finance-manage-inventory-costs.md)</span></span>  
[<span data-ttu-id="ac849-139">Finance</span><span class="sxs-lookup"><span data-stu-id="ac849-139">Finance</span></span>](finance.md)  
<span data-ttu-id="ac849-140">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="ac849-140">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

