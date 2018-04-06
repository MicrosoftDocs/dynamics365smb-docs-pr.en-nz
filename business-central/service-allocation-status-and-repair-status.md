---
title: Allocation Status and Repair Status | Microsoft Docs
description: Learn about the relationship between the repair status of service items and the allocation status of the allocation entries for them.
services: project-madeira
documentationcenter: 
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: resources, allocation, status, repairs
ms.date: 08/28/2017
ms.author: bholtorf
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 014ede5232017bb090fa6cd33816064a6c4b99b8
ms.contentlocale: en-nz
ms.lasthandoff: 03/22/2018

---
# <a name="allocation-status-and-repair-status-of-service-items"></a><span data-ttu-id="28f37-103">Allocation Status and Repair Status of Service Items</span><span class="sxs-lookup"><span data-stu-id="28f37-103">Allocation Status and Repair Status of Service Items</span></span>
<span data-ttu-id="28f37-104">The repair status of service items and the allocation status of the allocation entries for the service items have a certain relationship in Service Management.</span><span class="sxs-lookup"><span data-stu-id="28f37-104">The repair status of service items and the allocation status of the allocation entries for the service items have a certain relationship in Service Management.</span></span> <span data-ttu-id="28f37-105">The allocation status changes when you change the repair status of the service item to **Finished** or **Partly Serviced** and when you convert a service quote to a service order.</span><span class="sxs-lookup"><span data-stu-id="28f37-105">The allocation status changes when you change the repair status of the service item to **Finished** or **Partly Serviced** and when you convert a service quote to a service order.</span></span> <span data-ttu-id="28f37-106">The repair status of the service item changes when you cancel the service item allocation or reallocate the service item to another resource.</span><span class="sxs-lookup"><span data-stu-id="28f37-106">The repair status of the service item changes when you cancel the service item allocation or reallocate the service item to another resource.</span></span> <span data-ttu-id="28f37-107">You can view the repair status of service items in the **Service Tasks** window and you can update the repair status in the **Repair Status Code** field in the **Service Item Worksheet** window.</span><span class="sxs-lookup"><span data-stu-id="28f37-107">You can view the repair status of service items in the **Service Tasks** window and you can update the repair status in the **Repair Status Code** field in the **Service Item Worksheet** window.</span></span> <span data-ttu-id="28f37-108">You can view the allocation status in the **Status** field in the **Resource Allocations** window.</span><span class="sxs-lookup"><span data-stu-id="28f37-108">You can view the allocation status in the **Status** field in the **Resource Allocations** window.</span></span>  
  
## <a name="changing-repair-status"></a><span data-ttu-id="28f37-109">Changing Repair Status</span><span class="sxs-lookup"><span data-stu-id="28f37-109">Changing Repair Status</span></span>  
<span data-ttu-id="28f37-110">When you change the repair status of a service item on a service item line, there is a search for a corresponding allocation entry for this service item that has the status **Active**.</span><span class="sxs-lookup"><span data-stu-id="28f37-110">When you change the repair status of a service item on a service item line, there is a search for a corresponding allocation entry for this service item that has the status **Active**.</span></span> <span data-ttu-id="28f37-111">If such an allocation entry is found, the status is updated in one of the following ways:</span><span class="sxs-lookup"><span data-stu-id="28f37-111">If such an allocation entry is found, the status is updated in one of the following ways:</span></span>  
  
* <span data-ttu-id="28f37-112">If you change the repair status to **Finished**, the allocation status is changed from **Active** to **Finished**.</span><span class="sxs-lookup"><span data-stu-id="28f37-112">If you change the repair status to **Finished**, the allocation status is changed from **Active** to **Finished**.</span></span>  
* <span data-ttu-id="28f37-113">If you change the repair status to **Partly Serviced**, that is, some of the service has been completed, or **Referred**, that is, no service has been done, the allocation status is changed from **Active** to **Reallocation Needed**.</span><span class="sxs-lookup"><span data-stu-id="28f37-113">If you change the repair status to **Partly Serviced**, that is, some of the service has been completed, or **Referred**, that is, no service has been done, the allocation status is changed from **Active** to **Reallocation Needed**.</span></span>  
* <span data-ttu-id="28f37-114">When a service order allocation entry is created that indicates that no resource has been allocated, the **Status** field in the **Resource Allocation** window is set to **Nonactive**.</span><span class="sxs-lookup"><span data-stu-id="28f37-114">When a service order allocation entry is created that indicates that no resource has been allocated, the **Status** field in the **Resource Allocation** window is set to **Nonactive**.</span></span>  
* <span data-ttu-id="28f37-115">The allocation entry status is set to **Cancelled** when you reallocate the referred service item in the service order allocation entry, which indicates that the allocated resource or resource group has not attempted the service task.</span><span class="sxs-lookup"><span data-stu-id="28f37-115">The allocation entry status is set to **Canceled** when you reallocate the referred service item in the service order allocation entry, which indicates that the allocated resource or resource group has not attempted the service task.</span></span>  
  
