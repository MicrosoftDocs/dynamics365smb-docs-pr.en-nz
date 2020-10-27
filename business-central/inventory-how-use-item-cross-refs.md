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
# <a name="use-item-cross-references"></a>Use Item Cross References
If you set up a cross reference between the item description that you use for an item and the description that the vendor of that item uses, then the vendor's item description is automatically inserted on purchase documents for the vendor when you fill in the **Cross-Reference No.** field. The same functionality applies for customer item numbers on sales documents.

The following procedures describe how to use item cross references on the purchase side. The steps are similar for the sales side.

> [!NOTE]
> It's becoming more common for item identifiers such as GTINs or GUIDs to contain 30 or more characters, which is more than the current feature for item cross references can handle. If you need to use references that contain more than 30 characters, your administrator can turn on the **Write longer item references** feature on the [Feature Management](https://businesscentral.dynamics.com/?page=xzy) page (link requires that you have a [!INCLUDE[d365fin](includes/d365fin_md.md)] tenant). How you use references doesn't change, but the names of things like pages and buttons will. For example, the **Item Cross-Reference Entries** page will become the **Item Reference Entries** page.

## <a name="to-set-up-an-item-cross-reference-to-a-vendors-item-description"></a>To set up an item cross reference to a vendor's item description

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items** , and then choose the related link.
2. Open the card for an item for which you want to create a cross reference to the item description that the vendor uses for that item.
3. Choose the **Cross References** action.

     If you cannot find the **Cross References** action, choose to view more options, and then find it under **Related** > **Item** .
  
4. On a new line on the **Item Cross-Reference Entries** page, fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)].

## <a name="to-enter-a-vendors-item-description-on-a-purchase-order"></a>To enter a vendor's item description on a purchase order

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchase Orders** , and then choose the related link.
2. Create a purchase order for the vendor that you set up an item cross reference for in the previous procedure.
3. Create a purchase line for the item that you set up an item cross reference for in the previous procedure.
4. In the **Cross-Reference No.** field, select the item cross reference that you have created, and then choose the **OK** button.

The **Description** field on the line is overwritten with the vendor's item description, as set up on the item cross-reference entry.

## <a name="see-also"></a>See Also
[Register New Items](inventory-how-register-new-items.md)  
[Inventory](inventory-manage-inventory.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
