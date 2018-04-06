---
title: Issue, Print, Cancel, and Void Checks| Microsoft Docs
description: Describes how to issue cheques using the payment journal, print cheques, and void or view cheque ledger entries in Finance and Operations, Business edition.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: payment journal, print check, vendor payment, creditor, debt, balance due, AP
ms.date: 06/06/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: b3f8bece0d0d1de9a6fd17b84df73d466ccdf403
ms.contentlocale: en-nz
ms.lasthandoff: 03/22/2018

---
# <a name="work-with-checks"></a><span data-ttu-id="f4585-103">Work With Cheques</span><span class="sxs-lookup"><span data-stu-id="f4585-103">Work With Checks</span></span>
<span data-ttu-id="f4585-104">You can issue electronic and manual checks in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="f4585-104">You can issue electronic and manual checks in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="f4585-105">Both methods use the payment journal to issue cheques to vendors.</span><span class="sxs-lookup"><span data-stu-id="f4585-105">Both methods use the payment journal to issue checks to vendors.</span></span> <span data-ttu-id="f4585-106">You can also void cheques and view cheque ledger entries.</span><span class="sxs-lookup"><span data-stu-id="f4585-106">You can also void checks and view check ledger entries.</span></span>

<span data-ttu-id="f4585-107">The process of issuing cheques suggests payments, creates ledger entries, and prints the computer cheques.</span><span class="sxs-lookup"><span data-stu-id="f4585-107">The process of issuing checks suggests payments, creates ledger entries, and prints the computer checks.</span></span>

> [!NOTE]  
>   <span data-ttu-id="f4585-108">To make sure that your bank only clears validated cheques and amounts, you can send them a file that contains vendor, cheque, and payment information.</span><span class="sxs-lookup"><span data-stu-id="f4585-108">To make sure that your bank only clears validated checks and amounts, you can send them a file that contains vendor, check, and payment information.</span></span> <span data-ttu-id="f4585-109">For more information, see [Export a Positive Pay file](finance-how-positive-pay.md).</span><span class="sxs-lookup"><span data-stu-id="f4585-109">For more information, see [Export a Positive Pay file](finance-how-positive-pay.md).</span></span>

<span data-ttu-id="f4585-110">Your printer must be correctly set up with the cheque forms, and you must define which cheque layout to use.</span><span class="sxs-lookup"><span data-stu-id="f4585-110">Your printer must be correctly set up with the check forms, and you must define which check layout to use.</span></span> <span data-ttu-id="f4585-111">For more information, see [Define Cheque Layouts](finance-how-define-check-layouts.md)</span><span class="sxs-lookup"><span data-stu-id="f4585-111">For more information, see [Define Check Layouts](finance-how-define-check-layouts.md)</span></span>

