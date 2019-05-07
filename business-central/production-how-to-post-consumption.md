---
title: How to Batch Post Consumption | Microsoft Docs
description: If the flushing method is **Manual**, you must post the components manually, using a consumption journal.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2019
ms.author: sgroespe
ms.openlocfilehash: 121dec9b91d0dd5215d9953e50154873a5ae2402
ms.sourcegitcommit: bd78a5d990c9e83174da1409076c22df8b35eafd
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 03/31/2019
ms.locfileid: "921356"
---
# <a name="batch-post-production-consumption"></a><span data-ttu-id="e7186-103">Batch Post Production Consumption</span><span class="sxs-lookup"><span data-stu-id="e7186-103">Batch Post Production Consumption</span></span>
<span data-ttu-id="e7186-104">If the flushing method is **Manual**, you must post the components manually, using a consumption journal.</span><span class="sxs-lookup"><span data-stu-id="e7186-104">If the flushing method is **Manual**, you must post the components manually, using a consumption journal.</span></span>

<span data-ttu-id="e7186-105">You can also set the system up to automatically post (*flush*) components when you start or finish production orders.</span><span class="sxs-lookup"><span data-stu-id="e7186-105">You can also set the system up to automatically post (*flush*) components when you start or finish production orders.</span></span> <span data-ttu-id="e7186-106">For more information, see [Enable Flushing of Components According to Operation Output](production-how-to-flush-components-according-to-operation-output.md).</span><span class="sxs-lookup"><span data-stu-id="e7186-106">For more information, see [Enable Flushing of Components According to Operation Output](production-how-to-flush-components-according-to-operation-output.md).</span></span>

## <a name="to-post-consumption-for-one-or-more-production-order-lines"></a><span data-ttu-id="e7186-107">To post consumption for one or more production order lines</span><span class="sxs-lookup"><span data-stu-id="e7186-107">To post consumption for one or more production order lines</span></span>  
1.  <span data-ttu-id="e7186-108">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Consumption Journal**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="e7186-108">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Consumption Journal**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="e7186-109">Fill in the fields with the production order data and the consumption data.</span><span class="sxs-lookup"><span data-stu-id="e7186-109">Fill in the fields with the production order data and the consumption data.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

    <span data-ttu-id="e7186-110">If the warehouse location where the components are stored is set up to use bins but does not require pick processing, assign a bin code to the journal line to indicate where the items should be taken from in the warehouse.</span><span class="sxs-lookup"><span data-stu-id="e7186-110">If the warehouse location where the components are stored is set up to use bins but does not require pick processing, assign a bin code to the journal line to indicate where the items should be taken from in the warehouse.</span></span> <span data-ttu-id="e7186-111">For more information, see [Pick for Production or Assembly](warehouse-how-to-pick-for-production.md).</span><span class="sxs-lookup"><span data-stu-id="e7186-111">For more information, see [Pick for Production or Assembly](warehouse-how-to-pick-for-production.md).</span></span>  
3.  <span data-ttu-id="e7186-112">Choose the **Post** action to post the consumption.</span><span class="sxs-lookup"><span data-stu-id="e7186-112">Choose the **Post** action to post the consumption.</span></span> <span data-ttu-id="e7186-113">The related item ledger entries are reduced.</span><span class="sxs-lookup"><span data-stu-id="e7186-113">The related item ledger entries are reduced.</span></span>

## <a name="see-also"></a><span data-ttu-id="e7186-114">See Also</span><span class="sxs-lookup"><span data-stu-id="e7186-114">See Also</span></span>  
<span data-ttu-id="e7186-115">[Manufacturing](production-manage-manufacturing.md)  </span><span class="sxs-lookup"><span data-stu-id="e7186-115">[Manufacturing](production-manage-manufacturing.md)  </span></span>  
[<span data-ttu-id="e7186-116">Setting Up Manufacturing</span><span class="sxs-lookup"><span data-stu-id="e7186-116">Setting Up Manufacturing</span></span>](production-configure-production-processes.md)  
<span data-ttu-id="e7186-117">[Planning](production-planning.md)    </span><span class="sxs-lookup"><span data-stu-id="e7186-117">[Planning](production-planning.md)    </span></span>  
[<span data-ttu-id="e7186-118">Inventory</span><span class="sxs-lookup"><span data-stu-id="e7186-118">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="e7186-119">Purchasing</span><span class="sxs-lookup"><span data-stu-id="e7186-119">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="e7186-120">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="e7186-120">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
