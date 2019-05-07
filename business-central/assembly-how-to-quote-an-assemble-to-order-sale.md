---
title: How to Quote an Assemble-to-Order Sale | Microsoft Docs
description: You can use assembly management to customise an assembly item to a customer’s request during the sales process.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: kit, kitting
ms.date: 04/01/2019
ms.author: sgroespe
ms.openlocfilehash: b69433a365e6c67f31863f8289cddb21d0f7f4b7
ms.sourcegitcommit: bd78a5d990c9e83174da1409076c22df8b35eafd
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 03/31/2019
ms.locfileid: "936501"
---
# <a name="quote-an-assemble-to-order-sale"></a><span data-ttu-id="f5269-103">Quote an Assemble-to-Order Sale</span><span class="sxs-lookup"><span data-stu-id="f5269-103">Quote an Assemble-to-Order Sale</span></span>
<span data-ttu-id="f5269-104">You can use assembly management to customise an assembly item to a customer’s request during the sales process.</span><span class="sxs-lookup"><span data-stu-id="f5269-104">You can use assembly management to customize an assembly item to a customer’s request during the sales process.</span></span> <span data-ttu-id="f5269-105">For more information, see [Sell Items Assembled to Order](assembly-how-to-sell-items-assembled-to-order.md).</span><span class="sxs-lookup"><span data-stu-id="f5269-105">For more information, see [Sell Items Assembled to Order](assembly-how-to-sell-items-assembled-to-order.md).</span></span>  

<span data-ttu-id="f5269-106">As when you sell any other type of item, you can also create a sales quote for a customised assembly item before converting it to a sales order.</span><span class="sxs-lookup"><span data-stu-id="f5269-106">As when you sell any other type of item, you can also create a sales quote for a customized assembly item before converting it to a sales order.</span></span> <span data-ttu-id="f5269-107">This process involves several extra steps when you compare it to creating a regular sales quote, and it uses a variation of a linked assembly order, which is an assembly quote.</span><span class="sxs-lookup"><span data-stu-id="f5269-107">This process involves several extra steps when you compare it to creating a regular sales quote, and it uses a variation of a linked assembly order, which is an assembly quote.</span></span>

> [!NOTE]  
>  <span data-ttu-id="f5269-108">Like all types of quotes, the quantities on assembly quotes are not used in availability, planning, or reservations.</span><span class="sxs-lookup"><span data-stu-id="f5269-108">Like all types of quotes, the quantities on assembly quotes are not used in availability, planning, or reservations.</span></span>  

## <a name="to-create-a-sales-quote-for-an-assemble-to-order-item"></a><span data-ttu-id="f5269-109">To create a sales quote for an assemble-to-order item</span><span class="sxs-lookup"><span data-stu-id="f5269-109">To create a sales quote for an assemble-to-order item</span></span>  
1.  <span data-ttu-id="f5269-110">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Quote**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="f5269-110">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Quote**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="f5269-111">Create a sales quote line with one line for an assembly item.</span><span class="sxs-lookup"><span data-stu-id="f5269-111">Create a sales quote line with one line for an assembly item.</span></span> <span data-ttu-id="f5269-112">For more information, see [Make Sales Quotes](sales-how-make-offers.md).</span><span class="sxs-lookup"><span data-stu-id="f5269-112">For more information, see [Make Sales Quotes](sales-how-make-offers.md).</span></span>  
3.  <span data-ttu-id="f5269-113">In the **Qty. to Assemble to Order** field, enter the full quantity.</span><span class="sxs-lookup"><span data-stu-id="f5269-113">In the **Qty. to Assemble to Order** field, enter the full quantity.</span></span>

    > [!NOTE]  
    >  <span data-ttu-id="f5269-114">You should not quote a partial quantity.</span><span class="sxs-lookup"><span data-stu-id="f5269-114">You should not quote a partial quantity.</span></span> <span data-ttu-id="f5269-115">Therefore, you must enter the same quantity that you entered in the **Quantity** field on the sales quote line.</span><span class="sxs-lookup"><span data-stu-id="f5269-115">Therefore, you must enter the same quantity that you entered in the **Quantity** field on the sales quote line.</span></span>  

