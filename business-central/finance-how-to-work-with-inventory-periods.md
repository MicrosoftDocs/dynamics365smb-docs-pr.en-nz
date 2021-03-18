---
title: How to Work with Inventory Periods | Microsoft Docs
description: You can control the timeframe in which people can post post changes to inventory by defining inventory periods.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: inventory, periods
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 36a2419cba4ff67d1857c1e1ec971a607f4fd355
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "5389815"
---
# <a name="work-with-inventory-periods"></a><span data-ttu-id="cd118-103">Work with Inventory Periods</span><span class="sxs-lookup"><span data-stu-id="cd118-103">Work with Inventory Periods</span></span>
<span data-ttu-id="cd118-104">Inventory periods define a period of time in which you can post changes to inventory.</span><span class="sxs-lookup"><span data-stu-id="cd118-104">Inventory periods define a period of time in which you can post changes to inventory.</span></span> <span data-ttu-id="cd118-105">An inventory period is defined by the date on which it ends, or the ending date.</span><span class="sxs-lookup"><span data-stu-id="cd118-105">An inventory period is defined by the date on which it ends, or the ending date.</span></span> <span data-ttu-id="cd118-106">When you close an inventory period, you cannot post any changes to inventory, either expected or invoiced, before this ending date.</span><span class="sxs-lookup"><span data-stu-id="cd118-106">When you close an inventory period, you cannot post any changes to inventory, either expected or invoiced, before this ending date.</span></span> <span data-ttu-id="cd118-107">You cannot post any new values to inventory before the ending date.</span><span class="sxs-lookup"><span data-stu-id="cd118-107">You cannot post any new values to inventory before the ending date.</span></span> <span data-ttu-id="cd118-108">If you have open item entries in the closed period, meaning positive quantities that have not yet been applied to outbound transactions, you can still apply outbound quantities to these entries, even if the period is closed.</span><span class="sxs-lookup"><span data-stu-id="cd118-108">If you have open item entries in the closed period, meaning positive quantities that have not yet been applied to outbound transactions, you can still apply outbound quantities to these entries, even if the period is closed.</span></span>  

<span data-ttu-id="cd118-109">The following sections describe how to:</span><span class="sxs-lookup"><span data-stu-id="cd118-109">The following sections describe how to:</span></span>

* <span data-ttu-id="cd118-110">Create inventory periods.</span><span class="sxs-lookup"><span data-stu-id="cd118-110">Create inventory periods.</span></span>  
* <span data-ttu-id="cd118-111">Close inventory periods.</span><span class="sxs-lookup"><span data-stu-id="cd118-111">Close inventory periods.</span></span>  
* <span data-ttu-id="cd118-112">Reopen inventory periods.</span><span class="sxs-lookup"><span data-stu-id="cd118-112">Reopen inventory periods.</span></span>  

## <a name="to-create-an-inventory-period"></a><span data-ttu-id="cd118-113">To create an inventory period</span><span class="sxs-lookup"><span data-stu-id="cd118-113">To create an inventory period</span></span>  
1. <span data-ttu-id="cd118-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Inventory Periods**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="cd118-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Inventory Periods**, and then choose the related link.</span></span>  
2. <span data-ttu-id="cd118-115">Create a new line.</span><span class="sxs-lookup"><span data-stu-id="cd118-115">Create a new line.</span></span>  
3. <span data-ttu-id="cd118-116">In the **Ending Date** field, enter the last date in the inventory period that you want to define.</span><span class="sxs-lookup"><span data-stu-id="cd118-116">In the **Ending Date** field, enter the last date in the inventory period that you want to define.</span></span> <span data-ttu-id="cd118-117">When the period is closed, you will not be able to post inventory changes before this date.</span><span class="sxs-lookup"><span data-stu-id="cd118-117">When the period is closed, you will not be able to post inventory changes before this date.</span></span>  
4. <span data-ttu-id="cd118-118">Enter a descriptive name in the **Name** field.</span><span class="sxs-lookup"><span data-stu-id="cd118-118">Enter a descriptive name in the **Name** field.</span></span> <span data-ttu-id="cd118-119">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="cd118-119">Choose the **OK** button.</span></span>  

