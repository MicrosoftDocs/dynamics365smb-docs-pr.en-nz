---
title: Status Field on Documents
description: Learn about the 'Open' and 'Released' status on quote, order, or credit memo documents.
author: rubenseishima
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.search.keywords: document, status, quote, order, credit memo, released, open, pending approval, pending prepayment,
ms.search.form: ''
ms.date: 09/19/2022
ms.author: a-reishima
ms.openlocfilehash: c96909b4ee37673ee7b0c752224478a144ad853e
ms.sourcegitcommit: 8ad79e0ec6e625796af298f756a142624f514cf3
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 09/30/2022
ms.locfileid: "9608387"
---
# <a name="status-field-on-documents"></a>Status Field on Documents

When you create a quote, order, or credit memo, the **Status** field on the document header contains the status **Open** by default.

After you have filled in the document, you can release it, and [!INCLUDE[prod_short](includes/prod_short.md)] changes the value in the **Status** field to **Released**. This status indicates that the order is ready for the next stage of processing before it is posted.

| Status | Description |
| ------ | ----------- |
| Open   | You can make changes to the document. |
| Released | The document has been released to the next stage of processing and you cannot make changes to lines of type *Item* and *Fixed Asset*.<br /><br />You can reopen a released document if you want to make changes to its contents. To move the adjusted document to the next stage of processing, you must once again release the document. |
| Pending Approval   | The document is waiting to be approved. |
| Pending Prepayment | A prepayment invoice has been posted for the document. |

## <a name="releasing"></a>Releasing

You can use the release process in different ways to ease your normal work flow, for example, to follow company procedures about approvals or to start warehouse activities.

### <a name="approval-procedures"></a>Approval procedures

Your company can use the release procedure to indicate that another user has approved the document or that an external contact can meet the specifications on the document, as shown in these examples:

* You can only release a purchase order when your vendor has indicated that they are prepared to fulfill the order.
* You create an order and a second user must approve it, perhaps for security reasons, before you are allowed to release it.
* A credit memo that you have created must be released by the manager responsible for approving all refunds.

Learn more about approval workflows at [Use Workflows](across-use-workflows.md).

### <a name="warehouse-activities"></a>Warehouse activities

If the order status is **Open**, the warehouse will not begin to prepare the shipment, and does not expect to receive the items on a purchase order. When you release the order, you indicate that the order is complete, and that the warehouse can include it in their activities.

## <a name="reopening-a-released-order"></a>Reopening a released order

You can make changes to a released order by reopening it. However, you can only increase the quantity of the lines already processed by the warehouse.

When you have made your changes and you release the order again, the goods and services tax (GST) and the invoice discount are recalculated.

If you make changes to a released order, you must notify the warehouse about the changes.

> [!NOTE]
> If you want to post a single open order or credit memo without releasing it first, the program will automatically release the document when you post it. If you post your orders or credit memos by using the **Post Batch** function, you can choose only to post the orders or credit memos that you have released.

## <a name="see-also"></a>See also

[Sell Products with a Customer Sales Order](sales-how-sell-products.md)  
[Record Purchases with Purchase Invoices](purchasing-how-record-purchases.md)  
[Ship Items](warehouse-how-ship-items.md)  
[Receive Items](warehouse-how-receive-items.md)  
[Use Approval Workflows](across-how-use-approval-workflows.md)  
[Sorting, Searching, and Filtering Lists](ui-enter-criteria-filters.md)  
[Archive Documents](across-how-to-archive-documents.md)  
[General Business Functionality](ui-across-business-areas.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
