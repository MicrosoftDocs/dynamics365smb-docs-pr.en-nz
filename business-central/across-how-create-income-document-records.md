---
title: Create Records of Incoming Documents| Microsoft Docs
description: You can create records of incoming documents, such as e-invoices, and manage OCR tasks, eCommerce, and document exchange.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: electronic document, e-invoice, incoming document, OCR, ecommerce, document exchange, import invoice
ms.date: 06/02/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: f80438923773822eba0abc7dfa7dae45b0e87637
ms.contentlocale: en-nz
ms.lasthandoff: 03/22/2018

---
# <a name="create-incoming-document-records"></a>Create Incoming Document Records
In the **Incoming Documents** window, you can use different functions to review expense receipts, manage OCR tasks, and convert incoming document files, manually or automatically, to the relevant documents or journal lines. The external files can be attached at any process stage, including to posted documents and to the resulting vendor, customer, and general ledger entries.

To record an external document in [!INCLUDE[d365fin](includes/d365fin_md.md)], you must first create or complete an incoming document record. You can do this manually, or you can take a photo of the external document and then create the incoming document record with the image file attached.

Before you can use the Incoming Documents feature, you must perform the required setup. For more information, see [Set Up Incoming Documents](across-how-setup-income-documents.md).

## <a name="to-approve-or-reject-an-incoming-document"></a>To approve or reject an incoming document
If you do want to allow users to create invoices or general journal lines from incoming document records unless they are approved, you can set up approvers who must approve the records before they can be processed.

1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Incoming Documents**, and then choose the related link.
2. Select the line with the document that you want to approve or reject, and then choose the **Approve** or **Reject** actions.

If you approve the incoming document record, the **Released** check box on the incoming document line is selected. The user in charge of creating, for example, purchase invoices can proceed to process the record.

## <a name="to-create-an-incoming-document-record-by-taking-a-photo"></a>To create an incoming document record by taking a photo
> [!NOTE]  
>   The following procedure only applies to the [!INCLUDE[d365fin](includes/d365fin_md.md)] Tablet and Phone clients.

1. On the app bar, choose the **Create Incoming Document from Camera** tile, and then go to step 4.
2. Alternatively, on the app bar, choose the options button, choose **Incoming Documents**, and then choose **All**.
3. In the **Incoming Documents** window, choose the ellipsis button, and then choose **Create from Camera**. The camera on the tablet or phone is activated.
4. Take a photo of a document, such as a purchase receipt, that you want to process as an incoming document, and then choose the **OK** button.

    A new incoming document record is created, with the image attached.

## <a name="to-attach-an-image-to-an-incoming-document-record-by-taking-a-photo"></a>To attach an image to an incoming document record by taking a photo
> [!NOTE]  
>   The following procedure only applies to the [!INCLUDE[d365fin](includes/d365fin_md.md)] Tablet and Phone clients.

1. On the app bar, choose the options button, choose **Incoming Documents**, and then choose **All**.
2. Open the card for an existing incoming document record.
3. In the **Incoming Document** window, choose the ellipsis button, and then choose **Attach Image from Camera**. The camera on the tablet or phone is activated.
4. Take a photo of a document, such as a purchase receipt, that you want to process as an incoming document, and then choose the **OK** button.

    The image is attached to the incoming document record.

## <a name="to-create-an-incoming-document-record-manually"></a>To create an incoming document record manually
1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Incoming Documents**, and then choose the related link.
2. Choose the **Create from File** action.  
3. In the **Insert File** window, select a file, and then choose **Open**. The file is automatically attached.
4. Alternatively, choose the **New** action.
5. To attach a file, choose the **Attach File** action.
6. In the **Insert File** window, select the file that represents the incoming document in question, and then choose the **Open** button.
7. In the **Incoming Document** window, fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="see-also"></a>See Also
[Process Incoming Documents](across-process-income-documents.md)  
[Incoming Documents](across-income-documents.md)  
[Purchasing](purchasing-manage-purchasing.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

