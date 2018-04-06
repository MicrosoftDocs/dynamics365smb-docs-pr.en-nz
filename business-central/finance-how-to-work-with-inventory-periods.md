---
title: How to Work with Inventory Periods | Microsoft Docs
description: You can control the timeframe in which people can post post changes to inventory by defining inventory periods.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: inventory, periods
ms.date: 08/07/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: d302483ca2d66870670aaa0914533472a807d04f
ms.contentlocale: en-nz
ms.lasthandoff: 03/22/2018

---
# <a name="work-with-inventory-periods"></a><span data-ttu-id="8dca3-103">Work with Inventory Periods</span><span class="sxs-lookup"><span data-stu-id="8dca3-103">Work with Inventory Periods</span></span>
<span data-ttu-id="8dca3-104">Inventory periods define a period of time in which you can post changes to inventory.</span><span class="sxs-lookup"><span data-stu-id="8dca3-104">Inventory periods define a period of time in which you can post changes to inventory.</span></span> <span data-ttu-id="8dca3-105">An inventory period is defined by the date on which it ends, or the ending date.</span><span class="sxs-lookup"><span data-stu-id="8dca3-105">An inventory period is defined by the date on which it ends, or the ending date.</span></span> <span data-ttu-id="8dca3-106">When you close an inventory period, you cannot post any changes to inventory, either expected or invoiced, before this ending date.</span><span class="sxs-lookup"><span data-stu-id="8dca3-106">When you close an inventory period, you cannot post any changes to inventory, either expected or invoiced, before this ending date.</span></span> <span data-ttu-id="8dca3-107">You cannot post any new values to inventory before the ending date.</span><span class="sxs-lookup"><span data-stu-id="8dca3-107">You cannot post any new values to inventory before the ending date.</span></span> <span data-ttu-id="8dca3-108">If you have open item entries in the closed period, meaning positive quantities that have not yet been applied to outbound transactions, you can still apply outbound quantities to these entries, even if the period is closed.</span><span class="sxs-lookup"><span data-stu-id="8dca3-108">If you have open item entries in the closed period, meaning positive quantities that have not yet been applied to outbound transactions, you can still apply outbound quantities to these entries, even if the period is closed.</span></span>  

<span data-ttu-id="8dca3-109">The following sections describe how to:</span><span class="sxs-lookup"><span data-stu-id="8dca3-109">The following sections describe how to:</span></span>  

* <span data-ttu-id="8dca3-110">Create inventory periods.</span><span class="sxs-lookup"><span data-stu-id="8dca3-110">Create inventory periods.</span></span>  
* <span data-ttu-id="8dca3-111">Close inventory periods.</span><span class="sxs-lookup"><span data-stu-id="8dca3-111">Close inventory periods.</span></span>  
* <span data-ttu-id="8dca3-112">Reopen inventory periods.</span><span class="sxs-lookup"><span data-stu-id="8dca3-112">Reopen inventory periods.</span></span>  

## <a name="to-create-an-inventory-period"></a><span data-ttu-id="8dca3-113">To create an inventory period</span><span class="sxs-lookup"><span data-stu-id="8dca3-113">To create an inventory period</span></span>  
1. <span data-ttu-id="8dca3-114">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Inventory Periods**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="8dca3-114">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Inventory Periods**, and then choose the related link.</span></span>  
2. <span data-ttu-id="8dca3-115">Create a new line.</span><span class="sxs-lookup"><span data-stu-id="8dca3-115">Create a new line.</span></span>  
3. <span data-ttu-id="8dca3-116">In the **Ending Date** field, enter the last date in the inventory period that you want to define.</span><span class="sxs-lookup"><span data-stu-id="8dca3-116">In the **Ending Date** field, enter the last date in the inventory period that you want to define.</span></span> <span data-ttu-id="8dca3-117">When the period is closed, you will not be able to post inventory changes before this date.</span><span class="sxs-lookup"><span data-stu-id="8dca3-117">When the period is closed, you will not be able to post inventory changes before this date.</span></span>  
4. <span data-ttu-id="8dca3-118">Enter a descriptive name in the **Name** field.</span><span class="sxs-lookup"><span data-stu-id="8dca3-118">Enter a descriptive name in the **Name** field.</span></span> <span data-ttu-id="8dca3-119">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="8dca3-119">Choose the **OK** button.</span></span>  

