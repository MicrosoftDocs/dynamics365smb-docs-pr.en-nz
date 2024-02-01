---
title: 'Add Attachments, Links, and Notes on Records'
description: 'Attach a hyperlink to a document or a website to a specific record, such as a customer or document.'
author: brentholtorf
ms.author: bholtorf
ms.reviewer: ivkoleti
ms.topic: how-to
ms.date: 09/15/2023
ms.custom: bap-template
ms-service: dynamics-365-business-central
ms.service: dynamics-365-business-central
---
# <a name="manage-attachments-links-and-notes-on-cards-and-documents"></a>Manage attachments, links, and notes on cards and documents

On most list pages, cards, and documents, you can attach files, add links, and write notes on the **Attachments** tab of the **FactBox** pane. The number in the tab title indicates how many attached files, links, or notes exist for the card or document.

On the **Lines** FastTab, you can also use the **Attachments** action to attach documents to a specific line. For example, you might want to attach design specifications to an item on a purchase invoice.

Attachments, links, and notes stay attached to the card or document while it's processed into other states. For example, from an ongoing sales order to a posted sales invoice. However, none of the attachment types are output from the system, for example, when printing or when saving to a file.

You can also add attachments to the emails you send from [!INCLUDE [prod_short](includes/prod_short.md)]. When you send an email directly from a document, such as a sales quote, the **Add file from source document** action lets you choose files that are attached to it. You can only choose files that are attached to the document. You can't choose files that are attached to lines.

> [!NOTE]
> When you partially ship and invoice a sales or purchase order, the attachment will only be attached to the final invoice of the order. Similarly, when you invoice deferrals, the attachment is attached to the G/L entries for the document but not for the deferral entries.
>
> If you delete an order before it is invoiced, the attachment is also removed.
>
> When you use the **Get Receipt Lines** action on a purchase invoice, the attachment on the related purchase order is added to the purchase invoice.

## <a name="to-attach-a-file-to-a-purchase-invoice"></a>To attach a file to a purchase invoice

You can attach any type of file, such as text, image, or video files, to a card, document, or a line on a document. This is useful, for example, when you want to store a vendor's invoice as a PDF file on the related purchase invoice in [!INCLUDE[prod_short](includes/prod_short.md)].

> [!NOTE]
> Files attached with the Incoming Documents feature aren't included on the **Attachments** tab. For more information, see [Incoming Documents](across-income-documents.md). The same is true for files that are attached to lines on documents.

The following procedure is based on a purchase invoice. The steps are similar for all other supported documents and cards.

> [!TIP]
> If your attachment is specific to a line on a document, you can attach it to the line. Choose the line, and then choose the **Attachments** action.

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchase Invoices**, and then choose the related link.
2. Open the purchase invoice that you want to attach a file to.
3. On the **FactBox** pane, choose the **Attachments** tab.
4. Choose the value behind the **Documents** field, such as "0".
5. On the **Attached Documents** page, in the **Attachment** field.
6. On the **Attach a document** dialogue box, do one of the following steps to attach a file:

   [!INCLUDE[file-upload](includes/file-upload.md)]

The file is now attached to the purchase invoice.

## <a name="to-view-an-attached-file"></a>To view an attached file

1. On the FactBox, open the **Attachments** tab.
2. Choose the value behind the **Documents** field, such as "1".
3. On the **Attached Documents** page, choose the **Preview** action.
4. Open the downloaded file.

## <a name="to-save-a-document-as-a-pdf-attachment"></a>To save a document as a PDF attachment

Whenever you need to save a document as a file, you can use the **Attach as PDF** action to capture the current document content as a PDF file attached to the FactBox of the document. This is useful, for example, when documents follow multiple steps in a process, such as a sales process or an approval workflow, and you want to refer to a printout of the previous step.

The following procedure is based on a sales order. The steps are similar for all supported documents.

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.
2. Select a sales order, and then choose the **Attach as PDF** action.

A PDF file with the current content of the sales order is added to the **Attachments** tab in the FactBox.

## <a name="to-add-a-link-from-an-item-card"></a>To add a link from an item card

You can add a link from a card or document to any URL. This is useful, for example, when you want to link an item card with the supplier's item catalogue.

The following procedure is based on an item card. The steps are similar for all other supported cards and documents.

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.
2. Select the item that you want to add a link from, and then choose the **Attachments** tab in the FactBox.
3. In the **Links**, choose the **+** icon.
4. In the **Link Address** field, enter the link.

    The link must be a valid internet or intranet URL.

5. In the **Description** field, enter any information about the link.  
6. Choose the **OK** button.

The link is now attached to the item card.  

## <a name="to-write-a-note-on-a-sales-order"></a>To write a note on a sales order

You can write a note on a document or card, for example, to communicate special instructions to other users of the document or card. You can include file links and URLs in notes.

> [!NOTE]
> Notes on the **Attachments** tab are not related to internal notes functionality, which is mainly used to communicate between workflow users. For more information, see [Setting Up Workflow Notifications](across-setting-up-workflow-notifications.md).

The following procedure is based on a sales order. The steps are similar for all other supported documents and cards.

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.
2. Select the sales order that you want to write a note on, and then choose the **Attachments** tab in the FactBox.
3. In the **Notes** section, choose the **+** icon.
4. In the **Note** field, write any text, such as "This is an urgent order.".
5. Choose the **OK** button.

The note is now attached to the sales order.

## <a name="see-also"></a>See also
[Work with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  
[Incoming Documents](across-income-documents.md)  
[Setting Up Workflow Notifications](across-setting-up-workflow-notifications.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]
