---
title: How to Set Up Work Hours and Service Hours | Microsoft Docs
description: You can specify the usual service working hours in your company. These service hours are used to calculate the response date and time for service orders and quotes, and to send response time warnings.
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
ms.openlocfilehash: 043f1b9044e65e4aba52690f5f62cebcbd397f8d
ms.contentlocale: en-nz
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-set-up-work-hours-and-service-hours"></a><span data-ttu-id="2fc69-104">How to: Set Up Work Hours and Service Hours</span><span class="sxs-lookup"><span data-stu-id="2fc69-104">How to: Set Up Work Hours and Service Hours</span></span>
<span data-ttu-id="2fc69-105">Typically, a service management system tracks resource hours and service order status in order to forecast workloads and service needs.</span><span class="sxs-lookup"><span data-stu-id="2fc69-105">Typically, a service management system tracks resource hours and service order status in order to forecast workloads and service needs.</span></span> [!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="2fc69-106"> has built-in tools that you can customise to record this kind of information.</span><span class="sxs-lookup"><span data-stu-id="2fc69-106"> has built-in tools that you can customize to record this kind of information.</span></span>  
  
<span data-ttu-id="2fc69-107">After you set the default service hours of your company, you can calculate response times for service orders or send warnings or alerts when service calls come in.</span><span class="sxs-lookup"><span data-stu-id="2fc69-107">After you set the default service hours of your company, you can calculate response times for service orders or send warnings or alerts when service calls come in.</span></span> <span data-ttu-id="2fc69-108">The alert feature is implemented together with the job scheduler.</span><span class="sxs-lookup"><span data-stu-id="2fc69-108">The alert feature is implemented together with the job scheduler.</span></span>   
  
<span data-ttu-id="2fc69-109">As you work on a service order, you will want to update it's status so that you can monitor progress.</span><span class="sxs-lookup"><span data-stu-id="2fc69-109">As you work on a service order, you will want to update it's status so that you can monitor progress.</span></span> <span data-ttu-id="2fc69-110">The service order status reflects the repair status of all the service items in the service order.</span><span class="sxs-lookup"><span data-stu-id="2fc69-110">The service order status reflects the repair status of all the service items in the service order.</span></span> <span data-ttu-id="2fc69-111">For more information, see [Understanding Service Order and Repair Status](service-order-repair-status.md).</span><span class="sxs-lookup"><span data-stu-id="2fc69-111">For more information, see [Understanding Service Order and Repair Status](service-order-repair-status.md).</span></span> 

## <a name="to-set-up-default-service-hours"></a><span data-ttu-id="2fc69-112">To set up default service hours</span><span class="sxs-lookup"><span data-stu-id="2fc69-112">To set up default service hours</span></span>  
<span data-ttu-id="2fc69-113">You use the **Default Service Hours** window to set up the usual service working hours in your company.</span><span class="sxs-lookup"><span data-stu-id="2fc69-113">You use the **Default Service Hours** window to set up the usual service working hours in your company.</span></span> <span data-ttu-id="2fc69-114">These service hours are used to calculate the response date and time for service orders and quotes and to send response time warnings.</span><span class="sxs-lookup"><span data-stu-id="2fc69-114">These service hours are used to calculate the response date and time for service orders and quotes and to send response time warnings.</span></span> <span data-ttu-id="2fc69-115">The default service hours are used for service contracts unless you specify special service hours for a contract.</span><span class="sxs-lookup"><span data-stu-id="2fc69-115">The default service hours are used for service contracts unless you specify special service hours for a contract.</span></span>  
  
1. <span data-ttu-id="2fc69-116">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Default Service Hours**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="2fc69-116">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Default Service Hours**, and then choose the related link.</span></span>  
2. <span data-ttu-id="2fc69-117">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="2fc69-117">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  
  
> [!IMPORTANT]  
>  <span data-ttu-id="2fc69-118">If you leave the lines in the **Default Service Hours** window empty, the default value is 24 hours, valid only for calendar working days.</span><span class="sxs-lookup"><span data-stu-id="2fc69-118">If you leave the lines in the **Default Service Hours** window empty, the default value is 24 hours, valid only for calendar working days.</span></span>  
  
## <a name="to-set-up-work-hour-templates"></a><span data-ttu-id="2fc69-119">To set up work-hour templates</span><span class="sxs-lookup"><span data-stu-id="2fc69-119">To set up work-hour templates</span></span>
<span data-ttu-id="2fc69-120">You can use the **Work-Hour Template** window to set up templates that contain the typical working hours in your company.</span><span class="sxs-lookup"><span data-stu-id="2fc69-120">You can use the **Work-Hour Template** window to set up templates that contain the typical working hours in your company.</span></span> <span data-ttu-id="2fc69-121">For example, you can create templates for full time technicians and part time technicians.</span><span class="sxs-lookup"><span data-stu-id="2fc69-121">For example, you can create templates for full time technicians and part time technicians.</span></span> <span data-ttu-id="2fc69-122">You can use work-hour templates when you add capacity to resources.</span><span class="sxs-lookup"><span data-stu-id="2fc69-122">You can use work-hour templates when you add capacity to resources.</span></span>  
  
1. <span data-ttu-id="2fc69-123">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Work Hour Templates**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="2fc69-123">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Work Hour Templates**, and then choose the related link.</span></span>  
2. <span data-ttu-id="2fc69-124">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="2fc69-124">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  
  
> [!Note]
> <span data-ttu-id="2fc69-125">After you enter work hours for each day, the value in the **Total per Week** field is calculated automatically.</span><span class="sxs-lookup"><span data-stu-id="2fc69-125">After you enter work hours for each day, the value in the **Total per Week** field is calculated automatically.</span></span>  

## <a name="to-set-up-contract-specific-service-hours"></a><span data-ttu-id="2fc69-126">To set up contract specific service hours</span><span class="sxs-lookup"><span data-stu-id="2fc69-126">To set up contract specific service hours</span></span>  
<span data-ttu-id="2fc69-127">You can use the **Service Hours** window to set up specific service hours for the customer that owns the service contract.</span><span class="sxs-lookup"><span data-stu-id="2fc69-127">You can use the **Service Hours** window to set up specific service hours for the customer that owns the service contract.</span></span> <span data-ttu-id="2fc69-128">Service hours are used to calculate the response date and time for service orders and quotes that belong to the service contract.</span><span class="sxs-lookup"><span data-stu-id="2fc69-128">Service hours are used to calculate the response date and time for service orders and quotes that belong to the service contract.</span></span>  
  
<span data-ttu-id="2fc69-129">If you do not set up specific service hours for the service contract, the default service hours for service contracts are used.</span><span class="sxs-lookup"><span data-stu-id="2fc69-129">If you do not set up specific service hours for the service contract, the default service hours for service contracts are used.</span></span>  
  
1. <span data-ttu-id="2fc69-130">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Service Contracts**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="2fc69-130">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Service Contracts**, and then choose the related link.</span></span>  
2. <span data-ttu-id="2fc69-131">Open the service contract you want to set up specific service hours for, and choose **Service Hours**.</span><span class="sxs-lookup"><span data-stu-id="2fc69-131">Open the service contract you want to set up specific service hours for, and choose **Service Hours**.</span></span>  
4. <span data-ttu-id="2fc69-132">To set up service hours based on default service hours, choose the **Copy Default Service Hours** action.</span><span class="sxs-lookup"><span data-stu-id="2fc69-132">To set up service hours based on default service hours, choose the **Copy Default Service Hours** action.</span></span>  
5. <span data-ttu-id="2fc69-133">Edit the fields in the service hours entries.</span><span class="sxs-lookup"><span data-stu-id="2fc69-133">Edit the fields in the service hours entries.</span></span> <span data-ttu-id="2fc69-134">Insert or delete entries to set up the service hours for the contract.</span><span class="sxs-lookup"><span data-stu-id="2fc69-134">Insert or delete entries to set up the service hours for the contract.</span></span> <span data-ttu-id="2fc69-135">Note that the fields **Day**, **Starting Time** and **Ending Time** are required for each line.</span><span class="sxs-lookup"><span data-stu-id="2fc69-135">Note that the fields **Day**, **Starting Time** and **Ending Time** are required for each line.</span></span>  
6. <span data-ttu-id="2fc69-136">If you want the service hours to be valid from a specific date, fill in the **Starting Date** field.</span><span class="sxs-lookup"><span data-stu-id="2fc69-136">If you want the service hours to be valid from a specific date, fill in the **Starting Date** field.</span></span>  
7. <span data-ttu-id="2fc69-137">If you want the service hours to be valid on holidays, select the check box in the **Valid on Holidays** field.</span><span class="sxs-lookup"><span data-stu-id="2fc69-137">If you want the service hours to be valid on holidays, select the check box in the **Valid on Holidays** field.</span></span>  

## <a name="see-also"></a><span data-ttu-id="2fc69-138">See Also</span><span class="sxs-lookup"><span data-stu-id="2fc69-138">See Also</span></span>  
[<span data-ttu-id="2fc69-139">Understanding Allocation Status and Repair Status</span><span class="sxs-lookup"><span data-stu-id="2fc69-139">Understanding Allocation Status and Repair Status</span></span>](service-allocation-status-and-repair-status.md)  
[<span data-ttu-id="2fc69-140">Setting Up Service Management</span><span class="sxs-lookup"><span data-stu-id="2fc69-140">Setting Up Service Management</span></span>](service-setup-service.md)  
[<span data-ttu-id="2fc69-141">Understanding Service Order and Repair Status</span><span class="sxs-lookup"><span data-stu-id="2fc69-141">Understanding Service Order and Repair Status</span></span>](service-order-repair-status.md)  

