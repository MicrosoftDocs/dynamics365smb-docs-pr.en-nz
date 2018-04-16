---
title: Design Details - Inventory Periods | Microsoft Docs
description: Backdated transactions or cost adjustments often affect balances and stock valuations for accounting periods that may be considered closed. This can have adverse effects on accurate reporting, especially within global corporations. The Inventory Periods feature can be used to avoid such problems by opening or closing inventory periods to limit posting in a set period of time.
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
ms.sourcegitcommit: acef03f32124c5983846bc6ed0c4d332c9c8b347
ms.openlocfilehash: 8ac32d8ec4d438be99e0dbcada61473ca91c1c45
ms.contentlocale: en-nz
ms.lasthandoff: 04/16/2018

---
# <a name="design-details-inventory-periods"></a><span data-ttu-id="5b6dd-105">Design Details: Inventory Periods</span><span class="sxs-lookup"><span data-stu-id="5b6dd-105">Design Details: Inventory Periods</span></span>
<span data-ttu-id="5b6dd-106">Backdated transactions or cost adjustments often affect balances and stock valuations for accounting periods that may be considered closed.</span><span class="sxs-lookup"><span data-stu-id="5b6dd-106">Backdated transactions or cost adjustments often affect balances and stock valuations for accounting periods that may be considered closed.</span></span> <span data-ttu-id="5b6dd-107">This can have adverse effects on accurate reporting, especially within global corporations.</span><span class="sxs-lookup"><span data-stu-id="5b6dd-107">This can have adverse effects on accurate reporting, especially within global corporations.</span></span> <span data-ttu-id="5b6dd-108">The Inventory Periods feature can be used to avoid such problems by opening or closing inventory periods to limit posting in a set period of time.</span><span class="sxs-lookup"><span data-stu-id="5b6dd-108">The Inventory Periods feature can be used to avoid such problems by opening or closing inventory periods to limit posting in a set period of time.</span></span>  

 <span data-ttu-id="5b6dd-109">An inventory period is a period of time, defined by an ending date, in which you post inventory transactions.</span><span class="sxs-lookup"><span data-stu-id="5b6dd-109">An inventory period is a period of time, defined by an ending date, in which you post inventory transactions.</span></span> <span data-ttu-id="5b6dd-110">When you close an inventory period, no value changes can be posted in the closed period.</span><span class="sxs-lookup"><span data-stu-id="5b6dd-110">When you close an inventory period, no value changes can be posted in the closed period.</span></span> <span data-ttu-id="5b6dd-111">This includes new value postings, expected or invoiced postings, changes to existing values, and cost adjustments.</span><span class="sxs-lookup"><span data-stu-id="5b6dd-111">This includes new value postings, expected or invoiced postings, changes to existing values, and cost adjustments.</span></span> <span data-ttu-id="5b6dd-112">However, you can still apply to an open item ledger entry that falls in the closed period.</span><span class="sxs-lookup"><span data-stu-id="5b6dd-112">However, you can still apply to an open item ledger entry that falls in the closed period.</span></span> <span data-ttu-id="5b6dd-113">For more information, see [Design Details: Item Application](design-details-item-application.md).</span><span class="sxs-lookup"><span data-stu-id="5b6dd-113">For more information, see [Design Details: Item Application](design-details-item-application.md).</span></span>  

 <span data-ttu-id="5b6dd-114">To make sure that all transaction entries in a closed period are final, the following conditions must be met before an inventory period can close:</span><span class="sxs-lookup"><span data-stu-id="5b6dd-114">To make sure that all transaction entries in a closed period are final, the following conditions must be met before an inventory period can close:</span></span>  

- <span data-ttu-id="5b6dd-115">All outbound item ledger entries in the period must be closed (no negative inventory).</span><span class="sxs-lookup"><span data-stu-id="5b6dd-115">All outbound item ledger entries in the period must be closed (no negative inventory).</span></span>  
- <span data-ttu-id="5b6dd-116">All item costs in the period must be adjusted.</span><span class="sxs-lookup"><span data-stu-id="5b6dd-116">All item costs in the period must be adjusted.</span></span>  
- <span data-ttu-id="5b6dd-117">All released and finished production orders in the period must be cost adjusted.</span><span class="sxs-lookup"><span data-stu-id="5b6dd-117">All released and finished production orders in the period must be cost adjusted.</span></span>  

  <span data-ttu-id="5b6dd-118">When you close an inventory period, an inventory period entry is created by using the number of the last item register that falls in the inventory period.</span><span class="sxs-lookup"><span data-stu-id="5b6dd-118">When you close an inventory period, an inventory period entry is created by using the number of the last item register that falls in the inventory period.</span></span> <span data-ttu-id="5b6dd-119">In addition, the time, date, and user code of the user closing the period are recorded in the inventory period entry.</span><span class="sxs-lookup"><span data-stu-id="5b6dd-119">In addition, the time, date, and user code of the user closing the period are recorded in the inventory period entry.</span></span> <span data-ttu-id="5b6dd-120">By using this information with the last item register for the previous period, you can see which inventory transactions were posted in the inventory period.</span><span class="sxs-lookup"><span data-stu-id="5b6dd-120">By using this information with the last item register for the previous period, you can see which inventory transactions were posted in the inventory period.</span></span> <span data-ttu-id="5b6dd-121">It is also possible to reopen inventory periods if you need to post in a closed period.</span><span class="sxs-lookup"><span data-stu-id="5b6dd-121">It is also possible to reopen inventory periods if you need to post in a closed period.</span></span> <span data-ttu-id="5b6dd-122">When you reopen an inventory period, an inventory period entry is created.</span><span class="sxs-lookup"><span data-stu-id="5b6dd-122">When you reopen an inventory period, an inventory period entry is created.</span></span>  

## <a name="see-also"></a><span data-ttu-id="5b6dd-123">See Also</span><span class="sxs-lookup"><span data-stu-id="5b6dd-123">See Also</span></span>  
 <span data-ttu-id="5b6dd-124">[Design Details: Inventory Costing](design-details-inventory-costing.md) [Managing Inventory Costs](finance-manage-inventory-costs.md) [Finance](finance.md)</span><span class="sxs-lookup"><span data-stu-id="5b6dd-124">[Design Details: Inventory Costing](design-details-inventory-costing.md) [Managing Inventory Costs](finance-manage-inventory-costs.md) [Finance](finance.md)</span></span>  
 [<span data-ttu-id="5b6dd-125">Working with Financials</span><span class="sxs-lookup"><span data-stu-id="5b6dd-125">Working with Financials</span></span>](ui-work-product.md)

