---
title: Trace Item-Tracked Items
description: You can see where an item-tracked item was used, including how and when it was received or produced, transferred, sold, consumed, or returned. You can also find all current instances of a specific serial or lot number in the database. You do this by using the Item Tracing and the Find Entries features.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: bbfe0237beb58f22d3be7bc388d7b2726f05d4ba
ms.sourcegitcommit: 0953171d39e1232a7c126142d68cac858234a20e
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 06/09/2021
ms.locfileid: "6214769"
---
# <a name="trace-item-tracked-items"></a><span data-ttu-id="81885-105">Trace Item-Tracked Items</span><span class="sxs-lookup"><span data-stu-id="81885-105">Trace Item-Tracked Items</span></span>
<span data-ttu-id="81885-106">You can see where an item-tracked item was used, including how and when it was received or produced, transferred, sold, consumed, or returned.</span><span class="sxs-lookup"><span data-stu-id="81885-106">You can see where an item-tracked item was used, including how and when it was received or produced, transferred, sold, consumed, or returned.</span></span> <span data-ttu-id="81885-107">You can also find all current instances of a specific serial or lot number in the database.</span><span class="sxs-lookup"><span data-stu-id="81885-107">You can also find all current instances of a specific serial or lot number in the database.</span></span> <span data-ttu-id="81885-108">You do this by using the Item Tracing and the [Find Entries](ui-find-entries.md) features.</span><span class="sxs-lookup"><span data-stu-id="81885-108">You do this by using the Item Tracing and the [Find Entries](ui-find-entries.md) features.</span></span>  

<span data-ttu-id="81885-109">These features can be particularly useful in quality control when you need to find out which customers received products with a particular lot number or when you need to find out which lot a defective component came from.</span><span class="sxs-lookup"><span data-stu-id="81885-109">These features can be particularly useful in quality control when you need to find out which customers received products with a particular lot number or when you need to find out which lot a defective component came from.</span></span>  

 <span data-ttu-id="81885-110">On the **Item Tracing** page, you can trace forwards and backwards in a sequence of posted inventory transactions for the serial or lot number.</span><span class="sxs-lookup"><span data-stu-id="81885-110">On the **Item Tracing** page, you can trace forwards and backwards in a sequence of posted inventory transactions for the serial or lot number.</span></span>  

 <span data-ttu-id="81885-111">On the **Find Entries** page, you cannot see the sequence of transactions, but you can see all records of the serial or lot number, both posted entries and open records.</span><span class="sxs-lookup"><span data-stu-id="81885-111">On the **Find Entries** page, you cannot see the sequence of transactions, but you can see all records of the serial or lot number, both posted entries and open records.</span></span>  

 <span data-ttu-id="81885-112">The two features can be used in combination by transferring a traced serial or lot number to the **Find Entries** page to finish a complete trace scenario.</span><span class="sxs-lookup"><span data-stu-id="81885-112">The two features can be used in combination by transferring a traced serial or lot number to the **Find Entries** page to finish a complete trace scenario.</span></span> <!-- For more information, see [Walkthrough: Tracing Serial-Lot Numbers](walkthrough-tracing-serial-lot-numbers.md).   -->

## <a name="to-trace-item-tracked-items"></a><span data-ttu-id="81885-113">To trace item-tracked items</span><span class="sxs-lookup"><span data-stu-id="81885-113">To trace item-tracked items</span></span>  

