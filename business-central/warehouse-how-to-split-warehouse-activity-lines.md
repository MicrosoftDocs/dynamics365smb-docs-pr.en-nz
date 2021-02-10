---
title: How to Split Warehouse Activity Lines | Microsoft Docs
description: In warehouse put-aways, movements, or picks, and in inventory put-aways and inventory picks, bins are suggested for the picking or putting away of items. The actual quantity in the bin suggested may not be sufficient, or there is not enough room in the suggested bin to put away the required quantity. In these cases, you need to split the line, so that the items for one line are either taken from or placed into more than one bin.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 7c2889c3b051ed20c07f474fd4ff47fdac60aa2d
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 12/17/2020
ms.locfileid: "4755908"
---
# <a name="split-warehouse-activity-lines"></a><span data-ttu-id="37f7c-105">Split Warehouse Activity Lines</span><span class="sxs-lookup"><span data-stu-id="37f7c-105">Split Warehouse Activity Lines</span></span>
<span data-ttu-id="37f7c-106">In warehouse put-aways, movements, or picks, and in inventory put-aways and inventory picks, bins are suggested for the picking or putting away of items.</span><span class="sxs-lookup"><span data-stu-id="37f7c-106">In warehouse put-aways, movements, or picks, and in inventory put-aways and inventory picks, bins are suggested for the picking or putting away of items.</span></span> <span data-ttu-id="37f7c-107">The actual quantity in the bin suggested may not be sufficient, or there is not enough room in the suggested bin to put away the required quantity.</span><span class="sxs-lookup"><span data-stu-id="37f7c-107">The actual quantity in the bin suggested may not be sufficient, or there is not enough room in the suggested bin to put away the required quantity.</span></span> <span data-ttu-id="37f7c-108">In these cases, you need to split the line, so that the items for one line are either taken from or placed into more than one bin.</span><span class="sxs-lookup"><span data-stu-id="37f7c-108">In these cases, you need to split the line, so that the items for one line are either taken from or placed into more than one bin.</span></span>  

<span data-ttu-id="37f7c-109">The following procedure applies to warehouse documents, such as warehouse put-away, movement, and pick lines, or inventory put-away, movement, and pick lines.</span><span class="sxs-lookup"><span data-stu-id="37f7c-109">The following procedure applies to warehouse documents, such as warehouse put-away, movement, and pick lines, or inventory put-away, movement, and pick lines.</span></span>  

## <a name="to-split-warehouse-activity-lines"></a><span data-ttu-id="37f7c-110">To split warehouse activity lines</span><span class="sxs-lookup"><span data-stu-id="37f7c-110">To split warehouse activity lines</span></span>  
1.  <span data-ttu-id="37f7c-111">Open a warehouse activity line where you are trying to handle an insufficient quantity.</span><span class="sxs-lookup"><span data-stu-id="37f7c-111">Open a warehouse activity line where you are trying to handle an insufficient quantity.</span></span>  
2.  <span data-ttu-id="37f7c-112">In the **Qty. to Handle** field, enter the reduced quantity that you are able to handle.</span><span class="sxs-lookup"><span data-stu-id="37f7c-112">In the **Qty. to Handle** field, enter the reduced quantity that you are able to handle.</span></span>  
3.  <span data-ttu-id="37f7c-113">On the **Lines** FastTab, choose the **Actions** action, choose the **Functions** action, and then choose the **Split Line** action.</span><span class="sxs-lookup"><span data-stu-id="37f7c-113">On the **Lines** FastTab, choose the **Actions** action, choose the **Functions** action, and then choose the **Split Line** action.</span></span> <span data-ttu-id="37f7c-114">A new line appears, which is a copy of the original line, except that the **Qty. to Handle** field contains the quantity that you removed from the original line.</span><span class="sxs-lookup"><span data-stu-id="37f7c-114">A new line appears, which is a copy of the original line, except that the **Qty. to Handle** field contains the quantity that you removed from the original line.</span></span>  
4.  <span data-ttu-id="37f7c-115">Assign an appropriate bin and, if you are using directed put-away and pick, a zone, to this new line, or continue splitting the line as necessary until you find appropriate bins for all of the quantity.</span><span class="sxs-lookup"><span data-stu-id="37f7c-115">Assign an appropriate bin and, if you are using directed put-away and pick, a zone, to this new line, or continue splitting the line as necessary until you find appropriate bins for all of the quantity.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="37f7c-116">If the location uses directed put-away and pick and you split the lines, you must be familiar with the warehouse and be able to choose a bin that matches the storage requirements of the item and that fulfills the general requirements of the warehouse document.</span><span class="sxs-lookup"><span data-stu-id="37f7c-116">If the location uses directed put-away and pick and you split the lines, you must be familiar with the warehouse and be able to choose a bin that matches the storage requirements of the item and that fulfills the general requirements of the warehouse document.</span></span> <span data-ttu-id="37f7c-117">For example, you would not split a line on a pick document and place some items in the bulk storage.</span><span class="sxs-lookup"><span data-stu-id="37f7c-117">For example, you would not split a line on a pick document and place some items in the bulk storage.</span></span>  

## <a name="see-also"></a><span data-ttu-id="37f7c-118">See Also</span><span class="sxs-lookup"><span data-stu-id="37f7c-118">See Also</span></span>  
[<span data-ttu-id="37f7c-119">Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="37f7c-119">Warehouse Management</span></span>](warehouse-manage-warehouse.md)  
[<span data-ttu-id="37f7c-120">Inventory</span><span class="sxs-lookup"><span data-stu-id="37f7c-120">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="37f7c-121">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span><span class="sxs-lookup"><span data-stu-id="37f7c-121">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span></span>  
<span data-ttu-id="37f7c-122">[Assembly Management](assembly-assemble-items.md)  </span><span class="sxs-lookup"><span data-stu-id="37f7c-122">[Assembly Management](assembly-assemble-items.md)  </span></span>  
[<span data-ttu-id="37f7c-123">Design Details: Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="37f7c-123">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="37f7c-124">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="37f7c-124">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>
