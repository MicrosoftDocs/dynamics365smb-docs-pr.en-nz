---
title: Optional Activities for Closing Periods | Microsoft Docs
description: This topic outlines the optional processes and activities for closing accounting periods in Business Central.
services: project-madeira
documentationcenter: ''
author: jswymer
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: year closing, close accounting period, close fiscal year, aging, creditor payments, vendor payments
ms.date: 04/01/2021
ms.author: jswymer
ms.openlocfilehash: 6f1bbed79a2f5d817e3f486cfb4207e5b285aef2
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 03/31/2021
ms.locfileid: "5775266"
---
# <a name="overview-of-tasks-to-close-accounting-periods"></a><span data-ttu-id="98180-103">Overview of Tasks to Close Accounting Periods</span><span class="sxs-lookup"><span data-stu-id="98180-103">Overview of Tasks to Close Accounting Periods</span></span>
[!INCLUDE[prod_short](includes/prod_short.md)] <span data-ttu-id="98180-104">does not force you to close periods, however, there are many period-end (month-end) activities that you can do.</span><span class="sxs-lookup"><span data-stu-id="98180-104">does not force you to close periods, however, there are many period-end (month-end) activities that you can do.</span></span> <span data-ttu-id="98180-105">This topic provides an overview of optional processes and activities for closing periods.</span><span class="sxs-lookup"><span data-stu-id="98180-105">This topic provides an overview of optional processes and activities for closing periods.</span></span>  

## <a name="general-ledger"></a><span data-ttu-id="98180-106">General Ledger</span><span class="sxs-lookup"><span data-stu-id="98180-106">General Ledger</span></span>
* <span data-ttu-id="98180-107">Specify system-wide and user-specific posting periods.</span><span class="sxs-lookup"><span data-stu-id="98180-107">Specify system-wide and user-specific posting periods.</span></span>  

    <span data-ttu-id="98180-108">This specifies the dates between which you allow posting.</span><span class="sxs-lookup"><span data-stu-id="98180-108">This specifies the dates between which you allow posting.</span></span> <span data-ttu-id="98180-109">Depending on your business, you may want to allow posting at the start of the period, or toward the end.</span><span class="sxs-lookup"><span data-stu-id="98180-109">Depending on your business, you may want to allow posting at the start of the period, or toward the end.</span></span> <span data-ttu-id="98180-110">For more information, see [Specify Posting Periods](finance-how-specify-posting-periods.md).</span><span class="sxs-lookup"><span data-stu-id="98180-110">For more information, see [Specify Posting Periods](finance-how-specify-posting-periods.md).</span></span>  
* <span data-ttu-id="98180-111">Make all necessary G/L adjustments.</span><span class="sxs-lookup"><span data-stu-id="98180-111">Make all necessary G/L adjustments.</span></span>  
* <span data-ttu-id="98180-112">Update and post Recurring Journals.</span><span class="sxs-lookup"><span data-stu-id="98180-112">Update and post Recurring Journals.</span></span>  
  <!--* Process Consolidations-->
* <span data-ttu-id="98180-113">Run account schedules as follows:</span><span class="sxs-lookup"><span data-stu-id="98180-113">Run account schedules as follows:</span></span>  
  * <span data-ttu-id="98180-114">Open the **Account Schedule** page, and then choose the **Print** action.</span><span class="sxs-lookup"><span data-stu-id="98180-114">Open the **Account Schedule** page, and then choose the **Print** action.</span></span>  

## <a name="sales-and-receivables"></a><span data-ttu-id="98180-115">Sales and Receivables</span><span class="sxs-lookup"><span data-stu-id="98180-115">Sales and Receivables</span></span>
* <span data-ttu-id="98180-116">Post all sales orders, invoices, credit memos, and return orders.</span><span class="sxs-lookup"><span data-stu-id="98180-116">Post all sales orders, invoices, credit memos, and return orders.</span></span>  
* <span data-ttu-id="98180-117">Post all cash receipt journals.</span><span class="sxs-lookup"><span data-stu-id="98180-117">Post all cash receipt journals.</span></span>  
* <span data-ttu-id="98180-118">Update and post recurring journals that are related to sales and receivables.</span><span class="sxs-lookup"><span data-stu-id="98180-118">Update and post recurring journals that are related to sales and receivables.</span></span>  
* <span data-ttu-id="98180-119">Reconcile accounts receivable to the general ledger.</span><span class="sxs-lookup"><span data-stu-id="98180-119">Reconcile accounts receivable to the general ledger.</span></span>  
* <span data-ttu-id="98180-120">Run the **Delete Invoiced Sales Orders** batch job.</span><span class="sxs-lookup"><span data-stu-id="98180-120">Run the **Delete Invoiced Sales Orders** batch job.</span></span>  

