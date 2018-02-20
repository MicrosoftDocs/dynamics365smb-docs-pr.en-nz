---
title: Scenario Example - Defining Dynamic Allocations Based on Items Sold | Microsoft Docs
description: This topic shows an example of how to define allocations by using the dynamic allocation method.
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
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: d8622d11cd23e506d1b85b18dbe5facb740c7753
ms.contentlocale: en-nz
ms.lasthandoff: 01/30/2018

---
# <a name="scenario-example-defining-dynamic-allocations-based-on-items-sold"></a><span data-ttu-id="a6c79-103">Scenario Example: Defining Dynamic Allocations Based on Items Sold</span><span class="sxs-lookup"><span data-stu-id="a6c79-103">Scenario Example: Defining Dynamic Allocations Based on Items Sold</span></span>
<span data-ttu-id="a6c79-104">This topic shows an example of how to define allocations by using the dynamic allocation method.</span><span class="sxs-lookup"><span data-stu-id="a6c79-104">This topic shows an example of how to define allocations by using the dynamic allocation method.</span></span> <span data-ttu-id="a6c79-105">In the example, you change the dynamic allocation of the costs for the SALES cost centre to support the new cost object IT EQUIPMENT.</span><span class="sxs-lookup"><span data-stu-id="a6c79-105">In the example, you change the dynamic allocation of the costs for the SALES cost center to support the new cost object IT EQUIPMENT.</span></span> <span data-ttu-id="a6c79-106">IT EQUIPMENT packages have item numbers in the range from 8904-W to 8924-W.</span><span class="sxs-lookup"><span data-stu-id="a6c79-106">IT EQUIPMENT packages have item numbers in the range from 8904-W to 8924-W.</span></span> <span data-ttu-id="a6c79-107">You use the previous year’s sales figures to calculate the share.</span><span class="sxs-lookup"><span data-stu-id="a6c79-107">You use the previous year’s sales figures to calculate the share.</span></span> <span data-ttu-id="a6c79-108">The allocation is posted to the helping cost type 9903.</span><span class="sxs-lookup"><span data-stu-id="a6c79-108">The allocation is posted to the helping cost type 9903.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="a6c79-109">The example uses the demo data in the [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="a6c79-109">The example uses the demo data in the [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  

## <a name="to-define-dynamic-allocations-based-on-items-sold-in-the-previous-year"></a><span data-ttu-id="a6c79-110">To define dynamic allocations based on items sold in the previous year</span><span class="sxs-lookup"><span data-stu-id="a6c79-110">To define dynamic allocations based on items sold in the previous year</span></span>  

1.  <span data-ttu-id="a6c79-111">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Cost Allocations**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="a6c79-111">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Cost Allocations**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="a6c79-112">In the **Cost Allocation** window, choose the **New** action.</span><span class="sxs-lookup"><span data-stu-id="a6c79-112">In the **Cost Allocation** window, choose the **New** action.</span></span>  
3.  <span data-ttu-id="a6c79-113">In the **ID** field, press Enter or enter an ID.</span><span class="sxs-lookup"><span data-stu-id="a6c79-113">In the **ID** field, press Enter or enter an ID.</span></span>  
4.  <span data-ttu-id="a6c79-114">In the **Level** field, enter **1**.</span><span class="sxs-lookup"><span data-stu-id="a6c79-114">In the **Level** field, enter **1**.</span></span>  
5.  <span data-ttu-id="a6c79-115">In the **Valid From** and **Valid To** fields, enter appropriate dates.</span><span class="sxs-lookup"><span data-stu-id="a6c79-115">In the **Valid From** and **Valid To** fields, enter appropriate dates.</span></span>  
6.  <span data-ttu-id="a6c79-116">In the **Cost Centre Code** field, enter **SALES**.</span><span class="sxs-lookup"><span data-stu-id="a6c79-116">In the **Cost Center Code** field, enter **SALES**.</span></span>  
7.  <span data-ttu-id="a6c79-117">In the **Credit to Cost Type** field, enter the cost type **9903**.</span><span class="sxs-lookup"><span data-stu-id="a6c79-117">In the **Credit to Cost Type** field, enter the cost type **9903**.</span></span>  
8.  <span data-ttu-id="a6c79-118">In the **Target Cost Type** field, enter the cost type **9903**.</span><span class="sxs-lookup"><span data-stu-id="a6c79-118">In the **Target Cost Type** field, enter the cost type **9903**.</span></span>  
9. <span data-ttu-id="a6c79-119">In the **Target Cost Object** field, choose **New** to create a new cost object IT EQUIPMENT and fill in fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="a6c79-119">In the **Target Cost Object** field, choose **New** to create a new cost object IT EQUIPMENT and fill in fields as necessary.</span></span> <span data-ttu-id="a6c79-120">Select **IT EQUIPMENT**.</span><span class="sxs-lookup"><span data-stu-id="a6c79-120">Select **IT EQUIPMENT**.</span></span> <span data-ttu-id="a6c79-121">Leave the **Target Cost Centre** field blank.</span><span class="sxs-lookup"><span data-stu-id="a6c79-121">Leave the **Target Cost Center** field blank.</span></span>  
10. <span data-ttu-id="a6c79-122">In the **Allocation Target Type** field, select **All Costs** to define how all accumulated costs are allocated.</span><span class="sxs-lookup"><span data-stu-id="a6c79-122">In the **Allocation Target Type** field, select **All Costs** to define how all accumulated costs are allocated.</span></span>  
11. <span data-ttu-id="a6c79-123">In the **Base** field, select the allocation base **Items Sold (Amount)**.</span><span class="sxs-lookup"><span data-stu-id="a6c79-123">In the **Base** field, select the allocation base **Items Sold (Amount)**.</span></span>  
12. <span data-ttu-id="a6c79-124">In the **No. Filter** field, enter **8904-W..8924-W**.</span><span class="sxs-lookup"><span data-stu-id="a6c79-124">In the **No. Filter** field, enter **8904-W..8924-W**.</span></span>  
13. <span data-ttu-id="a6c79-125">In the **Date Filter Code** field, enter **Last Year**.</span><span class="sxs-lookup"><span data-stu-id="a6c79-125">In the **Date Filter Code** field, enter **Last Year**.</span></span>  
14. <span data-ttu-id="a6c79-126">Choose the **Calculate Allocation Key** action to calculate the share.</span><span class="sxs-lookup"><span data-stu-id="a6c79-126">Choose the **Calculate Allocation Key** action to calculate the share.</span></span>  

    > [!IMPORTANT]  
    >  [!INCLUDE[d365fin](includes/d365fin_md.md)] <span data-ttu-id="a6c79-127"> uses the previous years’ sales figures to calculate a share of 1596.50 LCY with 100 percent for the IT EQUIPMENT packages.</span><span class="sxs-lookup"><span data-stu-id="a6c79-127">uses the previous years’ sales figures to calculate a share of 1596.50 LCY with 100 percent for the IT EQUIPMENT packages.</span></span> <span data-ttu-id="a6c79-128">This means that all of the items sold last year will be allocated to the cost object IT EQUIPMENT.</span><span class="sxs-lookup"><span data-stu-id="a6c79-128">This means that all of the items sold last year will be allocated to the cost object IT EQUIPMENT.</span></span>  

## <a name="see-also"></a><span data-ttu-id="a6c79-129">See Also</span><span class="sxs-lookup"><span data-stu-id="a6c79-129">See Also</span></span>  
 <span data-ttu-id="a6c79-130">[Setting Filters for Dynamic Allocation Bases](finance-setting-filters-for-dynamic-allocation-bases.md) </span><span class="sxs-lookup"><span data-stu-id="a6c79-130">[Setting Filters for Dynamic Allocation Bases](finance-setting-filters-for-dynamic-allocation-bases.md) </span></span>  
 <span data-ttu-id="a6c79-131">[Set Up Allocation Source and Targets](finance-how-to-set-up-allocation-source-and-targets.md) </span><span class="sxs-lookup"><span data-stu-id="a6c79-131">[Set Up Allocation Source and Targets](finance-how-to-set-up-allocation-source-and-targets.md) </span></span>  
 <span data-ttu-id="a6c79-132">[Defining and Allocating Costs](finance-define-and-allocate-costs.md) </span><span class="sxs-lookup"><span data-stu-id="a6c79-132">[Defining and Allocating Costs](finance-define-and-allocate-costs.md) </span></span>  
 <span data-ttu-id="a6c79-133">[Terminology in Cost Accounting](finance-terminology-in-cost-accounting.md) </span><span class="sxs-lookup"><span data-stu-id="a6c79-133">[Terminology in Cost Accounting](finance-terminology-in-cost-accounting.md) </span></span>  
 [<span data-ttu-id="a6c79-134">About Cost Accounting</span><span class="sxs-lookup"><span data-stu-id="a6c79-134">About Cost Accounting</span></span>](finance-about-cost-accounting.md)

