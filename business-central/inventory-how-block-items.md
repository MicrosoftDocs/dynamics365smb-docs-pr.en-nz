---
title: How to Block Items from Sales or Purchasing
description: In Business Central, an item can be marked as blocked for sales, blocked for purchase, or blocked for all purposes.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2019
ms.author: sgroespe
ms.openlocfilehash: e13d59e939e71a252e08afc26d2fb1ec76b247c9
ms.sourcegitcommit: bd78a5d990c9e83174da1409076c22df8b35eafd
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 03/31/2019
ms.locfileid: "917542"
---
# <a name="block-items-from-sales-or-purchasing"></a><span data-ttu-id="24a6b-103">Block Items from Sales or Purchasing</span><span class="sxs-lookup"><span data-stu-id="24a6b-103">Block Items from Sales or Purchasing</span></span>
<span data-ttu-id="24a6b-104">You can block an item from being entered on sales or purchase lines, and you can block it from being posted in any transaction.</span><span class="sxs-lookup"><span data-stu-id="24a6b-104">You can block an item from being entered on sales or purchase lines, and you can block it from being posted in any transaction.</span></span>  

<span data-ttu-id="24a6b-105">The following table illustrates what occurs when items are blocked.</span><span class="sxs-lookup"><span data-stu-id="24a6b-105">The following table illustrates what occurs when items are blocked.</span></span>  

|<span data-ttu-id="24a6b-106">Option</span><span class="sxs-lookup"><span data-stu-id="24a6b-106">Option</span></span>|<span data-ttu-id="24a6b-107">Description</span><span class="sxs-lookup"><span data-stu-id="24a6b-107">Description</span></span>|  
|--------------------|------------|  
|<span data-ttu-id="24a6b-108">**Sales Blocked**</span><span class="sxs-lookup"><span data-stu-id="24a6b-108">**Sales Blocked**</span></span>|<span data-ttu-id="24a6b-109">You cannot enter the item in a sales document or in a sales item journal.</span><span class="sxs-lookup"><span data-stu-id="24a6b-109">You cannot enter the item in a sales document or in a sales item journal.</span></span>|  
|<span data-ttu-id="24a6b-110">**Purchasing Blocked**</span><span class="sxs-lookup"><span data-stu-id="24a6b-110">**Purchasing Blocked**</span></span>|<span data-ttu-id="24a6b-111">You cannot enter the item in a purchase document, in a purchase item journal, or in purchase planning processes.</span><span class="sxs-lookup"><span data-stu-id="24a6b-111">You cannot enter the item in a purchase document, in a purchase item journal, or in purchase planning processes.</span></span>|  
|<span data-ttu-id="24a6b-112">**Blocked**</span><span class="sxs-lookup"><span data-stu-id="24a6b-112">**Blocked**</span></span>|<span data-ttu-id="24a6b-113">You cannot use the item for any item transaction.</span><span class="sxs-lookup"><span data-stu-id="24a6b-113">You cannot use the item for any item transaction.</span></span> <span data-ttu-id="24a6b-114">For more information about blocking an item for all purposes, see Item Card.</span><span class="sxs-lookup"><span data-stu-id="24a6b-114">For more information about blocking an item for all purposes, see Item Card.</span></span>|  

## <a name="to-block-an-item-from-being-entered-on-sales-lines"></a><span data-ttu-id="24a6b-115">To block an item from being entered on sales lines</span><span class="sxs-lookup"><span data-stu-id="24a6b-115">To block an item from being entered on sales lines</span></span>  

1.  <span data-ttu-id="24a6b-116">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="24a6b-116">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="24a6b-117">Select the item that you want to block, and then select the **Sales Blocked** check box.</span><span class="sxs-lookup"><span data-stu-id="24a6b-117">Select the item that you want to block, and then select the **Sales Blocked** check box.</span></span>  

<span data-ttu-id="24a6b-118">If you try to enter the item on a sales document or journal line, you will now get an error message that the item is blocked.</span><span class="sxs-lookup"><span data-stu-id="24a6b-118">If you try to enter the item on a sales document or journal line, you will now get an error message that the item is blocked.</span></span>

## <a name="to-block-an-item-from-being-entered-on-purchase-lines"></a><span data-ttu-id="24a6b-119">To block an item from being entered on purchase lines</span><span class="sxs-lookup"><span data-stu-id="24a6b-119">To block an item from being entered on purchase lines</span></span>  

1.  <span data-ttu-id="24a6b-120">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="24a6b-120">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="24a6b-121">Select the item that you want to block, and then select the **Purchasing Blocked** check box.</span><span class="sxs-lookup"><span data-stu-id="24a6b-121">Select the item that you want to block, and then select the **Purchasing Blocked** check box.</span></span>  

<span data-ttu-id="24a6b-122">If you try to enter the item on a purchase document or journal line, you will now get an error message that the item is blocked.</span><span class="sxs-lookup"><span data-stu-id="24a6b-122">If you try to enter the item on a purchase document or journal line, you will now get an error message that the item is blocked.</span></span>

## <a name="to-block-an-item-from-being-posted"></a><span data-ttu-id="24a6b-123">To block an item from being posted</span><span class="sxs-lookup"><span data-stu-id="24a6b-123">To block an item from being posted</span></span>
1. <span data-ttu-id="24a6b-124">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="24a6b-124">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span></span>
2. <span data-ttu-id="24a6b-125">Select the item that you want to block, and then select the **Blocked** check box.</span><span class="sxs-lookup"><span data-stu-id="24a6b-125">Select the item that you want to block, and then select the **Blocked** check box.</span></span>

<span data-ttu-id="24a6b-126">If you try to post any type of transaction for the item, you will now get an error message that the item is blocked.</span><span class="sxs-lookup"><span data-stu-id="24a6b-126">If you try to post any type of transaction for the item, you will now get an error message that the item is blocked.</span></span>

## <a name="see-also"></a><span data-ttu-id="24a6b-127">See Also</span><span class="sxs-lookup"><span data-stu-id="24a6b-127">See Also</span></span>  
[<span data-ttu-id="24a6b-128">Register New Items</span><span class="sxs-lookup"><span data-stu-id="24a6b-128">Register New Items</span></span>](inventory-how-register-new-items.md)  
[<span data-ttu-id="24a6b-129">Inventory</span><span class="sxs-lookup"><span data-stu-id="24a6b-129">Inventory</span></span>](inventory-manage-inventory.md)  
