---
title: Set Up and Publish KPI Web Services for Account Schedules | Microsoft Docs
description: In the **Account Schedule KPI Web Service Setup** window, you set up how to show the account-schedule KPI data and which specific account schedules to base the KPIs on.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/08/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: dc1226724d1f953a3cf14a148e6d229ac0736bd3
ms.contentlocale: en-nz
ms.lasthandoff: 03/22/2018

---
# <a name="set-up-and-publish-kpi-web-services-based-on-account-schedules"></a><span data-ttu-id="5774b-103">Set Up and Publish KPI Web Services Based on Account Schedules</span><span class="sxs-lookup"><span data-stu-id="5774b-103">Set Up and Publish KPI Web Services Based on Account Schedules</span></span>
<span data-ttu-id="5774b-104">In the **Account Schedule KPI Web Service Setup** window, you set up how to show the account-schedule KPI data and which specific account schedules to base the KPIs on.</span><span class="sxs-lookup"><span data-stu-id="5774b-104">In the **Account Schedule KPI Web Service Setup** window, you set up how to show the account-schedule KPI data and which specific account schedules to base the KPIs on.</span></span> <span data-ttu-id="5774b-105">When you choose the **Publish Web Service** button, the specified account-schedule KPI data is added to the list of published web services in the **Web Services** window.</span><span class="sxs-lookup"><span data-stu-id="5774b-105">When you choose the **Publish Web Service** button, the specified account-schedule KPI data is added to the list of published web services in the **Web Services** window.</span></span>  

## <a name="to-set-up-and-publish-a-kpi-web-service-that-is-based-on-account-schedules"></a><span data-ttu-id="5774b-106">To set up and publish a KPI web service that is based on account schedules</span><span class="sxs-lookup"><span data-stu-id="5774b-106">To set up and publish a KPI web service that is based on account schedules</span></span>  

1.  <span data-ttu-id="5774b-107">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Account Schedule KPI Web Service Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="5774b-107">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Account Schedule KPI Web Service Setup**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="5774b-108">On the **General** FastTab, fill in the fields as described in the following table.</span><span class="sxs-lookup"><span data-stu-id="5774b-108">On the **General** FastTab, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="5774b-109">Field</span><span class="sxs-lookup"><span data-stu-id="5774b-109">Field</span></span>|<span data-ttu-id="5774b-110">Description</span><span class="sxs-lookup"><span data-stu-id="5774b-110">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="5774b-111">**Forecasted Values Start**</span><span class="sxs-lookup"><span data-stu-id="5774b-111">**Forecasted Values Start**</span></span>|<span data-ttu-id="5774b-112">Specify at what point in time forecasted values are shown on the account-schedule KPI graphic.</span><span class="sxs-lookup"><span data-stu-id="5774b-112">Specify at what point in time forecasted values are shown on the account-schedule KPI graphic.</span></span><br /><br /> <span data-ttu-id="5774b-113">The forecasted values are retrieved from the general ledger budget that you select in the **G/L Budget Name** field.</span><span class="sxs-lookup"><span data-stu-id="5774b-113">The forecasted values are retrieved from the general ledger budget that you select in the **G/L Budget Name** field.</span></span> <span data-ttu-id="5774b-114">**Note:**  To obtain KPIs that show forecasted figures after a certain date and actual figures before the date, you can change the **Allow Posting From** field in the **General Ledger Setup** window.</span><span class="sxs-lookup"><span data-stu-id="5774b-114">**Note:**  To obtain KPIs that show forecasted figures after a certain date and actual figures before the date, you can change the **Allow Posting From** field in the **General Ledger Setup** window.</span></span> <span data-ttu-id="5774b-115">For more information, see Allow Posting From.</span><span class="sxs-lookup"><span data-stu-id="5774b-115">For more information, see Allow Posting From.</span></span>|  
    |<span data-ttu-id="5774b-116">**G/L Budget Name**</span><span class="sxs-lookup"><span data-stu-id="5774b-116">**G/L Budget Name**</span></span>|<span data-ttu-id="5774b-117">Specify the name of the general ledger budget that provides forecasted values to the account-schedule KPI web service.</span><span class="sxs-lookup"><span data-stu-id="5774b-117">Specify the name of the general ledger budget that provides forecasted values to the account-schedule KPI web service.</span></span>|  
    |<span data-ttu-id="5774b-118">**Period**</span><span class="sxs-lookup"><span data-stu-id="5774b-118">**Period**</span></span>|<span data-ttu-id="5774b-119">Specify the period that the account-schedule KPI web service is based on.</span><span class="sxs-lookup"><span data-stu-id="5774b-119">Specify the period that the account-schedule KPI web service is based on.</span></span>|  
    |<span data-ttu-id="5774b-120">**View By**</span><span class="sxs-lookup"><span data-stu-id="5774b-120">**View By**</span></span>|<span data-ttu-id="5774b-121">Specify which time interval the account-schedule KPI is shown in.</span><span class="sxs-lookup"><span data-stu-id="5774b-121">Specify which time interval the account-schedule KPI is shown in.</span></span>|  
    |<span data-ttu-id="5774b-122">**Web Service Name**</span><span class="sxs-lookup"><span data-stu-id="5774b-122">**Web Service Name**</span></span>|<span data-ttu-id="5774b-123">Specify the name of the account-schedule KPI web service.</span><span class="sxs-lookup"><span data-stu-id="5774b-123">Specify the name of the account-schedule KPI web service.</span></span><br /><br /> <span data-ttu-id="5774b-124">This name will appear in the **Service Name** field in the **Web Services** window.</span><span class="sxs-lookup"><span data-stu-id="5774b-124">This name will appear in the **Service Name** field in the **Web Services** window.</span></span>|  

    <span data-ttu-id="5774b-125">Proceed to specify one or more account schedules that you want to publish as a KPI web service according to the setup that you made in the previous table.</span><span class="sxs-lookup"><span data-stu-id="5774b-125">Proceed to specify one or more account schedules that you want to publish as a KPI web service according to the setup that you made in the previous table.</span></span>  

