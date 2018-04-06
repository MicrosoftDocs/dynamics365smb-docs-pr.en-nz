---
title: Design Details - Variance | Microsoft Docs
description: Variance is defined as the difference between the actual cost and the standard cost, as described in the following formula.
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
ms.openlocfilehash: f01c57c3686764866c9d2a3c25d426e7f9a986a6
ms.contentlocale: en-nz
ms.lasthandoff: 03/22/2018

---
# <a name="design-details-variance"></a><span data-ttu-id="c2ea7-103">Design Details: Variance</span><span class="sxs-lookup"><span data-stu-id="c2ea7-103">Design Details: Variance</span></span>
<span data-ttu-id="c2ea7-104">Variance is defined as the difference between the actual cost and the standard cost, as described in the following formula.</span><span class="sxs-lookup"><span data-stu-id="c2ea7-104">Variance is defined as the difference between the actual cost and the standard cost, as described in the following formula.</span></span>  

 <span data-ttu-id="c2ea7-105">actual cost – standard cost = variance</span><span class="sxs-lookup"><span data-stu-id="c2ea7-105">actual cost – standard cost = variance</span></span>  

 <span data-ttu-id="c2ea7-106">If the actual cost changes, for example, because you post an item charge on a later date, then the variance is updated accordingly.</span><span class="sxs-lookup"><span data-stu-id="c2ea7-106">If the actual cost changes, for example, because you post an item charge on a later date, then the variance is updated accordingly.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="c2ea7-107">Revaluation does not affect the variance calculation, because revaluation only changes the inventory value.</span><span class="sxs-lookup"><span data-stu-id="c2ea7-107">Revaluation does not affect the variance calculation, because revaluation only changes the inventory value.</span></span>  

## <a name="example"></a><span data-ttu-id="c2ea7-108">Example</span><span class="sxs-lookup"><span data-stu-id="c2ea7-108">Example</span></span>  
 <span data-ttu-id="c2ea7-109">The following example illustrates how variance is calculated for purchased items.</span><span class="sxs-lookup"><span data-stu-id="c2ea7-109">The following example illustrates how variance is calculated for purchased items.</span></span> <span data-ttu-id="c2ea7-110">It is based on the following scenario:</span><span class="sxs-lookup"><span data-stu-id="c2ea7-110">It is based on the following scenario:</span></span>  

1.  <span data-ttu-id="c2ea7-111">The user purchases an item at LCY 90.00, but the standard cost is LCY 100.00.</span><span class="sxs-lookup"><span data-stu-id="c2ea7-111">The user purchases an item at LCY 90.00, but the standard cost is LCY 100.00.</span></span> <span data-ttu-id="c2ea7-112">Accordingly, the purchase variance is LCY –10.00.</span><span class="sxs-lookup"><span data-stu-id="c2ea7-112">Accordingly, the purchase variance is LCY –10.00.</span></span>  
2.  <span data-ttu-id="c2ea7-113">LCY 10.00 is credited to the purchase variance account.</span><span class="sxs-lookup"><span data-stu-id="c2ea7-113">LCY 10.00 is credited to the purchase variance account.</span></span>  
3.  <span data-ttu-id="c2ea7-114">The user posts an item charge of LCY 20.00.</span><span class="sxs-lookup"><span data-stu-id="c2ea7-114">The user posts an item charge of LCY 20.00.</span></span> <span data-ttu-id="c2ea7-115">Accordingly, the actual cost is increased to LCY 110.00, and the value of the purchase variance becomes LCY 10.00.</span><span class="sxs-lookup"><span data-stu-id="c2ea7-115">Accordingly, the actual cost is increased to LCY 110.00, and the value of the purchase variance becomes LCY 10.00.</span></span>  
4.  <span data-ttu-id="c2ea7-116">LCY 20.00 is debited to the purchase variance account.</span><span class="sxs-lookup"><span data-stu-id="c2ea7-116">LCY 20.00 is debited to the purchase variance account.</span></span> <span data-ttu-id="c2ea7-117">Accordingly, the net purchase variance becomes LCY 10.00.</span><span class="sxs-lookup"><span data-stu-id="c2ea7-117">Accordingly, the net purchase variance becomes LCY 10.00.</span></span>  
5.  <span data-ttu-id="c2ea7-118">The user revalues the item from LCY 100.00 to LCY 70.00.</span><span class="sxs-lookup"><span data-stu-id="c2ea7-118">The user revalues the item from LCY 100.00 to LCY 70.00.</span></span> <span data-ttu-id="c2ea7-119">This does not affect the variance calculation, only the inventory value.</span><span class="sxs-lookup"><span data-stu-id="c2ea7-119">This does not affect the variance calculation, only the inventory value.</span></span>  

 <span data-ttu-id="c2ea7-120">The following table shows the resulting value entries.</span><span class="sxs-lookup"><span data-stu-id="c2ea7-120">The following table shows the resulting value entries.</span></span>  

 <span data-ttu-id="c2ea7-121">![Purchase variance calculation](media/design_details_inventory_costing_11_purchase_variance.png "design_details_inventory_costing_11_purchase_variance")</span><span class="sxs-lookup"><span data-stu-id="c2ea7-121">![Purchase variance calculation](media/design_details_inventory_costing_11_purchase_variance.png "design_details_inventory_costing_11_purchase_variance")</span></span>  

