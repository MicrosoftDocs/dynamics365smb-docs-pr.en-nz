---
title: Date Calculation for Purchases | Microsoft Docs
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
ms.date: 10/01/2018
ms.author: sgroespe
ms.openlocfilehash: 08d2f6498019b8ee0a646cec891ff897a62dc9de
ms.sourcegitcommit: 1bcfaa99ea302e6b84b8361ca02730b135557fc1
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 03/08/2019
ms.locfileid: "822566"
---
# <a name="date-calculation-for-purchases"></a><span data-ttu-id="d30fa-104">Date Calculation for Purchases</span><span class="sxs-lookup"><span data-stu-id="d30fa-104">Date Calculation for Purchases</span></span>
[!INCLUDE[d365fin](includes/d365fin_md.md)] <span data-ttu-id="d30fa-105">automatically calculates the date on which you must order an item to have it in inventory on a certain date.</span><span class="sxs-lookup"><span data-stu-id="d30fa-105">automatically calculates the date on which you must order an item to have it in inventory on a certain date.</span></span> <span data-ttu-id="d30fa-106">This is the date on which you can expect items ordered on a particular date to be available for picking.</span><span class="sxs-lookup"><span data-stu-id="d30fa-106">This is the date on which you can expect items ordered on a particular date to be available for picking.</span></span>  

<span data-ttu-id="d30fa-107">If you specify a requested receipt date on a purchase order header, then the calculated order date is the date on which the order must be placed to receive the items on the date that you requested.</span><span class="sxs-lookup"><span data-stu-id="d30fa-107">If you specify a requested receipt date on a purchase order header, then the calculated order date is the date on which the order must be placed to receive the items on the date that you requested.</span></span> <span data-ttu-id="d30fa-108">Then, the date on which the items are available for picking is calculated and entered in the **Expected Receipt Date** field.</span><span class="sxs-lookup"><span data-stu-id="d30fa-108">Then, the date on which the items are available for picking is calculated and entered in the **Expected Receipt Date** field.</span></span>  

<span data-ttu-id="d30fa-109">If you do not specify a requested receipt date, then the order date on the line is used as the starting point for calculating the date on which you can expect to receive the items and the date on which the items are available for picking.</span><span class="sxs-lookup"><span data-stu-id="d30fa-109">If you do not specify a requested receipt date, then the order date on the line is used as the starting point for calculating the date on which you can expect to receive the items and the date on which the items are available for picking.</span></span>  

## <a name="calculating-with-a-requested-receipt-date"></a><span data-ttu-id="d30fa-110">Calculating with a Requested Receipt Date</span><span class="sxs-lookup"><span data-stu-id="d30fa-110">Calculating with a Requested Receipt Date</span></span>  
<span data-ttu-id="d30fa-111">If there is a requested receipt date on the purchase order line, then that date is used as the starting point for the following calculations.</span><span class="sxs-lookup"><span data-stu-id="d30fa-111">If there is a requested receipt date on the purchase order line, then that date is used as the starting point for the following calculations.</span></span>  

- <span data-ttu-id="d30fa-112">requested receipt date - lead time calculation = order date</span><span class="sxs-lookup"><span data-stu-id="d30fa-112">requested receipt date - lead time calculation = order date</span></span>  
- <span data-ttu-id="d30fa-113">requested receipt date + inbound whse. handling time + safety lead time = expected receipt date</span><span class="sxs-lookup"><span data-stu-id="d30fa-113">requested receipt date + inbound whse. handling time + safety lead time = expected receipt date</span></span>  

<span data-ttu-id="d30fa-114">If you entered a requested receipt date on the purchase order header, then that date is copied to the corresponding field on all the lines.</span><span class="sxs-lookup"><span data-stu-id="d30fa-114">If you entered a requested receipt date on the purchase order header, then that date is copied to the corresponding field on all the lines.</span></span> <span data-ttu-id="d30fa-115">You can change this date on any of the lines, or you can remove the date on the line.</span><span class="sxs-lookup"><span data-stu-id="d30fa-115">You can change this date on any of the lines, or you can remove the date on the line.</span></span>  

## <a name="calculating-without-a-requested-delivery-date"></a><span data-ttu-id="d30fa-116">Calculating without a Requested Delivery Date</span><span class="sxs-lookup"><span data-stu-id="d30fa-116">Calculating without a Requested Delivery Date</span></span>  
<span data-ttu-id="d30fa-117">If you enter a purchase order line without a requested delivery date, then the **Order Date** field on the line is filled with the date in the **Order Date** field on the purchase order header.</span><span class="sxs-lookup"><span data-stu-id="d30fa-117">If you enter a purchase order line without a requested delivery date, then the **Order Date** field on the line is filled with the date in the **Order Date** field on the purchase order header.</span></span> <span data-ttu-id="d30fa-118">This is either the date that you entered or the work date.</span><span class="sxs-lookup"><span data-stu-id="d30fa-118">This is either the date that you entered or the work date.</span></span> <span data-ttu-id="d30fa-119">The following dates are then calculated for the purchase order line, with the order date as the starting point.</span><span class="sxs-lookup"><span data-stu-id="d30fa-119">The following dates are then calculated for the purchase order line, with the order date as the starting point.</span></span>  

- <span data-ttu-id="d30fa-120">order date + lead time calculation = planned receipt date</span><span class="sxs-lookup"><span data-stu-id="d30fa-120">order date + lead time calculation = planned receipt date</span></span>  
- <span data-ttu-id="d30fa-121">planned receipt date + inbound whse. handling time + safety lead time = expected receipt date</span><span class="sxs-lookup"><span data-stu-id="d30fa-121">planned receipt date + inbound whse. handling time + safety lead time = expected receipt date</span></span>  

<span data-ttu-id="d30fa-122">If you change the order date on the line, such as when items are not available at your vendor until a later date, then the relevant dates on the line are automatically recalculated.</span><span class="sxs-lookup"><span data-stu-id="d30fa-122">If you change the order date on the line, such as when items are not available at your vendor until a later date, then the relevant dates on the line are automatically recalculated.</span></span>  

<span data-ttu-id="d30fa-123">If you change the order date on the header, then that date is copied to the **Order Date** field on all the lines, and all the related date fields are then recalculated.</span><span class="sxs-lookup"><span data-stu-id="d30fa-123">If you change the order date on the header, then that date is copied to the **Order Date** field on all the lines, and all the related date fields are then recalculated.</span></span>  

## <a name="see-also"></a><span data-ttu-id="d30fa-124">See Also</span><span class="sxs-lookup"><span data-stu-id="d30fa-124">See Also</span></span>  
 <span data-ttu-id="d30fa-125">[Date Calculation for Sales](sales-date-calculation-for-sales.md) </span><span class="sxs-lookup"><span data-stu-id="d30fa-125">[Date Calculation for Sales](sales-date-calculation-for-sales.md) </span></span>  
 [<span data-ttu-id="d30fa-126">Calculate Order Promising Dates</span><span class="sxs-lookup"><span data-stu-id="d30fa-126">Calculate Order Promising Dates</span></span>](sales-how-to-calculate-order-promising-dates.md)  
 <span data-ttu-id="d30fa-127">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="d30fa-127">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
