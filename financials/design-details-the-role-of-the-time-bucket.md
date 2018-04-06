---
title: Design Details - The Role of the Time Bucket | Microsoft Docs
description: The purpose of the time bucket is to collect demand events within the time window in order to make a joint supply order.
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
ms.openlocfilehash: eb1b1a401dabe09a77c44558e9f5a83388078aaa
ms.contentlocale: en-nz
ms.lasthandoff: 03/22/2018

---
# <a name="design-details-the-role-of-the-time-bucket"></a><span data-ttu-id="a1bfe-103">Design Details: The Role of the Time Bucket</span><span class="sxs-lookup"><span data-stu-id="a1bfe-103">Design Details: The Role of the Time Bucket</span></span>
<span data-ttu-id="a1bfe-104">The purpose of the time bucket is to collect demand events within the time window in order to make a joint supply order.</span><span class="sxs-lookup"><span data-stu-id="a1bfe-104">The purpose of the time bucket is to collect demand events within the time window in order to make a joint supply order.</span></span>  
  
 <span data-ttu-id="a1bfe-105">For reordering policies that use a reorder point, you can define a time bucket.</span><span class="sxs-lookup"><span data-stu-id="a1bfe-105">For reordering policies that use a reorder point, you can define a time bucket.</span></span> <span data-ttu-id="a1bfe-106">This ensures that demand within the same time period is accumulated before checking the impact on the projected inventory and whether the reorder point has been passed.</span><span class="sxs-lookup"><span data-stu-id="a1bfe-106">This ensures that demand within the same time period is accumulated before checking the impact on the projected inventory and whether the reorder point has been passed.</span></span> <span data-ttu-id="a1bfe-107">If the reorder point is passed, a new supply order is scheduled forward from the end of the period defined by the time bucket.</span><span class="sxs-lookup"><span data-stu-id="a1bfe-107">If the reorder point is passed, a new supply order is scheduled forward from the end of the period defined by the time bucket.</span></span> <span data-ttu-id="a1bfe-108">The time buckets begin on the planning starting date.</span><span class="sxs-lookup"><span data-stu-id="a1bfe-108">The time buckets begin on the planning starting date.</span></span>  
  
 <span data-ttu-id="a1bfe-109">The time-bucketed concept reflects the manual process of checking the inventory level on a frequent basis rather than for each transaction.</span><span class="sxs-lookup"><span data-stu-id="a1bfe-109">The time-bucketed concept reflects the manual process of checking the inventory level on a frequent basis rather than for each transaction.</span></span> <span data-ttu-id="a1bfe-110">The user needs to define the frequency (the time bucket).</span><span class="sxs-lookup"><span data-stu-id="a1bfe-110">The user needs to define the frequency (the time bucket).</span></span> <span data-ttu-id="a1bfe-111">For example, the user gathers all item needs from one vendor to place a weekly order.</span><span class="sxs-lookup"><span data-stu-id="a1bfe-111">For example, the user gathers all item needs from one vendor to place a weekly order.</span></span>  
  
 <span data-ttu-id="a1bfe-112">![](media/nav_app_supply_planning_2_reorder_cycle.png "NAV_APP_supply_planning_2_reorder_cycle")</span><span class="sxs-lookup"><span data-stu-id="a1bfe-112">![](media/nav_app_supply_planning_2_reorder_cycle.png "NAV_APP_supply_planning_2_reorder_cycle")</span></span>  
  
 <span data-ttu-id="a1bfe-113">The time bucket is generally used to avoid a cascade effect.</span><span class="sxs-lookup"><span data-stu-id="a1bfe-113">The time bucket is generally used to avoid a cascade effect.</span></span> <span data-ttu-id="a1bfe-114">For example, a balanced row of demand and supply where an early demand is cancelled, or a new one is created.</span><span class="sxs-lookup"><span data-stu-id="a1bfe-114">For example, a balanced row of demand and supply where an early demand is canceled, or a new one is created.</span></span> <span data-ttu-id="a1bfe-115">The result would be that every supply order (except the last one) is rescheduled.</span><span class="sxs-lookup"><span data-stu-id="a1bfe-115">The result would be that every supply order (except the last one) is rescheduled.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="a1bfe-116">See Also</span><span class="sxs-lookup"><span data-stu-id="a1bfe-116">See Also</span></span>  
 <span data-ttu-id="a1bfe-117">[Design Details: Reordering Policies](design-details-reordering-policies.md) </span><span class="sxs-lookup"><span data-stu-id="a1bfe-117">[Design Details: Reordering Policies](design-details-reordering-policies.md) </span></span>  
 <span data-ttu-id="a1bfe-118">[Design Details: Planning Parameters](design-details-planning-parameters.md) </span><span class="sxs-lookup"><span data-stu-id="a1bfe-118">[Design Details: Planning Parameters](design-details-planning-parameters.md) </span></span>  
 <span data-ttu-id="a1bfe-119">[Design Details: Handling Reordering Policies](design-details-handling-reordering-policies.md) </span><span class="sxs-lookup"><span data-stu-id="a1bfe-119">[Design Details: Handling Reordering Policies](design-details-handling-reordering-policies.md) </span></span>  
 [<span data-ttu-id="a1bfe-120">Design Details: Supply Planning</span><span class="sxs-lookup"><span data-stu-id="a1bfe-120">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)