## <a name="closing-inventory-periods"></a><span data-ttu-id="8dca3-120">Closing Inventory Periods</span><span class="sxs-lookup"><span data-stu-id="8dca3-120">Closing Inventory Periods</span></span>  
<span data-ttu-id="8dca3-121">The **Closed** field indicates whether or not the inventory period is closed to inventory value changes.</span><span class="sxs-lookup"><span data-stu-id="8dca3-121">The **Closed** field indicates whether or not the inventory period is closed to inventory value changes.</span></span> <span data-ttu-id="8dca3-122">You cannot edit this field.</span><span class="sxs-lookup"><span data-stu-id="8dca3-122">You cannot edit this field.</span></span>  

<span data-ttu-id="8dca3-123">You can close any inventory period, provided that the following is true:</span><span class="sxs-lookup"><span data-stu-id="8dca3-123">You can close any inventory period, provided that the following is true:</span></span>  

* <span data-ttu-id="8dca3-124">There are no open outbound item ledger entries, meaning negative inventory, in that period.</span><span class="sxs-lookup"><span data-stu-id="8dca3-124">There are no open outbound item ledger entries, meaning negative inventory, in that period.</span></span>  
* <span data-ttu-id="8dca3-125">The cost of all items has been adjusted using the **Adjust Cost – Item Entries** batch job.</span><span class="sxs-lookup"><span data-stu-id="8dca3-125">The cost of all items has been adjusted using the **Adjust Cost – Item Entries** batch job.</span></span>  

<span data-ttu-id="8dca3-126">This means that all outbound transaction quantities, such as those from sales orders, outbound transfers, sales invoices, purchase returns, or purchase credit memos, must be applied to existing quantity in inventory.</span><span class="sxs-lookup"><span data-stu-id="8dca3-126">This means that all outbound transaction quantities, such as those from sales orders, outbound transfers, sales invoices, purchase returns, or purchase credit memos, must be applied to existing quantity in inventory.</span></span>  

### <a name="to-close-an-inventory-period"></a><span data-ttu-id="8dca3-127">To close an inventory period</span><span class="sxs-lookup"><span data-stu-id="8dca3-127">To close an inventory period</span></span>  
1. <span data-ttu-id="8dca3-128">Before closing an inventory period, run the **Adjust Cost – Item Entries** batch job to ensure that all cost adjustments are posted.</span><span class="sxs-lookup"><span data-stu-id="8dca3-128">Before closing an inventory period, run the **Adjust Cost – Item Entries** batch job to ensure that all cost adjustments are posted.</span></span> <span data-ttu-id="8dca3-129">On the **Actions** tab, in the **Functions** group, choose **Adjust Cost – Item Entries**.</span><span class="sxs-lookup"><span data-stu-id="8dca3-129">On the **Actions** tab, in the **Functions** group, choose **Adjust Cost – Item Entries**.</span></span>  

     <span data-ttu-id="8dca3-130">Run the **Close Inventory Period – Test** report to determine if there are any open outbound item entries within the inventory period or any items whose cost has not yet been adjusted.</span><span class="sxs-lookup"><span data-stu-id="8dca3-130">Run the **Close Inventory Period – Test** report to determine if there are any open outbound item entries within the inventory period or any items whose cost has not yet been adjusted.</span></span>  
2. <span data-ttu-id="8dca3-131">Choose the **Close Inventory Period – Test** action.</span><span class="sxs-lookup"><span data-stu-id="8dca3-131">Choose the **Close Inventory Period – Test** action.</span></span>  

     <span data-ttu-id="8dca3-132">Run the **Post Inventory Cost to G/L** batch job to ensure that all costs are posted to the general ledger.</span><span class="sxs-lookup"><span data-stu-id="8dca3-132">Run the **Post Inventory Cost to G/L** batch job to ensure that all costs are posted to the general ledger.</span></span>  