## <a name="determining-the-standard-cost"></a><span data-ttu-id="c2ea7-122">Determining the Standard Cost</span><span class="sxs-lookup"><span data-stu-id="c2ea7-122">Determining the Standard Cost</span></span>  
 <span data-ttu-id="c2ea7-123">The standard cost is used when calculating variance and the amount to capitalise.</span><span class="sxs-lookup"><span data-stu-id="c2ea7-123">The standard cost is used when calculating variance and the amount to capitalize.</span></span> <span data-ttu-id="c2ea7-124">Since the standard cost can be changed over time because of manual update calculation, you need a point in time when the standard cost is fixed for variance calculation.</span><span class="sxs-lookup"><span data-stu-id="c2ea7-124">Since the standard cost can be changed over time because of manual update calculation, you need a point in time when the standard cost is fixed for variance calculation.</span></span> <span data-ttu-id="c2ea7-125">This point is when the inventory increase is invoiced.</span><span class="sxs-lookup"><span data-stu-id="c2ea7-125">This point is when the inventory increase is invoiced.</span></span> <span data-ttu-id="c2ea7-126">For produced or assembled items, the point when standard cost is determined is when the cost is adjusted.</span><span class="sxs-lookup"><span data-stu-id="c2ea7-126">For produced or assembled items, the point when standard cost is determined is when the cost is adjusted.</span></span>  

 <span data-ttu-id="c2ea7-127">The following table shows how different cost shares are calculated for produced and assembled items when you use the Calculate Standard Cost function.</span><span class="sxs-lookup"><span data-stu-id="c2ea7-127">The following table shows how different cost shares are calculated for produced and assembled items when you use the Calculate Standard Cost function.</span></span>  