4.  <span data-ttu-id="f5269-116">On the **Lines** FastTab, choose **Line**, choose **Assemble to Order**, and then choose **Assemble-to-Order Lines**.</span><span class="sxs-lookup"><span data-stu-id="f5269-116">On the **Lines** FastTab, choose **Line**, choose **Assemble to Order**, and then choose **Assemble-to-Order Lines**.</span></span> <span data-ttu-id="f5269-117">Alternatively, choose the **Qty. to Assemble to Order** field on the line.</span><span class="sxs-lookup"><span data-stu-id="f5269-117">Alternatively, choose the **Qty. to Assemble to Order** field on the line.</span></span>  
5.  <span data-ttu-id="f5269-118">On the **Assemble-to-Order Lines** page, review or modify the assembly order lines according to the quote that the customer is requesting.</span><span class="sxs-lookup"><span data-stu-id="f5269-118">On the **Assemble-to-Order Lines** page, review or modify the assembly order lines according to the quote that the customer is requesting.</span></span> <span data-ttu-id="f5269-119">If you want to view more information, choose the **Show Document** action to open the complete blanket quote order.</span><span class="sxs-lookup"><span data-stu-id="f5269-119">If you want to view more information, choose the **Show Document** action to open the complete blanket quote order.</span></span> <span data-ttu-id="f5269-120">You cannot change the contents of most fields, and you cannot post.</span><span class="sxs-lookup"><span data-stu-id="f5269-120">You cannot change the contents of most fields, and you cannot post.</span></span>  
6.  <span data-ttu-id="f5269-121">When you have adjusted the assembly order lines according to the quote, close the **Assemble-to-Order Lines** page to return to the **Sales Quote** page.</span><span class="sxs-lookup"><span data-stu-id="f5269-121">When you have adjusted the assembly order lines according to the quote, close the **Assemble-to-Order Lines** page to return to the **Sales Quote** page.</span></span>  
7.  <span data-ttu-id="f5269-122">If the customer accepts the quote, then create a sales order for the quoted assembly item.</span><span class="sxs-lookup"><span data-stu-id="f5269-122">If the customer accepts the quote, then create a sales order for the quoted assembly item.</span></span> <span data-ttu-id="f5269-123">For more information, see [Make Sales Quotes](sales-how-make-offers.md).</span><span class="sxs-lookup"><span data-stu-id="f5269-123">For more information, see [Make Sales Quotes](sales-how-make-offers.md).</span></span> <span data-ttu-id="f5269-124">The linked assembly quote and any customisations are linked to that new sales order to prepare for assembly of the item or items to be sold.</span><span class="sxs-lookup"><span data-stu-id="f5269-124">The linked assembly quote and any customizations are linked to that new sales order to prepare for assembly of the item or items to be sold.</span></span>  

## <a name="see-also"></a><span data-ttu-id="f5269-125">See Also</span><span class="sxs-lookup"><span data-stu-id="f5269-125">See Also</span></span>  
[<span data-ttu-id="f5269-126">Assembly Management</span><span class="sxs-lookup"><span data-stu-id="f5269-126">Assembly Management</span></span>](assembly-assemble-items.md)  
[<span data-ttu-id="f5269-127">Work with Bills of Material</span><span class="sxs-lookup"><span data-stu-id="f5269-127">Work with Bills of Material</span></span>](inventory-how-work-BOMs.md)  
[<span data-ttu-id="f5269-128">Inventory</span><span class="sxs-lookup"><span data-stu-id="f5269-128">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="f5269-129">Design Details: Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="f5269-129">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="f5269-130">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="f5269-130">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
