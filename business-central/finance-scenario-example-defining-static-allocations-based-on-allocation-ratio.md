---
title: Defining Static Allocations Based on Allocation Ratio | Microsoft Docs
description: Static allocation method is based on a definite value, such as square meters used, or an established allocation ratio such as 5:2:4.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: 036aa1f317c1b1de7fc1548e03d40eca8c25be89
ms.contentlocale: en-nz
ms.lasthandoff: 09/28/2018

---
# <a name="scenario-example-defining-static-allocations-based-on-allocation-ratio"></a><span data-ttu-id="8b2b1-103">Scenario Example: Defining Static Allocations Based on Allocation Ratio</span><span class="sxs-lookup"><span data-stu-id="8b2b1-103">Scenario Example: Defining Static Allocations Based on Allocation Ratio</span></span>
<span data-ttu-id="8b2b1-104">Static allocation method is based on a definite value, such as square meters used, or an established allocation ratio such as 5:2:4.</span><span class="sxs-lookup"><span data-stu-id="8b2b1-104">Static allocation method is based on a definite value, such as square meters used, or an established allocation ratio such as 5:2:4.</span></span>  

<span data-ttu-id="8b2b1-105">This topic describes how to define three new allocation target cost objects for the allocation source PROD cost centre using the established allocation ratio 5:2:4.</span><span class="sxs-lookup"><span data-stu-id="8b2b1-105">This topic describes how to define three new allocation target cost objects for the allocation source PROD cost center using the established allocation ratio 5:2:4.</span></span> <span data-ttu-id="8b2b1-106">The three target cost objects are ACCESSO, PAINT, and FITTINGS.</span><span class="sxs-lookup"><span data-stu-id="8b2b1-106">The three target cost objects are ACCESSO, PAINT, and FITTINGS.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="8b2b1-107">The example uses the demo data in the [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="8b2b1-107">The example uses the demo data in the [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  

## <a name="to-define-the-allocation-source-prod-cost-center-on-the-general-fasttab"></a><span data-ttu-id="8b2b1-108">To define the allocation source PROD cost centre on the General FastTab</span><span class="sxs-lookup"><span data-stu-id="8b2b1-108">To define the allocation source PROD cost center on the General FastTab</span></span>  

1.  <span data-ttu-id="8b2b1-109">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Cost Allocation**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="8b2b1-109">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Cost Allocation**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="8b2b1-110">In the **Cost Allocation** window, choose the **New** action.</span><span class="sxs-lookup"><span data-stu-id="8b2b1-110">In the **Cost Allocation** window, choose the **New** action.</span></span>  
3.  <span data-ttu-id="8b2b1-111">In the **ID** field, press Enter or enter an ID.</span><span class="sxs-lookup"><span data-stu-id="8b2b1-111">In the **ID** field, press Enter or enter an ID.</span></span>  
4.  <span data-ttu-id="8b2b1-112">In the **Level** field, enter **1**.</span><span class="sxs-lookup"><span data-stu-id="8b2b1-112">In the **Level** field, enter **1**.</span></span>  
5.  <span data-ttu-id="8b2b1-113">In the **Valid From** and **Valid To** fields, enter appropriate dates.</span><span class="sxs-lookup"><span data-stu-id="8b2b1-113">In the **Valid From** and **Valid To** fields, enter appropriate dates.</span></span>  
6.  <span data-ttu-id="8b2b1-114">In the **Cost Centre Code** field, enter **PROD**.</span><span class="sxs-lookup"><span data-stu-id="8b2b1-114">In the **Cost Center Code** field, enter **PROD**.</span></span>  
7.  <span data-ttu-id="8b2b1-115">In the **Credit to Cost Type** field, enter the cost type **9903**.</span><span class="sxs-lookup"><span data-stu-id="8b2b1-115">In the **Credit to Cost Type** field, enter the cost type **9903**.</span></span>  

## <a name="to-define-the-allocation-target-cost-objects-on-the-lines-fasttab"></a><span data-ttu-id="8b2b1-116">To define the allocation target cost objects on the Lines FastTab</span><span class="sxs-lookup"><span data-stu-id="8b2b1-116">To define the allocation target cost objects on the Lines FastTab</span></span>  

1.  <span data-ttu-id="8b2b1-117">On the first line, in the **Target Cost Type** field, enter **9903**.</span><span class="sxs-lookup"><span data-stu-id="8b2b1-117">On the first line, in the **Target Cost Type** field, enter **9903**.</span></span>  
2.  <span data-ttu-id="8b2b1-118">On the first line, in the **Target Cost Object** field, select **ACCESSO**.</span><span class="sxs-lookup"><span data-stu-id="8b2b1-118">On the first line, in the **Target Cost Object** field, select **ACCESSO**.</span></span>  
3.  <span data-ttu-id="8b2b1-119">On the first line, in the **Allocation Target Type** field, select **All Costs** to define how all accrued costs are allocated.</span><span class="sxs-lookup"><span data-stu-id="8b2b1-119">On the first line, in the **Allocation Target Type** field, select **All Costs** to define how all accrued costs are allocated.</span></span>  
4.  <span data-ttu-id="8b2b1-120">On the first line, in the **Base** field, select **Static** to use the static allocation method.</span><span class="sxs-lookup"><span data-stu-id="8b2b1-120">On the first line, in the **Base** field, select **Static** to use the static allocation method.</span></span>  
5.  <span data-ttu-id="8b2b1-121">On the first line, in the **Share** field, enter the allocation ratio **5**.</span><span class="sxs-lookup"><span data-stu-id="8b2b1-121">On the first line, in the **Share** field, enter the allocation ratio **5**.</span></span>  
6.  <span data-ttu-id="8b2b1-122">On the second line, in the **Target Cost Type** field, enter **9903**.</span><span class="sxs-lookup"><span data-stu-id="8b2b1-122">On the second line, in the **Target Cost Type** field, enter **9903**.</span></span>  
7.  <span data-ttu-id="8b2b1-123">On the second line, in the **Target Cost Object** field, select **PAINT**.</span><span class="sxs-lookup"><span data-stu-id="8b2b1-123">On the second line, in the **Target Cost Object** field, select **PAINT**.</span></span>  
8.  <span data-ttu-id="8b2b1-124">On the second line, in the **Allocation Target Type** field, select **All Costs** to define how all accrued costs are allocated.</span><span class="sxs-lookup"><span data-stu-id="8b2b1-124">On the second line, in the **Allocation Target Type** field, select **All Costs** to define how all accrued costs are allocated.</span></span>  
9. <span data-ttu-id="8b2b1-125">On the second line, in the **Base** field, select **Static** to use the static allocation method.</span><span class="sxs-lookup"><span data-stu-id="8b2b1-125">On the second line, in the **Base** field, select **Static** to use the static allocation method.</span></span>  
10. <span data-ttu-id="8b2b1-126">On the second line, in the **Share** field, enter the allocation ratio **2**.</span><span class="sxs-lookup"><span data-stu-id="8b2b1-126">On the second line, in the **Share** field, enter the allocation ratio **2**.</span></span>  
11. <span data-ttu-id="8b2b1-127">On the third line, in the **Target Cost Type** field, enter **9903**.</span><span class="sxs-lookup"><span data-stu-id="8b2b1-127">On the third line, in the **Target Cost Type** field, enter **9903**.</span></span>  
12. <span data-ttu-id="8b2b1-128">On the third line, in the **Target Cost Object** field, select **FITTINGS**.</span><span class="sxs-lookup"><span data-stu-id="8b2b1-128">On the third line, in the **Target Cost Object** field, select **FITTINGS**.</span></span>  
13. <span data-ttu-id="8b2b1-129">On the third line, in the **Allocation Target Type** field, select **All Costs** to define how all accrued costs are allocated.</span><span class="sxs-lookup"><span data-stu-id="8b2b1-129">On the third line, in the **Allocation Target Type** field, select **All Costs** to define how all accrued costs are allocated.</span></span>  
14. <span data-ttu-id="8b2b1-130">On the third line, in the **Base** field, select **Static** to use the static allocation method.</span><span class="sxs-lookup"><span data-stu-id="8b2b1-130">On the third line, in the **Base** field, select **Static** to use the static allocation method.</span></span>  
15. <span data-ttu-id="8b2b1-131">On the third line, in the **Share** field, enter the allocation ratio **4**.</span><span class="sxs-lookup"><span data-stu-id="8b2b1-131">On the third line, in the **Share** field, enter the allocation ratio **4**.</span></span>  

> [!IMPORTANT]  
>  [!INCLUDE[d365fin](includes/d365fin_md.md)] <span data-ttu-id="8b2b1-132">automatically calculates the **Percent** field using a percentage rate that is dependent on all three allocation ratios that are entered in the **Share** field for all three lines.</span><span class="sxs-lookup"><span data-stu-id="8b2b1-132">automatically calculates the **Percent** field using a percentage rate that is dependent on all three allocation ratios that are entered in the **Share** field for all three lines.</span></span>  

## <a name="see-also"></a><span data-ttu-id="8b2b1-133">See Also</span><span class="sxs-lookup"><span data-stu-id="8b2b1-133">See Also</span></span>  
<span data-ttu-id="8b2b1-134">[Set Up Allocation Source and Targets](finance-how-to-set-up-allocation-source-and-targets.md) </span><span class="sxs-lookup"><span data-stu-id="8b2b1-134">[Set Up Allocation Source and Targets](finance-how-to-set-up-allocation-source-and-targets.md) </span></span>  
<span data-ttu-id="8b2b1-135">[Defining and Allocating Costs](finance-define-and-allocate-costs.md) </span><span class="sxs-lookup"><span data-stu-id="8b2b1-135">[Defining and Allocating Costs](finance-define-and-allocate-costs.md) </span></span>  
<span data-ttu-id="8b2b1-136">[Scenario Example: Defining Dynamic Allocations Based on Items Sold](finance-scenario-example-defining-dynamic-allocations-based-on-items-sold.md) </span><span class="sxs-lookup"><span data-stu-id="8b2b1-136">[Scenario Example: Defining Dynamic Allocations Based on Items Sold](finance-scenario-example-defining-dynamic-allocations-based-on-items-sold.md) </span></span>  
[<span data-ttu-id="8b2b1-137">Defining and Allocating Costs</span><span class="sxs-lookup"><span data-stu-id="8b2b1-137">Defining and Allocating Costs</span></span>](finance-define-and-allocate-costs.md)

