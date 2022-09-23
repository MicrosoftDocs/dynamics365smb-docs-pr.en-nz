---
title: Create and Manage Catalogue Items
description: Describes how to sell items that you don't keep in your list of items.
author: brentholtorf
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: non-inventoriable
ms.search.forms: 5725, 5726, 5732
ms.date: 06/20/2022
ms.author: bholtorf
ms.openlocfilehash: deeca03327afa4b231cb9b4ce23088334fa50153
ms.sourcegitcommit: 3acadf94fa34ca57fc137cb2296e644fbabc1a60
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 09/19/2022
ms.locfileid: "9532123"
---
# <a name="work-with-catalog-items"></a>Work with Catalogue Items

Catalogue items are items that you don't manage in [!INCLUDE[prod_short](includes/prod_short.md)] until you sell them. When you use the **Select Catalogue Item** action to add a catalogue item to a line on a sales order or quote, the catalogue item is converted to a regular item.

> [!NOTE]  
> You cannot select a catalogue item from the **Sales Invoice** page.

A catalogue item typically has the item number of the vendor who supplies it. Before you can convert a catalogue item to a normal item, you must specify how to convert vendor item numbers to your item numbering. For more information, see [Specify how catalogue item numbers are converted to your own numbering](#specify-how-catalog-item-numbers-are-converted-to-your-own-numbering).  

> [!IMPORTANT]
> Catalogue items are not to be mistaken with non-inventory items, which are regular items that are given the type **Non-Inventory** to keep them out of availability and costing calculations, for example, because they are only used internally and have a low cost. For more information, see [About Item Types](inventory-about-item-types.md).

## <a name="create-a-catalog-item"></a>Create a catalogue item

Catalogue item cards have much less information than normal item cards because you only use them to offer on quotes and in other ways. For that reason, they must be converted to normal item cards before you can post sales transactions for them.

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Catalogue Items**, and then choose the related link.
2. Choose the **New** action.
3. Fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="specify-how-catalog-item-numbers-are-converted-to-your-own-numbering"></a>Specify how catalogue item numbers are converted to your own numbering

Before you can convert a catalogue item to a normal item, you must specify how to convert vendor item numbers to your item numbering.

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Catalogue Item Setup**, and then choose the related link.
2. Fill in the fields as necessary.

## <a name="convert-a-catalog-item-to-a-normal-item"></a>Convert a catalogue item to a normal item

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Catalogue Items**, and then choose the related link.
2. Open the card for a catalogue item that you want to convert to a normal item.
3. On the **Catalogue Item Card** page, choose the **Create Item** action.

A new item card pre-filled with information from the catalogue item and a relevant item template is created. You can then fill or edit fields on the new item card as necessary. For more information, see [Register New Items](inventory-how-register-new-items.md).

## <a name="to-sell-a-catalog-item-and-convert-it-to-a-normal-item"></a>To sell a catalogue item, and convert it to a normal item

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.
2. Choose the **New** action. Fill in the fields on the **General** FastTab as for any sales order. For more information, see [Sell Products](sales-how-sell-products.md).
3. On a new sales line, in the **Type** field, select **Item**, but leave the **No.** field empty.
4. Choose the **Line** action, and then choose the **Select Catalogue Items** action.

    The catalogue item is converted to a normal item. A new item card prefilled with information from the catalogue item and a relevant item template is created.
5. On the **Catalogue Items** page, select the catalogue item that you want to sell, and then choose the **OK** button.
6. When the sales order is complete, choose the **Post** action.

You can then fill or edit fields on the new item card as necessary. For more information, see [Register New Items](inventory-how-register-new-items.md).

> [!NOTE]  
> An item reference is automatically item between the vendor's item number and your new item number. For more information, see [Use Item References](inventory-how-use-item-cross-refs.md).

## <a name="see-related-microsoft-training"></a>See related [Microsoft training](/training/modules/create-sales-documents-dynamics-365-business-central/)

## <a name="see-also"></a>See also

[Register New Items](inventory-how-register-new-items.md)  
[Create Special Orders](sales-how-to-create-special-orders.md)  
[Inventory](inventory-manage-inventory.md)  
[Work with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]