## <a name="purchases-and-payables"></a><span data-ttu-id="98180-121">Purchases and Payables</span><span class="sxs-lookup"><span data-stu-id="98180-121">Purchases and Payables</span></span>
* <span data-ttu-id="98180-122">Post all purchase orders, invoices, credit memos, and return orders.</span><span class="sxs-lookup"><span data-stu-id="98180-122">Post all purchase orders, invoices, credit memos, and return orders.</span></span>  
* <span data-ttu-id="98180-123">Post all payment journals.</span><span class="sxs-lookup"><span data-stu-id="98180-123">Post all payment journals.</span></span>  
* <span data-ttu-id="98180-124">Update and post recurring journals that are related to purchases & payables.</span><span class="sxs-lookup"><span data-stu-id="98180-124">Update and post recurring journals that are related to purchases & payables.</span></span>  
* <span data-ttu-id="98180-125">Run the **Aged Accounts Payable** report and reconcile accounts payable to the general ledger.</span><span class="sxs-lookup"><span data-stu-id="98180-125">Run the **Aged Accounts Payable** report and reconcile accounts payable to the general ledger.</span></span>  
* <span data-ttu-id="98180-126">Run the **Delete Invoiced Purchase Orders** batch job.</span><span class="sxs-lookup"><span data-stu-id="98180-126">Run the **Delete Invoiced Purchase Orders** batch job.</span></span>  

<span data-ttu-id="98180-127">Fixed Assets</span><span class="sxs-lookup"><span data-stu-id="98180-127">Fixed Assets</span></span>
* <span data-ttu-id="98180-128">Post all maintenance costs have been posted through the fixed asset journals or invoices.</span><span class="sxs-lookup"><span data-stu-id="98180-128">Post all maintenance costs have been posted through the fixed asset journals or invoices.</span></span>
* <span data-ttu-id="98180-129">Post adjustments.</span><span class="sxs-lookup"><span data-stu-id="98180-129">Post adjustments.</span></span>
* <span data-ttu-id="98180-130">Post appreciation.</span><span class="sxs-lookup"><span data-stu-id="98180-130">Post appreciation.</span></span>
* <span data-ttu-id="98180-131">Post depreciation.</span><span class="sxs-lookup"><span data-stu-id="98180-131">Post depreciation.</span></span>
* <span data-ttu-id="98180-132">Update and post the recurring fixed asset journal.</span><span class="sxs-lookup"><span data-stu-id="98180-132">Update and post the recurring fixed asset journal.</span></span>

<span data-ttu-id="98180-133">Intercompany</span><span class="sxs-lookup"><span data-stu-id="98180-133">Intercompany</span></span>
* <span data-ttu-id="98180-134">Process Intercompany Transactions</span><span class="sxs-lookup"><span data-stu-id="98180-134">Process Intercompany Transactions</span></span>

## <a name="calculate-and-process-sales-tax"></a><span data-ttu-id="98180-135">Calculate and Process Sales Tax</span><span class="sxs-lookup"><span data-stu-id="98180-135">Calculate and Process Sales Tax</span></span>
* <span data-ttu-id="98180-136">Complete Tax Statements.</span><span class="sxs-lookup"><span data-stu-id="98180-136">Complete Tax Statements.</span></span>  

## <a name="see-also"></a><span data-ttu-id="98180-137">See Also</span><span class="sxs-lookup"><span data-stu-id="98180-137">See Also</span></span>
[<span data-ttu-id="98180-138">Closing Years and Periods</span><span class="sxs-lookup"><span data-stu-id="98180-138">Closing Years and Periods</span></span>](year-close-years-periods.md)  
[<span data-ttu-id="98180-139">Closing Books</span><span class="sxs-lookup"><span data-stu-id="98180-139">Closing Books</span></span>](year-close-books.md)  
<span data-ttu-id="98180-140">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="98180-140">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>


[!INCLUDE[footer-include](includes/footer-banner.md)]