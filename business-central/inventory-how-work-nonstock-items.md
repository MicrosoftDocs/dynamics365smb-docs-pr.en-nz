---
title: Create and Manage Catalogue Items| Microsoft Docs
description: Describes how to trade in items that are in your vendors list of items but not in your own list of items.
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: non-inventoriable
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 33b900f1ac9e295921e7f3d6ea72cc93939d8a1b
ms.openlocfilehash: c65d498fb63668a6cd83f61303ae99c54d0a2452
ms.contentlocale: en-nz
ms.lasthandoff: 11/26/2018

---
# <a name="work-with-catalog-items"></a><span data-ttu-id="ea450-103">Work with Catalogue Items</span><span class="sxs-lookup"><span data-stu-id="ea450-103">Work with Catalog Items</span></span>
<span data-ttu-id="ea450-104">You can offer certain items to your customers for their convenience, which you do not want to manage in your system until you start selling them.</span><span class="sxs-lookup"><span data-stu-id="ea450-104">You can offer certain items to your customers for their convenience, which you do not want to manage in your system until you start selling them.</span></span> <span data-ttu-id="ea450-105">When you want to start managing such items in your system, you can convert them to normal item cards in two ways.</span><span class="sxs-lookup"><span data-stu-id="ea450-105">When you want to start managing such items in your system, you can convert them to normal item cards in two ways.</span></span>

* <span data-ttu-id="ea450-106">From a catalogue item card, create a new item card based on a template.</span><span class="sxs-lookup"><span data-stu-id="ea450-106">From a catalog item card, create a new item card based on a template.</span></span>
* <span data-ttu-id="ea450-107">From a sales order line of type **Item** with an empty **No** field, select a catalogue item.</span><span class="sxs-lookup"><span data-stu-id="ea450-107">From a sales order line of type **Item** with an empty **No** field, select a catalog item.</span></span> <span data-ttu-id="ea450-108">An item card is then automatically created for the catalogue item.</span><span class="sxs-lookup"><span data-stu-id="ea450-108">An item card is then automatically created for the catalog item.</span></span>

> [!NOTE]  
> <span data-ttu-id="ea450-109">You cannot select a catalogue item from the **Sales Invoice** page.</span><span class="sxs-lookup"><span data-stu-id="ea450-109">You cannot select a catalog item from the **Sales Invoice** page.</span></span><br /><br />
> <span data-ttu-id="ea450-110">You can select a catalogue item from the **Sales Quote** page, but the catalogue item will not be converted to a normal item when you use the **Make Order** function.</span><span class="sxs-lookup"><span data-stu-id="ea450-110">You can select a catalog item from the **Sales Quote** page, but the catalog item will not be converted to a normal item when you use the **Make Order** function.</span></span>

<span data-ttu-id="ea450-111">A catalogue item typically has the item number of the vendor who supplies it.</span><span class="sxs-lookup"><span data-stu-id="ea450-111">A catalog item typically has the item number of the vendor who supplies it.</span></span> <span data-ttu-id="ea450-112">To enable conversion of a catalogue item card to a normal item card, you must first set up how vendor item numbering is converted to your own item numbering.</span><span class="sxs-lookup"><span data-stu-id="ea450-112">To enable conversion of a catalog item card to a normal item card, you must first set up how vendor item numbering is converted to your own item numbering.</span></span>   

> [!Important]
> <span data-ttu-id="ea450-113">Catalogue items are not to be mistaken with non-inventory items, which are regular items that are given the type **Non-Inventory** to keep them out of availability and costing calculations, for example, because they are only used internally and have a low cost.</span><span class="sxs-lookup"><span data-stu-id="ea450-113">Catalog items are not to be mistaken with non-inventory items, which are regular items that are given the type **Non-Inventory** to keep them out of availability and costing calculations, for example, because they are only used internally and have a low cost.</span></span> <span data-ttu-id="ea450-114">For more information, see [About Item Types](inventory-about-item-types.md).</span><span class="sxs-lookup"><span data-stu-id="ea450-114">For more information, see [About Item Types](inventory-about-item-types.md).</span></span>

