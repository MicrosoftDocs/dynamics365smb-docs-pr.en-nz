---
title: Amend or cancel unpaid purchase invoices
description: 'Explains how to correct, cancel, or undo a posted purchase invoice and automatically create a purchase credit memo.'
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bholtorf
ms.topic: conceptual
ms.search.keywords: 'undo, credit memo, return'
ms.search.form: '138, 140, 146'
ms.date: 04/19/2024
ms.service: dynamics-365-business-central
---
# Correct or cancel unpaid purchase invoices

You can correct or cancel a posted purchase invoice. This is useful if you want to correct a typing mistake, or if you want to change the purchase early in the order process.

If you have already paid for products on the posted purchase invoice, you can't correct or cancel it from the posted purchase invoice itself. Instead, you must manually create a purchase credit memo to reverse the purchase, optionally managed with a purchase return order. The same applies if you want to modify a posted purchase invoice that was based on combined purchase receipts. For more information, see [Process Purchase Returns or Cancellations](purchasing-how-process-purchase-returns-cancellations.md).

On the **Posted Purchase Invoice** page, you can choose the **Correct** button or the **Cancel** button. When you correct or cancel a posted purchase invoice, the corrective purchase credit memo is applied to all general ledger and inventory ledger entries that were created when the initial purchase invoice was posted. This reverses the posted purchase invoice in your financial records and leaves the corrective posted purchase credit memo for your audit trail. The video describes the use of **Correct** and **Cancel**.
<br><br>
> [!Video https://www.microsoft.com/videoplayer/embed/RE4dhoc?rel=0]

## To correct a posted purchase invoice

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Posted Purchase Invoices**, and then choose the related link.  
2. Select the posted purchase invoice that you want to correct.  

    > [!NOTE]  
    >   If the **Canceled** check box is selected, then you cannot correct the posted purchase invoice because it has already been corrected or canceled.
3. On the **Posted Purchase Invoice** page, choose **Correct**.

    A new purchase invoice with the same information is created where you can make the correction. For more information, see [Record Purchases](purchasing-how-record-purchases.md). The **Cancelled** field on the initial posted purchase invoice is changed to **Yes**.

    A purchase credit memo is automatically created and posted to void the initial posted purchase invoice.
4. Choose **Show Corrective Credit Memo** to view the posted purchase credit memo that voids the initial posted purchase invoice.

## To cancel a posted purchase invoice

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Posted Purchase Invoices**, and then choose the related link.  
2. Select the posted purchase invoice that you want to cancel.

    > [!NOTE]  
    >   If the **Canceled** check box is selected, then you cannot cancel the posted purchase invoice because it has already been canceled or corrected.
3. On the **Posted Purchase Invoice** page, choose **Cancel**.

    A purchase credit memo is automatically created and posted to void the initial posted purchase invoice. The **Cancelled** field on the initial posted purchase invoice is changed to **Yes**.
4. Choose **Show Corrective Credit Memo** to view the posted purchase credit memo that voids the initial posted purchase invoice.

### Partial invoice posting also supported

If the cancellation is related to a partial invoice posting, then the originating purchase order line is updated to reflect the cancelled invoiced quantity. The **Qty. to Invoice** and **Quantity Invoiced** fields on the related purchase order line are reset to the values before the partial posting.

## See also

[Purchasing](purchasing-manage-purchasing.md)  
[Record Purchases](purchasing-how-record-purchases.md)  
[Work with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]
