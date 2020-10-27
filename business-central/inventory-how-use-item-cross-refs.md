---
title: Use Item Cross-References| Microsoft Docs
description: Set up references between the descriptions that you and your vendor use for an item so you can insert the vendor's item description on purchase documents.
services: project-madeira
documentationcenter: ''
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: item reference, cross reference, inventory
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 056897c799dd12755432637690446a0797c9f18c
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 10/01/2020
ms.locfileid: "3919454"
---
# <a name="use-item-cross-references"></a><span data-ttu-id="0d064-103">Use Item Cross References</span><span class="sxs-lookup"><span data-stu-id="0d064-103">Use Item Cross References</span></span>
<span data-ttu-id="0d064-104">If you set up a cross reference between the item description that you use for an item and the description that the vendor of that item uses, then the vendor's item description is automatically inserted on purchase documents for the vendor when you fill in the **Cross-Reference No.**</span><span class="sxs-lookup"><span data-stu-id="0d064-104">If you set up a cross reference between the item description that you use for an item and the description that the vendor of that item uses, then the vendor's item description is automatically inserted on purchase documents for the vendor when you fill in the **Cross-Reference No.**</span></span> <span data-ttu-id="0d064-105">field.</span><span class="sxs-lookup"><span data-stu-id="0d064-105">field.</span></span> <span data-ttu-id="0d064-106">The same functionality applies for customer item numbers on sales documents.</span><span class="sxs-lookup"><span data-stu-id="0d064-106">The same functionality applies for customer item numbers on sales documents.</span></span>

<span data-ttu-id="0d064-107">The following procedures describe how to use item cross references on the purchase side.</span><span class="sxs-lookup"><span data-stu-id="0d064-107">The following procedures describe how to use item cross references on the purchase side.</span></span> <span data-ttu-id="0d064-108">The steps are similar for the sales side.</span><span class="sxs-lookup"><span data-stu-id="0d064-108">The steps are similar for the sales side.</span></span>

> [!NOTE]
> <span data-ttu-id="0d064-109">It's becoming more common for item identifiers such as GTINs or GUIDs to contain 30 or more characters, which is more than the current feature for item cross references can handle.</span><span class="sxs-lookup"><span data-stu-id="0d064-109">It's becoming more common for item identifiers such as GTINs or GUIDs to contain 30 or more characters, which is more than the current feature for item cross references can handle.</span></span> <span data-ttu-id="0d064-110">If you need to use references that contain more than 30 characters, your administrator can turn on the **Write longer item references** feature on the [Feature Management](https://businesscentral.dynamics.com/?page=xzy) page (link requires that you have a [!INCLUDE[d365fin](includes/d365fin_md.md)] tenant).</span><span class="sxs-lookup"><span data-stu-id="0d064-110">If you need to use references that contain more than 30 characters, your administrator can turn on the **Write longer item references** feature on the [Feature Management](https://businesscentral.dynamics.com/?page=xzy) page (link requires that you have a [!INCLUDE[d365fin](includes/d365fin_md.md)] tenant).</span></span> <span data-ttu-id="0d064-111">How you use references doesn't change, but the names of things like pages and buttons will.</span><span class="sxs-lookup"><span data-stu-id="0d064-111">How you use references doesn't change, but the names of things like pages and buttons will.</span></span> <span data-ttu-id="0d064-112">For example, the **Item Cross-Reference Entries** page will become the **Item Reference Entries** page.</span><span class="sxs-lookup"><span data-stu-id="0d064-112">For example, the **Item Cross-Reference Entries** page will become the **Item Reference Entries** page.</span></span>

## <a name="to-set-up-an-item-cross-reference-to-a-vendors-item-description"></a><span data-ttu-id="0d064-113">To set up an item cross reference to a vendor's item description</span><span class="sxs-lookup"><span data-stu-id="0d064-113">To set up an item cross reference to a vendor's item description</span></span>

1. <span data-ttu-id="0d064-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items** , and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="0d064-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items** , and then choose the related link.</span></span>
2. <span data-ttu-id="0d064-115">Open the card for an item for which you want to create a cross reference to the item description that the vendor uses for that item.</span><span class="sxs-lookup"><span data-stu-id="0d064-115">Open the card for an item for which you want to create a cross reference to the item description that the vendor uses for that item.</span></span>
3. <span data-ttu-id="0d064-116">Choose the **Cross References** action.</span><span class="sxs-lookup"><span data-stu-id="0d064-116">Choose the **Cross References** action.</span></span>

     <span data-ttu-id="0d064-117">If you cannot find the **Cross References** action, choose to view more options, and then find it under **Related** > **Item** .</span><span class="sxs-lookup"><span data-stu-id="0d064-117">If you cannot find the **Cross References** action, choose to view more options, and then find it under **Related** > **Item** .</span></span>
  
4. <span data-ttu-id="0d064-118">On a new line on the **Item Cross-Reference Entries** page, fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="0d064-118">On a new line on the **Item Cross-Reference Entries** page, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]<span data-ttu-id="0d064-119">.</span><span class="sxs-lookup"><span data-stu-id="0d064-119">.</span></span>

## <a name="to-enter-a-vendors-item-description-on-a-purchase-order"></a><span data-ttu-id="0d064-120">To enter a vendor's item description on a purchase order</span><span class="sxs-lookup"><span data-stu-id="0d064-120">To enter a vendor's item description on a purchase order</span></span>

1. <span data-ttu-id="0d064-121">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchase Orders** , and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="0d064-121">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchase Orders** , and then choose the related link.</span></span>
2. <span data-ttu-id="0d064-122">Create a purchase order for the vendor that you set up an item cross reference for in the previous procedure.</span><span class="sxs-lookup"><span data-stu-id="0d064-122">Create a purchase order for the vendor that you set up an item cross reference for in the previous procedure.</span></span>
3. <span data-ttu-id="0d064-123">Create a purchase line for the item that you set up an item cross reference for in the previous procedure.</span><span class="sxs-lookup"><span data-stu-id="0d064-123">Create a purchase line for the item that you set up an item cross reference for in the previous procedure.</span></span>
4. <span data-ttu-id="0d064-124">In the **Cross-Reference No.**</span><span class="sxs-lookup"><span data-stu-id="0d064-124">In the **Cross-Reference No.**</span></span> <span data-ttu-id="0d064-125">field, select the item cross reference that you have created, and then choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="0d064-125">field, select the item cross reference that you have created, and then choose the **OK** button.</span></span>

<span data-ttu-id="0d064-126">The **Description** field on the line is overwritten with the vendor's item description, as set up on the item cross-reference entry.</span><span class="sxs-lookup"><span data-stu-id="0d064-126">The **Description** field on the line is overwritten with the vendor's item description, as set up on the item cross-reference entry.</span></span>

## <a name="see-also"></a><span data-ttu-id="0d064-127">See Also</span><span class="sxs-lookup"><span data-stu-id="0d064-127">See Also</span></span>
[<span data-ttu-id="0d064-128">Register New Items</span><span class="sxs-lookup"><span data-stu-id="0d064-128">Register New Items</span></span>](inventory-how-register-new-items.md)  
[<span data-ttu-id="0d064-129">Inventory</span><span class="sxs-lookup"><span data-stu-id="0d064-129">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="0d064-130">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="0d064-130">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
