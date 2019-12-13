---
title: How to Plan Project Orders | Microsoft Docs
description: This planning task starts from a sales order and uses the **Sales Order Planning** page. Once you have created a project production order, you can plan it further by using the **Order Planning** page.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2019
ms.author: sgroespe
ms.openlocfilehash: c090843a5adcca7fcdb5ba857ca06172a805fe90
ms.sourcegitcommit: cfc92eefa8b06fb426482f54e393f0e6e222f712
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 12/03/2019
ms.locfileid: "2877775"
---
# <a name="plan-project-orders"></a><span data-ttu-id="6f84f-104">Plan Project Orders</span><span class="sxs-lookup"><span data-stu-id="6f84f-104">Plan Project Orders</span></span>
<span data-ttu-id="6f84f-105">This planning task starts from a sales order and uses the **Sales Order Planning** page.</span><span class="sxs-lookup"><span data-stu-id="6f84f-105">This planning task starts from a sales order and uses the **Sales Order Planning** page.</span></span> <span data-ttu-id="6f84f-106">Once you have created a project production order, you can plan it further by using the **Order Planning** page.</span><span class="sxs-lookup"><span data-stu-id="6f84f-106">Once you have created a project production order, you can plan it further by using the **Order Planning** page.</span></span>  

## <a name="to-create-a-project-production-order"></a><span data-ttu-id="6f84f-107">To create a project production order</span><span class="sxs-lookup"><span data-stu-id="6f84f-107">To create a project production order</span></span>  

1.  <span data-ttu-id="6f84f-108">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="6f84f-108">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="6f84f-109">Select the sales order that represents the production project, and then choose the **Planning** action.</span><span class="sxs-lookup"><span data-stu-id="6f84f-109">Select the sales order that represents the production project, and then choose the **Planning** action.</span></span>  
4.  <span data-ttu-id="6f84f-110">On the **Sales Order Planning** page, choose  the **Create Prod. Order** action.</span><span class="sxs-lookup"><span data-stu-id="6f84f-110">On the **Sales Order Planning** page, choose  the **Create Prod. Order** action.</span></span>  
5.  <span data-ttu-id="6f84f-111">On the **Create Order from Sales** page, in the **Order Type** field, select **Project Order**.</span><span class="sxs-lookup"><span data-stu-id="6f84f-111">On the **Create Order from Sales** page, in the **Order Type** field, select **Project Order**.</span></span>  
6.  <span data-ttu-id="6f84f-112">Choose the **Yes** button.</span><span class="sxs-lookup"><span data-stu-id="6f84f-112">Choose the **Yes** button.</span></span>  
7.  <span data-ttu-id="6f84f-113">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Production Orders**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="6f84f-113">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Production Orders**, and then choose the related link.</span></span>
8. <span data-ttu-id="6f84f-114">Open the production order just created.</span><span class="sxs-lookup"><span data-stu-id="6f84f-114">Open the production order just created.</span></span>  

    <span data-ttu-id="6f84f-115">Notice that the **Source Type** field of the production order contains **Sales Header** and the order has multiple lines, one for each sales line item that must be produced.</span><span class="sxs-lookup"><span data-stu-id="6f84f-115">Notice that the **Source Type** field of the production order contains **Sales Header** and the order has multiple lines, one for each sales line item that must be produced.</span></span>  
9. <span data-ttu-id="6f84f-116">Choose the **Planning** action.</span><span class="sxs-lookup"><span data-stu-id="6f84f-116">Choose the **Planning** action.</span></span>
10. <span data-ttu-id="6f84f-117">On the **Order Planning** page, choose the **Refresh** action to calculate new demand.</span><span class="sxs-lookup"><span data-stu-id="6f84f-117">On the **Order Planning** page, choose the **Refresh** action to calculate new demand.</span></span>  

