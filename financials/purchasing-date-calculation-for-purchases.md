---
title: Date Calculation for Purchases | Microsoft Docs
description: The program automatically calculates the date on which you must order an item to have it in inventory on a certain date. This is the date on which you can expect items ordered on a particular date to be available for picking.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/10/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: 7a37b1ef9e4a73faf8d04398dbc4023eb04ab9f6
ms.contentlocale: en-nz
ms.lasthandoff: 03/22/2018

---
# <a name="date-calculation-for-purchases"></a><span data-ttu-id="3e7a8-104">Date Calculation for Purchases</span><span class="sxs-lookup"><span data-stu-id="3e7a8-104">Date Calculation for Purchases</span></span>
[!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="3e7a8-105"> automatically calculates the date on which you must order an item to have it in inventory on a certain date.</span><span class="sxs-lookup"><span data-stu-id="3e7a8-105"> automatically calculates the date on which you must order an item to have it in inventory on a certain date.</span></span> <span data-ttu-id="3e7a8-106">This is the date on which you can expect items ordered on a particular date to be available for picking.</span><span class="sxs-lookup"><span data-stu-id="3e7a8-106">This is the date on which you can expect items ordered on a particular date to be available for picking.</span></span>  

<span data-ttu-id="3e7a8-107">If you specify a requested receipt date on a purchase order header, then the calculated order date is the date on which the order must be placed to receive the items on the date that you requested.</span><span class="sxs-lookup"><span data-stu-id="3e7a8-107">If you specify a requested receipt date on a purchase order header, then the calculated order date is the date on which the order must be placed to receive the items on the date that you requested.</span></span> <span data-ttu-id="3e7a8-108">Then, the date on which the items are available for picking is calculated and entered in the **Expected Receipt Date** field.</span><span class="sxs-lookup"><span data-stu-id="3e7a8-108">Then, the date on which the items are available for picking is calculated and entered in the **Expected Receipt Date** field.</span></span>  

<span data-ttu-id="3e7a8-109">If you do not specify a requested receipt date, then the order date on the line is used as the starting point for calculating the date on which you can expect to receive the items and the date on which the items are available for picking.</span><span class="sxs-lookup"><span data-stu-id="3e7a8-109">If you do not specify a requested receipt date, then the order date on the line is used as the starting point for calculating the date on which you can expect to receive the items and the date on which the items are available for picking.</span></span>  

## <a name="calculating-with-a-requested-receipt-date"></a><span data-ttu-id="3e7a8-110">Calculating with a Requested Receipt Date</span><span class="sxs-lookup"><span data-stu-id="3e7a8-110">Calculating with a Requested Receipt Date</span></span>  
<span data-ttu-id="3e7a8-111">If there is a requested receipt date on the purchase order line, then that date is used as the starting point for the following calculations.</span><span class="sxs-lookup"><span data-stu-id="3e7a8-111">If there is a requested receipt date on the purchase order line, then that date is used as the starting point for the following calculations.</span></span>  

- <span data-ttu-id="3e7a8-112">requested receipt date - lead time calculation = order date</span><span class="sxs-lookup"><span data-stu-id="3e7a8-112">requested receipt date - lead time calculation = order date</span></span>  
- <span data-ttu-id="3e7a8-113">requested receipt date + inbound whse. handling time + safety lead time = expected receipt date</span><span class="sxs-lookup"><span data-stu-id="3e7a8-113">requested receipt date + inbound whse. handling time + safety lead time = expected receipt date</span></span>  

<span data-ttu-id="3e7a8-114">If you entered a requested receipt date on the purchase order header, then that date is copied to the corresponding field on all the lines.</span><span class="sxs-lookup"><span data-stu-id="3e7a8-114">If you entered a requested receipt date on the purchase order header, then that date is copied to the corresponding field on all the lines.</span></span> <span data-ttu-id="3e7a8-115">You can change this date on any of the lines, or you can remove the date on the line.</span><span class="sxs-lookup"><span data-stu-id="3e7a8-115">You can change this date on any of the lines, or you can remove the date on the line.</span></span>  

## <a name="calculating-without-a-requested-delivery-date"></a><span data-ttu-id="3e7a8-116">Calculating without a Requested Delivery Date</span><span class="sxs-lookup"><span data-stu-id="3e7a8-116">Calculating without a Requested Delivery Date</span></span>  
<span data-ttu-id="3e7a8-117">If you enter a purchase order line without a requested delivery date, then the **Order Date** field on the line is filled with the date in the **Order Date** field on the purchase order header.</span><span class="sxs-lookup"><span data-stu-id="3e7a8-117">If you enter a purchase order line without a requested delivery date, then the **Order Date** field on the line is filled with the date in the **Order Date** field on the purchase order header.</span></span> <span data-ttu-id="3e7a8-118">This is either the date that you entered or the work date.</span><span class="sxs-lookup"><span data-stu-id="3e7a8-118">This is either the date that you entered or the work date.</span></span> <span data-ttu-id="3e7a8-119">The following dates are then calculated for the purchase order line, with the order date as the starting point.</span><span class="sxs-lookup"><span data-stu-id="3e7a8-119">The following dates are then calculated for the purchase order line, with the order date as the starting point.</span></span>  

- <span data-ttu-id="3e7a8-120">order date + lead time calculation = planned receipt date</span><span class="sxs-lookup"><span data-stu-id="3e7a8-120">order date + lead time calculation = planned receipt date</span></span>  
- <span data-ttu-id="3e7a8-121">planned receipt date + inbound whse. handling time + safety lead time = expected receipt date</span><span class="sxs-lookup"><span data-stu-id="3e7a8-121">planned receipt date + inbound whse. handling time + safety lead time = expected receipt date</span></span>  

<span data-ttu-id="3e7a8-122">If you change the order date on the line, such as when items are not available at your vendor until a later date, then the relevant dates on the line are automatically recalculated.</span><span class="sxs-lookup"><span data-stu-id="3e7a8-122">If you change the order date on the line, such as when items are not available at your vendor until a later date, then the relevant dates on the line are automatically recalculated.</span></span>  

<span data-ttu-id="3e7a8-123">If you change the order date on the header, then that date is copied to the **Order Date** field on all the lines, and all the related date fields are then recalculated.</span><span class="sxs-lookup"><span data-stu-id="3e7a8-123">If you change the order date on the header, then that date is copied to the **Order Date** field on all the lines, and all the related date fields are then recalculated.</span></span>  

## <a name="see-also"></a><span data-ttu-id="3e7a8-124">See Also</span><span class="sxs-lookup"><span data-stu-id="3e7a8-124">See Also</span></span>  
 <span data-ttu-id="3e7a8-125">[Date Calculation for Sales](sales-date-calculation-for-sales.md) </span><span class="sxs-lookup"><span data-stu-id="3e7a8-125">[Date Calculation for Sales](sales-date-calculation-for-sales.md) </span></span>  
 [<span data-ttu-id="3e7a8-126">Calculate Order Promising Dates</span><span class="sxs-lookup"><span data-stu-id="3e7a8-126">Calculate Order Promising Dates</span></span>](sales-how-to-calculate-order-promising-dates.md)  
 <span data-ttu-id="3e7a8-127">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="3e7a8-127">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