## <a name="to-create-a-catalog-item"></a><span data-ttu-id="ea450-115">To create a catalogue item</span><span class="sxs-lookup"><span data-stu-id="ea450-115">To create a catalog item</span></span>
<span data-ttu-id="ea450-116">Catalogue item cards have much less information than normal item cards because you only use them to offer on quotes and in other ways.</span><span class="sxs-lookup"><span data-stu-id="ea450-116">Catalog item cards have much less information than normal item cards because you only use them to offer on quotes and in other ways.</span></span> <span data-ttu-id="ea450-117">For that reason, they must be converted to normal item cards before you can post sales transactions for them.</span><span class="sxs-lookup"><span data-stu-id="ea450-117">For that reason, they must be converted to normal item cards before you can post sales transactions for them.</span></span>

1. <span data-ttu-id="ea450-118">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Catalogue Items**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="ea450-118">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Catalog Items**, and then choose the related link.</span></span>
2. <span data-ttu-id="ea450-119">Choose the **New** action.</span><span class="sxs-lookup"><span data-stu-id="ea450-119">Choose the **New** action.</span></span>
3. <span data-ttu-id="ea450-120">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="ea450-120">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="to-set-up-how-catalog-item-numbers-are-converted-to-your-own-numbering"></a><span data-ttu-id="ea450-121">To set up how catalogue item numbers are converted to your own numbering</span><span class="sxs-lookup"><span data-stu-id="ea450-121">To set up how catalog item numbers are converted to your own numbering</span></span>
<span data-ttu-id="ea450-122">To enable conversion of a catalogue item card to a normal item card, you must first set up how the vendor's item numbering is converted to your own item number format.</span><span class="sxs-lookup"><span data-stu-id="ea450-122">To enable conversion of a catalog item card to a normal item card, you must first set up how the vendor's item numbering is converted to your own item number format.</span></span>

1. <span data-ttu-id="ea450-123">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Catalogue Item Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="ea450-123">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Catalog Item Setup**, and then choose the related link.</span></span>
2. <span data-ttu-id="ea450-124">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="ea450-124">Fill in the fields as necessary.</span></span>

## <a name="to-convert-a-catalog-item-to-a-normal-item"></a><span data-ttu-id="ea450-125">To convert a catalogue item to a normal item</span><span class="sxs-lookup"><span data-stu-id="ea450-125">To convert a catalog item to a normal item</span></span>
1. <span data-ttu-id="ea450-126">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Catalogue Items**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="ea450-126">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Catalog Items**, and then choose the related link.</span></span>
2. <span data-ttu-id="ea450-127">Open the card for a catalogue item that you want to convert to a normal item.</span><span class="sxs-lookup"><span data-stu-id="ea450-127">Open the card for a catalog item that you want to convert to a normal item.</span></span>
3. <span data-ttu-id="ea450-128">On the **Catalogue Item Card** page, choose the **Create Item** action.</span><span class="sxs-lookup"><span data-stu-id="ea450-128">On the **Catalog Item Card** page, choose the **Create Item** action.</span></span>

<span data-ttu-id="ea450-129">A new item card prefilled with information from the catalogue item and a relevant item template is created.</span><span class="sxs-lookup"><span data-stu-id="ea450-129">A new item card prefilled with information from the catalog item and a relevant item template is created.</span></span> <span data-ttu-id="ea450-130">You can then fill or edit fields on the new item card as necessary.</span><span class="sxs-lookup"><span data-stu-id="ea450-130">You can then fill or edit fields on the new item card as necessary.</span></span> <span data-ttu-id="ea450-131">For more information, see [Register New Items](inventory-how-register-new-items.md).</span><span class="sxs-lookup"><span data-stu-id="ea450-131">For more information, see [Register New Items](inventory-how-register-new-items.md).</span></span>