## <a name="closing-inventory-periods"></a><span data-ttu-id="cd118-120">Closing Inventory Periods</span><span class="sxs-lookup"><span data-stu-id="cd118-120">Closing Inventory Periods</span></span>  
<span data-ttu-id="cd118-121">The **Closed** field indicates whether or not the inventory period is closed to inventory value changes.</span><span class="sxs-lookup"><span data-stu-id="cd118-121">The **Closed** field indicates whether or not the inventory period is closed to inventory value changes.</span></span> <span data-ttu-id="cd118-122">You cannot edit this field.</span><span class="sxs-lookup"><span data-stu-id="cd118-122">You cannot edit this field.</span></span>  

<span data-ttu-id="cd118-123">You can close any inventory period, provided that the following is true:</span><span class="sxs-lookup"><span data-stu-id="cd118-123">You can close any inventory period, provided that the following is true:</span></span>  

* <span data-ttu-id="cd118-124">There are no open outbound item ledger entries, meaning negative inventory, in that period.</span><span class="sxs-lookup"><span data-stu-id="cd118-124">There are no open outbound item ledger entries, meaning negative inventory, in that period.</span></span>  
* <span data-ttu-id="cd118-125">The cost of all items has been adjusted using the **Adjust Cost – Item Entries** batch job.</span><span class="sxs-lookup"><span data-stu-id="cd118-125">The cost of all items has been adjusted using the **Adjust Cost – Item Entries** batch job.</span></span>  

<span data-ttu-id="cd118-126">This means that all outbound transaction quantities, such as those from sales orders, outbound transfers, sales invoices, purchase returns, or purchase credit memos, must be applied to existing quantity in inventory.</span><span class="sxs-lookup"><span data-stu-id="cd118-126">This means that all outbound transaction quantities, such as those from sales orders, outbound transfers, sales invoices, purchase returns, or purchase credit memos, must be applied to existing quantity in inventory.</span></span>  

### <a name="to-close-an-inventory-period"></a><span data-ttu-id="cd118-127">To close an inventory period</span><span class="sxs-lookup"><span data-stu-id="cd118-127">To close an inventory period</span></span>  
1. <span data-ttu-id="cd118-128">Before closing an inventory period, choose the **Adjust Cost – Item Entries** action to ensure that all cost adjustments are posted.</span><span class="sxs-lookup"><span data-stu-id="cd118-128">Before closing an inventory period, choose the **Adjust Cost – Item Entries** action to ensure that all cost adjustments are posted.</span></span>

     <span data-ttu-id="cd118-129">Run the **Close Inventory Period – Test** report to determine if there are any open outbound item entries within the inventory period or any items whose cost has not yet been adjusted.</span><span class="sxs-lookup"><span data-stu-id="cd118-129">Run the **Close Inventory Period – Test** report to determine if there are any open outbound item entries within the inventory period or any items whose cost has not yet been adjusted.</span></span>  
2. <span data-ttu-id="cd118-130">Choose the **Close Inventory Period – Test** action.</span><span class="sxs-lookup"><span data-stu-id="cd118-130">Choose the **Close Inventory Period – Test** action.</span></span>  

     <span data-ttu-id="cd118-131">Run the **Post Inventory Cost to G/L** batch job to ensure that all costs are posted to the general ledger.</span><span class="sxs-lookup"><span data-stu-id="cd118-131">Run the **Post Inventory Cost to G/L** batch job to ensure that all costs are posted to the general ledger.</span></span>  
