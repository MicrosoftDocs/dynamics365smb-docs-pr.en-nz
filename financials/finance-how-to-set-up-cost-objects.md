---
title: How to Set Up Cost Objects | Microsoft Docs
description: Learn how to set up cost objects, which are similar to dimensions for the general ledger.
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
ms.openlocfilehash: 45bfe558c8bdc1f7c0befc4c929e895c54b7d85f
ms.contentlocale: en-nz
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-set-up-cost-objects"></a><span data-ttu-id="bf63f-103">How to: Set Up Cost Objects</span><span class="sxs-lookup"><span data-stu-id="bf63f-103">How to: Set Up Cost Objects</span></span>
<span data-ttu-id="bf63f-104">Cost objects are projects, products, or services of a company.</span><span class="sxs-lookup"><span data-stu-id="bf63f-104">Cost objects are projects, products, or services of a company.</span></span> <span data-ttu-id="bf63f-105">The chart of cost objects is similar to the dimension information for the general ledger.</span><span class="sxs-lookup"><span data-stu-id="bf63f-105">The chart of cost objects is similar to the dimension information for the general ledger.</span></span> <span data-ttu-id="bf63f-106">You can set up the chart of cost objects in the following ways:</span><span class="sxs-lookup"><span data-stu-id="bf63f-106">You can set up the chart of cost objects in the following ways:</span></span>  

* <span data-ttu-id="bf63f-107">Transfer dimension values in the general ledger to the chart of cost objects.</span><span class="sxs-lookup"><span data-stu-id="bf63f-107">Transfer dimension values in the general ledger to the chart of cost objects.</span></span> <span data-ttu-id="bf63f-108">You can make any necessary adjustments after the transfer.</span><span class="sxs-lookup"><span data-stu-id="bf63f-108">You can make any necessary adjustments after the transfer.</span></span>  
* <span data-ttu-id="bf63f-109">Create a new chart of cost object that is independent of the general ledger or add a new cost object to an existing chart of cost objects.</span><span class="sxs-lookup"><span data-stu-id="bf63f-109">Create a new chart of cost object that is independent of the general ledger or add a new cost object to an existing chart of cost objects.</span></span> <span data-ttu-id="bf63f-110">You must create each cost object individually.</span><span class="sxs-lookup"><span data-stu-id="bf63f-110">You must create each cost object individually.</span></span>  

## <a name="to-transfer-dimension-values-from-the-general-ledger-to-the-chart-of-cost-objects"></a><span data-ttu-id="bf63f-111">To transfer dimension values from the general ledger to the chart of cost objects</span><span class="sxs-lookup"><span data-stu-id="bf63f-111">To transfer dimension values from the general ledger to the chart of cost objects</span></span>  
1.  <span data-ttu-id="bf63f-112">Set a dimension to be the cost object dimension in the **Update CA Dimensions** window.</span><span class="sxs-lookup"><span data-stu-id="bf63f-112">Set a dimension to be the cost object dimension in the **Update CA Dimensions** window.</span></span> <span data-ttu-id="bf63f-113">Only the values from this dimension are transferred.</span><span class="sxs-lookup"><span data-stu-id="bf63f-113">Only the values from this dimension are transferred.</span></span>  
2.  <span data-ttu-id="bf63f-114">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Chart of Cost Objects**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="bf63f-114">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Chart of Cost Objects**, and then choose the related link.</span></span>  
3.  <span data-ttu-id="bf63f-115">Choose the **Get Cost Objects from Dimension** action to transfer dimension values to the chart of cost objects.</span><span class="sxs-lookup"><span data-stu-id="bf63f-115">Choose the **Get Cost Objects from Dimension** action to transfer dimension values to the chart of cost objects.</span></span> <span data-ttu-id="bf63f-116">The function transfers the dimension values that you defined in step 1.</span><span class="sxs-lookup"><span data-stu-id="bf63f-116">The function transfers the dimension values that you defined in step 1.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="bf63f-117">You can set up the **Align Cost Object Dimension**  field to define a one-way synchronisation of dimension values from the general ledger to the chart of cost objects.</span><span class="sxs-lookup"><span data-stu-id="bf63f-117">You can set up the **Align Cost Object Dimension**  field to define a one-way synchronization of dimension values from the general ledger to the chart of cost objects.</span></span> <span data-ttu-id="bf63f-118">You cannot define a synchronisation of the chart of cost objects to dimension values from the general ledger.</span><span class="sxs-lookup"><span data-stu-id="bf63f-118">You cannot define a synchronization of the chart of cost objects to dimension values from the general ledger.</span></span>  

