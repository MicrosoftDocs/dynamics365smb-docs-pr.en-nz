---
title: Date Calculation for Sales | Microsoft Docs
description: The application automatically calculates the date on which you must order an item to have it in inventory on a certain date. This is the date on which you can expect items ordered on a particular date to be available for picking.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 26782d211d205bb5414c5bd423ccf240f70f197e
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 12/17/2020
ms.locfileid: "4748484"
---
# <a name="date-calculation-for-sales"></a><span data-ttu-id="dadd2-104">Date Calculation for Sales</span><span class="sxs-lookup"><span data-stu-id="dadd2-104">Date Calculation for Sales</span></span>
[!INCLUDE[prod_short](includes/prod_short.md)] <span data-ttu-id="dadd2-105">automatically calculates the earliest possible date that an item on a sales order line can be shipped.</span><span class="sxs-lookup"><span data-stu-id="dadd2-105">automatically calculates the earliest possible date that an item on a sales order line can be shipped.</span></span>

<span data-ttu-id="dadd2-106">If the customer has requested a specific delivery date, then the date on which the items must be available to pick to meet that delivery date is calculated.</span><span class="sxs-lookup"><span data-stu-id="dadd2-106">If the customer has requested a specific delivery date, then the date on which the items must be available to pick to meet that delivery date is calculated.</span></span>

<span data-ttu-id="dadd2-107">If the customer does not request a specific delivery date, then the date on which the items can be delivered is calculated, starting from the date on which the items are available for picking.</span><span class="sxs-lookup"><span data-stu-id="dadd2-107">If the customer does not request a specific delivery date, then the date on which the items can be delivered is calculated, starting from the date on which the items are available for picking.</span></span>

## <a name="calculating-a-requested-delivery-date"></a><span data-ttu-id="dadd2-108">Calculating a Requested Delivery Date</span><span class="sxs-lookup"><span data-stu-id="dadd2-108">Calculating a Requested Delivery Date</span></span>
<span data-ttu-id="dadd2-109">If you specify a requested delivery date on the sales order line, that date becomes the starting point for the following calculations.</span><span class="sxs-lookup"><span data-stu-id="dadd2-109">If you specify a requested delivery date on the sales order line, that date becomes the starting point for the following calculations.</span></span>

- <span data-ttu-id="dadd2-110">requested delivery date - shipping time = planned shipment date</span><span class="sxs-lookup"><span data-stu-id="dadd2-110">requested delivery date - shipping time = planned shipment date</span></span>
- <span data-ttu-id="dadd2-111">planned shipment date - outbound whse. handling time = shipment date</span><span class="sxs-lookup"><span data-stu-id="dadd2-111">planned shipment date - outbound whse. handling time = shipment date</span></span>

<span data-ttu-id="dadd2-112">If the items are available to pick on the shipment date, then the sales process can continue.</span><span class="sxs-lookup"><span data-stu-id="dadd2-112">If the items are available to pick on the shipment date, then the sales process can continue.</span></span> <span data-ttu-id="dadd2-113">Otherwise, a stock-out warning is displayed.</span><span class="sxs-lookup"><span data-stu-id="dadd2-113">Otherwise, a stock-out warning is displayed.</span></span>

> [!Note]
> <span data-ttu-id="dadd2-114">If your process is based on backward calculation, for example, if you use the requested delivery date to get the planned shipment date, we recommend that you use date formulas that have fixed durations, such as "5D" for five days or "1W" for one week.</span><span class="sxs-lookup"><span data-stu-id="dadd2-114">If your process is based on backward calculation, for example, if you use the requested delivery date to get the planned shipment date, we recommend that you use date formulas that have fixed durations, such as "5D" for five days or "1W" for one week.</span></span> <span data-ttu-id="dadd2-115">Date formulas without fixed durations, such as "CW" for current week or CM for current month, can result in incorrect date calculations.</span><span class="sxs-lookup"><span data-stu-id="dadd2-115">Date formulas without fixed durations, such as "CW" for current week or CM for current month, can result in incorrect date calculations.</span></span> <span data-ttu-id="dadd2-116">For more information about date formulas, see [Working with Calendar Dates and Times](ui-enter-date-ranges.md).</span><span class="sxs-lookup"><span data-stu-id="dadd2-116">For more information about date formulas, see [Working with Calendar Dates and Times](ui-enter-date-ranges.md).</span></span>

## <a name="calculating-the-earliest-possible-delivery-date"></a><span data-ttu-id="dadd2-117">Calculating the Earliest Possible Delivery Date</span><span class="sxs-lookup"><span data-stu-id="dadd2-117">Calculating the Earliest Possible Delivery Date</span></span>
<span data-ttu-id="dadd2-118">If you do not specify a requested delivery date on the sales order line, or if the requested delivery date cannot be met, then the earliest date on which that the items are available is calculated.</span><span class="sxs-lookup"><span data-stu-id="dadd2-118">If you do not specify a requested delivery date on the sales order line, or if the requested delivery date cannot be met, then the earliest date on which that the items are available is calculated.</span></span> <span data-ttu-id="dadd2-119">That date is then entered in the Shipment Date field on the line, and the date on which you plan to ship the items as well as the date on which they will be delivered to the customer are calculated using the following formulas.</span><span class="sxs-lookup"><span data-stu-id="dadd2-119">That date is then entered in the Shipment Date field on the line, and the date on which you plan to ship the items as well as the date on which they will be delivered to the customer are calculated using the following formulas.</span></span>

- <span data-ttu-id="dadd2-120">shipment date + outbound whse. handling time = planned shipment date</span><span class="sxs-lookup"><span data-stu-id="dadd2-120">shipment date + outbound whse. handling time = planned shipment date</span></span>
- <span data-ttu-id="dadd2-121">planned shipment date + shipping time = planned delivery date</span><span class="sxs-lookup"><span data-stu-id="dadd2-121">planned shipment date + shipping time = planned delivery date</span></span>


## <a name="see-also"></a><span data-ttu-id="dadd2-122">See Also</span><span class="sxs-lookup"><span data-stu-id="dadd2-122">See Also</span></span>  
 <span data-ttu-id="dadd2-123">[Date Calculation for Purchases](purchasing-date-calculation-for-purchases.md) </span><span class="sxs-lookup"><span data-stu-id="dadd2-123">[Date Calculation for Purchases](purchasing-date-calculation-for-purchases.md) </span></span>  
 [<span data-ttu-id="dadd2-124">Calculate Order Promising Dates</span><span class="sxs-lookup"><span data-stu-id="dadd2-124">Calculate Order Promising Dates</span></span>](sales-how-to-calculate-order-promising-dates.md)  
 <span data-ttu-id="dadd2-125">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="dadd2-125">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>
