---
title: Use OCR to Turn PDF into E-Invoices| Microsoft Docs
description: Describes how you can use an OCR service to convert incoming PDF or image files to electronic documents in Financials.
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: electronic document, e-invoice, incoming document, OCR, ecommerce, document exchange, import invoice
ms.date: 06/02/2017
ms.author: sgroespe
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: 020aeed82d6147641936dee2d7b860791c76d2ee
ms.contentlocale: en-nz
ms.lasthandoff: 07/07/2017


---
# <a name="how-to-use-ocr-to-turn-pdf-and-image-files-into-electronic-documents"></a>How to: Use OCR to Turn PDF and Image Files into Electronic Documents
From PDF or image files that you receive from your trading partners, you can have an external OCR service (Optical Character Recognition) generate electronic documents that can be converted to document records in [!INCLUDE[d365fin](includes/d365fin_md.md)]. For example, when you receive an invoice in PDF format from your vendor, you can send it to the OCR service from the **Incoming Documents** window. This is described in the first procedure.

As an alternative to sending the file from the **Incoming Documents** window, you can send the file to the OCR service by email. Then, when you receive the electronic document back, a related incoming document record is created automatically. This is described in the second procedure.

After some seconds, you receive the file back from the OCR service as an electronic invoice that can be converted to a purchase invoice for the vendor. This is described in the third procedure.

Because OCR is based on optical recognition, it is likely that the OCR service will interpret characters in your PDF or image files wrongly when it first processes a certain vendor’s documents, for example. It may not interpret the company logo as the vendor’s name or it may misinterpret the total amount on a receipt because of its layout. To avoid these errors going forward, you can correct the errors in a separate version of the **Incoming Document** window. Then you send the corrections back to the OCR service to train it to interpret the specific characters correctly next time it processes a PDF or image document for the same vendor. For more information, see the "To train the OCR service to avoid errors" section.

The traffic of files to and from the OCR service is processed by a dedicated job queue entry, which are created automatically when you enable the related service connection. For more information, see [How to: Set Up Incoming Documents](across-how-setup-income-documents.md).

## <a name="to-send-a-pdf-or-image-file-to-the-ocr-service-from-the-incoming-documents-window"></a>To send a PDF or image file to the OCR service from the **Incoming Documents** window
1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Incoming Documents**, and then choose the related link.
2. Create a new incoming document record and attach the file. For more information, see [How to: Create Incoming Document Records](across-how-create-income-document-records.md).  
3. In the **Incoming Documents** window, select one or more lines, and then choose the **Send to Job Queue** action.

    The value in the **OCR Status** field changes to **Ready**. The attached PDF or image file is sent to the OCR service by the job queue according to the schedule, provided that no errors exist.
4. Alternatively, in the **Incoming Documents** window, select one or more lines, and then choose the **Send to OCR Service** action.

The value in the **OCR Status** field changes to **Sent**, provided that no errors exist.

## <a name="to-send-a-pdf-or-image-file-to-the-ocr-service-by-email"></a>To send a PDF or image file to the OCR service by email
From your email application, you can send an email to the OCR service provider with the PDF or image file attached. For information about the email address to send to, see the OCR service provider’s web site.

Because no incoming document record exists for the file, a new record will be created automatically in the **Incoming Documents** window when you receive the resulting electronic document from the OCR service. For more information, see [How to: Create Incoming Document Records](across-how-create-income-document-records.md).

> [!NOTE]  
>   If you work on a tablet or phone, you can send the file to the OCR service as soon as you have taken a photo of the document, or you can create an incoming document directly. For more information, see the "To create incoming document records by taking a photo" section in [How to: Create Incoming Document Records](across-how-create-income-document-records.md).

## <a name="to-receive-the-resulting-electronic-document-from-the-ocr-service"></a>To receive the resulting electronic document from the OCR service.
The electronic document that is created by the OCR service from the PDF or image file is automatically received into the **Incoming Documents** window by the job queue entry that is set up when you enable the OCR service.

If you are not using a job queue, or you want to receive a finished OCR document sooner than per the job queue schedule, you can choose the **Receive from OCR Service** button. This will get any documents that are completed by the OCR service.

> [!NOTE]  
>   If the OCR service is set up to require manual verification of processed documents, then the **OCR Status** field will contain **Awaiting Verification**. In that case, perform the following steps to log in to the OCR service website to manually verify an OCR document.

1. In the **OCR Status** field, choose the **Awaiting Verification** hyperlink. Alternatively, choose the **Awaiting Verification** tile on the Home page.
2. On the OCR service website, log in using the credentials of your OCR service account. These are the credentials you also used when setting up the service. For more information, see the "To set up an OCR service" section in [How to: Set Up Incoming Documents](across-how-setup-income-documents.md).

    If you access the website from the **OCR Status** field, the document in question is displayed immediately after your sign in. If you access the website by choosing the tile on the Home page, on the first OCR service page that opens, you must choose the **Start** button on the **Verify** tab or double-click the document that you want to verify.

    Information for the OCR document is displayed, showing both the source content of the PDF or image file and the resulting OCR field values.
3. Review the various field values and manually edit or enter values in fields that the OCR service has tagged as uncertain.
4. Choose the **OK** button. The OCR process is completed and the resulting electronic document is sent to the **Incoming Documents** window in [!INCLUDE[d365fin](includes/d365fin_md.md)],  according to the job queue schedule.

    If you access the website by choosing the tile on the Home page, then any other OCR document to be verified is automatically displayed on the website.