3. <span data-ttu-id="8dca3-133">Choose the **Post Inventory to G/L** action.</span><span class="sxs-lookup"><span data-stu-id="8dca3-133">Choose the **Post Inventory to G/L** action.</span></span>  
4. <span data-ttu-id="8dca3-134">In the **Inventory Periods** window, select the inventory period you want to close.</span><span class="sxs-lookup"><span data-stu-id="8dca3-134">In the **Inventory Periods** window, select the inventory period you want to close.</span></span>  
5. <span data-ttu-id="8dca3-135">Choose the **Close Period** action.</span><span class="sxs-lookup"><span data-stu-id="8dca3-135">Choose the **Close Period** action.</span></span> <span data-ttu-id="8dca3-136">After the inventory period has been closed, you cannot post inventory changes before the ending date.</span><span class="sxs-lookup"><span data-stu-id="8dca3-136">After the inventory period has been closed, you cannot post inventory changes before the ending date.</span></span> <span data-ttu-id="8dca3-137">The cost of all items must be adjusted with the **Adjust Cost – Item Entries** batch job before you close the inventory period.</span><span class="sxs-lookup"><span data-stu-id="8dca3-137">The cost of all items must be adjusted with the **Adjust Cost – Item Entries** batch job before you close the inventory period.</span></span>  
6. <span data-ttu-id="8dca3-138">Choose the **Yes** button to confirm that you want to close the period, or choose **No** to cancel the closing.</span><span class="sxs-lookup"><span data-stu-id="8dca3-138">Choose the **Yes** button to confirm that you want to close the period, or choose **No** to cancel the closing.</span></span>  
7. <span data-ttu-id="8dca3-139">The inventory period is closed and a confirmation message is displayed when it is finished.</span><span class="sxs-lookup"><span data-stu-id="8dca3-139">The inventory period is closed and a confirmation message is displayed when it is finished.</span></span>  

## <a name="reopening-inventory-periods"></a><span data-ttu-id="8dca3-140">Reopening Inventory Periods</span><span class="sxs-lookup"><span data-stu-id="8dca3-140">Reopening Inventory Periods</span></span>  
<span data-ttu-id="8dca3-141">After you have closed the inventory period, you cannot delete the inventory period.</span><span class="sxs-lookup"><span data-stu-id="8dca3-141">After you have closed the inventory period, you cannot delete the inventory period.</span></span> <span data-ttu-id="8dca3-142">You can, however, reopen it, if you would like to allow posting before the ending date of the inventory period.</span><span class="sxs-lookup"><span data-stu-id="8dca3-142">You can, however, reopen it, if you would like to allow posting before the ending date of the inventory period.</span></span> <span data-ttu-id="8dca3-143">Reopening a period also reopens all inventory periods with ending dates later than the period you reopen.</span><span class="sxs-lookup"><span data-stu-id="8dca3-143">Reopening a period also reopens all inventory periods with ending dates later than the period you reopen.</span></span>  

### <a name="to-reopen-an-inventory-period"></a><span data-ttu-id="8dca3-144">To reopen an inventory period</span><span class="sxs-lookup"><span data-stu-id="8dca3-144">To reopen an inventory period</span></span>  
1. <span data-ttu-id="8dca3-145">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Inventory Periods**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="8dca3-145">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Inventory Periods**, and then choose the related link.</span></span>  
2. <span data-ttu-id="8dca3-146">Select the inventory period you want to reopen.</span><span class="sxs-lookup"><span data-stu-id="8dca3-146">Select the inventory period you want to reopen.</span></span>  
3. <span data-ttu-id="8dca3-147">Choose the **Reopen Period** period action.</span><span class="sxs-lookup"><span data-stu-id="8dca3-147">Choose the **Reopen Period** period action.</span></span> <span data-ttu-id="8dca3-148">Confirm that you want to reopen the period.</span><span class="sxs-lookup"><span data-stu-id="8dca3-148">Confirm that you want to reopen the period.</span></span>  
4. <span data-ttu-id="8dca3-149">All inventory periods with ending dates later than the period you selected are reopened.</span><span class="sxs-lookup"><span data-stu-id="8dca3-149">All inventory periods with ending dates later than the period you selected are reopened.</span></span>  

## <a name="see-also"></a><span data-ttu-id="8dca3-150">See Also</span><span class="sxs-lookup"><span data-stu-id="8dca3-150">See Also</span></span>  
[<span data-ttu-id="8dca3-151">Design Details: Inventory Periods</span><span class="sxs-lookup"><span data-stu-id="8dca3-151">Design Details: Inventory Periods</span></span>](design-details-inventory-periods.md)  
[<span data-ttu-id="8dca3-152">Finance</span><span class="sxs-lookup"><span data-stu-id="8dca3-152">Finance</span></span>](finance.md)  
[<span data-ttu-id="8dca3-153">Inventory</span><span class="sxs-lookup"><span data-stu-id="8dca3-153">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="8dca3-154">Working with Financials</span><span class="sxs-lookup"><span data-stu-id="8dca3-154">Working with Financials</span></span>](ui-work-product.md)