1.  <span data-ttu-id="81885-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Item Tracing**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="81885-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Item Tracing**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="81885-115">In the filter fields at the top of the page, enter the specific item numbers or a filter on the item numbers that you would like to trace.</span><span class="sxs-lookup"><span data-stu-id="81885-115">In the filter fields at the top of the page, enter the specific item numbers or a filter on the item numbers that you would like to trace.</span></span>  
3.  <span data-ttu-id="81885-116">In the **Show Components** field, select whether you would like to also see where the components for the items came from.</span><span class="sxs-lookup"><span data-stu-id="81885-116">In the **Show Components** field, select whether you would like to also see where the components for the items came from.</span></span> <span data-ttu-id="81885-117">Your options in this field are as follows.</span><span class="sxs-lookup"><span data-stu-id="81885-117">Your options in this field are as follows.</span></span>  

    |<span data-ttu-id="81885-118">Field</span><span class="sxs-lookup"><span data-stu-id="81885-118">Field</span></span>|<span data-ttu-id="81885-119">Description</span><span class="sxs-lookup"><span data-stu-id="81885-119">Description</span></span>|  
    |----------------------------------|---------------------------------------|  
    |<span data-ttu-id="81885-120">**No**</span><span class="sxs-lookup"><span data-stu-id="81885-120">**No**</span></span>|<span data-ttu-id="81885-121">Select this option if you do not want to see any components.</span><span class="sxs-lookup"><span data-stu-id="81885-121">Select this option if you do not want to see any components.</span></span>|  
    |<span data-ttu-id="81885-122">**Item-tracked Only**</span><span class="sxs-lookup"><span data-stu-id="81885-122">**Item-tracked Only**</span></span>|<span data-ttu-id="81885-123">Select this option if you want to see only components that have lot or serial numbers.</span><span class="sxs-lookup"><span data-stu-id="81885-123">Select this option if you want to see only components that have lot or serial numbers.</span></span>|  
    |<span data-ttu-id="81885-124">**All**</span><span class="sxs-lookup"><span data-stu-id="81885-124">**All**</span></span>|<span data-ttu-id="81885-125">Select this option if you want to see all components.</span><span class="sxs-lookup"><span data-stu-id="81885-125">Select this option if you want to see all components.</span></span>|  

4.  <span data-ttu-id="81885-126">In the **Trace Method** field, select the method you would like to use for tracing the item.</span><span class="sxs-lookup"><span data-stu-id="81885-126">In the **Trace Method** field, select the method you would like to use for tracing the item.</span></span> <span data-ttu-id="81885-127">The options are as follows</span><span class="sxs-lookup"><span data-stu-id="81885-127">The options are as follows</span></span>  

    |<span data-ttu-id="81885-128">Field</span><span class="sxs-lookup"><span data-stu-id="81885-128">Field</span></span>|<span data-ttu-id="81885-129">Description</span><span class="sxs-lookup"><span data-stu-id="81885-129">Description</span></span>|  
    |----------------------------------|---------------------------------------|  
    |<span data-ttu-id="81885-130">**Usage->Origin**</span><span class="sxs-lookup"><span data-stu-id="81885-130">**Usage->Origin**</span></span>|<span data-ttu-id="81885-131">This method traces the item starting from where it was used to where it came from.</span><span class="sxs-lookup"><span data-stu-id="81885-131">This method traces the item starting from where it was used to where it came from.</span></span> <span data-ttu-id="81885-132">For instance, if a manufactured item was sold to a customer, the **Item Tracing** page shows this with the sales shipment line first, which you can then expand to see from which production order it came.</span><span class="sxs-lookup"><span data-stu-id="81885-132">For instance, if a manufactured item was sold to a customer, the **Item Tracing** page shows this with the sales shipment line first, which you can then expand to see from which production order it came.</span></span>|  
    |<span data-ttu-id="81885-133">**Origin->Usage**</span><span class="sxs-lookup"><span data-stu-id="81885-133">**Origin->Usage**</span></span>|<span data-ttu-id="81885-134">This method traces the item starting from where it came into inventory to where it was used.</span><span class="sxs-lookup"><span data-stu-id="81885-134">This method traces the item starting from where it came into inventory to where it was used.</span></span> <span data-ttu-id="81885-135">For instance, if a manufactured item was sold to a customer, the **Item Tracing** page shows this with the finished production order first, which you can then expand to see sale shipment lines where the item was used.</span><span class="sxs-lookup"><span data-stu-id="81885-135">For instance, if a manufactured item was sold to a customer, the **Item Tracing** page shows this with the finished production order first, which you can then expand to see sale shipment lines where the item was used.</span></span>|  

