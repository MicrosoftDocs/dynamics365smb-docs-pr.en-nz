---
title: Create New Value Entries for Items in the Inventory| Microsoft Docs
description: Describes how to appreciate or depreciate the value entries of one or more items in the inventory by posting their current, calculated value.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: costing, inventory cost, value entries
ms.date: 08/07/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: 8460dac8478fa101a255d93110578fa9ea20516f
ms.contentlocale: en-nz
ms.lasthandoff: 01/30/2018

---
# <a name="revalue-inventory"></a><span data-ttu-id="0fb50-103">Revalue Inventory</span><span class="sxs-lookup"><span data-stu-id="0fb50-103">Revalue Inventory</span></span>
<span data-ttu-id="0fb50-104">If you want to appreciate or depreciate an item or a specific item ledger entry, you must use the revaluation journal.</span><span class="sxs-lookup"><span data-stu-id="0fb50-104">If you want to appreciate or depreciate an item or a specific item ledger entry, you must use the revaluation journal.</span></span>

## <a name="to-revalue-inventory"></a><span data-ttu-id="0fb50-105">To revalue inventory</span><span class="sxs-lookup"><span data-stu-id="0fb50-105">To revalue inventory</span></span>
1. <span data-ttu-id="0fb50-106">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Revaluation Journal**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="0fb50-106">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Revaluation Journal**, and then choose the related link.</span></span>
2. <span data-ttu-id="0fb50-107">Choose the **Calculate Inventory Value** action.</span><span class="sxs-lookup"><span data-stu-id="0fb50-107">Choose the **Calculate Inventory Value** action.</span></span>
3. <span data-ttu-id="0fb50-108">In the **Calculate Inventory Value** window, fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="0fb50-108">In the **Calculate Inventory Value** window, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4. <span data-ttu-id="0fb50-109">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="0fb50-109">Choose the **OK** button.</span></span>
5. <span data-ttu-id="0fb50-110">On each line in the **Revaluation Journal** window, in the **Unit Cost (Revalued)** field, enter the new unit cost.</span><span class="sxs-lookup"><span data-stu-id="0fb50-110">On each line in the **Revaluation Journal** window, in the **Unit Cost (Revalued)** field, enter the new unit cost.</span></span> <span data-ttu-id="0fb50-111">Alternatively, enter the new total amount in the **Inventory Value (Revalued)** field.</span><span class="sxs-lookup"><span data-stu-id="0fb50-111">Alternatively, enter the new total amount in the **Inventory Value (Revalued)** field.</span></span>

    <span data-ttu-id="0fb50-112">The relevant fields are automatically updated.</span><span class="sxs-lookup"><span data-stu-id="0fb50-112">The relevant fields are automatically updated.</span></span> <span data-ttu-id="0fb50-113">Note that the **Amount** field shows the actual change in inventory value for the selected item ledger entry.</span><span class="sxs-lookup"><span data-stu-id="0fb50-113">Note that the **Amount** field shows the actual change in inventory value for the selected item ledger entry.</span></span> <span data-ttu-id="0fb50-114">It calculates the difference between the **Inventory Value (Calculated)** field and the **Inventory Value (Revalued)** field.</span><span class="sxs-lookup"><span data-stu-id="0fb50-114">It calculates the difference between the **Inventory Value (Calculated)** field and the **Inventory Value (Revalued)** field.</span></span>
6. <span data-ttu-id="0fb50-115">When you have completed all lines in the revaluation journal, choose the **Post** action.</span><span class="sxs-lookup"><span data-stu-id="0fb50-115">When you have completed all lines in the revaluation journal, choose the **Post** action.</span></span>

<span data-ttu-id="0fb50-116">New value entries are now created to reflect the revaluations that you have posted.</span><span class="sxs-lookup"><span data-stu-id="0fb50-116">New value entries are now created to reflect the revaluations that you have posted.</span></span> <span data-ttu-id="0fb50-117">You can see the new values on the respective item cards.</span><span class="sxs-lookup"><span data-stu-id="0fb50-117">You can see the new values on the respective item cards.</span></span>

## <a name="see-also"></a><span data-ttu-id="0fb50-118">See Also</span><span class="sxs-lookup"><span data-stu-id="0fb50-118">See Also</span></span>
[<span data-ttu-id="0fb50-119">Design Details: Revaluation</span><span class="sxs-lookup"><span data-stu-id="0fb50-119">Design Details: Revaluation</span></span>](design-details-revaluation.md)  
[<span data-ttu-id="0fb50-120">Inventory</span><span class="sxs-lookup"><span data-stu-id="0fb50-120">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="0fb50-121">Sales</span><span class="sxs-lookup"><span data-stu-id="0fb50-121">Sales</span></span>](sales-manage-sales.md)  
[<span data-ttu-id="0fb50-122">Purchasing</span><span class="sxs-lookup"><span data-stu-id="0fb50-122">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="0fb50-123">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="0fb50-123">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

