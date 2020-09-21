---
title: Link a Sales Order to a Purchase Order for Direct Shipment | Microsoft Docs
description: Describes how to create a sales order linked to a purchase order to enable shipment directly from the vendor to the customer.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: direct shipment
ms.date: 08/17/2020
ms.author: edupont
ms.openlocfilehash: 0c93b138762f5a01fc06e3577e7597facf7abb5c
ms.sourcegitcommit: a80afd4e5075018716efad76d82a54e158f1392d
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 09/09/2020
ms.locfileid: "3781776"
---
# <a name="make-drop-shipments"></a>Make Drop Shipments

A drop shipment is the shipment of items from one of your vendors directly to one of your customers.

When a sales order is marked for drop shipment, and you create a purchase order specifying the customer in the **Ship-to** field, **Customer Address**, you can link the two documents to instruct the vendor to ship directly to the customer.
<br><br>  
  
> [!Video https://www.microsoft.com/en-us/videoplayer/embed/RE4mOyM?rel=0]

## <a name="to-create-a-sales-order-for-drop-shipment"></a>To create a sales order for drop shipment

To prepare a drop shipment, you create a sales order for an item and indicate on the sales line that the sale requires drop shipment.

1. Create a sales order for an item. For more information, see [Sell Products](sales-how-sell-products.md).
2. On the sales order line for the drop shipment, select the **Drop Shipment** check box. Use the **Choose Columns** function if the field is not visible. For more information, see [Personalise Your Workspace](ui-personalization-user.md).

## <a name="to-create-the-purchase-order-for-drop-shipment"></a>To create the purchase order for drop shipment

To prepare a drop shipment, you indicate on the purchase order that it must be shipped to your customer, not to yourself.

1. Create a purchase order. Do not fill any fields on the lines. For more information, see [Record Purchases](purchasing-how-record-purchases.md).
2. In the **Ship-to** field, select **Customer Address**.
3. In the **Customer** field, select the customer that you are selling to.
4. Choose the **Drop Shipments** action, and then choose the **Get Sales Order** action.
5. On the **Sales List** page, select the sales order that you prepared in [To create a sales order for drop shipment](sales-how-drop-shipment.md#to-create-a-sales-order-for-drop-shipment).
6. Choose the **OK** button.

The line information from the sales order is inserted on the purchase order line(s).

You can now instruct the vendor to ship the items to your customer, for example, by mailing the purchase order as a PDF.     

## <a name="to-create-multiple-purchase-orders-for-drop-shipments"></a>To create multiple purchase orders for drop shipments

You can also use the requisition worksheet to create the purchase order for the vendor. The advantage of using the requisition worksheet is that it can create purchase orders for all outstanding drop shipments, so you don't have to create each one individually.

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Requistion Worksheets**, and then choose the related link.
2. Choose the **Drop Shipments** action, and then choose the **Get Sales Order** action.
3. Choose the **OK** button.
4. Review the purchase order lines, and in the **Vendor No.** field, select vendor that supplies required goods. 
5. Choose the **Carry Out Action Message** action to convert reviewed lines to a purchase order.

## <a name="to-view-the-linked-purchase-order-from-the-sales-order"></a>To view the linked purchase order from the sales order

* Select the drop-shipment sales order line, choose the **Order** action, choose the **Drop Shipment** action, and then choose the **Purchase Order** action.

## <a name="to-post-a-drop-shipment"></a>To post a drop shipment

After the vendor ships the items, you can post the sales order as shipped. You can also post the purchase order, but only with the **Receive** option until the sales order has been invoiced.

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.
2. Open the sales order that you created in [To create a sales order for drop shipment](#to-create-a-sales-order-for-drop-shipment).
3. In the **Qty. to Ship** field, specify how many of the order quantity to ship, the full or a partial order quantity.
4. Choose the **Post** or **Post and Send** action.
5. Choose either the **Ship** option to invoice later, or the **Ship and Invoice** option to invoice immediately.

## <a name="see-also"></a>See Also

[Create Special Orders](sales-how-to-create-special-orders.md)  
[Purchase Items for a Sale](purchasing-how-purchase-products-sale.md)  
[Sell Products](sales-how-sell-products.md)  
[Record Purchases](purchasing-how-record-purchases.md)  
[Sales](sales-manage-sales.md)  
[Inventory](inventory-manage-inventory.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
