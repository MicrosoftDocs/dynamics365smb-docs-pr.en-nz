---
title: How to Set Up Shipping Methods | Microsoft Docs
description: You can set up a code for each of your offered shipment methods, such as  and enter information about them.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: incoterms
ms.date: 10/01/2019
ms.author: sgroespe
ms.openlocfilehash: 75a3e689083e64f446e84b2bc3b1d26961e3d898
ms.sourcegitcommit: cfc92eefa8b06fb426482f54e393f0e6e222f712
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 12/03/2019
ms.locfileid: "2877559"
---
# <a name="set-up-shipment-methods"></a>Set Up Shipment Methods
Shipment methods, also called incoterms, often depend on the items, the customers, and the vendors. For example, if the customer lives on an island, they can choose to have items always shipped by air or always by sea. Some customers may require next day delivery. Some may want to pick up the order. On the customer and vendor cards, you can specify what sort of delivery is desired.

You set up the description and code for each shipment method on the **Shipment Methods** page. For example, you can set up the code FOB, and enter Free on Board in the **Description** field. You can then enter the code in **Shipment Method Code** fields elsewhere in the system, such as on a customer card. Then when you create new orders, invoices, credit memos, and so on, the system will enter the description represented by the code. You can change it on the document as needed.

## <a name="to-set-up-a-shipment-code"></a>To set up a shipment code
1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Shipment Methods**, and then choose the related link.
2. On the **Shipment Methods** page, choose the **New** action.
3. On the new line, specify a code and description for the shipment method.

## <a name="see-also"></a>See Also
[Incoterms](https://iccwbo.org/resources-for-business/incoterms-rules)  
[Set Up Shipping Agents](sales-how-to-set-up-shipping-agents.md)  
[Track Packages](sales-how-track-packages.md)    
[Warehouse Management](warehouse-manage-warehouse.md)  
[Inventory](inventory-manage-inventory.md)  
[Setting Up Warehouse Management](warehouse-setup-warehouse.md)     
[Assembly Management](assembly-assemble-items.md)    
[Design Details: Warehouse Management](design-details-warehouse-management.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  
