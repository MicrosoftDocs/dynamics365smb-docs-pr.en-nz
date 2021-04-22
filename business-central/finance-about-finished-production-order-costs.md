---
title: About Finished Production Order Costs | Microsoft Docs
description: Finishing the production order is an important task in completing the costing lifecycle of the item that is being produced. Final costs, including variances in a standard cost environment, actuals in a FIFO, Average, or LIFO cost environment, are calculated using the Adjust Cost - Item Entries batch job.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.search.keywords: ''
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: b250a495504272b93565752043c23e1988ca1dab
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 03/31/2021
ms.locfileid: "5781077"
---
# <a name="about-finished-production-order-costs"></a><span data-ttu-id="42c31-104">About Finished Production Order Costs</span><span class="sxs-lookup"><span data-stu-id="42c31-104">About Finished Production Order Costs</span></span>
<span data-ttu-id="42c31-105">Finishing the production order is an important task in completing the costing lifecycle of the item that is being produced.</span><span class="sxs-lookup"><span data-stu-id="42c31-105">Finishing the production order is an important task in completing the costing lifecycle of the item that is being produced.</span></span> <span data-ttu-id="42c31-106">Final costs, including variances in a standard cost environment, actuals in a FIFO, Average, or LIFO cost environment, are calculated using the **Adjust Cost - Item Entries** batch job, which allows for financial reconciliation of the costs of item production.</span><span class="sxs-lookup"><span data-stu-id="42c31-106">Final costs, including variances in a standard cost environment, actuals in a FIFO, Average, or LIFO cost environment, are calculated using the **Adjust Cost - Item Entries** batch job, which allows for financial reconciliation of the costs of item production.</span></span> <span data-ttu-id="42c31-107">For a production order to be considered for cost adjustment, the status must be **Finished**.</span><span class="sxs-lookup"><span data-stu-id="42c31-107">For a production order to be considered for cost adjustment, the status must be **Finished**.</span></span> <span data-ttu-id="42c31-108">It is therefore critical that upon completion, the status of a production order is changed to **Finished**.</span><span class="sxs-lookup"><span data-stu-id="42c31-108">It is therefore critical that upon completion, the status of a production order is changed to **Finished**.</span></span>  

## <a name="example"></a><span data-ttu-id="42c31-109">Example</span><span class="sxs-lookup"><span data-stu-id="42c31-109">Example</span></span>  
 <span data-ttu-id="42c31-110">In a standard cost environment, when you consume material to produce an item, stated simply, the cost of the item plus labour and overhead go into WIP.</span><span class="sxs-lookup"><span data-stu-id="42c31-110">In a standard cost environment, when you consume material to produce an item, stated simply, the cost of the item plus labor and overhead go into WIP.</span></span> <span data-ttu-id="42c31-111">When the item is produced, WIP is reduced by the amount of the standard cost of the item.</span><span class="sxs-lookup"><span data-stu-id="42c31-111">When the item is produced, WIP is reduced by the amount of the standard cost of the item.</span></span> <span data-ttu-id="42c31-112">Typically, these costs do not net to zero.</span><span class="sxs-lookup"><span data-stu-id="42c31-112">Typically, these costs do not net to zero.</span></span> <span data-ttu-id="42c31-113">So that these costs can net to zero, you must run the **Adjust Cost - Item Entries** batch job, noting that only production orders with the status of **Finished** will be considered for adjustment.</span><span class="sxs-lookup"><span data-stu-id="42c31-113">So that these costs can net to zero, you must run the **Adjust Cost - Item Entries** batch job, noting that only production orders with the status of **Finished** will be considered for adjustment.</span></span>  

## <a name="see-also"></a><span data-ttu-id="42c31-114">See Also</span><span class="sxs-lookup"><span data-stu-id="42c31-114">See Also</span></span>  
[<span data-ttu-id="42c31-115">Managing Inventory Costs</span><span class="sxs-lookup"><span data-stu-id="42c31-115">Managing Inventory Costs</span></span>](finance-manage-inventory-costs.md)  
[<span data-ttu-id="42c31-116">Manufacturing</span><span class="sxs-lookup"><span data-stu-id="42c31-116">Manufacturing</span></span>](production-manage-manufacturing.md)  
<span data-ttu-id="42c31-117">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="42c31-117">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>


[!INCLUDE[footer-include](includes/footer-banner.md)]