<span data-ttu-id="6f84f-118">The order header line for the project order is displayed with all unfulfilled demand lines expanded under it.</span><span class="sxs-lookup"><span data-stu-id="6f84f-118">The order header line for the project order is displayed with all unfulfilled demand lines expanded under it.</span></span> <span data-ttu-id="6f84f-119">Although the production order contains lines for several produced items, the total demand for all production order lines is listed under one order header line on the **Order Planning** page, and the original customer name is displayed.</span><span class="sxs-lookup"><span data-stu-id="6f84f-119">Although the production order contains lines for several produced items, the total demand for all production order lines is listed under one order header line on the **Order Planning** page, and the original customer name is displayed.</span></span> <span data-ttu-id="6f84f-120">You can now proceed to plan for the demand as described in [Plan for New Demand Order by Order](production-how-to-plan-for-new-demand.md).</span><span class="sxs-lookup"><span data-stu-id="6f84f-120">You can now proceed to plan for the demand as described in [Plan for New Demand Order by Order](production-how-to-plan-for-new-demand.md).</span></span>  

> [!NOTE]  
>  <span data-ttu-id="6f84f-121">Demand lines in the project production order that have **Prod. Order** in their **Replenishment System** field represent underlying production orders.</span><span class="sxs-lookup"><span data-stu-id="6f84f-121">Demand lines in the project production order that have **Prod. Order** in their **Replenishment System** field represent underlying production orders.</span></span> <span data-ttu-id="6f84f-122">After you have generated these production orders, you must again calculate a plan on the **Order Planning** page to identify any unfulfilled component demand for them.</span><span class="sxs-lookup"><span data-stu-id="6f84f-122">After you have generated these production orders, you must again calculate a plan on the **Order Planning** page to identify any unfulfilled component demand for them.</span></span> <span data-ttu-id="6f84f-123">In that case, they are displayed as demand lines under a normal production order header line, meaning, the project relation is no longer visible on the page.</span><span class="sxs-lookup"><span data-stu-id="6f84f-123">In that case, they are displayed as demand lines under a normal production order header line, meaning, the project relation is no longer visible on the page.</span></span> <span data-ttu-id="6f84f-124">However, if you are using the Order Tracking feature, then you can look back and forth to all supply orders made under the original sales order.</span><span class="sxs-lookup"><span data-stu-id="6f84f-124">However, if you are using the Order Tracking feature, then you can look back and forth to all supply orders made under the original sales order.</span></span>  

## <a name="see-also"></a><span data-ttu-id="6f84f-125">See Also</span><span class="sxs-lookup"><span data-stu-id="6f84f-125">See Also</span></span>
<span data-ttu-id="6f84f-126">[Planning](production-planning.md) </span><span class="sxs-lookup"><span data-stu-id="6f84f-126">[Planning](production-planning.md) </span></span>  
[<span data-ttu-id="6f84f-127">Setting Up Manufacturing</span><span class="sxs-lookup"><span data-stu-id="6f84f-127">Setting Up Manufacturing</span></span>](production-configure-production-processes.md)  
<span data-ttu-id="6f84f-128">[Manufacturing](production-manage-manufacturing.md)  </span><span class="sxs-lookup"><span data-stu-id="6f84f-128">[Manufacturing](production-manage-manufacturing.md)  </span></span>  
[<span data-ttu-id="6f84f-129">Inventory</span><span class="sxs-lookup"><span data-stu-id="6f84f-129">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="6f84f-130">Purchasing</span><span class="sxs-lookup"><span data-stu-id="6f84f-130">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="6f84f-131">[Design Details: Supply Planning](design-details-supply-planning.md) </span><span class="sxs-lookup"><span data-stu-id="6f84f-131">[Design Details: Supply Planning](design-details-supply-planning.md) </span></span>  
[<span data-ttu-id="6f84f-132">Setup Best Practices: Supply Planning</span><span class="sxs-lookup"><span data-stu-id="6f84f-132">Setup Best Practices: Supply Planning</span></span>](setup-best-practices-supply-planning.md)  
<span data-ttu-id="6f84f-133">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="6f84f-133">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