<span data-ttu-id="bf63f-119">The chart of cost objects now contains all specified dimension values from the general ledger and includes titles and subtotals.</span><span class="sxs-lookup"><span data-stu-id="bf63f-119">The chart of cost objects now contains all specified dimension values from the general ledger and includes titles and subtotals.</span></span>  

## <a name="to-create-new-cost-objects-in-the-chart-of-cost-objects-window"></a><span data-ttu-id="bf63f-120">To create new cost objects in the Chart of Cost Objects window</span><span class="sxs-lookup"><span data-stu-id="bf63f-120">To create new cost objects in the Chart of Cost Objects window</span></span>  
<span data-ttu-id="bf63f-121">You can set up and maintain cost objects in either the **Cost Object Card** card or in the **Chart of Cost Objects** window.</span><span class="sxs-lookup"><span data-stu-id="bf63f-121">You can set up and maintain cost objects in either the **Cost Object Card** card or in the **Chart of Cost Objects** window.</span></span> <span data-ttu-id="bf63f-122">In this procedure, you set up cost objects in the **Chart of Cost Objects** window.</span><span class="sxs-lookup"><span data-stu-id="bf63f-122">In this procedure, you set up cost objects in the **Chart of Cost Objects** window.</span></span>  

1.  <span data-ttu-id="bf63f-123">Open the **Chart of Cost Objects** window in edit mode.</span><span class="sxs-lookup"><span data-stu-id="bf63f-123">Open the **Chart of Cost Objects** window in edit mode.</span></span>  
2.  <span data-ttu-id="bf63f-124">In the **Code** field, enter the cost object code.</span><span class="sxs-lookup"><span data-stu-id="bf63f-124">In the **Code** field, enter the cost object code.</span></span> <span data-ttu-id="bf63f-125">All cost objects must have a code.</span><span class="sxs-lookup"><span data-stu-id="bf63f-125">All cost objects must have a code.</span></span>  
3.  <span data-ttu-id="bf63f-126">In the **Name** field, enter the cost object name.</span><span class="sxs-lookup"><span data-stu-id="bf63f-126">In the **Name** field, enter the cost object name.</span></span>  
4.  <span data-ttu-id="bf63f-127">Choose the drop-down arrow in the **Line Type** field to specify the purpose of the cost object.</span><span class="sxs-lookup"><span data-stu-id="bf63f-127">Choose the drop-down arrow in the **Line Type** field to specify the purpose of the cost object.</span></span>  

    * <span data-ttu-id="bf63f-128">For cost objects of the **Total** line type, fill in the **Total From/To** field.</span><span class="sxs-lookup"><span data-stu-id="bf63f-128">For cost objects of the **Total** line type, fill in the **Total From/To** field.</span></span> <span data-ttu-id="bf63f-129">Use the **or** operator, which is a vertical line (**&#124;**), to set ranges of cost objects.</span><span class="sxs-lookup"><span data-stu-id="bf63f-129">Use the **or** operator, which is a vertical line (**&#124;**), to set ranges of cost objects.</span></span>  
    * <span data-ttu-id="bf63f-130">For cost objects of the **End-Total** line type, this field is filled in automatically when you use  the indent function.</span><span class="sxs-lookup"><span data-stu-id="bf63f-130">For cost objects of the **End-Total** line type, this field is filled in automatically when you use  the indent function.</span></span>  
5.  <span data-ttu-id="bf63f-131">Fill in the **Sorting Order** field.</span><span class="sxs-lookup"><span data-stu-id="bf63f-131">Fill in the **Sorting Order** field.</span></span>  
6.  <span data-ttu-id="bf63f-132">Chose the next empty line to create a new cost object, and then repeat steps 2 through 5.</span><span class="sxs-lookup"><span data-stu-id="bf63f-132">Chose the next empty line to create a new cost object, and then repeat steps 2 through 5.</span></span>  
7.  <span data-ttu-id="bf63f-133">After you have set up all the cost objects, choose the **Indent Cost Objects** action.</span><span class="sxs-lookup"><span data-stu-id="bf63f-133">After you have set up all the cost objects, choose the **Indent Cost Objects** action.</span></span> <span data-ttu-id="bf63f-134">Choose the **Yes** button.</span><span class="sxs-lookup"><span data-stu-id="bf63f-134">Choose the **Yes** button.</span></span>  

> [!IMPORTANT]  
>  <span data-ttu-id="bf63f-135">If you have entered definitions in the **Total From/To** fields for **End-Total** cost objects before you run the indent function, then you must enter them again.</span><span class="sxs-lookup"><span data-stu-id="bf63f-135">If you have entered definitions in the **Total From/To** fields for **End-Total** cost objects before you run the indent function, then you must enter them again.</span></span> <span data-ttu-id="bf63f-136">The function overwrites the values in all **End-Total** fields.</span><span class="sxs-lookup"><span data-stu-id="bf63f-136">The function overwrites the values in all **End-Total** fields.</span></span>  

## <a name="see-also"></a><span data-ttu-id="bf63f-137">See Also</span><span class="sxs-lookup"><span data-stu-id="bf63f-137">See Also</span></span>  
[<span data-ttu-id="bf63f-138">Accounting for Costs</span><span class="sxs-lookup"><span data-stu-id="bf63f-138">Accounting for Costs</span></span>](finance-manage-cost-accounting.md)  
<span data-ttu-id="bf63f-139">[Defining Cost Centres and Cost Objects for Chart of Accounts](finance-defining-cost-centers-and-cost-objects-for-chart-of-accounts.md) </span><span class="sxs-lookup"><span data-stu-id="bf63f-139">[Defining Cost Centers and Cost Objects for Chart of Accounts](finance-defining-cost-centers-and-cost-objects-for-chart-of-accounts.md) </span></span>  
<span data-ttu-id="bf63f-140">[Balances Between Cost Type, Cost Centre, and Cost Object](finance-balances-between-cost-type-cost-center-and-cost-object.md) </span><span class="sxs-lookup"><span data-stu-id="bf63f-140">[Balances Between Cost Type, Cost Center, and Cost Object](finance-balances-between-cost-type-cost-center-and-cost-object.md) </span></span>  
<span data-ttu-id="bf63f-141">[Setting Up Cost Accounting](finance-set-up-cost-accounting.md) </span><span class="sxs-lookup"><span data-stu-id="bf63f-141">[Setting Up Cost Accounting](finance-set-up-cost-accounting.md) </span></span>  
<span data-ttu-id="bf63f-142">[Terminology in Cost Accounting](finance-terminology-in-cost-accounting.md) </span><span class="sxs-lookup"><span data-stu-id="bf63f-142">[Terminology in Cost Accounting](finance-terminology-in-cost-accounting.md) </span></span>  
[<span data-ttu-id="bf63f-143">About Cost Accounting</span><span class="sxs-lookup"><span data-stu-id="bf63f-143">About Cost Accounting</span></span>](finance-about-cost-accounting.md)  
<span data-ttu-id="bf63f-144">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="bf63f-144">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

