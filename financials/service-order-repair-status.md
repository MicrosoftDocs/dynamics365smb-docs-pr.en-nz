---
title: Set Up Statuses for Service Orders and Repairs | Microsoft Docs
description: You must set up nine repair status options that identify the progress of repair and maintenance of service items in service orders.
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
ms.openlocfilehash: 36925a08f7fdfffedf13902a5c6feaaa8b0929a4
ms.contentlocale: en-nz
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-set-up-statuses-for-service-orders-and-repairs"></a><span data-ttu-id="705c2-103">How to: Set Up Statuses for Service Orders and Repairs</span><span class="sxs-lookup"><span data-stu-id="705c2-103">How to: Set Up Statuses for Service Orders and Repairs</span></span>
<span data-ttu-id="705c2-104">You must set up repair status options that identify the progress of repair and maintenance of service items in service orders.</span><span class="sxs-lookup"><span data-stu-id="705c2-104">You must set up repair status options that identify the progress of repair and maintenance of service items in service orders.</span></span> <span data-ttu-id="705c2-105">You must set up at least nine repair status options that identify situations or actions taken when servicing service items.</span><span class="sxs-lookup"><span data-stu-id="705c2-105">You must set up at least nine repair status options that identify situations or actions taken when servicing service items.</span></span>  

<span data-ttu-id="705c2-106">You can set the priority level for service order status options.</span><span class="sxs-lookup"><span data-stu-id="705c2-106">You can set the priority level for service order status options.</span></span> <span data-ttu-id="705c2-107">There four priorities are High, Medium High, Medium Low, and Low.</span><span class="sxs-lookup"><span data-stu-id="705c2-107">There four priorities are High, Medium High, Medium Low, and Low.</span></span>  
  
<span data-ttu-id="705c2-108">When you change the repair status of a service item in a service order, the service order status is updated.</span><span class="sxs-lookup"><span data-stu-id="705c2-108">When you change the repair status of a service item in a service order, the service order status is updated.</span></span> <span data-ttu-id="705c2-109">The repair status of each service item is linked to the service order status.</span><span class="sxs-lookup"><span data-stu-id="705c2-109">The repair status of each service item is linked to the service order status.</span></span> <span data-ttu-id="705c2-110">If the service items are linked to two or more service order status options, the service order status with the highest priority is selected.</span><span class="sxs-lookup"><span data-stu-id="705c2-110">If the service items are linked to two or more service order status options, the service order status with the highest priority is selected.</span></span>  

## <a name="to-set-up-a-repair-status"></a><span data-ttu-id="705c2-111">To set up a repair status</span><span class="sxs-lookup"><span data-stu-id="705c2-111">To set up a repair status</span></span>  
1. <span data-ttu-id="705c2-112">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Repair Status**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="705c2-112">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Repair Status**, and then choose the related link.</span></span> <span data-ttu-id="705c2-113">2.</span><span class="sxs-lookup"><span data-stu-id="705c2-113">2.</span></span> <span data-ttu-id="705c2-114">Create a new repair status.</span><span class="sxs-lookup"><span data-stu-id="705c2-114">Create a new repair status.</span></span>  
3. <span data-ttu-id="705c2-115">Fill in the **Code** and **Description** fields.</span><span class="sxs-lookup"><span data-stu-id="705c2-115">Fill in the **Code** and **Description** fields.</span></span>  
4. <span data-ttu-id="705c2-116">In the **Service Order Status** field, choose the order status to link the repair status to.</span><span class="sxs-lookup"><span data-stu-id="705c2-116">In the **Service Order Status** field, choose the order status to link the repair status to.</span></span> <span data-ttu-id="705c2-117">The **Priority** field displays the priority of the service order status you have chosen.</span><span class="sxs-lookup"><span data-stu-id="705c2-117">The **Priority** field displays the priority of the service order status you have chosen.</span></span>  
5. <span data-ttu-id="705c2-118">Choose a repair status.</span><span class="sxs-lookup"><span data-stu-id="705c2-118">Choose a repair status.</span></span> <span data-ttu-id="705c2-119">You can choose only one.</span><span class="sxs-lookup"><span data-stu-id="705c2-119">You can choose only one.</span></span>  
6. <span data-ttu-id="705c2-120">To be able to post service orders, including service items, with this repair status, choose the **Posting Allowed** field.</span><span class="sxs-lookup"><span data-stu-id="705c2-120">To be able to post service orders, including service items, with this repair status, choose the **Posting Allowed** field.</span></span>  
7. <span data-ttu-id="705c2-121">To be able to manually change the service order status option to **Pending** in service orders including service items with this repair status, choose the **Pending Status Allowed** check box.</span><span class="sxs-lookup"><span data-stu-id="705c2-121">To be able to manually change the service order status option to **Pending** in service orders including service items with this repair status, choose the **Pending Status Allowed** check box.</span></span>  
8. <span data-ttu-id="705c2-122">Choose the **In Process Status Allowed**, **Finished Status Allowed**, and **On Hold Status Allowed** check boxes in the same way.</span><span class="sxs-lookup"><span data-stu-id="705c2-122">Choose the **In Process Status Allowed**, **Finished Status Allowed**, and **On Hold Status Allowed** check boxes in the same way.</span></span>
  
## <a name="to-set-up-service-status-priorities"></a><span data-ttu-id="705c2-123">To set up service status priorities</span><span class="sxs-lookup"><span data-stu-id="705c2-123">To set up service status priorities</span></span>  
1. <span data-ttu-id="705c2-124">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Service Order Status**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="705c2-124">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Service Order Status**, and then choose the related link.</span></span>  
2. <span data-ttu-id="705c2-125">Select the service order status you want to set a priority for.</span><span class="sxs-lookup"><span data-stu-id="705c2-125">Select the service order status you want to set a priority for.</span></span>  
3. <span data-ttu-id="705c2-126">In the **Priority** field, choose the priority you want for this service order status.</span><span class="sxs-lookup"><span data-stu-id="705c2-126">In the **Priority** field, choose the priority you want for this service order status.</span></span> <span data-ttu-id="705c2-127">Repeat this step for each status.</span><span class="sxs-lookup"><span data-stu-id="705c2-127">Repeat this step for each status.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="705c2-128">See Also</span><span class="sxs-lookup"><span data-stu-id="705c2-128">See Also</span></span>  
[<span data-ttu-id="705c2-129">Understanding Service Order Status and Repair Status</span><span class="sxs-lookup"><span data-stu-id="705c2-129">Understanding Service Order Status and Repair Status</span></span>]()  
[<span data-ttu-id="705c2-130">Setting Up Service Management</span><span class="sxs-lookup"><span data-stu-id="705c2-130">Setting Up Service Management</span></span>](service-setup-service.md)  

