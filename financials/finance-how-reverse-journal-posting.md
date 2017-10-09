---
title: Undo a Posting by Posting a Reversing Entry| Microsoft Docs
description: If you have made an erroneous posting in the general journal, then you can use the Reverse Transaction function to undo the posting with a correct audit trail.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: reimbursement
ms.date: 08/03/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 802171d4f421270cb7e9b4f9dfedec9b9fe5ddc6
ms.contentlocale: en-nz
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-reverse-postings"></a><span data-ttu-id="d02fb-103">How to: Reverse Postings</span><span class="sxs-lookup"><span data-stu-id="d02fb-103">How to: Reverse Postings</span></span>
<span data-ttu-id="d02fb-104">To undo an erroneous journal posting, you select the entry and create a reverse entry (entries identical to the original entry but with opposite sign in the amount field) with the same document number and posting date as the original entry.</span><span class="sxs-lookup"><span data-stu-id="d02fb-104">To undo an erroneous journal posting, you select the entry and create a reverse entry (entries identical to the original entry but with opposite sign in the amount field) with the same document number and posting date as the original entry.</span></span> <span data-ttu-id="d02fb-105">After reversing an entry, you must make the correct entry.</span><span class="sxs-lookup"><span data-stu-id="d02fb-105">After reversing an entry, you must make the correct entry.</span></span>

<span data-ttu-id="d02fb-106">You can only reverse entries that are posted from a general journal line.</span><span class="sxs-lookup"><span data-stu-id="d02fb-106">You can only reverse entries that are posted from a general journal line.</span></span> <span data-ttu-id="d02fb-107">An entry can only be reversed once.</span><span class="sxs-lookup"><span data-stu-id="d02fb-107">An entry can only be reversed once.</span></span>

<span data-ttu-id="d02fb-108">For more information about posting from a general journal, see [How to: Post Transactions Directly to the General Ledger](finance-how-post-transactions-directly.md).</span><span class="sxs-lookup"><span data-stu-id="d02fb-108">For more information about posting from a general journal, see [How to: Post Transactions Directly to the General Ledger](finance-how-post-transactions-directly.md).</span></span>

<span data-ttu-id="d02fb-109">If you have made an incorrect negative quantity posting, such as a purchase order with the wrong number of items and posted it as received but not invoiced, then you can undo the posting.</span><span class="sxs-lookup"><span data-stu-id="d02fb-109">If you have made an incorrect negative quantity posting, such as a purchase order with the wrong number of items and posted it as received but not invoiced, then you can undo the posting.</span></span>

<span data-ttu-id="d02fb-110">If you have made an incorrect positive quantity posting, such as a purchase return order with the wrong number of items and posted it as shipped but not invoiced, then you can undo the posting.</span><span class="sxs-lookup"><span data-stu-id="d02fb-110">If you have made an incorrect positive quantity posting, such as a purchase return order with the wrong number of items and posted it as shipped but not invoiced, then you can undo the posting.</span></span>   

## <a name="to-reverse-the-journal-posting-of-a-general-ledger-entry"></a><span data-ttu-id="d02fb-111">To reverse the journal posting of a general ledger entry</span><span class="sxs-lookup"><span data-stu-id="d02fb-111">To reverse the journal posting of a general ledger entry</span></span>
<span data-ttu-id="d02fb-112">You can reverse entries from all **Ledger Entries** windows.</span><span class="sxs-lookup"><span data-stu-id="d02fb-112">You can reverse entries from all **Ledger Entries** windows.</span></span> <span data-ttu-id="d02fb-113">The following procedure is based on the **General Ledger Entries** window.</span><span class="sxs-lookup"><span data-stu-id="d02fb-113">The following procedure is based on the **General Ledger Entries** window.</span></span>
1. <span data-ttu-id="d02fb-114">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **General Ledger Entries**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="d02fb-114">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **General Ledger Entries**, and then choose the related link.</span></span>
2. <span data-ttu-id="d02fb-115">Select the entry that you want to reverse, and then choose the **Reverse Transaction** action.</span><span class="sxs-lookup"><span data-stu-id="d02fb-115">Select the entry that you want to reverse, and then choose the **Reverse Transaction** action.</span></span> <span data-ttu-id="d02fb-116">Note that is must originate from a journal posting.</span><span class="sxs-lookup"><span data-stu-id="d02fb-116">Note that is must originate from a journal posting.</span></span>
3. <span data-ttu-id="d02fb-117">In the **Reverse Transaction Entries** window, select the relevant entry, and then choose the **Reverse** action.</span><span class="sxs-lookup"><span data-stu-id="d02fb-117">In the **Reverse Transaction Entries** window, select the relevant entry, and then choose the **Reverse** action.</span></span>
4. <span data-ttu-id="d02fb-118">Choose the **Yes** button on the confirmation message.</span><span class="sxs-lookup"><span data-stu-id="d02fb-118">Choose the **Yes** button on the confirmation message.</span></span>

## <a name="to-undo-a-quantity-posting-on-a-posted-purchase-receipt"></a><span data-ttu-id="d02fb-119">To undo a quantity posting on a posted purchase receipt</span><span class="sxs-lookup"><span data-stu-id="d02fb-119">To undo a quantity posting on a posted purchase receipt</span></span>  

