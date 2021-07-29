---
title: How to Combine Shipments on a Single Invoice | Microsoft Docs
description: If you want to invoice more than one shipment at a time, you can use the combined shipments feature.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 1465ce4baadec43d28731dab50870af3c10bd77e
ms.sourcegitcommit: a7cb0be8eae6ece95f5259d7de7a48b385c9cfeb
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 07/08/2021
ms.locfileid: "6442741"
---
# <a name="combine-shipments-on-a-single-invoice"></a>Combine Shipments on a Single Invoice
If you want to invoice more than one shipment at a time, you can use the combined shipments feature.  

Before you can create a combined shipment, more than one sales shipment for the same customer in the same currency must be posted. In other words, you must have create two or more sales orders and post them as shipped, but not invoiced. 

## <a name="to-manually-combine-shipments-on-a-single-invoice"></a>To manually combine shipments on a single invoice  
1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Invoices**, and then choose the related link.  
2. Choose the **New** action. For more information, see [Invoice Sales](sales-how-invoice-sales.md).
3. In the **Sell-to Customer No.** field, enter the customer who will receive the invoice for the shipped items.  
4. On the **Lines** FastTab, choose the **Get Shipment Lines** action.  
5. Select the shipment line that you want to include in the invoice:  

    - To insert all lines, select all lines and choose the **OK** button.  
    - To insert specific lines, select the lines and choose the **OK** button. You can use the Ctrl key to select multiple nonsequential lines.  

    If an incorrect shipment line was selected or you want to start over, you can simply delete the lines on the invoice and re-run the **Get Shipment Lines** function.  
7. To post the invoice, choose the **Post** action.  

## <a name="to-automatically-combine-shipments-on-a-single-invoice"></a>To automatically combine shipments on a single invoice  
[!INCLUDE[prod_short](includes/prod_short.md)] will select only sales orders where **Combine Shipments** is chosen. 

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Combine Shipments**, and then choose the related link. The batch job request page opens.  
2. Fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. Choose the **Post Invoices** check box.  
4. Choose the **OK** button.  

> [!NOTE]  
>  You will need to manually post the invoices if the **Post Invoices** check box was not selected on the batch job.  

## <a name="to-remove-open-sales-orders-after-combined-shipment-posting"></a>To remove open sales orders after combined shipment posting 
When shipments are combined on an invoice and posted, a posted sales invoice is created for the invoiced lines. The **Quantity Invoiced** field on the originating blanket sales order or sales order is updated based on the invoiced quantity.  

When you invoice shipments in this way, the orders from which the shipments were posted still exist, even if they have been fully shipped and invoiced.   

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Delete Invoiced Sales Orders**, and then select the link.  
2. Specify in the **No.** filter field which sales orders to delete.  
3. Choose the **OK** button.  

Alternatively, delete individual sales orders manually.  

Repeat steps 1 through 3 for any other affected documents, such as blanket sales orders.

## <a name="see-also"></a>See Also  
[Sales](sales-manage-sales.md)  
[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]