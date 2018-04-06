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
ms.date: 01/25/2018
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 960ae581a3f933c6e9c2ed5183944ddf62ca5965
ms.contentlocale: en-nz
ms.lasthandoff: 03/22/2018

---
# <a name="enable-application-of-ledger-entries-in-different-currencies"></a><span data-ttu-id="1342d-103">Enable Application of Ledger Entries in Different Currencies</span><span class="sxs-lookup"><span data-stu-id="1342d-103">Enable Application of Ledger Entries in Different Currencies</span></span>
<span data-ttu-id="1342d-104">If you purchase from a vendor in one currency and submit payment in another currency, you can apply the payment to the purchase.</span><span class="sxs-lookup"><span data-stu-id="1342d-104">If you purchase from a vendor in one currency and submit payment in another currency, you can apply the payment to the purchase.</span></span>

<span data-ttu-id="1342d-105">Likewise, if you sell to a customer in one currency and receive payment in another currency, you can apply the payment to the sales invoice.</span><span class="sxs-lookup"><span data-stu-id="1342d-105">Likewise, if you sell to a customer in one currency and receive payment in another currency, you can apply the payment to the sales invoice.</span></span>

<span data-ttu-id="1342d-106">The following procedure describes how to set this up for vendor ledger entries in the **Purchases & Payables Setup** window.</span><span class="sxs-lookup"><span data-stu-id="1342d-106">The following procedure describes how to set this up for vendor ledger entries in the **Purchases & Payables Setup** window.</span></span> <span data-ttu-id="1342d-107">The setup is similar for customer ledger entries in the **Sales & Receivables Setup** window.</span><span class="sxs-lookup"><span data-stu-id="1342d-107">The setup is similar for customer ledger entries in the **Sales & Receivables Setup** window.</span></span>

## <a name="to-enable-application-of-vendor-ledger-entries-in-different-currencies"></a><span data-ttu-id="1342d-108">To enable application of vendor ledger entries in different currencies</span><span class="sxs-lookup"><span data-stu-id="1342d-108">To enable application of vendor ledger entries in different currencies</span></span>
1. <span data-ttu-id="1342d-109">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Purchases & Payables Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="1342d-109">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Purchases & Payables Setup**, and then choose the related link.</span></span>
2. <span data-ttu-id="1342d-110">In the **Appln. between Currencies** field, select one of the following options.</span><span class="sxs-lookup"><span data-stu-id="1342d-110">In the **Appln. between Currencies** field, select one of the following options.</span></span>

| <span data-ttu-id="1342d-111">Option</span><span class="sxs-lookup"><span data-stu-id="1342d-111">Option</span></span> | <span data-ttu-id="1342d-112">Description</span><span class="sxs-lookup"><span data-stu-id="1342d-112">Description</span></span> |
| --- | --- |
| <span data-ttu-id="1342d-113">None</span><span class="sxs-lookup"><span data-stu-id="1342d-113">None</span></span> |<span data-ttu-id="1342d-114">Application between currencies is not allowed.</span><span class="sxs-lookup"><span data-stu-id="1342d-114">Application between currencies is not allowed.</span></span> |
| <span data-ttu-id="1342d-115">EMU</span><span class="sxs-lookup"><span data-stu-id="1342d-115">EMU</span></span> |<span data-ttu-id="1342d-116">Application between EMU currencies is allowed.</span><span class="sxs-lookup"><span data-stu-id="1342d-116">Application between EMU currencies is allowed.</span></span> |
| <span data-ttu-id="1342d-117">All</span><span class="sxs-lookup"><span data-stu-id="1342d-117">All</span></span> |<span data-ttu-id="1342d-118">Application between all currencies is allowed.</span><span class="sxs-lookup"><span data-stu-id="1342d-118">Application between all currencies is allowed.</span></span> |

## <a name="to-set-up-gl-accounts-for-currency-application-rounding-differences"></a><span data-ttu-id="1342d-119">To set up G/L accounts for currency application rounding differences</span><span class="sxs-lookup"><span data-stu-id="1342d-119">To set up G/L accounts for currency application rounding differences</span></span>  
<span data-ttu-id="1342d-120">If you apply entries in different currencies, you must set up the general ledger accounts to which you want to post rounding differences.</span><span class="sxs-lookup"><span data-stu-id="1342d-120">If you apply entries in different currencies, you must set up the general ledger accounts to which you want to post rounding differences.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="1342d-121">You must set up the general ledger accounts before you complete the task.</span><span class="sxs-lookup"><span data-stu-id="1342d-121">You must set up the general ledger accounts before you complete the task.</span></span> <span data-ttu-id="1342d-122">For more information, see [Understanding the General Ledger and the Chart of Accounts](finance-general-ledger.md).</span><span class="sxs-lookup"><span data-stu-id="1342d-122">For more information, see [Understanding the General Ledger and the Chart of Accounts](finance-general-ledger.md).</span></span>

1. <span data-ttu-id="1342d-123">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Customer Posting Groups**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="1342d-123">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Customer Posting Groups**, and then choose the related link.</span></span>  
2. <span data-ttu-id="1342d-124">In the **Debit Curr. Appln. Rndg. Acc.** and **Credit Curr. Appln. Rndg. Acc.** fields, enter the relevant general ledger accounts to post rounding differences.</span><span class="sxs-lookup"><span data-stu-id="1342d-124">In the **Debit Curr. Appln. Rndg. Acc.** and **Credit Curr. Appln. Rndg. Acc.** fields, enter the relevant general ledger accounts to post rounding differences.</span></span>  
3. <span data-ttu-id="1342d-125">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Vendor Posting Groups**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="1342d-125">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Vendor Posting Groups**, and then choose the related link.</span></span>  
4. <span data-ttu-id="1342d-126">In the **Debit Curr. Appln. Rndg. Acc.** and **Credit Curr. Appln. Rndg. Acc.** fields, enter the relevant general ledger accounts to post rounding differences.</span><span class="sxs-lookup"><span data-stu-id="1342d-126">In the **Debit Curr. Appln. Rndg. Acc.** and **Credit Curr. Appln. Rndg. Acc.** fields, enter the relevant general ledger accounts to post rounding differences.</span></span>  

## <a name="see-also"></a><span data-ttu-id="1342d-127">See Also</span><span class="sxs-lookup"><span data-stu-id="1342d-127">See Also</span></span>
[<span data-ttu-id="1342d-128">Managing Payables</span><span class="sxs-lookup"><span data-stu-id="1342d-128">Managing Payables</span></span>](payables-manage-payables.md)  
[<span data-ttu-id="1342d-129">Managing Receivables</span><span class="sxs-lookup"><span data-stu-id="1342d-129">Managing Receivables</span></span>](receivables-manage-receivables.md)  
<span data-ttu-id="1342d-130">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="1342d-130">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