5. Repeat step 4 for any other OCR document to be verified.

Now you can proceed to create document records for the received electronic documents in [!INCLUDE[d365fin](includes/d365fin_md.md)], manually or automatically. For more information, see the next procedure. You can also connect the new incoming document record to existing posted or non-posted document so that the source file is easy to access from [!INCLUDE[d365fin](includes/d365fin_md.md)]. For more information, see [Process Incoming Documents](across-process-income-documents.md).

## <a name="to-create-a-purchase-invoice-from-an-electronic-document-received-from-the-ocr-service"></a>To create a purchase invoice from an electronic document received from the OCR service
The following procedure describes how to create a purchase invoice record from a vendor invoice received as an electronic document from the OCR service. The procedure is the same when you create, for example, a general journal line from an expense receipt.

> [!NOTE]  
>   The **Description** and **No.** fields on the created document lines will only be filled if you have first mapped text found on the OCR document to the two fields in [!INCLUDE[d365fin](includes/d365fin_md.md)]. You can do this either as item cross-references, for document lines of type Item, or as text-to-account mappings, for document or journal lines of type G/L Account. For more information, see the tooltip for the **Cross References** action on item cards and the related procedure, [How to: Map Text on Recurring Payments to Accounts for Automatic Reconciliation](receivables-how-map-text-recurring-payments-accounts-auto-reconcilliation.md).

For incoming documents, you typically use the **Map Text to Account** action to define that a certain text on a vendor invoice received from the OCR service is mapped to a certain vendor account. Going forward, any part of the incoming document description that exists as a mapping text means that the **No.** field on resulting document or journal lines of type G/L Account are filled with the vendor in question.

In addition to mapping to a vendor account or G/L accounts, you can also map to a bank account. This is practical, for example, for electronic documents for expenses that are already paid where you want to create a general journal line that is ready to post to a bank account.

1. Select the incoming document line for the electronic vendor document received from the OCR service.
2. To map text on the document to the vendor's account, a debit account, choose the **Map Text to Account** action, and then fill in the **Text-to-Account Mapping** window with information that will apply to the vendor going forward. For more information, see [How to: Map Text on Recurring Payments to Accounts for Automatic Reconciliation](receivables-how-map-text-recurring-payments-accounts-auto-reconcilliation.md).
3. To map the item numbers on the document to your descriptions of the vendor's items, open the card of each item, and then choose the **Cross References** action to set up cross-references between your item descriptions and those of the vendor.
4. In the **Incoming Documents** window, choose the **Create Document** action.

A purchase invoice will be created in [!INCLUDE[d365fin](includes/d365fin_md.md)] based on the information in the electronic vendor document that you received from the OCR service.

Any validation errors, typically related to wrong or missing master data in [!INCLUDE[d365fin](includes/d365fin_md.md)], will be shown on the **Errors and Warnings** FastTab. For more information, see the "To handle errors when receiving electronic documents" section.

## <a name="to-handle-errors-when-receiving-electronic-documents"></a>To handle errors when receiving electronic documents
1. In the **Incoming Documents** window, select the line for an electronic document received from the OCR service with errors. This is indicated by the Error value in the **OCR Status** field.
2. Choose the **Edit** action to open the **Incoming Document** window.
3. On the **Errors and Warnings** FastTab, select the message, and then choose the **Open Related Record** action.
4. The window that contains the wrong or missing data, such as a vendor card with a missing field value, opens.
5. Correct the error or errors as described in each error message.
6. Proceed to process the incoming electronic document by choosing the **Create Manually** action again.
7. Repeat steps 5 and 6 for any remaining errors until the electronic document can be received successfully.

## <a name="to-train-the-ocr-service-to-avoid-errors"></a>To train the OCR service to avoid errors
Because OCR is based on optical recognition, it is likely that the OCR service will interpret characters in your PDF or image files wrongly when it first processes documents from a certain vendor, for example. It may not interpret the company logo as the vendor’s name or it may misinterpret the total amount on an expense receipt because of its layout. To avoid such errors going forward, you can correct data received by the OCR service and then send the feedback to the service.

The **OCR Data Correction** window, which you open from the **Incoming Document** window, shows the fields from the **Financial Information** FastTab in two columns, one with the OCR data editable and one with the OCR data read-only. When you choose the **Send OCR Feedback** button, the content of the **OCR Data Correction** window is sent to the OCR service. Next time the service processes PDF or image files that contain the data in question, your corrections will be incorporated to avoid the same errors.

1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Incoming Documents**, and then choose the related link.
2. Open an incoming document record that contains data received from OCR service, which you want to correct.
3. In the **Incoming Document** window, choose the **Correct OCR Data** action.
4. In the **OCR Data Correction** window, overwrite the data in the editable column for each field that has an incorrect value.
5. To undo corrections that you have made since you opened the **OCR Data Correction** window, choose the **Reset OCR Data** action.
6. To send the corrections to the OCR service, choose the **Send OCR Feedback** action.
7. To save the corrections, close the **OCR Data Correction** window.

The fields on the **Financial Information** FastTab in the **Incoming Document** window are updated with any new values that you entered in step 4.

## <a name="see-also"></a>See Also
[Process Incoming Documents](across-process-income-documents.md)  
[Incoming Documents](across-income-documents.md)  
[Purchasing](purchasing-manage-purchasing.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