3.  <span data-ttu-id="5774b-126">On the **Account Schedules** FastTab, fill in the fields as described in the following table.</span><span class="sxs-lookup"><span data-stu-id="5774b-126">On the **Account Schedules** FastTab, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="5774b-127">Field</span><span class="sxs-lookup"><span data-stu-id="5774b-127">Field</span></span>|<span data-ttu-id="5774b-128">Description</span><span class="sxs-lookup"><span data-stu-id="5774b-128">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="5774b-129">**Acc. Schedule Name**</span><span class="sxs-lookup"><span data-stu-id="5774b-129">**Acc. Schedule Name**</span></span>|<span data-ttu-id="5774b-130">Specify the account schedule that the KPI web service is based on.</span><span class="sxs-lookup"><span data-stu-id="5774b-130">Specify the account schedule that the KPI web service is based on.</span></span>|  
    |<span data-ttu-id="5774b-131">**Acc. Schedule Description**</span><span class="sxs-lookup"><span data-stu-id="5774b-131">**Acc. Schedule Description**</span></span>|<span data-ttu-id="5774b-132">Specify the description of the account schedule that the KPI web service is based on.</span><span class="sxs-lookup"><span data-stu-id="5774b-132">Specify the description of the account schedule that the KPI web service is based on.</span></span>|  

4.  <span data-ttu-id="5774b-133">Repeat step 3 for all the account schedules that you want to base the account-schedule KPI web service on.</span><span class="sxs-lookup"><span data-stu-id="5774b-133">Repeat step 3 for all the account schedules that you want to base the account-schedule KPI web service on.</span></span>  
5.  <span data-ttu-id="5774b-134">To view or edit the selected account schedule, on the **Account Schedule** FastTab, choose the **Edit Account Schedule** action.</span><span class="sxs-lookup"><span data-stu-id="5774b-134">To view or edit the selected account schedule, on the **Account Schedule** FastTab, choose the **Edit Account Schedule** action.</span></span>  
6.  <span data-ttu-id="5774b-135">To view the account-schedule KPI data that you have set up, choose the **Account Schedule KPI Web Service** action.</span><span class="sxs-lookup"><span data-stu-id="5774b-135">To view the account-schedule KPI data that you have set up, choose the **Account Schedule KPI Web Service** action.</span></span>  
7.  <span data-ttu-id="5774b-136">To publish the account-schedule KPI web service, choose the **Publish Web Service** action.</span><span class="sxs-lookup"><span data-stu-id="5774b-136">To publish the account-schedule KPI web service, choose the **Publish Web Service** action.</span></span> <span data-ttu-id="5774b-137">The web service is added to the list of published web services in the **Web Services** window.</span><span class="sxs-lookup"><span data-stu-id="5774b-137">The web service is added to the list of published web services in the **Web Services** window.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="5774b-138">You can also publish the KPI web service by pointing to the **Account Schedule KPI Web Service Setup** page object from the **Web Services** window.</span><span class="sxs-lookup"><span data-stu-id="5774b-138">You can also publish the KPI web service by pointing to the **Account Schedule KPI Web Service Setup** page object from the **Web Services** window.</span></span> <span data-ttu-id="5774b-139">For more information, see [Publish a Web Service](across-how-publish-web-service.md).</span><span class="sxs-lookup"><span data-stu-id="5774b-139">For more information, see [Publish a Web Service](across-how-publish-web-service.md).</span></span>  

## <a name="see-also"></a><span data-ttu-id="5774b-140">See Also</span><span class="sxs-lookup"><span data-stu-id="5774b-140">See Also</span></span>  
[<span data-ttu-id="5774b-141">Business Intelligence</span><span class="sxs-lookup"><span data-stu-id="5774b-141">Business Intelligence</span></span>](bi.md)  
[<span data-ttu-id="5774b-142">Finance</span><span class="sxs-lookup"><span data-stu-id="5774b-142">Finance</span></span>](finance.md)  
[<span data-ttu-id="5774b-143">Setting Up Finance</span><span class="sxs-lookup"><span data-stu-id="5774b-143">Setting Up Finance</span></span>](finance-setup-finance.md)  
[<span data-ttu-id="5774b-144">The General Ledger and the Chart of Accounts</span><span class="sxs-lookup"><span data-stu-id="5774b-144">The General Ledger and the Chart of Accounts</span></span>](finance-general-ledger.md)  
<span data-ttu-id="5774b-145">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="5774b-145">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