|<span data-ttu-id="c2ea7-128">Cost Share</span><span class="sxs-lookup"><span data-stu-id="c2ea7-128">Cost Share</span></span>|<span data-ttu-id="c2ea7-129">Purchased Item</span><span class="sxs-lookup"><span data-stu-id="c2ea7-129">Purchased Item</span></span>|<span data-ttu-id="c2ea7-130">Produced/Assembled Item</span><span class="sxs-lookup"><span data-stu-id="c2ea7-130">Produced/Assembled Item</span></span>|  
|----------------|--------------------|------------------------------|  
|<span data-ttu-id="c2ea7-131">**Standard Cost**</span><span class="sxs-lookup"><span data-stu-id="c2ea7-131">**Standard Cost**</span></span>||<span data-ttu-id="c2ea7-132">Single-Level Material Cost + Single-Level Capacity Cost + Single-Level Subcontrd. Cost + Single-Level Cap. Ovhd. Cost + Single-Level Mfg. Ovhd. Cost</span><span class="sxs-lookup"><span data-stu-id="c2ea7-132">Single-Level Material Cost + Single-Level Capacity Cost + Single-Level Subcontrd. Cost + Single-Level Cap. Ovhd. Cost + Single-Level Mfg. Ovhd. Cost</span></span>|  
|<span data-ttu-id="c2ea7-133">**Single-Level Material Cost**</span><span class="sxs-lookup"><span data-stu-id="c2ea7-133">**Single-Level Material Cost**</span></span>|<span data-ttu-id="c2ea7-134">Unit Cost</span><span class="sxs-lookup"><span data-stu-id="c2ea7-134">Unit Cost</span></span>|<span data-ttu-id="c2ea7-135">![Equation 1](media/design_details_inventory_costing_11_equation_1.png "design_details_inventory_costing_11_equation_1")</span><span class="sxs-lookup"><span data-stu-id="c2ea7-135">![Equation 1](media/design_details_inventory_costing_11_equation_1.png "design_details_inventory_costing_11_equation_1")</span></span>|  
|<span data-ttu-id="c2ea7-136">**Single-Level Capacity Cost**</span><span class="sxs-lookup"><span data-stu-id="c2ea7-136">**Single-Level Capacity Cost**</span></span>|<span data-ttu-id="c2ea7-137">Not applicable</span><span class="sxs-lookup"><span data-stu-id="c2ea7-137">Not applicable</span></span>|<span data-ttu-id="c2ea7-138">![Equation 2](media/design_details_inventory_costing_11_equation_2.png "design_details_inventory_costing_11_equation_2")</span><span class="sxs-lookup"><span data-stu-id="c2ea7-138">![Equation 2](media/design_details_inventory_costing_11_equation_2.png "design_details_inventory_costing_11_equation_2")</span></span>|  
|<span data-ttu-id="c2ea7-139">**Single-Level Subcontrd. Cost**</span><span class="sxs-lookup"><span data-stu-id="c2ea7-139">**Single-Level Subcontrd. Cost**</span></span>|<span data-ttu-id="c2ea7-140">Not applicable</span><span class="sxs-lookup"><span data-stu-id="c2ea7-140">Not applicable</span></span>|<span data-ttu-id="c2ea7-141">![Equation 3](media/design_details_inventory_costing_11_equation_3.png "design_details_inventory_costing_11_equation_3")</span><span class="sxs-lookup"><span data-stu-id="c2ea7-141">![Equation 3](media/design_details_inventory_costing_11_equation_3.png "design_details_inventory_costing_11_equation_3")</span></span>|  
|<span data-ttu-id="c2ea7-142">**Single-Level Cap. Ovhd Cost**</span><span class="sxs-lookup"><span data-stu-id="c2ea7-142">**Single-Level Cap. Ovhd Cost**</span></span>|<span data-ttu-id="c2ea7-143">Not applicable</span><span class="sxs-lookup"><span data-stu-id="c2ea7-143">Not applicable</span></span>|<span data-ttu-id="c2ea7-144">![Equation 4](media/design_details_inventory_costing_11_equation_4.png "design_details_inventory_costing_11_equation_4")</span><span class="sxs-lookup"><span data-stu-id="c2ea7-144">![Equation 4](media/design_details_inventory_costing_11_equation_4.png "design_details_inventory_costing_11_equation_4")</span></span>|  
|<span data-ttu-id="c2ea7-145">**Single-Level Mfg. Ovhd Cost**</span><span class="sxs-lookup"><span data-stu-id="c2ea7-145">**Single-Level Mfg. Ovhd Cost**</span></span>|<span data-ttu-id="c2ea7-146">Not applicable</span><span class="sxs-lookup"><span data-stu-id="c2ea7-146">Not applicable</span></span>|<span data-ttu-id="c2ea7-147">(Single-Level Material Cost + Single-Level Capacity Cost + Single-Level Subcontrd. Cost) \* Indirect Cost % / 100 + Overhead Rate</span><span class="sxs-lookup"><span data-stu-id="c2ea7-147">(Single-Level Material Cost + Single-Level Capacity Cost + Single-Level Subcontrd. Cost) \* Indirect Cost % / 100 + Overhead Rate</span></span>|  
|<span data-ttu-id="c2ea7-148">**Rolled-up Material Cost**</span><span class="sxs-lookup"><span data-stu-id="c2ea7-148">**Rolled-up Material Cost**</span></span>|<span data-ttu-id="c2ea7-149">Unit Cost</span><span class="sxs-lookup"><span data-stu-id="c2ea7-149">Unit Cost</span></span>|<span data-ttu-id="c2ea7-150">![Equation 5](media/design_details_inventory_costing_11_equation_5.png "design_details_inventory_costing_11_equation_5")</span><span class="sxs-lookup"><span data-stu-id="c2ea7-150">![Equation 5](media/design_details_inventory_costing_11_equation_5.png "design_details_inventory_costing_11_equation_5")</span></span>|  
|<span data-ttu-id="c2ea7-151">**Rolled-up Capacity Cost**</span><span class="sxs-lookup"><span data-stu-id="c2ea7-151">**Rolled-up Capacity Cost**</span></span>|<span data-ttu-id="c2ea7-152">Not applicable</span><span class="sxs-lookup"><span data-stu-id="c2ea7-152">Not applicable</span></span>|<span data-ttu-id="c2ea7-153">![Equation 6](media/design_details_inventory_costing_11_equation_6.png "design_details_inventory_costing_11_equation_6")</span><span class="sxs-lookup"><span data-stu-id="c2ea7-153">![Equation 6](media/design_details_inventory_costing_11_equation_6.png "design_details_inventory_costing_11_equation_6")</span></span>|  
|<span data-ttu-id="c2ea7-154">**Rolled-Up Subcontracted Cost**</span><span class="sxs-lookup"><span data-stu-id="c2ea7-154">**Rolled-Up Subcontracted Cost**</span></span>|<span data-ttu-id="c2ea7-155">Not applicable</span><span class="sxs-lookup"><span data-stu-id="c2ea7-155">Not applicable</span></span>|<span data-ttu-id="c2ea7-156">![Equation 7](media/design_details_inventory_costing_11_equation_7.png "design_details_inventory_costing_11_equation_7")</span><span class="sxs-lookup"><span data-stu-id="c2ea7-156">![Equation 7](media/design_details_inventory_costing_11_equation_7.png "design_details_inventory_costing_11_equation_7")</span></span>|  
|<span data-ttu-id="c2ea7-157">**Rolled-up Capacity Ovhd. Cost**</span><span class="sxs-lookup"><span data-stu-id="c2ea7-157">**Rolled-up Capacity Ovhd. Cost**</span></span>|<span data-ttu-id="c2ea7-158">Not applicable</span><span class="sxs-lookup"><span data-stu-id="c2ea7-158">Not applicable</span></span>|<span data-ttu-id="c2ea7-159">![Equation 8](media/design_details_inventory_costing_11_equation_8.png "design_details_inventory_costing_11_equation_8")</span><span class="sxs-lookup"><span data-stu-id="c2ea7-159">![Equation 8](media/design_details_inventory_costing_11_equation_8.png "design_details_inventory_costing_11_equation_8")</span></span>|  
|<span data-ttu-id="c2ea7-160">**Rolled-up Mfg. Ovhd. Cost**</span><span class="sxs-lookup"><span data-stu-id="c2ea7-160">**Rolled-up Mfg. Ovhd. Cost**</span></span>|<span data-ttu-id="c2ea7-161">Not applicable</span><span class="sxs-lookup"><span data-stu-id="c2ea7-161">Not applicable</span></span>|<span data-ttu-id="c2ea7-162">![Equation 9](media/design_details_inventory_costing_11_equation_9.png "design_details_inventory_costing_11_equation_9")</span><span class="sxs-lookup"><span data-stu-id="c2ea7-162">![Equation 9](media/design_details_inventory_costing_11_equation_9.png "design_details_inventory_costing_11_equation_9")</span></span>|  

## <a name="see-also"></a><span data-ttu-id="c2ea7-163">See Also</span><span class="sxs-lookup"><span data-stu-id="c2ea7-163">See Also</span></span>  
 <span data-ttu-id="c2ea7-164">[Design Details: Inventory Costing](design-details-inventory-costing.md) </span><span class="sxs-lookup"><span data-stu-id="c2ea7-164">[Design Details: Inventory Costing](design-details-inventory-costing.md) </span></span>  
 <span data-ttu-id="c2ea7-165">[Design Details: Costing Methods](design-details-costing-methods.md) [Managing Inventory Costs](finance-manage-inventory-costs.md)</span><span class="sxs-lookup"><span data-stu-id="c2ea7-165">[Design Details: Costing Methods](design-details-costing-methods.md) [Managing Inventory Costs](finance-manage-inventory-costs.md)</span></span>  
 [<span data-ttu-id="c2ea7-166">Finance</span><span class="sxs-lookup"><span data-stu-id="c2ea7-166">Finance</span></span>](finance.md)  
 <span data-ttu-id="c2ea7-167">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="c2ea7-167">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