## <a name="to-sell-a-catalog-item-and-convert-it-to-a-normal-item"></a><span data-ttu-id="ea450-132">To sell a catalogue item, and convert it to a normal item</span><span class="sxs-lookup"><span data-stu-id="ea450-132">To sell a catalog item, and convert it to a normal item</span></span>
1. <span data-ttu-id="ea450-133">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="ea450-133">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.</span></span>
2. <span data-ttu-id="ea450-134">Choose the **New** action.</span><span class="sxs-lookup"><span data-stu-id="ea450-134">Choose the **New** action.</span></span> <span data-ttu-id="ea450-135">Fill in the fields on the **General** FastTab as for any sales order.</span><span class="sxs-lookup"><span data-stu-id="ea450-135">Fill in the fields on the **General** FastTab as for any sales order.</span></span> <span data-ttu-id="ea450-136">For more information, see [Sell Products](sales-how-sell-products.md).</span><span class="sxs-lookup"><span data-stu-id="ea450-136">For more information, see [Sell Products](sales-how-sell-products.md).</span></span>
3. <span data-ttu-id="ea450-137">On a new sales line, in the **Type** field, select **Item**, but leave the **No.**</span><span class="sxs-lookup"><span data-stu-id="ea450-137">On a new sales line, in the **Type** field, select **Item**, but leave the **No.**</span></span> <span data-ttu-id="ea450-138">field empty.</span><span class="sxs-lookup"><span data-stu-id="ea450-138">field empty.</span></span>
4. <span data-ttu-id="ea450-139">Choose the **Line** action, and then choose the **Select Catalogue Items** action.</span><span class="sxs-lookup"><span data-stu-id="ea450-139">Choose the **Line** action, and then choose the **Select Catalog Items** action.</span></span>

    <span data-ttu-id="ea450-140">The catalogue item is converted to a normal item.</span><span class="sxs-lookup"><span data-stu-id="ea450-140">The catalog item is converted to a normal item.</span></span> <span data-ttu-id="ea450-141">A new item card prefilled with information from the catalogue item and a relevant item template is created.</span><span class="sxs-lookup"><span data-stu-id="ea450-141">A new item card prefilled with information from the catalog item and a relevant item template is created.</span></span>
5. <span data-ttu-id="ea450-142">On the **Catalogue Items** page, select the catalogue item that you want to sell, and then choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="ea450-142">On the **Catalog Items** page, select the catalog item that you want to sell, and then choose the **OK** button.</span></span>
6. <span data-ttu-id="ea450-143">When the sales order is complete, choose the **Post** action.</span><span class="sxs-lookup"><span data-stu-id="ea450-143">When the sales order is complete, choose the **Post** action.</span></span>

<span data-ttu-id="ea450-144">You can then fill or edit fields on the new item card as necessary.</span><span class="sxs-lookup"><span data-stu-id="ea450-144">You can then fill or edit fields on the new item card as necessary.</span></span> <span data-ttu-id="ea450-145">For more information, see [Register New Items](inventory-how-register-new-items.md).</span><span class="sxs-lookup"><span data-stu-id="ea450-145">For more information, see [Register New Items](inventory-how-register-new-items.md).</span></span>

> [!NOTE]  
>   <span data-ttu-id="ea450-146">An Item cross reference record is automatically created for the vendor of the item between the vendor's item number and your new item number.</span><span class="sxs-lookup"><span data-stu-id="ea450-146">An Item cross reference record is automatically created for the vendor of the item between the vendor's item number and your new item number.</span></span>

## <a name="see-also"></a><span data-ttu-id="ea450-147">See Also</span><span class="sxs-lookup"><span data-stu-id="ea450-147">See Also</span></span>
[<span data-ttu-id="ea450-148">Register New Items</span><span class="sxs-lookup"><span data-stu-id="ea450-148">Register New Items</span></span>](inventory-how-register-new-items.md)  
<span data-ttu-id="ea450-149">[Create Special Orders](sales-how-to-create-special-orders.md)|</span><span class="sxs-lookup"><span data-stu-id="ea450-149">[Create Special Orders](sales-how-to-create-special-orders.md)|</span></span>  
[<span data-ttu-id="ea450-150">Inventory</span><span class="sxs-lookup"><span data-stu-id="ea450-150">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="ea450-151">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="ea450-151">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

