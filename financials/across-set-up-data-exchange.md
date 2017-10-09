---
title: Set up data exchange | Microsoft Docs
description: Set up the data exchange framework in Dynamics 365 for Financials.
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/21/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 5c0fcfd6ef178c5917a4a07ba81a9bef9b4522aa
ms.contentlocale: en-nz
ms.lasthandoff: 09/22/2017

---
# <a name="setting-up-data-exchange"></a>Setting Up Data Exchange
Before you can send and receive electronic documents or import and export bank files, you must set up the data exchange framework to process the involved files. In addition, you must set up related areas, such as master data for customers that you send electronic invoices to or the bank data conversion service in case you use the external service provider to convert your bank files. For more information, see [Exchanging Data as Electronic Documents](across-data-exchange.md).  

 When [!INCLUDE[d365fin](includes/d365fin_md.md)] is set up to exchange data with external files, users can use the setup in common business tasks, such as sending and receiving electronic documents and importing and exporting bank files.  

 The following table describes a sequence of tasks, with links to the topics that describe them.  

|**To**|**See**|  
|------------|-------------|  
|Set up the preconfigured document exchange service to enable sending and receiving electronic documents from and to [!INCLUDE[d365fin](includes/d365fin_md.md)].|[How to: Set Up a Document Exchange Service](across-how-to-set-up-a-document-exchange-service.md)|  
|Set up the preconfigured OCR service to turn PDF or image files into electronic documents that can be converted to document records in [!INCLUDE[d365fin](includes/d365fin_md.md)]|[How to: Set Up Incoming Documents](across-how-setup-income-documents.md)|  
|Set up one of two preconfigured services for updated exchange rates to get the latest currency exchange rates into the **Currencies** window.|[How to: Update Currency Exchange Rates](finance-how-update-currencies.md)|  
|Set up various master data, such as company information, customers, vendors, items, and units of measure, related to mapping data in [!INCLUDE[d365fin](includes/d365fin_md.md)]|[How to: Set Up Electronic Document Sending and Receiving](across-how-to-set-up-electronic-document-sending-and-receiving.md)|  
|Set up a bank account, a vendor, and a payment journal for SEPA credit transfer.|[How to: Set Up SEPA Credit Transfer](finance-how-to-set-up-sepa-credit-transfer.md)|  
|Prepare bank account formats, payment methods, and customer agreements for SEPA direct debit.|[How to: Set Up SEPA Direct Debit](finance-how-to-set-up-sepa-direct-debit.md)|  
|Set up user authentication and the URL of the bank data conversion service provider that is required to have bank files converted to your bank’s format.|[How to: Set Up the Bank Data Conversion Service](bank-how-setup-bank-data-conversion-service.md)|  
|Set up and enable an external service that enables you to import bank statements directly as bank feeds.|[How to: Set Up the Bank Statement Service](bank-how-setup-bank-statement-service.md)|  
|After the Bank Statement service is enabled, link bank accounts in [!INCLUDE[d365fin](includes/d365fin_md.md)]|[How to: Set Up Bank Accounts](bank-how-setup-bank-accounts.md)|  
|Prepare to set up a new data exchange definition for a data file or stream by using the file’s XML schema to prefill the **Column Definitions** FastTab in the **Posting Exchange Definition** window.|[How to: Use XML Schemas to Prepare Data Exchange Definitions](across-how-to-use-xml-schemas-to-prepare-data-exchange-definitions.md)|  
|Set up the Data Exchange Framework to enable users to receive a new purchase document format, send a new sales document format, import a new bank file, or other data exchange.|[How to: Set Up Data Exchange Definitions](across-how-to-set-up-data-exchange-definitions.md)|  

## <a name="see-also"></a>See Also  
[Exchanging Data as Electronic Documents](across-data-exchange.md)  
[Exchange Data](across-exchange-data.md)   
[Incoming Documents](across-income-documents.md)  
[General Business Functionality](ui-across-business-areas.md)  

