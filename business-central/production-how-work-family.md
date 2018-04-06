---
title: How to Use Item Families in Manufacturing | Microsoft Docs
description: The main task in customising a base calendar for your company, or one of its business partners, is to enter any changes to working and nonworking day status.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/05/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 51c505decb595f1da3aba61a73a1f2a55608fc22
ms.contentlocale: en-nz
ms.lasthandoff: 03/22/2018

---
# <a name="work-with-production-families"></a><span data-ttu-id="16d35-103">Work with Production Families</span><span class="sxs-lookup"><span data-stu-id="16d35-103">Work with Production Families</span></span>
<span data-ttu-id="16d35-104">A production family is a group of individual items whose relationship is based on the similarity of their manufacturing processes.</span><span class="sxs-lookup"><span data-stu-id="16d35-104">A production family is a group of individual items whose relationship is based on the similarity of their manufacturing processes.</span></span> <span data-ttu-id="16d35-105">By forming production families, some items can be manufactured twice or more in one production, which will optimise material consumption.</span><span class="sxs-lookup"><span data-stu-id="16d35-105">By forming production families, some items can be manufactured twice or more in one production, which will optimize material consumption.</span></span>

<span data-ttu-id="16d35-106">In the **Quantity** field in the **Family** window, you enter the quantity that will be produced when the whole family has been manufactured once.</span><span class="sxs-lookup"><span data-stu-id="16d35-106">In the **Quantity** field in the **Family** window, you enter the quantity that will be produced when the whole family has been manufactured once.</span></span>

## <a name="example"></a><span data-ttu-id="16d35-107">Example</span><span class="sxs-lookup"><span data-stu-id="16d35-107">Example</span></span>
<span data-ttu-id="16d35-108">In punching processes, four pieces of the same item can be produced from one sheet and 10 pieces of another, different, item at the same time.</span><span class="sxs-lookup"><span data-stu-id="16d35-108">In punching processes, four pieces of the same item can be produced from one sheet and 10 pieces of another, different, item at the same time.</span></span> <span data-ttu-id="16d35-109">The punching machine will punch all 14 pieces in one step.</span><span class="sxs-lookup"><span data-stu-id="16d35-109">The punching machine will punch all 14 pieces in one step.</span></span>

<span data-ttu-id="16d35-110">Forming production families reduces the scrap quantity because what would normally be leftover scrap, when producing big pieces, will be used instead to produce small items.</span><span class="sxs-lookup"><span data-stu-id="16d35-110">Forming production families reduces the scrap quantity because what would normally be leftover scrap, when producing big pieces, will be used instead to produce small items.</span></span>

## <a name="to-set-up-a-production-family"></a><span data-ttu-id="16d35-111">To set up a production family</span><span class="sxs-lookup"><span data-stu-id="16d35-111">To set up a production family</span></span>
1. <span data-ttu-id="16d35-112">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Families**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="16d35-112">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Families**, and then choose the related link.</span></span>
2. <span data-ttu-id="16d35-113">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="16d35-113">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="to-produce-based-on-a-production-familily"></a><span data-ttu-id="16d35-114">To produce based on a production familily</span><span class="sxs-lookup"><span data-stu-id="16d35-114">To produce based on a production familily</span></span>
1. <span data-ttu-id="16d35-115">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Firm Planned Prod. Orders**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="16d35-115">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Firm Planned Prod. Orders**, and then choose the related link.</span></span>
2. <span data-ttu-id="16d35-116">Create a new production order.</span><span class="sxs-lookup"><span data-stu-id="16d35-116">Create a new production order.</span></span> <span data-ttu-id="16d35-117">For more information, see [Create Production orders](production-how-to-create-production-orders.md).</span><span class="sxs-lookup"><span data-stu-id="16d35-117">For more information, see [Create Production orders](production-how-to-create-production-orders.md).</span></span>
3. <span data-ttu-id="16d35-118">In the **Source Type** field, select **Family**.</span><span class="sxs-lookup"><span data-stu-id="16d35-118">In the **Source Type** field, select **Family**.</span></span>  
4. <span data-ttu-id="16d35-119">In the **Source No.** field, select the relevant production family.</span><span class="sxs-lookup"><span data-stu-id="16d35-119">In the **Source No.** field, select the relevant production family.</span></span>

## <a name="see-also"></a><span data-ttu-id="16d35-120">See Also</span><span class="sxs-lookup"><span data-stu-id="16d35-120">See Also</span></span>
[<span data-ttu-id="16d35-121">Create Production BOMs</span><span class="sxs-lookup"><span data-stu-id="16d35-121">Create Production BOMs</span></span>](production-how-to-create-production-boms.md)  
[<span data-ttu-id="16d35-122">Setting Up Manufacturing</span><span class="sxs-lookup"><span data-stu-id="16d35-122">Setting Up Manufacturing</span></span>](production-configure-production-processes.md)  
<span data-ttu-id="16d35-123">[Manufacturing](production-manage-manufacturing.md)  </span><span class="sxs-lookup"><span data-stu-id="16d35-123">[Manufacturing](production-manage-manufacturing.md)  </span></span>  
<span data-ttu-id="16d35-124">[Planning](production-planning.md) </span><span class="sxs-lookup"><span data-stu-id="16d35-124">[Planning](production-planning.md) </span></span>  
[<span data-ttu-id="16d35-125">Inventory</span><span class="sxs-lookup"><span data-stu-id="16d35-125">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="16d35-126">Purchasing</span><span class="sxs-lookup"><span data-stu-id="16d35-126">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="16d35-127">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="16d35-127">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

