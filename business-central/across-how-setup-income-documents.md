---
title: Set Up Incoming Documents
description: 'Set up the Incoming Documents feature to create electronic documents, manage OCR tasks, import invoices, and convert image files.'
author: SorenGP
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 'electronic document, e-invoice, incoming document, OCR, ecommerce, document exchange, import invoice'
ms.date: 06/14/2022
ms.author: edupont
---
# <a name="set-up-incoming-documents"></a><a name="set-up-incoming-documents"></a>Set Up Incoming Documents

If you create general journal lines from incoming document records, you must specify on the **Incoming Documents Setup** page which journal template and batch to use.

When the **Incoming Documents** feature is set up, you can use different functions to review expense receipts, manage OCR tasks, and convert incoming document files, manually or automatically, to the relevant documents or journal lines. The external files can be attached at any process stage, including to posted documents and to the resulting vendor, customer, and general ledger entries. For more information, see [Create Incoming Documents Records](across-how-create-income-document-records.md).

## <a name="to-set-up-the-incoming-documents-feature"></a><a name="to-set-up-the-incoming-documents-feature"></a>To set up the Incoming Documents feature

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Incoming Document Setup**, and then choose the related link.
2. Fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

As part of the setup, you must decide if you want to require approval of incoming documents. To require approval, you must [set up approvers and approval workflows](#to-set-up-approvers-of-incoming-document-records). If your organisation doesn't intend to require approval, you can skip the next section.

Finally, if you use an OCR service to convert PDF or image files representing incoming documents, [you must it set up](#to-set-up-an-ocr-service). Otherwise, you can also skip that section.

## <a name="to-set-up-approvers-of-incoming-document-records"></a><a name="to-set-up-approvers-of-incoming-document-records"></a>To set up approvers of incoming document records

If you don't want users to create invoices or general journal lines from incoming document records unless the documents are first approved, set up an approval process for the incoming documents. Approvers of incoming documents must be set up as approval workflow users.

Before you can create workflows that involve approval steps, you must set up the workflow users who are involved in approval processes. On the **Approval User Setup** page, you also set amount limits for specific types of requests and define substitute approvers to whom approval requests are delegated when the original approver is absent. For more information, see [Set Up Approval Users](across-how-to-set-up-approval-users.md).

## <a name="to-set-up-an-ocr-service"></a><a name="to-set-up-an-ocr-service"></a>To set up an OCR service

To turn PDF and image files into electronic documents that you can convert to invoices, credit memos, or journal lines, set up the OCR feature. Alternatively, you can create entries manually to represent the external documents.

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **OCR Service Setup**, and then choose the related link.
2. Fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

> [!NOTE]  
> You login data is automatically encrypted.

For more information, see [Use OCR to Turn PDF and Image Files into Electronic Documents](across-how-use-ocr-pdf-images-files.md).  

## <a name="see-related-microsoft-training"></a><a name="see-related-microsoft-training"></a>See related [Microsoft training](/training/modules/incoming-documents-dynamics-365-business-central/)

## <a name="see-also"></a><a name="see-also"></a>See also

[Incoming Documents](across-income-documents.md)  
[Purchasing](purchasing-manage-purchasing.md)  
[Work with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]
