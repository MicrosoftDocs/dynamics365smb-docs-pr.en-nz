---
title: Define Which Incoming Docs to See
description: 'Adjust the default view of incoming documents, such as e-invoices, to improve your overview of processed and unprocessed records.'
author: brentholtorf
ms.topic: conceptual
ms.devlang: al
ms.search.keywords: 'electronic document, e-invoice, incoming document, OCR, ecommerce, document exchange, import invoice'
ms.date: 06/14/2022
ms.author: bholtorf
ms.service: dynamics-365-business-central
---
# <a name="manage-many-incoming-document-records"></a>Manage Many Incoming Document Records

As you create or process incoming document records, the number of lines on the **Incoming Documents** page may grow to an extent where you lose overview. Therefore, you can set incoming document records to *Processed* to remove them from the default view. When you choose the **Show All** action, you can view both processed and unprocessed records.

> [!NOTE]  
> You cannot edit information, attach files, or perform other processes on incoming document records that are set to *Processed*. You must first set it to *Unprocessed*.

The **Processed** check box is automatically selected on incoming document records that have been processed, but you can also select or deselect the check box manually. Depending on your business process, an incoming document record may be processed when a related document has been created for it or a file has been attached.

> [!NOTE]  
> When you open the **Incoming Documents** page with the **My Incoming Documents** action on the Role Centre, only unprocessed incoming document records are shown by default. This is referred to in this topic as "the default view".

## <a name="to-remove-incoming-document-records-from-the-default-view"></a>To remove incoming document records from the default view

1. On the **Incoming Documents** page, select one or more lines for incoming document records that you want to remove from the default view.
2. Choose the **Set to Processed** action.

    The incoming document records are removed from the default view, and the **Processed** check box is selected on the lines.

> [!NOTE]  
> You can also perform this action for the individual record on the **Incoming Document Card** page.

## <a name="to-view-all-incoming-document-records"></a>To view all incoming document records

1. On the **Incoming Documents** page, choose the **Show All** action.

All incoming document records are displayed, including records where the **Processed** check box isn't selected.

## <a name="to-add-incoming-document-records-to-the-default-view"></a>To add incoming document records to the default view

1. On the **Incoming Documents** page, choose the **Show All** action.
2. Select one or more lines for incoming document records that you want to appear in the default view.
3. Choose the **Set to Unprocessed** action.  

> [!NOTE]  
> You can also perform this action for the individual record on the **Incoming Document Card** page.

## <a name="see-also"></a>See also
  
[Create Incoming Document Records](across-how-create-income-document-records.md)
[Create Incoming Document Records Directly from Documents and Entries](across-how-connect-disconnect-income-document-records.md)
[Incoming Documents](across-income-documents.md)  
[Purchasing](purchasing-manage-purchasing.md)  
[Work with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]
