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
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: 3c368af3347c72f2cf355876ed5574151095f993
ms.contentlocale: en-nz
ms.lasthandoff: 09/28/2018

---
# <a name="set-up-stockkeeping-units"></a><span data-ttu-id="5d0c2-103">Set Up Stockkeeping Units</span><span class="sxs-lookup"><span data-stu-id="5d0c2-103">Set Up Stockkeeping Units</span></span>
<span data-ttu-id="5d0c2-104">You can use stockkeeping units to record information about your items for a specific location or a specific variant code.</span><span class="sxs-lookup"><span data-stu-id="5d0c2-104">You can use stockkeeping units to record information about your items for a specific location or a specific variant code.</span></span>  

 <span data-ttu-id="5d0c2-105">Stockkeeping units are a supplement to item cards.</span><span class="sxs-lookup"><span data-stu-id="5d0c2-105">Stockkeeping units are a supplement to item cards.</span></span> <span data-ttu-id="5d0c2-106">They do not replace them, although they are related to them.</span><span class="sxs-lookup"><span data-stu-id="5d0c2-106">They do not replace them, although they are related to them.</span></span> <span data-ttu-id="5d0c2-107">Stockkeeping units allow you to differentiate information about an item for a specific location, such as a warehouse or distribution centre, or a specific variant, such as different shelf numbers and different replenishment information, for the same item.</span><span class="sxs-lookup"><span data-stu-id="5d0c2-107">Stockkeeping units allow you to differentiate information about an item for a specific location, such as a warehouse or distribution center, or a specific variant, such as different shelf numbers and different replenishment information, for the same item.</span></span>  

## <a name="to-set-up-a-stockkeeping-unit"></a><span data-ttu-id="5d0c2-108">To set up a stockkeeping unit</span><span class="sxs-lookup"><span data-stu-id="5d0c2-108">To set up a stockkeeping unit</span></span>  

1.  <span data-ttu-id="5d0c2-109">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Stockkeeping Units**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="5d0c2-109">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Stockkeeping Units**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="5d0c2-110">Choose the **New** action.</span><span class="sxs-lookup"><span data-stu-id="5d0c2-110">Choose the **New** action.</span></span>  
3.  <span data-ttu-id="5d0c2-111">Fill in the fields on the card.</span><span class="sxs-lookup"><span data-stu-id="5d0c2-111">Fill in the fields on the card.</span></span> <span data-ttu-id="5d0c2-112">The following fields are required: **Item No.**, **Location Code**, and/or **Variant Code**.</span><span class="sxs-lookup"><span data-stu-id="5d0c2-112">The following fields are required: **Item No.**, **Location Code**, and/or **Variant Code**.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

<span data-ttu-id="5d0c2-113">When you have set up the first stockkeeping unit for an item, the **Stockkeeping Unit Exists** check box on the **Item** card is selected.</span><span class="sxs-lookup"><span data-stu-id="5d0c2-113">When you have set up the first stockkeeping unit for an item, the **Stockkeeping Unit Exists** check box on the **Item** card is selected.</span></span>  

<span data-ttu-id="5d0c2-114">To create several stockkeeping units for an item, use the **Create Stockkeeping Unit** batch job.</span><span class="sxs-lookup"><span data-stu-id="5d0c2-114">To create several stockkeeping units for an item, use the **Create Stockkeeping Unit** batch job.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="5d0c2-115">The information on the **Stockkeeping Unit** card has priority over the **Item** card.</span><span class="sxs-lookup"><span data-stu-id="5d0c2-115">The information on the **Stockkeeping Unit** card has priority over the **Item** card.</span></span>  

## <a name="see-also"></a><span data-ttu-id="5d0c2-116">See Also</span><span class="sxs-lookup"><span data-stu-id="5d0c2-116">See Also</span></span>  
[<span data-ttu-id="5d0c2-117">Register New Items</span><span class="sxs-lookup"><span data-stu-id="5d0c2-117">Register New Items</span></span>](inventory-how-register-new-items.md)  
[<span data-ttu-id="5d0c2-118">Setting Up Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="5d0c2-118">Setting Up Warehouse Management</span></span>](warehouse-setup-warehouse.md)  
[<span data-ttu-id="5d0c2-119">Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="5d0c2-119">Warehouse Management</span></span>](warehouse-manage-warehouse.md)  
[<span data-ttu-id="5d0c2-120">Inventory</span><span class="sxs-lookup"><span data-stu-id="5d0c2-120">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="5d0c2-121">[Assembly Management](assembly-assemble-items.md)  </span><span class="sxs-lookup"><span data-stu-id="5d0c2-121">[Assembly Management](assembly-assemble-items.md)  </span></span>  
[<span data-ttu-id="5d0c2-122">Design Details: Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="5d0c2-122">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="5d0c2-123">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="5d0c2-123">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  