## <a name="to-issue-checks"></a><span data-ttu-id="f4585-112">To issue cheques</span><span class="sxs-lookup"><span data-stu-id="f4585-112">To issue checks</span></span>
1. <span data-ttu-id="f4585-113">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Payment Journals**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="f4585-113">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Payment Journals**, and then choose the related link.</span></span>
2. <span data-ttu-id="f4585-114">Fill in the journal with relevant payments, for example by using the Suggest Vendor Payments function.</span><span class="sxs-lookup"><span data-stu-id="f4585-114">Fill in the journal with relevant payments, for example by using the Suggest Vendor Payments function.</span></span> <span data-ttu-id="f4585-115">For more information, see [Suggest Vendor Payments](payables-how-suggest-vendor-payments.md).</span><span class="sxs-lookup"><span data-stu-id="f4585-115">For more information, see [Suggest Vendor Payments](payables-how-suggest-vendor-payments.md).</span></span>
3. <span data-ttu-id="f4585-116">In the **Bank Payment Type** field on journal lines for payment that you want to make with cheques, select one of the following options:</span><span class="sxs-lookup"><span data-stu-id="f4585-116">In the **Bank Payment Type** field on journal lines for payment that you want to make with checks, select one of the following options:</span></span>

   * <span data-ttu-id="f4585-117">**Computer Cheque**: Select this option if you want to print a cheque for the amount on the payment journal line.</span><span class="sxs-lookup"><span data-stu-id="f4585-117">**Computer Check**: Select this option if you want to print a check for the amount on the payment journal line.</span></span> <span data-ttu-id="f4585-118">You must print the checks before you can post the journal lines.</span><span class="sxs-lookup"><span data-stu-id="f4585-118">You must print the checks before you can post the journal lines.</span></span> <span data-ttu-id="f4585-119">You can only select **Computer Cheque** if the **Bal. Account Type** or the **Account Type** is **Bank Account**.</span><span class="sxs-lookup"><span data-stu-id="f4585-119">You can only select **Computer Check** if the **Bal. Account Type** or the **Account Type** is **Bank Account**.</span></span>
   * <span data-ttu-id="f4585-120">**Manual Cheque**: Select this option if you have created a cheque manually and want to create a corresponding cheque ledger entry for this amount.</span><span class="sxs-lookup"><span data-stu-id="f4585-120">**Manual Check**: Select this option if you have created a check manually and want to create a corresponding check ledger entry for this amount.</span></span> <span data-ttu-id="f4585-121">By using this option, you cannot print checks from [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="f4585-121">By using this option, you cannot print checks from [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="f4585-122">You can only select **Manual Cheque** if the **Bal. Account Type** or the **Account Type** is **Bank Account**.</span><span class="sxs-lookup"><span data-stu-id="f4585-122">You can only select **Manual Check** if the **Bal. Account Type** or the **Account Type** is **Bank Account**.</span></span>

     > [!NOTE]  
>   <span data-ttu-id="f4585-123">You must print computer checks before you post the related journal lines.</span><span class="sxs-lookup"><span data-stu-id="f4585-123">You must print computer checks before you post the related journal lines.</span></span>
4. <span data-ttu-id="f4585-124">In case of computer cheques, choose **Print Cheque**.</span><span class="sxs-lookup"><span data-stu-id="f4585-124">In case of computer checks, choose **Print Check**.</span></span>
5. <span data-ttu-id="f4585-125">In the **Check** window, fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="f4585-125">In the **Check** window, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
6. <span data-ttu-id="f4585-126">Choose the **Print** button.</span><span class="sxs-lookup"><span data-stu-id="f4585-126">Choose the **Print** button.</span></span>

> [!NOTE]  
>   <span data-ttu-id="f4585-127">If you want to print cheques in more than one currency from different bank accounts, you must run the **Print Cheque** batch job separately for each currency and specify the appropriate bank account.</span><span class="sxs-lookup"><span data-stu-id="f4585-127">If you want to print checks in more than one currency from different bank accounts, you must run the **Print Check** batch job separately for each currency and specify the appropriate bank account.</span></span>

## <a name="to-cancel-printed-checks-that-are-not-posted"></a><span data-ttu-id="f4585-128">To cancel printed cheques that are not posted</span><span class="sxs-lookup"><span data-stu-id="f4585-128">To cancel printed checks that are not posted</span></span>
<span data-ttu-id="f4585-129">You can cancel non-posted cheques after they have been printed by using the **Void Cheque** action in the **Payment Journal** window.</span><span class="sxs-lookup"><span data-stu-id="f4585-129">You can cancel non-posted checks after they have been printed by using the **Void Check** action in the **Payment Journal** window.</span></span>

1. <span data-ttu-id="f4585-130">In the **Payment Journal** window, choose the **Void Cheque**, and then choose which cheques to cancel.</span><span class="sxs-lookup"><span data-stu-id="f4585-130">In the **Payment Journal** window, choose the **Void Check**, and then choose which checks to cancel.</span></span>

## <a name="to-void-checks"></a><span data-ttu-id="f4585-131">To void cheques</span><span class="sxs-lookup"><span data-stu-id="f4585-131">To void checks</span></span>
<span data-ttu-id="f4585-132">When cheque payment have been posted, you can only cancel (void) cheques from the resulting bank ledger entries.</span><span class="sxs-lookup"><span data-stu-id="f4585-132">When check payment have been posted, you can only cancel (void) checks from the resulting bank ledger entries.</span></span>

1. <span data-ttu-id="f4585-133">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Bank Accounts**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="f4585-133">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Bank Accounts**, and then choose the related link.</span></span>
2. <span data-ttu-id="f4585-134">Select the relevant bank account, choose the **Edit** action, and then choose the **Cheque Ledger Entries** action.</span><span class="sxs-lookup"><span data-stu-id="f4585-134">Select the relevant bank account, choose the **Edit** action, and then choose the **Check Ledger Entries** action.</span></span>
3. <span data-ttu-id="f4585-135">In the **Cheque Ledger Entries** window, choose the **Void Cheque** action.</span><span class="sxs-lookup"><span data-stu-id="f4585-135">In the **Check Ledger Entries** window, choose the **Void Check** action.</span></span>
4. <span data-ttu-id="f4585-136">Select the **Void Cheque Only** check box.</span><span class="sxs-lookup"><span data-stu-id="f4585-136">Select the **Void Check Only** check box.</span></span>
5. <span data-ttu-id="f4585-137">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="f4585-137">Choose the **OK** button.</span></span>

## <a name="see-also"></a><span data-ttu-id="f4585-138">See Also</span><span class="sxs-lookup"><span data-stu-id="f4585-138">See Also</span></span>
[<span data-ttu-id="f4585-139">Managing Payables</span><span class="sxs-lookup"><span data-stu-id="f4585-139">Managing Payables</span></span>](payables-manage-payables.md)  
[<span data-ttu-id="f4585-140">Setting Up Banking</span><span class="sxs-lookup"><span data-stu-id="f4585-140">Setting Up Banking</span></span>](bank-setup-banking.md)  
[<span data-ttu-id="f4585-141">Export a Positive Pay file</span><span class="sxs-lookup"><span data-stu-id="f4585-141">Export a Positive Pay file</span></span>](finance-how-positive-pay.md)  
<span data-ttu-id="f4585-142">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="f4585-142">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  