1.  <span data-ttu-id="d02fb-120">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Posted Purchase Receipts**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="d02fb-120">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Posted Purchase Receipts**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="d02fb-121">Open the posted receipt that you want to undo.</span><span class="sxs-lookup"><span data-stu-id="d02fb-121">Open the posted receipt that you want to undo.</span></span>  
3.  <span data-ttu-id="d02fb-122">Select the line or lines that you want to undo.</span><span class="sxs-lookup"><span data-stu-id="d02fb-122">Select the line or lines that you want to undo.</span></span>  
4.  <span data-ttu-id="d02fb-123">Choose **Undo Receipt** action.</span><span class="sxs-lookup"><span data-stu-id="d02fb-123">Choose **Undo Receipt** action.</span></span>

    <span data-ttu-id="d02fb-124">A corrective line is inserted under the selected receipt line.</span><span class="sxs-lookup"><span data-stu-id="d02fb-124">A corrective line is inserted under the selected receipt line.</span></span>  

    <span data-ttu-id="d02fb-125">If the quantity was received in a warehouse receipt, then a corrective line is inserted in the posted warehouse receipt.</span><span class="sxs-lookup"><span data-stu-id="d02fb-125">If the quantity was received in a warehouse receipt, then a corrective line is inserted in the posted warehouse receipt.</span></span>  

    <span data-ttu-id="d02fb-126">The **Quantity Received** and **Qty. Rcd. Not Invoiced** fields on the related purchase order are set to zero.</span><span class="sxs-lookup"><span data-stu-id="d02fb-126">The **Quantity Received** and **Qty. Rcd. Not Invoiced** fields on the related purchase order are set to zero.</span></span>

## <a name="to-undo-and-then-redo-a-quantity-posting-on-a-posted-return-shipment"></a><span data-ttu-id="d02fb-127">To undo and then redo a quantity posting on a posted return shipment</span><span class="sxs-lookup"><span data-stu-id="d02fb-127">To undo and then redo a quantity posting on a posted return shipment</span></span>

1.  <span data-ttu-id="d02fb-128">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Posted Return Shipments**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="d02fb-128">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Posted Return Shipments**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="d02fb-129">Open the posted return shipment that you want to undo.</span><span class="sxs-lookup"><span data-stu-id="d02fb-129">Open the posted return shipment that you want to undo.</span></span>
3. <span data-ttu-id="d02fb-130">Select the line or lines you want to undo.</span><span class="sxs-lookup"><span data-stu-id="d02fb-130">Select the line or lines you want to undo.</span></span>  

4.  <span data-ttu-id="d02fb-131">Choose the **Undo Return Shipment** action.</span><span class="sxs-lookup"><span data-stu-id="d02fb-131">Choose the **Undo Return Shipment** action.</span></span>  

    <span data-ttu-id="d02fb-132">A corrective line is inserted in the posted document, and the **Return Qty. Shipped** and **Return Shpd. Not Invd.** fields on the return order are set to zero.</span><span class="sxs-lookup"><span data-stu-id="d02fb-132">A corrective line is inserted in the posted document, and the **Return Qty. Shipped** and **Return Shpd. Not Invd.** fields on the return order are set to zero.</span></span>  

    <span data-ttu-id="d02fb-133">Now go back to the purchase return order to redo the posting.</span><span class="sxs-lookup"><span data-stu-id="d02fb-133">Now go back to the purchase return order to redo the posting.</span></span>  

5.  <span data-ttu-id="d02fb-134">In the **Posted Return Shipment** window, take a note of the number in the **Return Order No.**</span><span class="sxs-lookup"><span data-stu-id="d02fb-134">In the **Posted Return Shipment** window, take a note of the number in the **Return Order No.**</span></span> <span data-ttu-id="d02fb-135">field.</span><span class="sxs-lookup"><span data-stu-id="d02fb-135">field.</span></span>  
6.  <span data-ttu-id="d02fb-136">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Purchase Return Orders**, and then select the related link.</span><span class="sxs-lookup"><span data-stu-id="d02fb-136">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Purchase Return Orders**, and then select the related link.</span></span>  
7.  <span data-ttu-id="d02fb-137">Open the return order in question, and then choose the **Reopen** action.</span><span class="sxs-lookup"><span data-stu-id="d02fb-137">Open the return order in question, and then choose the **Reopen** action.</span></span>  
8.  <span data-ttu-id="d02fb-138">Correct the entry in the **Quantity** field and post the purchase return order again.</span><span class="sxs-lookup"><span data-stu-id="d02fb-138">Correct the entry in the **Quantity** field and post the purchase return order again.</span></span>  

## <a name="see-also"></a><span data-ttu-id="d02fb-139">See Also</span><span class="sxs-lookup"><span data-stu-id="d02fb-139">See Also</span></span>
[<span data-ttu-id="d02fb-140">How to: Post Transactions Directly to the General Ledger</span><span class="sxs-lookup"><span data-stu-id="d02fb-140">How to: Post Transactions Directly to the General Ledger</span></span>](finance-how-post-transactions-directly.md)  
[<span data-ttu-id="d02fb-141">Working with General Journals</span><span class="sxs-lookup"><span data-stu-id="d02fb-141">Working with General Journals</span></span>](ui-work-general-journals.md)  
[<span data-ttu-id="d02fb-142">Finance</span><span class="sxs-lookup"><span data-stu-id="d02fb-142">Finance</span></span>](finance.md)  
<span data-ttu-id="d02fb-143">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="d02fb-143">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  

