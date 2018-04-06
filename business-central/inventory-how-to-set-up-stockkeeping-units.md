---
title: How to Set Up Stockkeeping Units | Microsoft Docs
description: You can use stockkeeping units to record information about your items for a specific location or a specific variant code.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/23/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 4870e82d4390e0a96a137579d035fee0e54b19eb
ms.contentlocale: en-nz
ms.lasthandoff: 03/22/2018

---
# <a name="set-up-stockkeeping-units"></a><span data-ttu-id="eafea-103">Set Up Stockkeeping Units</span><span class="sxs-lookup"><span data-stu-id="eafea-103">Set Up Stockkeeping Units</span></span>
<span data-ttu-id="eafea-104">You can use stockkeeping units to record information about your items for a specific location or a specific variant code.</span><span class="sxs-lookup"><span data-stu-id="eafea-104">You can use stockkeeping units to record information about your items for a specific location or a specific variant code.</span></span>  

 <span data-ttu-id="eafea-105">Stockkeeping units are a supplement to item cards.</span><span class="sxs-lookup"><span data-stu-id="eafea-105">Stockkeeping units are a supplement to item cards.</span></span> <span data-ttu-id="eafea-106">They do not replace them, although they are related to them.</span><span class="sxs-lookup"><span data-stu-id="eafea-106">They do not replace them, although they are related to them.</span></span> <span data-ttu-id="eafea-107">Stockkeeping units allow you to differentiate information about an item for a specific location, such as a warehouse or distribution centre, or a specific variant, such as different shelf numbers and different replenishment information, for the same item.</span><span class="sxs-lookup"><span data-stu-id="eafea-107">Stockkeeping units allow you to differentiate information about an item for a specific location, such as a warehouse or distribution center, or a specific variant, such as different shelf numbers and different replenishment information, for the same item.</span></span>  

## <a name="to-set-up-a-stockkeeping-unit"></a><span data-ttu-id="eafea-108">To set up a stockkeeping unit</span><span class="sxs-lookup"><span data-stu-id="eafea-108">To set up a stockkeeping unit</span></span>  

1.  <span data-ttu-id="eafea-109">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Stockkeeping Units**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="eafea-109">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Stockkeeping Units**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="eafea-110">Choose the **New** action.</span><span class="sxs-lookup"><span data-stu-id="eafea-110">Choose the **New** action.</span></span>  
3.  <span data-ttu-id="eafea-111">Fill in the fields on the card.</span><span class="sxs-lookup"><span data-stu-id="eafea-111">Fill in the fields on the card.</span></span> <span data-ttu-id="eafea-112">The following fields are required: **Item No.**, **Location Code**, and/or **Variant Code**.</span><span class="sxs-lookup"><span data-stu-id="eafea-112">The following fields are required: **Item No.**, **Location Code**, and/or **Variant Code**.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

<span data-ttu-id="eafea-113">When you have set up the first stockkeeping unit for an item, the **Stockkeeping Unit Exists** check box on the **Item** card is selected.</span><span class="sxs-lookup"><span data-stu-id="eafea-113">When you have set up the first stockkeeping unit for an item, the **Stockkeeping Unit Exists** check box on the **Item** card is selected.</span></span>  

<span data-ttu-id="eafea-114">To create several stockkeeping units for an item, use the **Create Stockkeeping Unit** batch job.</span><span class="sxs-lookup"><span data-stu-id="eafea-114">To create several stockkeeping units for an item, use the **Create Stockkeeping Unit** batch job.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="eafea-115">The information on the **Stockkeeping Unit** card has priority over the **Item** card.</span><span class="sxs-lookup"><span data-stu-id="eafea-115">The information on the **Stockkeeping Unit** card has priority over the **Item** card.</span></span>  

## <a name="see-also"></a><span data-ttu-id="eafea-116">See Also</span><span class="sxs-lookup"><span data-stu-id="eafea-116">See Also</span></span>  
[<span data-ttu-id="eafea-117">Register New Items</span><span class="sxs-lookup"><span data-stu-id="eafea-117">Register New Items</span></span>](inventory-how-register-new-items.md)  
[<span data-ttu-id="eafea-118">Setting Up Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="eafea-118">Setting Up Warehouse Management</span></span>](warehouse-setup-warehouse.md)  
[<span data-ttu-id="eafea-119">Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="eafea-119">Warehouse Management</span></span>](warehouse-manage-warehouse.md)  
[<span data-ttu-id="eafea-120">Inventory</span><span class="sxs-lookup"><span data-stu-id="eafea-120">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="eafea-121">[Assembly Management](assembly-assemble-items.md)  </span><span class="sxs-lookup"><span data-stu-id="eafea-121">[Assembly Management](assembly-assemble-items.md)  </span></span>  
[<span data-ttu-id="eafea-122">Design Details: Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="eafea-122">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="eafea-123">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="eafea-123">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
