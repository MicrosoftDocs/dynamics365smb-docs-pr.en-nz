---
title: How to Use Item Families in Manufacturing | Microsoft Docs
description: The main task in customising a base calendar for your company, or one of its business partners, is to enter any changes to working and nonworking day status.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 4c926b8f7663c805f07bcd7c85339b109f85a7ff
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "5383216"
---
# <a name="work-with-production-families"></a><span data-ttu-id="0c9a0-103">Work with Production Families</span><span class="sxs-lookup"><span data-stu-id="0c9a0-103">Work with Production Families</span></span>
<span data-ttu-id="0c9a0-104">A production family is a group of individual items whose relationship is based on the similarity of their manufacturing processes.</span><span class="sxs-lookup"><span data-stu-id="0c9a0-104">A production family is a group of individual items whose relationship is based on the similarity of their manufacturing processes.</span></span> <span data-ttu-id="0c9a0-105">By forming production families, some items can be manufactured twice or more in one production, which will optimise material consumption.</span><span class="sxs-lookup"><span data-stu-id="0c9a0-105">By forming production families, some items can be manufactured twice or more in one production, which will optimize material consumption.</span></span>

<span data-ttu-id="0c9a0-106">In the **Quantity** field on the **Family** page, you enter the quantity that will be produced when the whole family has been manufactured once.</span><span class="sxs-lookup"><span data-stu-id="0c9a0-106">In the **Quantity** field on the **Family** page, you enter the quantity that will be produced when the whole family has been manufactured once.</span></span>

## <a name="example"></a><span data-ttu-id="0c9a0-107">Example</span><span class="sxs-lookup"><span data-stu-id="0c9a0-107">Example</span></span>
<span data-ttu-id="0c9a0-108">In punching processes, four pieces of the same item can be produced from one sheet and 10 pieces of another, different, item at the same time.</span><span class="sxs-lookup"><span data-stu-id="0c9a0-108">In punching processes, four pieces of the same item can be produced from one sheet and 10 pieces of another, different, item at the same time.</span></span> <span data-ttu-id="0c9a0-109">The punching machine will punch all 14 pieces in one step.</span><span class="sxs-lookup"><span data-stu-id="0c9a0-109">The punching machine will punch all 14 pieces in one step.</span></span>

<span data-ttu-id="0c9a0-110">Forming production families reduces the scrap quantity because what would normally be leftover scrap, when producing big pieces, will be used instead to produce small items.</span><span class="sxs-lookup"><span data-stu-id="0c9a0-110">Forming production families reduces the scrap quantity because what would normally be leftover scrap, when producing big pieces, will be used instead to produce small items.</span></span>

## <a name="to-set-up-a-production-family"></a><span data-ttu-id="0c9a0-111">To set up a production family</span><span class="sxs-lookup"><span data-stu-id="0c9a0-111">To set up a production family</span></span>
1. <span data-ttu-id="0c9a0-112">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Families**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="0c9a0-112">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Families**, and then choose the related link.</span></span>
2. <span data-ttu-id="0c9a0-113">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="0c9a0-113">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="to-produce-based-on-a-production-family"></a><span data-ttu-id="0c9a0-114">To produce based on a production family</span><span class="sxs-lookup"><span data-stu-id="0c9a0-114">To produce based on a production family</span></span>
1. <span data-ttu-id="0c9a0-115">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Firm Planned Prod. Orders**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="0c9a0-115">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Firm Planned Prod. Orders**, and then choose the related link.</span></span>
2. <span data-ttu-id="0c9a0-116">Create a new production order.</span><span class="sxs-lookup"><span data-stu-id="0c9a0-116">Create a new production order.</span></span> <span data-ttu-id="0c9a0-117">For more information, see [Create Production orders](production-how-to-create-production-orders.md).</span><span class="sxs-lookup"><span data-stu-id="0c9a0-117">For more information, see [Create Production orders](production-how-to-create-production-orders.md).</span></span>
3. <span data-ttu-id="0c9a0-118">In the **Source Type** field, select **Family**.</span><span class="sxs-lookup"><span data-stu-id="0c9a0-118">In the **Source Type** field, select **Family**.</span></span>  
4. <span data-ttu-id="0c9a0-119">In the **Source No.** field, select the relevant production family.</span><span class="sxs-lookup"><span data-stu-id="0c9a0-119">In the **Source No.** field, select the relevant production family.</span></span>

## <a name="see-also"></a><span data-ttu-id="0c9a0-120">See Also</span><span class="sxs-lookup"><span data-stu-id="0c9a0-120">See Also</span></span>
[<span data-ttu-id="0c9a0-121">Create Production BOMs</span><span class="sxs-lookup"><span data-stu-id="0c9a0-121">Create Production BOMs</span></span>](production-how-to-create-production-boms.md)  
[<span data-ttu-id="0c9a0-122">Setting Up Manufacturing</span><span class="sxs-lookup"><span data-stu-id="0c9a0-122">Setting Up Manufacturing</span></span>](production-configure-production-processes.md)  
<span data-ttu-id="0c9a0-123">[Manufacturing](production-manage-manufacturing.md)  </span><span class="sxs-lookup"><span data-stu-id="0c9a0-123">[Manufacturing](production-manage-manufacturing.md)  </span></span>  
<span data-ttu-id="0c9a0-124">[Planning](production-planning.md) </span><span class="sxs-lookup"><span data-stu-id="0c9a0-124">[Planning](production-planning.md) </span></span>  
[<span data-ttu-id="0c9a0-125">Inventory</span><span class="sxs-lookup"><span data-stu-id="0c9a0-125">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="0c9a0-126">Purchasing</span><span class="sxs-lookup"><span data-stu-id="0c9a0-126">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="0c9a0-127">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="0c9a0-127">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>


[!INCLUDE[footer-include](includes/footer-banner.md)]