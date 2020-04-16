---
title: How to Set Up Put-away Templates | Microsoft Docs
description: With directed put-away and pick functionality, the most appropriate bin for your items at any given time is suggested, according to the put-away template that you have set up for the warehouse, the bin rankings you have given to the bins, and the minimum and maximum quantities that you have set up for fixed bins.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2020
ms.author: sgroespe
ms.openlocfilehash: 168a330bdb85c8d5ed18a9ce2b65339c82b4055e
ms.sourcegitcommit: 88e4b30eaf6fa32af0c1452ce2f85ff1111c75e2
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 04/01/2020
ms.locfileid: "3196155"
---
# <a name="set-up-put-away-templates"></a><span data-ttu-id="b2e35-103">Set Up Put-away Templates</span><span class="sxs-lookup"><span data-stu-id="b2e35-103">Set Up Put-away Templates</span></span>
<span data-ttu-id="b2e35-104">With directed put-away and pick functionality, the most appropriate bin for your items at any given time is suggested, according to the put-away template that you have set up for the warehouse, the bin rankings you have given to the bins, and the minimum and maximum quantities that you have set up for fixed bins.</span><span class="sxs-lookup"><span data-stu-id="b2e35-104">With directed put-away and pick functionality, the most appropriate bin for your items at any given time is suggested, according to the put-away template that you have set up for the warehouse, the bin rankings you have given to the bins, and the minimum and maximum quantities that you have set up for fixed bins.</span></span>  

<span data-ttu-id="b2e35-105">You can set up a number of put-away templates and select one of them to govern put-aways in general in your warehouse.</span><span class="sxs-lookup"><span data-stu-id="b2e35-105">You can set up a number of put-away templates and select one of them to govern put-aways in general in your warehouse.</span></span> <span data-ttu-id="b2e35-106">You can also select a put-away template for any item or stockkeeping unit that might have special put-away requirements.</span><span class="sxs-lookup"><span data-stu-id="b2e35-106">You can also select a put-away template for any item or stockkeeping unit that might have special put-away requirements.</span></span>  

## <a name="to-set-up-put-away-templates"></a><span data-ttu-id="b2e35-107">To set up put-away templates</span><span class="sxs-lookup"><span data-stu-id="b2e35-107">To set up put-away templates</span></span>  
1.  <span data-ttu-id="b2e35-108">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Put-away Templates**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="b2e35-108">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Put-away Templates**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="b2e35-109">Choose the **New** action.</span><span class="sxs-lookup"><span data-stu-id="b2e35-109">Choose the **New** action.</span></span>  
3.  <span data-ttu-id="b2e35-110">Enter a code that is the unique identifier of the template you are about to create.</span><span class="sxs-lookup"><span data-stu-id="b2e35-110">Enter a code that is the unique identifier of the template you are about to create.</span></span>  
4.  <span data-ttu-id="b2e35-111">Enter a short description, if you wish.</span><span class="sxs-lookup"><span data-stu-id="b2e35-111">Enter a short description, if you wish.</span></span>  
5.  <span data-ttu-id="b2e35-112">Fill in the first line with the bin requirements that you want fulfilled first and foremost when suggesting a put-away.</span><span class="sxs-lookup"><span data-stu-id="b2e35-112">Fill in the first line with the bin requirements that you want fulfilled first and foremost when suggesting a put-away.</span></span>  
6.  <span data-ttu-id="b2e35-113">Fill in the second line with the bin requirements that would be your second choice to fulfill in finding a bin for put-away.</span><span class="sxs-lookup"><span data-stu-id="b2e35-113">Fill in the second line with the bin requirements that would be your second choice to fulfill in finding a bin for put-away.</span></span> <span data-ttu-id="b2e35-114">The second line is used only if a bin that meets the requirements of the first line cannot be found.</span><span class="sxs-lookup"><span data-stu-id="b2e35-114">The second line is used only if a bin that meets the requirements of the first line cannot be found.</span></span>  
7.  <span data-ttu-id="b2e35-115">Continue to fill in the lines until you have described all the acceptable bin placements that you want to use in the put-away process.</span><span class="sxs-lookup"><span data-stu-id="b2e35-115">Continue to fill in the lines until you have described all the acceptable bin placements that you want to use in the put-away process.</span></span>  
8.  <span data-ttu-id="b2e35-116">On the last line in the put-away template, select the **Find Floating Bin** check box.</span><span class="sxs-lookup"><span data-stu-id="b2e35-116">On the last line in the put-away template, select the **Find Floating Bin** check box.</span></span>  

<span data-ttu-id="b2e35-117">You can create various put-away templates and then apply them as you see fit.</span><span class="sxs-lookup"><span data-stu-id="b2e35-117">You can create various put-away templates and then apply them as you see fit.</span></span> <span data-ttu-id="b2e35-118">The put-away template that you selected for the item or stockkeeping unit, if any is used first.</span><span class="sxs-lookup"><span data-stu-id="b2e35-118">The put-away template that you selected for the item or stockkeeping unit, if any is used first.</span></span> <span data-ttu-id="b2e35-119">If these fields are not filled in, then the put-away template that you selected for the warehouse on the **Bin Policies** FastTab on the location card is used.</span><span class="sxs-lookup"><span data-stu-id="b2e35-119">If these fields are not filled in, then the put-away template that you selected for the warehouse on the **Bin Policies** FastTab on the location card is used.</span></span>  

## <a name="see-also"></a><span data-ttu-id="b2e35-120">See Also</span><span class="sxs-lookup"><span data-stu-id="b2e35-120">See Also</span></span>  
[<span data-ttu-id="b2e35-121">Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="b2e35-121">Warehouse Management</span></span>](warehouse-manage-warehouse.md)  
[<span data-ttu-id="b2e35-122">Inventory</span><span class="sxs-lookup"><span data-stu-id="b2e35-122">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="b2e35-123">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span><span class="sxs-lookup"><span data-stu-id="b2e35-123">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span></span>  
<span data-ttu-id="b2e35-124">[Assembly Management](assembly-assemble-items.md)  </span><span class="sxs-lookup"><span data-stu-id="b2e35-124">[Assembly Management](assembly-assemble-items.md)  </span></span>  
[<span data-ttu-id="b2e35-125">Design Details: Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="b2e35-125">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="b2e35-126">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="b2e35-126">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
