---
title: Set Up Statuses for Service Orders and Repairs | Microsoft Docs
description: You must set up nine repair status options that identify the progress of repair and maintenance of service items in service orders.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2019
ms.author: sgroespe
ms.openlocfilehash: 65aab5ba1f88285ad843261d3c804dfb3e18432c
ms.sourcegitcommit: cfc92eefa8b06fb426482f54e393f0e6e222f712
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 12/03/2019
ms.locfileid: "2882366"
---
# <a name="set-up-statuses-for-service-orders-and-repairs"></a><span data-ttu-id="944dc-103">Set Up Statuses for Service Orders and Repairs</span><span class="sxs-lookup"><span data-stu-id="944dc-103">Set Up Statuses for Service Orders and Repairs</span></span>
<span data-ttu-id="944dc-104">You must set up repair status options that identify the progress of repair and maintenance of service items in service orders.</span><span class="sxs-lookup"><span data-stu-id="944dc-104">You must set up repair status options that identify the progress of repair and maintenance of service items in service orders.</span></span> <span data-ttu-id="944dc-105">You must set up at least nine repair status options that identify situations or actions taken when servicing service items.</span><span class="sxs-lookup"><span data-stu-id="944dc-105">You must set up at least nine repair status options that identify situations or actions taken when servicing service items.</span></span>  

<span data-ttu-id="944dc-106">You can set the priority level for service order status options.</span><span class="sxs-lookup"><span data-stu-id="944dc-106">You can set the priority level for service order status options.</span></span> <span data-ttu-id="944dc-107">There four priorities are High, Medium High, Medium Low, and Low.</span><span class="sxs-lookup"><span data-stu-id="944dc-107">There four priorities are High, Medium High, Medium Low, and Low.</span></span>  

<span data-ttu-id="944dc-108">When you change the repair status of a service item in a service order, the service order status is updated.</span><span class="sxs-lookup"><span data-stu-id="944dc-108">When you change the repair status of a service item in a service order, the service order status is updated.</span></span> <span data-ttu-id="944dc-109">The repair status of each service item is linked to the service order status.</span><span class="sxs-lookup"><span data-stu-id="944dc-109">The repair status of each service item is linked to the service order status.</span></span> <span data-ttu-id="944dc-110">If the service items are linked to two or more service order status options, the service order status with the highest priority is selected.</span><span class="sxs-lookup"><span data-stu-id="944dc-110">If the service items are linked to two or more service order status options, the service order status with the highest priority is selected.</span></span>  

## <a name="to-set-up-a-repair-status"></a><span data-ttu-id="944dc-111">To set up a repair status</span><span class="sxs-lookup"><span data-stu-id="944dc-111">To set up a repair status</span></span>  
1. <span data-ttu-id="944dc-112">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Repair Status**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="944dc-112">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Repair Status**, and then choose the related link.</span></span>
2. <span data-ttu-id="944dc-113">Create a new repair status.</span><span class="sxs-lookup"><span data-stu-id="944dc-113">Create a new repair status.</span></span>  
3. <span data-ttu-id="944dc-114">Fill in the **Code** and **Description** fields.</span><span class="sxs-lookup"><span data-stu-id="944dc-114">Fill in the **Code** and **Description** fields.</span></span>  
4. <span data-ttu-id="944dc-115">In the **Service Order Status** field, choose the order status to link the repair status to.</span><span class="sxs-lookup"><span data-stu-id="944dc-115">In the **Service Order Status** field, choose the order status to link the repair status to.</span></span> <span data-ttu-id="944dc-116">The **Priority** field displays the priority of the service order status you have chosen.</span><span class="sxs-lookup"><span data-stu-id="944dc-116">The **Priority** field displays the priority of the service order status you have chosen.</span></span>  
5. <span data-ttu-id="944dc-117">Choose a repair status.</span><span class="sxs-lookup"><span data-stu-id="944dc-117">Choose a repair status.</span></span> <span data-ttu-id="944dc-118">You can choose only one.</span><span class="sxs-lookup"><span data-stu-id="944dc-118">You can choose only one.</span></span>  
6. <span data-ttu-id="944dc-119">To be able to post service orders, including service items, with this repair status, choose the **Posting Allowed** field.</span><span class="sxs-lookup"><span data-stu-id="944dc-119">To be able to post service orders, including service items, with this repair status, choose the **Posting Allowed** field.</span></span>  
7. <span data-ttu-id="944dc-120">To be able to manually change the service order status option to **Pending** in service orders including service items with this repair status, choose the **Pending Status Allowed** check box.</span><span class="sxs-lookup"><span data-stu-id="944dc-120">To be able to manually change the service order status option to **Pending** in service orders including service items with this repair status, choose the **Pending Status Allowed** check box.</span></span>  
8. <span data-ttu-id="944dc-121">Choose the **In Process Status Allowed**, **Finished Status Allowed**, and **On Hold Status Allowed** check boxes in the same way.</span><span class="sxs-lookup"><span data-stu-id="944dc-121">Choose the **In Process Status Allowed**, **Finished Status Allowed**, and **On Hold Status Allowed** check boxes in the same way.</span></span>
  
## <a name="to-set-up-service-status-priorities"></a><span data-ttu-id="944dc-122">To set up service status priorities</span><span class="sxs-lookup"><span data-stu-id="944dc-122">To set up service status priorities</span></span>  
1. <span data-ttu-id="944dc-123">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Service Order Status**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="944dc-123">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Service Order Status**, and then choose the related link.</span></span>  
2. <span data-ttu-id="944dc-124">Select the service order status you want to set a priority for.</span><span class="sxs-lookup"><span data-stu-id="944dc-124">Select the service order status you want to set a priority for.</span></span>  
3. <span data-ttu-id="944dc-125">In the **Priority** field, choose the priority you want for this service order status.</span><span class="sxs-lookup"><span data-stu-id="944dc-125">In the **Priority** field, choose the priority you want for this service order status.</span></span> <span data-ttu-id="944dc-126">Repeat this step for each status.</span><span class="sxs-lookup"><span data-stu-id="944dc-126">Repeat this step for each status.</span></span>  

## <a name="see-also"></a><span data-ttu-id="944dc-127">See Also</span><span class="sxs-lookup"><span data-stu-id="944dc-127">See Also</span></span>  
[<span data-ttu-id="944dc-128">Service Order Status and Repair Status</span><span class="sxs-lookup"><span data-stu-id="944dc-128">Service Order Status and Repair Status</span></span>](service-service-order-status-and-repair-status.md)  
[<span data-ttu-id="944dc-129">Setting Up Service Management</span><span class="sxs-lookup"><span data-stu-id="944dc-129">Setting Up Service Management</span></span>](service-setup-service.md)  
