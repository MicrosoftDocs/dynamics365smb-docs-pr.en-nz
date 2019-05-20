---
title: Design Details - Maximum Qty. | Microsoft Docs
description: The Maximum Quantity policy is a way to maintain inventory using a reorder point.
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
redirect_url: design-details-handling-reordering-policies
ms.openlocfilehash: 857a01bac28d85a35668f3aa01e8807a6f6dc845
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 04/29/2019
ms.locfileid: "1239169"
---
# <a name="design-details-maximum-qty"></a><span data-ttu-id="8ece0-103">Design Details: Maximum Qty.</span><span class="sxs-lookup"><span data-stu-id="8ece0-103">Design Details: Maximum Qty.</span></span>
<span data-ttu-id="8ece0-104">The Maximum Quantity policy is a way to maintain inventory using a reorder point.</span><span class="sxs-lookup"><span data-stu-id="8ece0-104">The Maximum Quantity policy is a way to maintain inventory using a reorder point.</span></span>  

 <span data-ttu-id="8ece0-105">Everything regarding the Fixed Reorder Qty. policy also applies to this policy.</span><span class="sxs-lookup"><span data-stu-id="8ece0-105">Everything regarding the Fixed Reorder Qty. policy also applies to this policy.</span></span> <span data-ttu-id="8ece0-106">The only difference is the quantity of the suggested supply.</span><span class="sxs-lookup"><span data-stu-id="8ece0-106">The only difference is the quantity of the suggested supply.</span></span> <span data-ttu-id="8ece0-107">When using the maximum quantity policy, the reorder quantity will be defined dynamically based on the projected inventory level and will therefore usually differ from order to order.</span><span class="sxs-lookup"><span data-stu-id="8ece0-107">When using the maximum quantity policy, the reorder quantity will be defined dynamically based on the projected inventory level and will therefore usually differ from order to order.</span></span>  

## <a name="calculated-per-time-bucket"></a><span data-ttu-id="8ece0-108">Calculated per Time Bucket</span><span class="sxs-lookup"><span data-stu-id="8ece0-108">Calculated per Time Bucket</span></span>  
 <span data-ttu-id="8ece0-109">The reorder quantity is determined at the point of time (the end of a time bucket) when the planning system detects that the reorder point has been crossed.</span><span class="sxs-lookup"><span data-stu-id="8ece0-109">The reorder quantity is determined at the point of time (the end of a time bucket) when the planning system detects that the reorder point has been crossed.</span></span> <span data-ttu-id="8ece0-110">At this time, the system measures the gap from the current projected inventory level up to the specified maximum inventory.</span><span class="sxs-lookup"><span data-stu-id="8ece0-110">At this time, the system measures the gap from the current projected inventory level up to the specified maximum inventory.</span></span> <span data-ttu-id="8ece0-111">This constitutes the quantity that should be reordered.</span><span class="sxs-lookup"><span data-stu-id="8ece0-111">This constitutes the quantity that should be reordered.</span></span> <span data-ttu-id="8ece0-112">The system then checks if supply has already been ordered elsewhere to be received within the lead time and, if so, reduces the quantity of the new supply order by already ordered quantities.</span><span class="sxs-lookup"><span data-stu-id="8ece0-112">The system then checks if supply has already been ordered elsewhere to be received within the lead time and, if so, reduces the quantity of the new supply order by already ordered quantities.</span></span>  

 <span data-ttu-id="8ece0-113">The system will ensure that the projected inventory at least reaches the reorder point level – in case the user has forgotten to specify a maximum inventory quantity.</span><span class="sxs-lookup"><span data-stu-id="8ece0-113">The system will ensure that the projected inventory at least reaches the reorder point level – in case the user has forgotten to specify a maximum inventory quantity.</span></span>  

## <a name="combines-with-order-modifiers"></a><span data-ttu-id="8ece0-114">Combines with Order Modifiers</span><span class="sxs-lookup"><span data-stu-id="8ece0-114">Combines with Order Modifiers</span></span>  
 <span data-ttu-id="8ece0-115">Depending on the setup, it may be best to combine the Maximum Quantity policy with order modifiers to ensure a minimum order quantity or round it to an integer number of purchase units of measure, or split it into more lots as defined by the maximum order quantity.</span><span class="sxs-lookup"><span data-stu-id="8ece0-115">Depending on the setup, it may be best to combine the Maximum Quantity policy with order modifiers to ensure a minimum order quantity or round it to an integer number of purchase units of measure, or split it into more lots as defined by the maximum order quantity.</span></span>  

## <a name="combines-with-calendars"></a><span data-ttu-id="8ece0-116">Combines with Calendars</span><span class="sxs-lookup"><span data-stu-id="8ece0-116">Combines with Calendars</span></span>  
 <span data-ttu-id="8ece0-117">Before suggesting a new supply order to meet a reorder point, the planning system checks if the order is scheduled for a non-working day, according to any calendars that are defined in the **Base Calendar Code** field in the **Company Information** and **Location Card** pages.</span><span class="sxs-lookup"><span data-stu-id="8ece0-117">Before suggesting a new supply order to meet a reorder point, the planning system checks if the order is scheduled for a non-working day, according to any calendars that are  defined in the **Base Calendar Code** field in the **Company Information** and **Location Card** pages.</span></span>  

 <span data-ttu-id="8ece0-118">If the scheduled date is a non-working day, the planning system moves the order forward to the nearest working date.</span><span class="sxs-lookup"><span data-stu-id="8ece0-118">If the scheduled date is a non-working day, the planning system moves the order forward to the nearest working date.</span></span> <span data-ttu-id="8ece0-119">This may result in an order that meets a reorder point but does not meet some specific demand.</span><span class="sxs-lookup"><span data-stu-id="8ece0-119">This may result in an order that meets a reorder point but does not meet some specific demand.</span></span> <span data-ttu-id="8ece0-120">For such unbalanced demand, the planning system creates an extra supply.</span><span class="sxs-lookup"><span data-stu-id="8ece0-120">For such unbalanced demand, the planning system creates an extra supply.</span></span>  

## <a name="see-also"></a><span data-ttu-id="8ece0-121">See Also</span><span class="sxs-lookup"><span data-stu-id="8ece0-121">See Also</span></span>  
 <span data-ttu-id="8ece0-122">[Design Details: Reordering Policies](design-details-reordering-policies.md) </span><span class="sxs-lookup"><span data-stu-id="8ece0-122">[Design Details: Reordering Policies](design-details-reordering-policies.md) </span></span>  
 <span data-ttu-id="8ece0-123">[Design Details: Planning Parameters](design-details-planning-parameters.md) </span><span class="sxs-lookup"><span data-stu-id="8ece0-123">[Design Details: Planning Parameters](design-details-planning-parameters.md) </span></span>  
 <span data-ttu-id="8ece0-124">[Design Details: Handling Reordering Policies](design-details-handling-reordering-policies.md) </span><span class="sxs-lookup"><span data-stu-id="8ece0-124">[Design Details: Handling Reordering Policies](design-details-handling-reordering-policies.md) </span></span>  
 [<span data-ttu-id="8ece0-125">Design Details: Supply Planning</span><span class="sxs-lookup"><span data-stu-id="8ece0-125">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)