5.  <span data-ttu-id="81885-136">Choose the **Trace** action to run the trace.</span><span class="sxs-lookup"><span data-stu-id="81885-136">Choose the **Trace** action to run the trace.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="81885-137">If you have received the same lot on more transactions, then the **Item Tracing** page may not show all transactions.</span><span class="sxs-lookup"><span data-stu-id="81885-137">If you have received the same lot on more transactions, then the **Item Tracing** page may not show all transactions.</span></span> <span data-ttu-id="81885-138">Only applied transactions are shown.</span><span class="sxs-lookup"><span data-stu-id="81885-138">Only applied transactions are shown.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="81885-139">If additional transaction history under an item tracing line has already been traced by another line above it, then the **Already Traced** check box is selected.</span><span class="sxs-lookup"><span data-stu-id="81885-139">If additional transaction history under an item tracing line has already been traced by another line above it, then the **Already Traced** check box is selected.</span></span> <span data-ttu-id="81885-140">To provide a simpler view, such underlying lines are not shown.</span><span class="sxs-lookup"><span data-stu-id="81885-140">To provide a simpler view, such underlying lines are not shown.</span></span>  
>   
>  <span data-ttu-id="81885-141">To find the item tracing lines where the transaction history has already been traced, choose the **Go to Already Traced** button.</span><span class="sxs-lookup"><span data-stu-id="81885-141">To find the item tracing lines where the transaction history has already been traced, choose the **Go to Already Traced** button.</span></span> <span data-ttu-id="81885-142">The item tracing line in question is selected, and all underlying lines are expanded.</span><span class="sxs-lookup"><span data-stu-id="81885-142">The item tracing line in question is selected, and all underlying lines are expanded.</span></span>  

## <a name="to-find-item-tracked-items-with-find-entries"></a><span data-ttu-id="81885-143">To find item-tracked items with Find Entries</span><span class="sxs-lookup"><span data-stu-id="81885-143">To find item-tracked items with Find Entries</span></span>  

1. <span data-ttu-id="81885-144">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Find Entries**, and then select the related link.</span><span class="sxs-lookup"><span data-stu-id="81885-144">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Find Entries**, and then select the related link.</span></span>  
2. <span data-ttu-id="81885-145">Choose **Actions** > **Find by** > **Find by Item Reference**.</span><span class="sxs-lookup"><span data-stu-id="81885-145">Choose **Actions** > **Find by** > **Find by Item Reference**.</span></span>
3. <span data-ttu-id="81885-146">In the **Serial No.** and **Lot No.** fields, enter the item tracking numbers that you want to trace.</span><span class="sxs-lookup"><span data-stu-id="81885-146">In the **Serial No.** and **Lot No.** fields, enter the item tracking numbers that you want to trace.</span></span>  
4. <span data-ttu-id="81885-147">Choose the **Find** action to find all instances of the serial or lot number in the database.</span><span class="sxs-lookup"><span data-stu-id="81885-147">Choose the **Find** action to find all instances of the serial or lot number in the database.</span></span>  

## <a name="see-also"></a><span data-ttu-id="81885-148">See Also</span><span class="sxs-lookup"><span data-stu-id="81885-148">See Also</span></span>

[<span data-ttu-id="81885-149">Inventory</span><span class="sxs-lookup"><span data-stu-id="81885-149">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="81885-150">Work with Serial, Lot, and Package Numbers</span><span class="sxs-lookup"><span data-stu-id="81885-150">Work with Serial, Lot, and Package Numbers</span></span>](inventory-how-work-item-tracking.md)  
[<span data-ttu-id="81885-151">Design Details: Item Tracking</span><span class="sxs-lookup"><span data-stu-id="81885-151">Design Details: Item Tracking</span></span>](design-details-item-tracking.md)  
[<span data-ttu-id="81885-152">Design Details - Item Tracking and Reservations</span><span class="sxs-lookup"><span data-stu-id="81885-152">Design Details - Item Tracking and Reservations</span></span>](design-details-item-tracking-and-reservations.md)  
[<span data-ttu-id="81885-153">Reserve Items</span><span class="sxs-lookup"><span data-stu-id="81885-153">Reserve Items</span></span>](inventory-how-to-reserve-items.md)  
<span data-ttu-id="81885-154">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="81885-154">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>  
<!-- [Walkthrough: Tracing Serial-Lot Numbers](walkthrough-tracing-serial-lot-numbers.md)   -->
[<span data-ttu-id="81885-155">Find Entries</span><span class="sxs-lookup"><span data-stu-id="81885-155">Find Entries</span></span>](ui-find-entries.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]