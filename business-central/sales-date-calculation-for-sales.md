---
title: Date Calculation for Sales | Microsoft Docs
description: The program automatically calculates the date on which you must order an item to have it in inventory on a certain date. This is the date on which you can expect items ordered on a particular date to be available for picking.
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
ms.openlocfilehash: a620b7ed9d06cdd8adf7b12bea2b55aecea32bcc
ms.sourcegitcommit: bd78a5d990c9e83174da1409076c22df8b35eafd
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 03/31/2019
ms.locfileid: "918927"
---
# <a name="date-calculation-for-sales"></a><span data-ttu-id="85ab4-104">Date Calculation for Sales</span><span class="sxs-lookup"><span data-stu-id="85ab4-104">Date Calculation for Sales</span></span>
[!INCLUDE[d365fin](includes/d365fin_md.md)] <span data-ttu-id="85ab4-105">automatically calculates the earliest possible date that an item on a sales order line can be shipped.</span><span class="sxs-lookup"><span data-stu-id="85ab4-105">automatically calculates the earliest possible date that an item on a sales order line can be shipped.</span></span>

<span data-ttu-id="85ab4-106">If the customer has requested a specific delivery date, then the date on which the items must be available to pick to meet that delivery date is calculated.</span><span class="sxs-lookup"><span data-stu-id="85ab4-106">If the customer has requested a specific delivery date, then the date on which the items must be available to pick to meet that delivery date is calculated.</span></span>

<span data-ttu-id="85ab4-107">If the customer does not request a specific delivery date, then the date on which the items can be delivered is calculated, starting from the date on which the items are available for picking.</span><span class="sxs-lookup"><span data-stu-id="85ab4-107">If the customer does not request a specific delivery date, then the date on which the items can be delivered is calculated, starting from the date on which the items are available for picking.</span></span>

## <a name="calculating-a-requested-delivery-date"></a><span data-ttu-id="85ab4-108">Calculating a Requested Delivery Date</span><span class="sxs-lookup"><span data-stu-id="85ab4-108">Calculating a Requested Delivery Date</span></span>
<span data-ttu-id="85ab4-109">If you specify a requested delivery date on the sales order line, then that date is used as the starting point for the following calculations.</span><span class="sxs-lookup"><span data-stu-id="85ab4-109">If you specify a requested delivery date on the sales order line, then that date is used as the starting point for the following calculations.</span></span>

- <span data-ttu-id="85ab4-110">requested delivery date - shipping time = planned shipment date</span><span class="sxs-lookup"><span data-stu-id="85ab4-110">requested delivery date - shipping time = planned shipment date</span></span>
- <span data-ttu-id="85ab4-111">planned shipment date - outbound whse. handling time = shipment date</span><span class="sxs-lookup"><span data-stu-id="85ab4-111">planned shipment date - outbound whse. handling time = shipment date</span></span>

<span data-ttu-id="85ab4-112">If the items are available to pick on the shipment date, then the sales process can continue.</span><span class="sxs-lookup"><span data-stu-id="85ab4-112">If the items are available to pick on the shipment date, then the sales process can continue.</span></span>

<span data-ttu-id="85ab4-113">If the items are not available to be picked on the shipment date, then a stock-out warning is displayed.</span><span class="sxs-lookup"><span data-stu-id="85ab4-113">If the items are not available to be picked on the shipment date, then a stock-out warning is displayed.</span></span>

## <a name="calculating-the-earliest-possible-delivery-date"></a><span data-ttu-id="85ab4-114">Calculating the Earliest Possible Delivery Date</span><span class="sxs-lookup"><span data-stu-id="85ab4-114">Calculating the Earliest Possible Delivery Date</span></span>
<span data-ttu-id="85ab4-115">If you do not specify a requested delivery date on the sales order line, or if the requested delivery date cannot be met, then the earliest date on which that the items are available is calculated.</span><span class="sxs-lookup"><span data-stu-id="85ab4-115">If you do not specify a requested delivery date on the sales order line, or if the requested delivery date cannot be met, then the earliest date on which that the items are available is calculated.</span></span> <span data-ttu-id="85ab4-116">That date is then entered in the Shipment Date field on the line, and the date on which you plan to ship the items as well as the date on which they will be delivered to the customer are calculated using the following formulas.</span><span class="sxs-lookup"><span data-stu-id="85ab4-116">That date is then entered in the Shipment Date field on the line, and the date on which you plan to ship the items as well as the date on which they will be delivered to the customer are calculated using the following formulas.</span></span>

- <span data-ttu-id="85ab4-117">shipment date + outbound whse. handling time = planned shipment date</span><span class="sxs-lookup"><span data-stu-id="85ab4-117">shipment date + outbound whse. handling time = planned shipment date</span></span>
- <span data-ttu-id="85ab4-118">planned shipment date + shipping time = planned delivery date</span><span class="sxs-lookup"><span data-stu-id="85ab4-118">planned shipment date + shipping time = planned delivery date</span></span>


## <a name="see-also"></a><span data-ttu-id="85ab4-119">See Also</span><span class="sxs-lookup"><span data-stu-id="85ab4-119">See Also</span></span>  
 <span data-ttu-id="85ab4-120">[Date Calculation for Purchases](purchasing-date-calculation-for-purchases.md) </span><span class="sxs-lookup"><span data-stu-id="85ab4-120">[Date Calculation for Purchases](purchasing-date-calculation-for-purchases.md) </span></span>  
 [<span data-ttu-id="85ab4-121">Calculate Order Promising Dates</span><span class="sxs-lookup"><span data-stu-id="85ab4-121">Calculate Order Promising Dates</span></span>](sales-how-to-calculate-order-promising-dates.md)  
 <span data-ttu-id="85ab4-122">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="85ab4-122">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
