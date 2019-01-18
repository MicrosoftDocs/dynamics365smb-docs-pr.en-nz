---
title: Apply Entries in Different Currencies| Microsoft Docs
description: You can apply ledger entries in multiple currencies, for example, if you sell in one currency and receive payment in another.
services: project-madeira
documentationcenter: 
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: multiple currencies, payment, reconcile
ms.date: 10/01/2018
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 33b900f1ac9e295921e7f3d6ea72cc93939d8a1b
ms.openlocfilehash: 6d58c088c776a953cb76d102b7deeb3b8d69b42a
ms.contentlocale: en-nz
ms.lasthandoff: 11/26/2018

---
# <a name="enable-application-of-ledger-entries-in-different-currencies"></a><span data-ttu-id="3ac88-103">Enable Application of Ledger Entries in Different Currencies</span><span class="sxs-lookup"><span data-stu-id="3ac88-103">Enable Application of Ledger Entries in Different Currencies</span></span>
<span data-ttu-id="3ac88-104">If you purchase from a vendor in one currency and submit payment in another currency, you can apply the payment to the purchase.</span><span class="sxs-lookup"><span data-stu-id="3ac88-104">If you purchase from a vendor in one currency and submit payment in another currency, you can apply the payment to the purchase.</span></span>

<span data-ttu-id="3ac88-105">Likewise, if you sell to a customer in one currency and receive payment in another currency, you can apply the payment to the sales invoice.</span><span class="sxs-lookup"><span data-stu-id="3ac88-105">Likewise, if you sell to a customer in one currency and receive payment in another currency, you can apply the payment to the sales invoice.</span></span>

<span data-ttu-id="3ac88-106">The following procedure describes how to set this up for vendor ledger entries on the **Purchases & Payables Setup** page.</span><span class="sxs-lookup"><span data-stu-id="3ac88-106">The following procedure describes how to set this up for vendor ledger entries on the **Purchases & Payables Setup** page.</span></span> <span data-ttu-id="3ac88-107">The setup is similar for customer ledger entries on the **Sales & Receivables Setup** page.</span><span class="sxs-lookup"><span data-stu-id="3ac88-107">The setup is similar for customer ledger entries on the **Sales & Receivables Setup** page.</span></span>

## <a name="to-enable-application-of-vendor-ledger-entries-in-different-currencies"></a><span data-ttu-id="3ac88-108">To enable application of vendor ledger entries in different currencies</span><span class="sxs-lookup"><span data-stu-id="3ac88-108">To enable application of vendor ledger entries in different currencies</span></span>
1. <span data-ttu-id="3ac88-109">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchases & Payables Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="3ac88-109">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchases & Payables Setup**, and then choose the related link.</span></span>
2. <span data-ttu-id="3ac88-110">In the **Appln. between Currencies** field, select one of the following options.</span><span class="sxs-lookup"><span data-stu-id="3ac88-110">In the **Appln. between Currencies** field, select one of the following options.</span></span>

| <span data-ttu-id="3ac88-111">Option</span><span class="sxs-lookup"><span data-stu-id="3ac88-111">Option</span></span> | <span data-ttu-id="3ac88-112">Description</span><span class="sxs-lookup"><span data-stu-id="3ac88-112">Description</span></span> |
| --- | --- |
| <span data-ttu-id="3ac88-113">None</span><span class="sxs-lookup"><span data-stu-id="3ac88-113">None</span></span> |<span data-ttu-id="3ac88-114">Application between currencies is not allowed.</span><span class="sxs-lookup"><span data-stu-id="3ac88-114">Application between currencies is not allowed.</span></span> |
| <span data-ttu-id="3ac88-115">EMU</span><span class="sxs-lookup"><span data-stu-id="3ac88-115">EMU</span></span> |<span data-ttu-id="3ac88-116">Application between EMU currencies is allowed.</span><span class="sxs-lookup"><span data-stu-id="3ac88-116">Application between EMU currencies is allowed.</span></span> |
| <span data-ttu-id="3ac88-117">All</span><span class="sxs-lookup"><span data-stu-id="3ac88-117">All</span></span> |<span data-ttu-id="3ac88-118">Application between all currencies is allowed.</span><span class="sxs-lookup"><span data-stu-id="3ac88-118">Application between all currencies is allowed.</span></span> |

## <a name="to-set-up-gl-accounts-for-currency-application-rounding-differences"></a><span data-ttu-id="3ac88-119">To set up G/L accounts for currency application rounding differences</span><span class="sxs-lookup"><span data-stu-id="3ac88-119">To set up G/L accounts for currency application rounding differences</span></span>  
<span data-ttu-id="3ac88-120">If you apply entries in different currencies, you must set up the general ledger accounts to which you want to post rounding differences.</span><span class="sxs-lookup"><span data-stu-id="3ac88-120">If you apply entries in different currencies, you must set up the general ledger accounts to which you want to post rounding differences.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="3ac88-121">You must set up the general ledger accounts before you complete the task.</span><span class="sxs-lookup"><span data-stu-id="3ac88-121">You must set up the general ledger accounts before you complete the task.</span></span> <span data-ttu-id="3ac88-122">For more information, see [Understanding the General Ledger and the Chart of Accounts](finance-general-ledger.md).</span><span class="sxs-lookup"><span data-stu-id="3ac88-122">For more information, see [Understanding the General Ledger and the Chart of Accounts](finance-general-ledger.md).</span></span>

1. <span data-ttu-id="3ac88-123">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Customer Posting Groups**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="3ac88-123">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Customer Posting Groups**, and then choose the related link.</span></span>  
2. <span data-ttu-id="3ac88-124">In the **Debit Curr. Appln. Rndg. Acc.** and **Credit Curr. Appln. Rndg. Acc.** fields, enter the relevant general ledger accounts to post rounding differences.</span><span class="sxs-lookup"><span data-stu-id="3ac88-124">In the **Debit Curr. Appln. Rndg. Acc.** and **Credit Curr. Appln. Rndg. Acc.** fields, enter the relevant general ledger accounts to post rounding differences.</span></span>  
3. <span data-ttu-id="3ac88-125">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Vendor Posting Groups**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="3ac88-125">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Vendor Posting Groups**, and then choose the related link.</span></span>  
4. <span data-ttu-id="3ac88-126">In the **Debit Curr. Appln. Rndg. Acc.** and **Credit Curr. Appln. Rndg. Acc.** fields, enter the relevant general ledger accounts to post rounding differences.</span><span class="sxs-lookup"><span data-stu-id="3ac88-126">In the **Debit Curr. Appln. Rndg. Acc.** and **Credit Curr. Appln. Rndg. Acc.** fields, enter the relevant general ledger accounts to post rounding differences.</span></span>  

## <a name="see-also"></a><span data-ttu-id="3ac88-127">See Also</span><span class="sxs-lookup"><span data-stu-id="3ac88-127">See Also</span></span>
[<span data-ttu-id="3ac88-128">Managing Payables</span><span class="sxs-lookup"><span data-stu-id="3ac88-128">Managing Payables</span></span>](payables-manage-payables.md)  
[<span data-ttu-id="3ac88-129">Managing Receivables</span><span class="sxs-lookup"><span data-stu-id="3ac88-129">Managing Receivables</span></span>](receivables-manage-receivables.md)  
<span data-ttu-id="3ac88-130">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="3ac88-130">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

