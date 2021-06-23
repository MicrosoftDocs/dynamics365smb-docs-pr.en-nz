---
title: Create Production Orders from Sales Orders
description: You can create production orders from sales orders.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 05/28/2021
ms.author: edupont
ms.openlocfilehash: 438f4d4e1833ba607ceedb9f5d9450c0a4dbb680
ms.sourcegitcommit: f9a190933eadf4608f591e2f1b04c69f1e5c0dc7
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 05/28/2021
ms.locfileid: "6115252"
---
# <a name="create-production-orders-from-sales-orders"></a><span data-ttu-id="dc822-103">Create Production Orders from Sales Orders</span><span class="sxs-lookup"><span data-stu-id="dc822-103">Create Production Orders from Sales Orders</span></span>
<span data-ttu-id="dc822-104">You can create production orders for produced items directly from sales orders.</span><span class="sxs-lookup"><span data-stu-id="dc822-104">You can create production orders for produced items directly from sales orders.</span></span>  

## <a name="to-create-a-production-order-from-a-sales-order"></a><span data-ttu-id="dc822-105">To create a production order from a sales order</span><span class="sxs-lookup"><span data-stu-id="dc822-105">To create a production order from a sales order</span></span>  

1.  <span data-ttu-id="dc822-106">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="dc822-106">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="dc822-107">Select the sales order you want to create a production order for.</span><span class="sxs-lookup"><span data-stu-id="dc822-107">Select the sales order you want to create a production order for.</span></span>  
3.  <span data-ttu-id="dc822-108">Choose the **Planning** action.</span><span class="sxs-lookup"><span data-stu-id="dc822-108">Choose the **Planning** action.</span></span> <span data-ttu-id="dc822-109">On the **Sales Order Planning** page, you can view the availability of the sales order item.</span><span class="sxs-lookup"><span data-stu-id="dc822-109">On the **Sales Order Planning** page, you can view the availability of the sales order item.</span></span>  
4.  <span data-ttu-id="dc822-110">Choose the **Create Prod. Order** action.</span><span class="sxs-lookup"><span data-stu-id="dc822-110">Choose the **Create Prod. Order** action.</span></span>  
5.  <span data-ttu-id="dc822-111">Select the status and order type.</span><span class="sxs-lookup"><span data-stu-id="dc822-111">Select the status and order type.</span></span>  
6.  <span data-ttu-id="dc822-112">Choose the **Yes** button to create one or more production orders for the lines that have **Prod. Order** in their **Replenishment System** field.</span><span class="sxs-lookup"><span data-stu-id="dc822-112">Choose the **Yes** button to create one or more production orders for the lines that have **Prod. Order** in their **Replenishment System** field.</span></span>


> [!NOTE]  
> <span data-ttu-id="dc822-113">Demand lines in the created production order that have **Prod. Order** in their **Replenishment System** field represent underlying production orders.</span><span class="sxs-lookup"><span data-stu-id="dc822-113">Demand lines in the created production order that have **Prod. Order** in their **Replenishment System** field represent underlying production orders.</span></span> <span data-ttu-id="dc822-114">After you have generated these production orders, remember to identify any unfulfilled component demand for them using the **Order Planning** page or the **Replan** function from created orders.</span><span class="sxs-lookup"><span data-stu-id="dc822-114">After you have generated these production orders, remember to identify any unfulfilled component demand for them using the **Order Planning** page or the **Replan** function from created orders.</span></span> 

## <a name="order-type"></a><span data-ttu-id="dc822-115">Order type</span><span class="sxs-lookup"><span data-stu-id="dc822-115">Order type</span></span>  
<span data-ttu-id="dc822-116">You can choose between two ways to create the production orders as outlined in the following table.</span><span class="sxs-lookup"><span data-stu-id="dc822-116">You can choose between two ways to create the production orders as outlined in the following table.</span></span>

|<span data-ttu-id="dc822-117">Option</span><span class="sxs-lookup"><span data-stu-id="dc822-117">Option</span></span>|<span data-ttu-id="dc822-118">Description</span><span class="sxs-lookup"><span data-stu-id="dc822-118">Description</span></span>|
|------|-----------|
|<span data-ttu-id="dc822-119">Item Order</span><span class="sxs-lookup"><span data-stu-id="dc822-119">Item Order</span></span>|<span data-ttu-id="dc822-120">One production order is created for each needed production order that is represented by a line in the **Sales Order Planning** window.</span><span class="sxs-lookup"><span data-stu-id="dc822-120">One production order is created for each needed production order that is represented by a line in the **Sales Order Planning** window.</span></span>|
|<span data-ttu-id="dc822-121">Project Order</span><span class="sxs-lookup"><span data-stu-id="dc822-121">Project Order</span></span>|<span data-ttu-id="dc822-122">One production order is created for all needed production orders order that are represented by lines in the **Sales Order Planning** window.</span><span class="sxs-lookup"><span data-stu-id="dc822-122">One production order is created for all needed production orders order that are represented by lines in the **Sales Order Planning** window.</span></span> |

<span data-ttu-id="dc822-123">When you use project orders, the **Source Type** field of the production order contains **Sales Header** and the order has multiple lines, one for each sales line item that must be produced.</span><span class="sxs-lookup"><span data-stu-id="dc822-123">When you use project orders, the **Source Type** field of the production order contains **Sales Header** and the order has multiple lines, one for each sales line item that must be produced.</span></span>  


## <a name="see-also"></a><span data-ttu-id="dc822-124">See Also</span><span class="sxs-lookup"><span data-stu-id="dc822-124">See Also</span></span>  
[<span data-ttu-id="dc822-125">Setting Up Manufacturing</span><span class="sxs-lookup"><span data-stu-id="dc822-125">Setting Up Manufacturing</span></span>](production-configure-production-processes.md)  
<span data-ttu-id="dc822-126">[Manufacturing](production-manage-manufacturing.md)  </span><span class="sxs-lookup"><span data-stu-id="dc822-126">[Manufacturing](production-manage-manufacturing.md)  </span></span>  
[<span data-ttu-id="dc822-127">Inventory</span><span class="sxs-lookup"><span data-stu-id="dc822-127">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="dc822-128">Purchasing</span><span class="sxs-lookup"><span data-stu-id="dc822-128">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="dc822-129">[Design Details: Supply Planning](design-details-supply-planning.md) </span><span class="sxs-lookup"><span data-stu-id="dc822-129">[Design Details: Supply Planning](design-details-supply-planning.md) </span></span>  
[<span data-ttu-id="dc822-130">Setup Best Practices: Supply Planning</span><span class="sxs-lookup"><span data-stu-id="dc822-130">Setup Best Practices: Supply Planning</span></span>](setup-best-practices-supply-planning.md)  
<span data-ttu-id="dc822-131">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="dc822-131">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>


[!INCLUDE[footer-include](includes/footer-banner.md)]
