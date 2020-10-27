---
title: Correct or Cancel a Posted Sales Invoice | Microsoft Docs
description: Describes how to correct, undo, or cancel a posted sales invoice and apply a sales credit memo.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: undo, credit memo, return
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 3803ce840569d1b1668db64879e68395ee6f3a65
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 10/01/2020
ms.locfileid: "3926313"
---
# <a name="correct-or-cancel-unpaid-sales-invoices"></a>Correct or Cancel Unpaid Sales Invoices

You can correct or cancel a posted sales invoice. This is useful if you make a mistake or if the customer requests a change.

> [!NOTE]  
> After a posted sales invoice has been partially or fully paid, you cannot correct or cancel it from the posted sales invoice itself. Instead, you must manually create a sales credit memo to void the sale and reimburse the customer, optionally managed with a sales return order. For more information, see [Process Sales Returns or Cancellations](sales-how-process-sales-returns-cancellations.md).

On the **Posted Sales Invoice** page, you can choose the **Correct** action or the **Cancel** action to perform the actions that are described in the following table.

| Action | Description |
| --- | --- |
| **Correct** |The posted sales invoice is cancelled. A new sales invoice with the same information is created. You can make the correction and then continue the sales process. The new sales invoice has a different number than the initial sales invoice. A corrective sales credit memo is automatically created and posted to void the initial posted sales invoice. On the initial posted sales invoice, the Cancelled and Paid check boxes are selected. |
| **Cancel** |The posted sales invoice is cancelled. A corrective sales credit memo is automatically created and posted to void the initial posted sales invoice. On the initial posted sales invoice, the Cancelled and Paid check boxes are selected. |

When you correct or cancel a posted sales invoice, the corrective sales credit memo is applied to all general ledger and inventory ledger entries that were created when the initial sales invoice was posted. This reverses the posted sales invoice in your financial records and leaves the corrective posted sales credit memo for your audit trail.  

> [!TIP]
> If you have posted a prepayment invoice for a sales invoice that you then correct or cancel, you must correct or cancel the prepayment as well. For more information, see [Correct Prepayments](finance-how-to-correct-prepayments.md).

## <a name="to-correct-a-posted-sales-invoice"></a>To correct a posted sales invoice

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Posted Sales Invoices** , and then choose the related link.  
2. Select the posted sales invoice that you want to correct.

    > [!NOTE]  
    >   If the **Canceled** check box is selected, then you cannot correct the posted sales invoice because it has already been corrected or canceled.
3. On the **Posted Sales Invoice** page, choose the **Correct** action.  
4. A new sales invoice with the same information is created where you can make the correction. The **Cancelled** field on the initial posted sales invoice is changed to **Yes** .

    A sales credit memo is automatically created and posted to void the initial posted sales invoice.
5. Choose the **Show Corrective Credit Memo** action to view the posted sales credit memo that voids the initial posted sales invoice.

## <a name="to-cancel-a-posted-sales-invoice"></a>To cancel a posted sales invoice

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Posted Sales Invoices** , and then choose the related link.  
2. Select the posted sales invoice that you want to cancel.

    > [!NOTE]  
    >   If the **Canceled** check box is selected, then you cannot cancel the posted sales invoice because it has already been canceled or corrected.
3. On the **Posted Sales Invoice** page, choose the **Cancel** action.

    A sales credit memo is automatically created and posted to void the initial posted sales invoice. The **Cancelled** field on the initial posted sales invoice is changed to **Yes** .
4. Choose **Show Corrective Credit Memo** to view the posted sales credit memo that voids the initial posted sales invoice.

### <a name="partial-invoice-posting-also-supported"></a>Partial Invoice Posting also Supported

If the cancellation is related to a partial invoice posting, then the originating sales order line is updated to reflect the cancelled invoiced quantity. The **Qty. to Invoice** and **Qty. Invoiced** fields on the related sales order line are reset to the values before the partial posting.

## <a name="see-also"></a>See Also

[Sales](sales-manage-sales.md)  
[Setting Up Sales](sales-setup-sales.md)  
[Send Documents by Email](ui-how-send-documents-email.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
