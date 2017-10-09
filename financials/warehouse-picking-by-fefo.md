---
title: How to Enable Picking by FEFO | Microsoft Docs
description: First-Expired-First-Out (FEFO) is a sorting method that ensures that the oldest items, those with the earliest expiration dates, are picked first.
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
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 34d6e46146f3072da49cd28e4b4bf1b0f00d1369
ms.contentlocale: en-nz
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-enable-picking-items-by-fefo"></a><span data-ttu-id="fccba-103">How to: Enable Picking Items by FEFO</span><span class="sxs-lookup"><span data-stu-id="fccba-103">How to: Enable Picking Items by FEFO</span></span>
<span data-ttu-id="fccba-104">First-Expired-First-Out (FEFO) is a sorting method that ensures that the oldest items, those with the earliest expiration dates, are picked first.</span><span class="sxs-lookup"><span data-stu-id="fccba-104">First-Expired-First-Out (FEFO) is a sorting method that ensures that the oldest items, those with the earliest expiration dates, are picked first.</span></span>  

 <span data-ttu-id="fccba-105">This functionality only works when the following criteria are met:</span><span class="sxs-lookup"><span data-stu-id="fccba-105">This functionality only works when the following criteria are met:</span></span>  

-   <span data-ttu-id="fccba-106">The item must have a serial/lot number.</span><span class="sxs-lookup"><span data-stu-id="fccba-106">The item must have a serial/lot number.</span></span>  
-   <span data-ttu-id="fccba-107">On the item’s item tracking code setup, the **SN-Specific Warehouse Tracking** field or the **Lot-Specific Warehouse Tracking** field must be selected.</span><span class="sxs-lookup"><span data-stu-id="fccba-107">On the item’s item tracking code setup, the **SN-Specific Warehouse Tracking** field or the **Lot-Specific Warehouse Tracking** field must be selected.</span></span>  
-   <span data-ttu-id="fccba-108">The item must be posted to inventory with an expiration date.</span><span class="sxs-lookup"><span data-stu-id="fccba-108">The item must be posted to inventory with an expiration date.</span></span>  
-   <span data-ttu-id="fccba-109">On the location card, the **Require Pick** check box must be selected.</span><span class="sxs-lookup"><span data-stu-id="fccba-109">On the location card, the **Require Pick** check box must be selected.</span></span>  
-   <span data-ttu-id="fccba-110">On the location card, the **Pick According to FEFO** check box must be selected.</span><span class="sxs-lookup"><span data-stu-id="fccba-110">On the location card, the **Pick According to FEFO** check box must be selected.</span></span>  
-   <span data-ttu-id="fccba-111">On the location card, the **Bin Mandatory** check box must be selected.</span><span class="sxs-lookup"><span data-stu-id="fccba-111">On the location card, the **Bin Mandatory** check box must be selected.</span></span>  

 <span data-ttu-id="fccba-112">When all the criteria are met, then serial/lot-numbered items to be picked are sorted with the oldest first in all picks and movements, except for items that use SN-specific or lot-specific tracking.</span><span class="sxs-lookup"><span data-stu-id="fccba-112">When all the criteria are met, then serial/lot-numbered items to be picked are sorted with the oldest first in all picks and movements, except for items that use SN-specific or lot-specific tracking.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="fccba-113">If some serial/lot-numbered items use specific tracking, then those are respected first and under them, the remaining, non-specific, serial/lot numbers are listed according to FEFO.</span><span class="sxs-lookup"><span data-stu-id="fccba-113">If some serial/lot-numbered items use specific tracking, then those are respected first and under them, the remaining, non-specific, serial/lot numbers are listed according to FEFO.</span></span>  

 <span data-ttu-id="fccba-114">If two serial/lot-numbered items have the same expiration date, then the program selects the item with the lowest serial or lot number.</span><span class="sxs-lookup"><span data-stu-id="fccba-114">If two serial/lot-numbered items have the same expiration date, then the program selects the item with the lowest serial or lot number.</span></span> <span data-ttu-id="fccba-115">If the serial or lot numbers are the same, then the program selects the item that was registered first.</span><span class="sxs-lookup"><span data-stu-id="fccba-115">If the serial or lot numbers are the same, then the program selects the item that was registered first.</span></span>  

> [!NOTE]  
>  -   <span data-ttu-id="fccba-116">When picking serial/lot-numbered items in locations set up for directed put-away and pick, only quantities on bins of type *Pick* are picked according to FEFO.</span><span class="sxs-lookup"><span data-stu-id="fccba-116">When picking serial/lot-numbered items in locations set up for directed put-away and pick, only quantities on bins of type *Pick* are picked according to FEFO.</span></span>  
> -   <span data-ttu-id="fccba-117">To enable movements according to FEFO, either in the **Inventory Movement** window or the **Movement Worksheet** window, you must leave the **From Bin** field empty.</span><span class="sxs-lookup"><span data-stu-id="fccba-117">To enable movements according to FEFO, either in the **Inventory Movement** window or the **Movement Worksheet** window, you must leave the **From Bin** field empty.</span></span>  
> -   <span data-ttu-id="fccba-118">If the **Strict Expiration Posting** field is selected, then only items that are not expired will be included in the pick.</span><span class="sxs-lookup"><span data-stu-id="fccba-118">If the **Strict Expiration Posting** field is selected, then only items that are not expired will be included in the pick.</span></span> <span data-ttu-id="fccba-119">This applies even if you are not using Pick according to FEFO.</span><span class="sxs-lookup"><span data-stu-id="fccba-119">This applies even if you are not using Pick according to FEFO.</span></span>  

## <a name="see-also"></a><span data-ttu-id="fccba-120">See Also</span><span class="sxs-lookup"><span data-stu-id="fccba-120">See Also</span></span>  
<span data-ttu-id="fccba-121">[Picking Items](warehouse-pick-items.md) </span><span class="sxs-lookup"><span data-stu-id="fccba-121">[Picking Items](warehouse-pick-items.md) </span></span>  
<span data-ttu-id="fccba-122">[How to: Pick Items for Warehouse Shipment](warehouse-how-to-pick-items-for-warehouse-shipment.md) </span><span class="sxs-lookup"><span data-stu-id="fccba-122">[How to: Pick Items for Warehouse Shipment](warehouse-how-to-pick-items-for-warehouse-shipment.md) </span></span>  
<span data-ttu-id="fccba-123">[How to: Pick Items with Inventory Picks](warehouse-how-to-pick-items-with-inventory-picks.md) </span><span class="sxs-lookup"><span data-stu-id="fccba-123">[How to: Pick Items with Inventory Picks](warehouse-how-to-pick-items-with-inventory-picks.md) </span></span>  
[<span data-ttu-id="fccba-124">Design Details: Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="fccba-124">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
[<span data-ttu-id="fccba-125">Inventory</span><span class="sxs-lookup"><span data-stu-id="fccba-125">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="fccba-126">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="fccba-126">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

