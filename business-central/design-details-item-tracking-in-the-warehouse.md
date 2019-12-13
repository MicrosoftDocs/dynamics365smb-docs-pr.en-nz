---
title: Design Details - Item Tracking in the Warehouse | Microsoft Docs
description: Serial number and lot number handling is primarily a warehouse task and therefore all inbound and outbound warehouse documents have standard functionality for assigning and selecting item tracking numbers. However, because the reservation system is based on item ledger entries, warehouse activity documents that register only warehouse entries are not fully supported.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: design, item, tracking, serial number, lot number, outbound documents
ms.date: 10/01/2019
ms.author: sgroespe
ms.openlocfilehash: b7fdb0d6495f1512e1ab3bf80eb76a5dad9d87e5
ms.sourcegitcommit: cfc92eefa8b06fb426482f54e393f0e6e222f712
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 12/03/2019
ms.locfileid: "2880200"
---
# <a name="design-details-item-tracking-in-the-warehouse"></a><span data-ttu-id="47920-104">Design Details: Item Tracking in the Warehouse</span><span class="sxs-lookup"><span data-stu-id="47920-104">Design Details: Item Tracking in the Warehouse</span></span>
<span data-ttu-id="47920-105">Serial number and lot number handling is primarily a warehouse task and therefore all inbound and outbound warehouse documents have standard functionality for assigning and selecting item tracking numbers.</span><span class="sxs-lookup"><span data-stu-id="47920-105">Serial number and lot number handling is primarily a warehouse task and therefore all inbound and outbound warehouse documents have standard functionality for assigning and selecting item tracking numbers.</span></span>  

<span data-ttu-id="47920-106">However, because the reservation system is based on item ledger entries, warehouse activity documents that register only warehouse entries are not fully supported.</span><span class="sxs-lookup"><span data-stu-id="47920-106">However, because the reservation system is based on item ledger entries, warehouse activity documents that register only warehouse entries are not fully supported.</span></span> <span data-ttu-id="47920-107">Because reservations and item tracking numbers can be handled only at the location level, not at the bin and zone level, the **Item Tracking Lines** page cannot be opened from warehouse activity documents.</span><span class="sxs-lookup"><span data-stu-id="47920-107">Because reservations and item tracking numbers can be handled only at the location level, not at the bin and zone level, the **Item Tracking Lines** page cannot be opened from warehouse activity documents.</span></span> <span data-ttu-id="47920-108">The same applies to the **Reservation** page.</span><span class="sxs-lookup"><span data-stu-id="47920-108">The same applies to the **Reservation** page.</span></span>  

<span data-ttu-id="47920-109">After a serial or lot number has been added to an item at a warehouse location, it can be moved and reclassified freely within the warehouse by using an independent item tracking structure that is unrelated to the reservation system.</span><span class="sxs-lookup"><span data-stu-id="47920-109">After a serial or lot number has been added to an item at a warehouse location, it can be moved and reclassified freely within the warehouse by using an independent item tracking structure that is unrelated to the reservation system.</span></span> <span data-ttu-id="47920-110">**Serial No.** and **Lot No.** fields are accessed directly on warehouse document lines.</span><span class="sxs-lookup"><span data-stu-id="47920-110">**Serial No.** and **Lot No.** fields are accessed directly on warehouse document lines.</span></span> <span data-ttu-id="47920-111">When the serial or lot number later partakes in outbound posting, it is synchronised with the reservation system as a part of ordinary bin adjustment.</span><span class="sxs-lookup"><span data-stu-id="47920-111">When the serial or lot number later partakes in outbound posting, it is synchronized with the reservation system as a part of ordinary bin adjustment.</span></span> <span data-ttu-id="47920-112">For more information, see [Design Details: Integration with Inventory](design-details-integration-with-inventory.md).</span><span class="sxs-lookup"><span data-stu-id="47920-112">For more information, see [Design Details: Integration with Inventory](design-details-integration-with-inventory.md).</span></span>  

<span data-ttu-id="47920-113">However, the reservation system does take warehouse activities into consideration when it calculates availability.</span><span class="sxs-lookup"><span data-stu-id="47920-113">However, the reservation system does take warehouse activities into consideration when it calculates availability.</span></span> <span data-ttu-id="47920-114">For example, items that are allocated to picks, or registered as picked, cannot be reserved.</span><span class="sxs-lookup"><span data-stu-id="47920-114">For example, items that are allocated to picks, or registered as picked, cannot be reserved.</span></span> <span data-ttu-id="47920-115">For more information, see [Design Details: Warehouse Availability](design-details-availability-in-the-warehouse.md).</span><span class="sxs-lookup"><span data-stu-id="47920-115">For more information, see [Design Details: Warehouse Availability](design-details-availability-in-the-warehouse.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="47920-116">See Also</span><span class="sxs-lookup"><span data-stu-id="47920-116">See Also</span></span>  
[<span data-ttu-id="47920-117">Design Details: Item Tracking</span><span class="sxs-lookup"><span data-stu-id="47920-117">Design Details: Item Tracking</span></span>](design-details-item-tracking.md)  
[<span data-ttu-id="47920-118">Design Details: Integration with Inventory</span><span class="sxs-lookup"><span data-stu-id="47920-118">Design Details: Integration with Inventory</span></span>](design-details-integration-with-inventory.md)  
[<span data-ttu-id="47920-119">Design Details: Warehouse Availability</span><span class="sxs-lookup"><span data-stu-id="47920-119">Design Details: Warehouse Availability</span></span>](design-details-availability-in-the-warehouse.md)  
[<span data-ttu-id="47920-120">Design Details: Item Tracking Design</span><span class="sxs-lookup"><span data-stu-id="47920-120">Design Details: Item Tracking Design</span></span>](design-details-item-tracking-design.md)