<span data-ttu-id="28f37-116">The allocation status reflects when the service process is finished, or when another resource is necessary in order to finish the service of the service item.</span><span class="sxs-lookup"><span data-stu-id="28f37-116">The allocation status reflects when the service process is finished, or when another resource is necessary in order to finish the service of the service item.</span></span>  
  
## <a name="converting-service-quotes-to-service-orders"></a><span data-ttu-id="28f37-117">Converting Service Quotes to Service Orders</span><span class="sxs-lookup"><span data-stu-id="28f37-117">Converting Service Quotes to Service Orders</span></span>  
<span data-ttu-id="28f37-118">When you convert a service quote to a service order, the service order, the service items in the order and their allocation entries are updated in the following ways:</span><span class="sxs-lookup"><span data-stu-id="28f37-118">When you convert a service quote to a service order, the service order, the service items in the order and their allocation entries are updated in the following ways:</span></span>  
  
* <span data-ttu-id="28f37-119">The repair status of the service items is changed to **Initial**.</span><span class="sxs-lookup"><span data-stu-id="28f37-119">The repair status of the service items is changed to **Initial**.</span></span>  
* <span data-ttu-id="28f37-120">The service order status is changed to **Pending**.</span><span class="sxs-lookup"><span data-stu-id="28f37-120">The service order status is changed to **Pending**.</span></span>  
* <span data-ttu-id="28f37-121">There is a search for allocation entries for all the service items in the service order that have the status **Active**.</span><span class="sxs-lookup"><span data-stu-id="28f37-121">There is a search for allocation entries for all the service items in the service order that have the status **Active**.</span></span> <span data-ttu-id="28f37-122">If such allocation entries are found, their allocation status is changed from **Active** to **Reallocation Needed**.</span><span class="sxs-lookup"><span data-stu-id="28f37-122">If such allocation entries are found, their allocation status is changed from **Active** to **Reallocation Needed**.</span></span>  
  
## <a name="canceling-allocations"></a><span data-ttu-id="28f37-123">Cancelling Allocations</span><span class="sxs-lookup"><span data-stu-id="28f37-123">Canceling Allocations</span></span>  
<span data-ttu-id="28f37-124">When you cancel an allocation for a service item, [!INCLUDE[d365fin](includes/d365fin_md.md)] updates the allocation status of the corresponding allocation entry from **Active** to **Reallocation Needed**.</span><span class="sxs-lookup"><span data-stu-id="28f37-124">When you cancel an allocation for a service item, [!INCLUDE[d365fin](includes/d365fin_md.md)] updates the allocation status of the corresponding allocation entry from **Active** to **Reallocation Needed**.</span></span>

<span data-ttu-id="28f37-125">The repair status of the service item in the allocation entry is updated in the following ways:</span><span class="sxs-lookup"><span data-stu-id="28f37-125">The repair status of the service item in the allocation entry is updated in the following ways:</span></span>  
  
* <span data-ttu-id="28f37-126">If the repair status is **Initial**, the repair status is changed to **Referred** (no service has been started).</span><span class="sxs-lookup"><span data-stu-id="28f37-126">If the repair status is **Initial**, the repair status is changed to **Referred** (no service has been started).</span></span>  
* <span data-ttu-id="28f37-127">If the repair status is **In Process**, the repair status is changed to **Partly Serviced** (some service has been completed).</span><span class="sxs-lookup"><span data-stu-id="28f37-127">If the repair status is **In Process**, the repair status is changed to **Partly Serviced** (some service has been completed).</span></span>  
  
## <a name="reallocating-an-active-allocation-entry"></a><span data-ttu-id="28f37-128">Reallocating an Active Allocation Entry</span><span class="sxs-lookup"><span data-stu-id="28f37-128">Reallocating an Active Allocation Entry</span></span>  
<span data-ttu-id="28f37-129">When you reallocate a service item in an allocation entry that is **Active**, the allocation entry is updated in the following ways:</span><span class="sxs-lookup"><span data-stu-id="28f37-129">When you reallocate a service item in an allocation entry that is **Active**, the allocation entry is updated in the following ways:</span></span>  
  