3. <span data-ttu-id="cd118-132">Choose the **Post Inventory to G/L** action.</span><span class="sxs-lookup"><span data-stu-id="cd118-132">Choose the **Post Inventory to G/L** action.</span></span>  
4. <span data-ttu-id="cd118-133">On the **Inventory Periods** page, select the inventory period you want to close.</span><span class="sxs-lookup"><span data-stu-id="cd118-133">On the **Inventory Periods** page, select the inventory period you want to close.</span></span>  
5. <span data-ttu-id="cd118-134">Choose the **Close Period** action.</span><span class="sxs-lookup"><span data-stu-id="cd118-134">Choose the **Close Period** action.</span></span> <span data-ttu-id="cd118-135">After the inventory period has been closed, you cannot post inventory changes before the ending date.</span><span class="sxs-lookup"><span data-stu-id="cd118-135">After the inventory period has been closed, you cannot post inventory changes before the ending date.</span></span> <span data-ttu-id="cd118-136">The cost of all items must be adjusted with the **Adjust Cost – Item Entries** batch job before you close the inventory period.</span><span class="sxs-lookup"><span data-stu-id="cd118-136">The cost of all items must be adjusted with the **Adjust Cost – Item Entries** batch job before you close the inventory period.</span></span>  
6. <span data-ttu-id="cd118-137">Choose the **Yes** button to confirm that you want to close the period, or choose **No** to cancel the closing.</span><span class="sxs-lookup"><span data-stu-id="cd118-137">Choose the **Yes** button to confirm that you want to close the period, or choose **No** to cancel the closing.</span></span>  
7. <span data-ttu-id="cd118-138">The inventory period is closed and a confirmation message is displayed when it is finished.</span><span class="sxs-lookup"><span data-stu-id="cd118-138">The inventory period is closed and a confirmation message is displayed when it is finished.</span></span>  

## <a name="reopening-inventory-periods"></a><span data-ttu-id="cd118-139">Reopening Inventory Periods</span><span class="sxs-lookup"><span data-stu-id="cd118-139">Reopening Inventory Periods</span></span>  
<span data-ttu-id="cd118-140">After you have closed the inventory period, you cannot delete the inventory period.</span><span class="sxs-lookup"><span data-stu-id="cd118-140">After you have closed the inventory period, you cannot delete the inventory period.</span></span> <span data-ttu-id="cd118-141">You can, however, reopen it, if you would like to allow posting before the ending date of the inventory period.</span><span class="sxs-lookup"><span data-stu-id="cd118-141">You can, however, reopen it, if you would like to allow posting before the ending date of the inventory period.</span></span> <span data-ttu-id="cd118-142">Reopening a period also reopens all inventory periods with ending dates later than the period you reopen.</span><span class="sxs-lookup"><span data-stu-id="cd118-142">Reopening a period also reopens all inventory periods with ending dates later than the period you reopen.</span></span>  

### <a name="to-reopen-an-inventory-period"></a><span data-ttu-id="cd118-143">To reopen an inventory period</span><span class="sxs-lookup"><span data-stu-id="cd118-143">To reopen an inventory period</span></span>  
1. <span data-ttu-id="cd118-144">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Inventory Periods**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="cd118-144">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Inventory Periods**, and then choose the related link.</span></span>  
2. <span data-ttu-id="cd118-145">Select the inventory period you want to reopen.</span><span class="sxs-lookup"><span data-stu-id="cd118-145">Select the inventory period you want to reopen.</span></span>  
3. <span data-ttu-id="cd118-146">Choose the **Reopen Period** period action.</span><span class="sxs-lookup"><span data-stu-id="cd118-146">Choose the **Reopen Period** period action.</span></span> <span data-ttu-id="cd118-147">Confirm that you want to reopen the period.</span><span class="sxs-lookup"><span data-stu-id="cd118-147">Confirm that you want to reopen the period.</span></span>  
4. <span data-ttu-id="cd118-148">All inventory periods with ending dates later than the period you selected are reopened.</span><span class="sxs-lookup"><span data-stu-id="cd118-148">All inventory periods with ending dates later than the period you selected are reopened.</span></span>  

## <a name="see-also"></a><span data-ttu-id="cd118-149">See Also</span><span class="sxs-lookup"><span data-stu-id="cd118-149">See Also</span></span>  
[<span data-ttu-id="cd118-150">Design Details: Inventory Periods</span><span class="sxs-lookup"><span data-stu-id="cd118-150">Design Details: Inventory Periods</span></span>](design-details-inventory-periods.md)  
[<span data-ttu-id="cd118-151">Finance</span><span class="sxs-lookup"><span data-stu-id="cd118-151">Finance</span></span>](finance.md)  
[<span data-ttu-id="cd118-152">Inventory</span><span class="sxs-lookup"><span data-stu-id="cd118-152">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="cd118-153">Working with Financials</span><span class="sxs-lookup"><span data-stu-id="cd118-153">Working with Financials</span></span>](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]