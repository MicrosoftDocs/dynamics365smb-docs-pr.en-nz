---
title: How to Close Open Item Ledger Entries Resulting from Fixed Application in the Item Journal | Microsoft Docs
description: You can use the **Applies-from Entry** field on the **Item Journal** page to create a fixed application between an inbound transaction and the original outbound transaction. For example, to correct the outbound transaction or to process its return.
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
ms.openlocfilehash: 7f10b936ffbfcf1a4aa241cf58879560806254ec
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 04/29/2019
ms.locfileid: "1242047"
---
# <a name="close-open-item-ledger-entries-resulting-from-fixed-application-in-the-item-journal"></a><span data-ttu-id="be4e5-104">Close Open Item Ledger Entries Resulting from Fixed Application in the Item Journal</span><span class="sxs-lookup"><span data-stu-id="be4e5-104">Close Open Item Ledger Entries Resulting from Fixed Application in the Item Journal</span></span>
<span data-ttu-id="be4e5-105">You can use the **Applies-from Entry** field on the **Item Journal** page to create a fixed application between an inbound transaction and the original outbound transaction.</span><span class="sxs-lookup"><span data-stu-id="be4e5-105">You can use the **Applies-from Entry** field on the **Item Journal** page to create a fixed application between an inbound transaction and the original outbound transaction.</span></span> <span data-ttu-id="be4e5-106">For example, to correct the outbound transaction or to process its return.</span><span class="sxs-lookup"><span data-stu-id="be4e5-106">For example, to correct the outbound transaction or to process its return.</span></span> <span data-ttu-id="be4e5-107">For more information, see Applies-from Entry.</span><span class="sxs-lookup"><span data-stu-id="be4e5-107">For more information, see Applies-from Entry.</span></span>  

> [!IMPORTANT]  
>  <span data-ttu-id="be4e5-108">Fixed applications made in this manner only apply the cost, not the quantity.</span><span class="sxs-lookup"><span data-stu-id="be4e5-108">Fixed applications made in this manner only apply the cost, not the quantity.</span></span> <span data-ttu-id="be4e5-109">Accordingly, the posted positive item ledger entry will not close the applied outbound entry and will itself remain open.</span><span class="sxs-lookup"><span data-stu-id="be4e5-109">Accordingly, the posted positive item ledger entry will not close the applied outbound entry and will itself remain open.</span></span> <span data-ttu-id="be4e5-110">This also applies when you post a fixed application for a positive entry to a negative entry that has not been closed by a regular positive entry, then both the negative and the positive entries will remain open.</span><span class="sxs-lookup"><span data-stu-id="be4e5-110">This also applies when you post a fixed application for a positive entry to a negative entry that has not been closed by a regular positive entry, then both the negative and the positive entries will remain open.</span></span>  
>   
>  <span data-ttu-id="be4e5-111">This also means that you cannot close an inventory period if such an entry exists.</span><span class="sxs-lookup"><span data-stu-id="be4e5-111">This also means that you cannot close an inventory period if such an entry exists.</span></span>  

<span data-ttu-id="be4e5-112">The following procedure shows how to close such entries by performing two corrective postings in the item journal.</span><span class="sxs-lookup"><span data-stu-id="be4e5-112">The following procedure shows how to close such entries by performing two corrective postings in the item journal.</span></span>  

## <a name="to-close-open-item-ledger-entries-that-result-from-a-fixed-application-in-the-item-journal"></a><span data-ttu-id="be4e5-113">To close open item ledger entries that result from a fixed application in the item journal</span><span class="sxs-lookup"><span data-stu-id="be4e5-113">To close open item ledger entries that result from a fixed application in the item journal</span></span>  

1.  <span data-ttu-id="be4e5-114">Use the **Applies-from Entry** field to post a positive adjustment with the corresponding quantity.</span><span class="sxs-lookup"><span data-stu-id="be4e5-114">Use the **Applies-from Entry** field to post a positive adjustment with the corresponding quantity.</span></span> <span data-ttu-id="be4e5-115">This closes the original negative entry with a fixed application.</span><span class="sxs-lookup"><span data-stu-id="be4e5-115">This closes the original negative entry with a fixed application.</span></span>  
2.  <span data-ttu-id="be4e5-116">Use the **Applies-to Entry** field to post a negative adjustment.</span><span class="sxs-lookup"><span data-stu-id="be4e5-116">Use the **Applies-to Entry** field to post a negative adjustment.</span></span> <span data-ttu-id="be4e5-117">This closes the original corrective positive entry with a fixed application.</span><span class="sxs-lookup"><span data-stu-id="be4e5-117">This closes the original corrective positive entry with a fixed application.</span></span>  

## <a name="see-also"></a><span data-ttu-id="be4e5-118">See Also</span><span class="sxs-lookup"><span data-stu-id="be4e5-118">See Also</span></span>  
[<span data-ttu-id="be4e5-119"> Remove and Reapply Item Ledger Entries</span><span class="sxs-lookup"><span data-stu-id="be4e5-119"> Remove and Reapply Item Ledger Entries</span></span>](finance-how-to-remove-and-reapply-item-entries.md)  
 <span data-ttu-id="be4e5-120">[Process Sales Returns and Cancellations](sales-how-process-sales-returns-cancellations.md) </span><span class="sxs-lookup"><span data-stu-id="be4e5-120">[Process Sales Returns and Cancellations](sales-how-process-sales-returns-cancellations.md) </span></span>  
 <span data-ttu-id="be4e5-121">[Setting Up Inventory Valuation and Costing](finance-set-up-inventory-valuation-and-costing.md) </span><span class="sxs-lookup"><span data-stu-id="be4e5-121">[Setting Up Inventory Valuation and Costing](finance-set-up-inventory-valuation-and-costing.md) </span></span>  
 <span data-ttu-id="be4e5-122">[Managing Inventory Costs](finance-manage-inventory-costs.md) </span><span class="sxs-lookup"><span data-stu-id="be4e5-122">[Managing Inventory Costs](finance-manage-inventory-costs.md) </span></span>  
 [<span data-ttu-id="be4e5-123">Design Details: Costing Methods</span><span class="sxs-lookup"><span data-stu-id="be4e5-123">Design Details: Costing Methods</span></span>](design-details-costing-methods.md)