* <span data-ttu-id="28f37-130">If service was started when the allocation was **Active** (that is, if the repair status of the service item in the entry was changed to **In Process**), the allocation status is changed from **Active** to **Finished**.</span><span class="sxs-lookup"><span data-stu-id="28f37-130">If service was started when the allocation was **Active** (that is, if the repair status of the service item in the entry was changed to **In Process**), the allocation status is changed from **Active** to **Finished**.</span></span>  
* <span data-ttu-id="28f37-131">If service was not started when the allocation was **Active**, the allocation status is changed from **Active** to **Cancelled**.</span><span class="sxs-lookup"><span data-stu-id="28f37-131">If service was not started when the allocation was **Active**, the allocation status is changed from **Active** to **Canceled**.</span></span>  
  
<span data-ttu-id="28f37-132">The repair status of the service item in the allocation entry is updated in the same way as if you had cancelled the allocation:</span><span class="sxs-lookup"><span data-stu-id="28f37-132">The repair status of the service item in the allocation entry is updated in the same way as if you had canceled the allocation:</span></span>  
  
* <span data-ttu-id="28f37-133">If the repair status is **Initial**, the repair status is changed to **Referred** (no service has been started).</span><span class="sxs-lookup"><span data-stu-id="28f37-133">If the repair status is **Initial**, the repair status is changed to **Referred** (no service has been started).</span></span>  
* <span data-ttu-id="28f37-134">If the repair status is **In Process**, the repair status is changed to **Partly Serviced** (some service has been completed).</span><span class="sxs-lookup"><span data-stu-id="28f37-134">If the repair status is **In Process**, the repair status is changed to **Partly Serviced** (some service has been completed).</span></span>  
  
<span data-ttu-id="28f37-135">A new allocation entry that contains the new resource is created that has the status **Active**.</span><span class="sxs-lookup"><span data-stu-id="28f37-135">A new allocation entry that contains the new resource is created that has the status **Active**.</span></span>  
  
## <a name="reallocating-a-service-item"></a><span data-ttu-id="28f37-136">Reallocating a Service Item</span><span class="sxs-lookup"><span data-stu-id="28f37-136">Reallocating a Service Item</span></span>  
<span data-ttu-id="28f37-137">When you reallocate a service item in an allocation entry that has the status **Reallocation Needed**, the allocation entry is updated in the following ways:</span><span class="sxs-lookup"><span data-stu-id="28f37-137">When you reallocate a service item in an allocation entry that has the status **Reallocation Needed**, the allocation entry is updated in the following ways:</span></span>  
  
* <span data-ttu-id="28f37-138">If service was started when the allocation was **Active** (that is, if the repair status of the service item in the entry was changed to **In Process**), the allocation status is changed from **Reallocation Needed** to **Finished**.</span><span class="sxs-lookup"><span data-stu-id="28f37-138">If service was started when the allocation was **Active** (that is, if the repair status of the service item in the entry was changed to **In Process**), the allocation status is changed from **Reallocation Needed** to **Finished**.</span></span>  
* <span data-ttu-id="28f37-139">If service was not started when the allocation was **Active**, the allocation status is changed from **Reallocation Needed** to **Cancelled**.</span><span class="sxs-lookup"><span data-stu-id="28f37-139">If service was not started when the allocation was **Active**, the allocation status is changed from **Reallocation Needed** to **Canceled**.</span></span>  
  
<span data-ttu-id="28f37-140">A new allocation entry that contains the new resource is created that has the status **Active**.</span><span class="sxs-lookup"><span data-stu-id="28f37-140">A new allocation entry that contains the new resource is created that has the status **Active**.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="28f37-141">See Also</span><span class="sxs-lookup"><span data-stu-id="28f37-141">See Also</span></span>  
[<span data-ttu-id="28f37-142">Set Up Resource Allocations</span><span class="sxs-lookup"><span data-stu-id="28f37-142">Set Up Resource Allocations</span></span>](service-how-setup-resource-allocation.md)  
[<span data-ttu-id="28f37-143">Allocate Resources</span><span class="sxs-lookup"><span data-stu-id="28f37-143">Allocate Resources</span></span>](service-how-to-allocate-resources.md)  

