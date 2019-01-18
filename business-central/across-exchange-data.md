---
title: Exchange Data | Microsoft Docs
description: You can exchange data between Business Central and external files or streams in connection with common business tasks, such as sending and receiving electronic documents and importing and exporting bank files.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: caf7cf5afe370af0c4294c794c0ff9bc8ff4c31c
ms.openlocfilehash: 678b15b8d15dba477ac09c2651964525f4afe26a
ms.contentlocale: en-nz
ms.lasthandoff: 11/22/2018

---
# <a name="exchanging-data"></a>Exchanging Data
You can exchange data between [!INCLUDE[d365fin](includes/d365fin_md.md)] and external files or streams in connection with common business tasks, such as sending and receiving electronic documents and importing and exporting bank files.  

Before you can send and receive electronic documents or import and export bank files, you must set up the data exchange framework to process the involved data files or streams. In addition, you must set up related areas. These include master data for customers that you send electronic invoices to and the bank data conversion service in case you distribute bank file conversions to an external service provider. For more information, see [Setting Up Data Exchange](across-set-up-data-exchange.md).  

 The following table describes a sequence of tasks, with links to the topics that describe them.  

|**To**|**See**|  
|------------|-------------|  
|Convert sales document records in [!INCLUDE[d365fin](includes/d365fin_md.md)] to a standardised format and send them as electronic documents that your customers can receive into their system.|[Send Electronic Documents](sales-how-to-send-electronic-documents.md)|  
|Send PDF or image files to a provider of OCR services, and receive them back as electronic documents that can be converted to document records in [!INCLUDE[d365fin](includes/d365fin_md.md)].|[Use OCR to Turn PDF and Image Files into Electronic Documents](across-how-use-ocr-pdf-images-files.md)|  
|Receive electronic documents, either from the OCR service or the document exchange service, in a standardised format that you convert to the relevant document records in [!INCLUDE[d365fin](includes/d365fin_md.md)].|[Receive and Convert Electronic Documents](purchasing-how-to-receive-and-convert-electronic-documents.md)|  
|Prepare to import a bank statement file into the **Payment Reconciliation Journal** page as the first step in reconciling payments or into the **Bank Acc. Reconciliation** page as the first step in reconciling bank accounts.|[Set Up the Envestnet Yodlee Bank Feeds Service](bank-how-setup-bank-statement-service.md)|  
|Export payments from the **Payment Journal** page to a bank file that you upload to your electronic bank account for processing.|[Export Payments to a Bank File](payables-how-export-payments-bank-file.md)|
|Make electronic payments according to the EU SEPA Credit Transfer standard.|[Making Payments with Bank Data Conversion Service or SEPA Credit Transfer](finance-make-payments-with-bank-data-conversion-service-or-sepa-credit-transfer.md)|  
|Instruct your bank to transfer payment amounts from your customers’ bank accounts to your company’s account according to your setup of SEPA direct debit.|[Create SEPA Direct Debit Collection Entries and Export to a Bank File](finance-how-create-sepa-direct-debit-collection-entries-export-bank-file.md)|  
|Use a service provider of currency exchange rates to update the **Currencies** page.|[Update Currency Exchange Rates](finance-how-update-currencies.md)|  
|View which file elements are mapped to fields in [!INCLUDE[d365fin](includes/d365fin_md.md)] when importing SEPA CAMT statement files.|[Field Mapping When Importing SEPA CAMT Files](across-field-mapping-when-importing-sepa-camt-files.md)|  
|View which fields in [!INCLUDE[d365fin](includes/d365fin_md.md)] are mapped to file elements when exporting payment files by using the Bank Date Conversion Service feature.|[Field Mapping When Exporting Payment Files Using Bank Data Conversion Service](across-field-mapping-when-exporting-payment-files-using-bank-data-conversion-service.md)|  

## <a name="see-also"></a>See Also  
[Setting Up Data Exchange](across-set-up-data-exchange.md)  
[Exchanging Data Electronically](across-data-exchange.md)  
[Invoice Sales](sales-how-invoice-sales.md)   
[Record Purchases](purchasing-how-record-purchases.md)  
[Incoming Documents](across-income-documents.md)  
[General Business Functionality](ui-across-business-areas.md)  

