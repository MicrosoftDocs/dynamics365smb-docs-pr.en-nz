---
title: Field Mapping When Importing SEPA CAMT Files | Microsoft Docs
description: In European markets, you can import bank statement files in the regional SEPA standards (Single Euro Payments Area).
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
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: abda752ed574245c6d38adb6ee1441bb2b2c80fc
ms.contentlocale: en-nz
ms.lasthandoff: 03/22/2018

---
# <a name="field-mapping-when-importing-sepa-camt-files"></a>Field Mapping When Importing SEPA CAMT Files
[!INCLUDE[d365fin](includes/d365fin_md.md)] supports the regional SEPA standards (Single Euro Payments Area) for importing SEPA bank statements (CAMT format). For more information, see [Set Up the Bank Data Conversion Service](bank-how-setup-bank-data-conversion-service.md).  

 The SEPA CAMT standard itself has local variations. Therefore, you may have to modify the generic data exchange definition (represented by the **SEPA CAMT** code in the **Posting Exchange Definitions** window) to adapt it to a local variation of the standard. The following tables show the element-to-field mapping for tables 81, 273, and 274 in the SEPA CAMT implementation in [!INCLUDE[d365fin](includes/d365fin_md.md)].  

 For information about creating or adjusting a data exchange definition, see [Set Up Data Exchange Definitions](across-how-to-set-up-data-exchange-definitions.md).  

## <a name="camt-data-mapping-to-fields-in-the-general-journal-table-81"></a>CAMT data mapping to fields in the General Journal table (81)  

|Element Path|Message Element|Data Type|Description|Negative-Sign Identifier|Field No.|Field Name|  
|------------------|---------------------|---------------|-----------------|-------------------------------|---------------|----------------|  
|Stmt/Ntry/Amt|Amount|Decimal|The amount of money in the cash entry||13|Amount|  
|Stmt/Ntry/CdtDbtInd|CreditDebitIndicator|Text|Indicates whether the entry is a credit or a debit entry|DBIT|13|Amount|  
|Stmt/Ntry/BookgDt/Dt|Date|Date|The date when an entry is posted to an account on the account servicer's books||5|Posting Date|  
|Stmt/Ntry/BookgDt/DtTm|DateTime|DateTime|The date and time when an entry is posted to an account on the account servicer's books||5|Posting Date|  
|Stmt/Ntry/NtryDtls/TxDtls/RltdPties/Dbtr/Nm|Name|Text|The name of the party that owes an amount of money to the (ultimate) creditor||1221|Payer Information|  
|Stmt/Ntry/NtryDtls/TxDtls/RmtInf/Ustrd|Unstructured|Text|Information supplied to enable the matching/reconciliation of an entry with the items that the payment is intended to settle, such as commercial invoices in an accounts-receivable system, in an unstructured form||8|Description|  
|Stmt/Ntry/AddtlNtryInf|AdditionalEntryInformation|Text|Additional information about the entry||1222|Transaction Information|  

## <a name="camt-data-mapping-to-fields-in-the-bank-acc-reconciliation-table-273"></a>CAMT data mapping to fields in the Bank Acc. Reconciliation table (273)  

|Element Path|Message Element|Data Type|Description|Negative-Sign Identifier|Field No.|Field Name|  
|------------------|---------------------|---------------|-----------------|-------------------------------|---------------|----------------|  
|Stmt/CreDtTm|CreationDateTime|Date|The date and time when the message was created||3|Statement Date|  
|Stmt/Bal/Amt|Amount|Decimal|The amount resulting from the netted amounts for all debit and credit entries||4|Statement Ending Balance|  

## <a name="camt-data-mapping-to-fields-in-the-bank-acc-reconciliation-line-table-274"></a>CAMT data mapping to fields in the Bank Acc. Reconciliation Line table (274)  

|Element Path|Message Element|Data Type|Description|Negative-Sign Identifier|Field No.|Field Name|  
|------------------|---------------------|---------------|-----------------|-------------------------------|---------------|----------------|  
|Stmt/Ntry/Amt|Amount|Decimal|The amount of money in the cash entry||7|Statement Amount|  
|Stmt/Ntry/CdtDbtInd|CreditDebitIndicator|Text|Indicates whether the entry is a credit or a debit entry|DBIT|7|Statement Amount|  
|Stmt/Ntry/BookgDt/Dt|Date|Date|The date when an entry is posted to an account on the account servicer's books||5|Transaction Date|  
|Stmt/Ntry/BookgDt/DtTm|DateTime|DateTime|The date and time when an entry is posted to an account on the account servicer's books||5|Transaction Date|  
|Stmt/Ntry/ValDt/Dt|Date|Date|The date when assets become available to the account owner in case of a credit entry, or cease to be available to the account owner in case of a debit entry||12|Value Date|  
|Stmt/Ntry/ValDt/DtTm|DateTime|DateTime|The date and time when assets become available to the account owner in case of a credit entry, or cease to be available to the account owner in case of a debit entry||12|Value Date|  
|Stmt/Ntry/NtryDtls/TxDtls/RltdPties/Dbtr/Nm|Name|Text|The name of the party that owes an amount of money to the (ultimate) creditor||15|Payer Information|  
|Stmt/Ntry/NtryDtls/TxDtls/RmtInf/Ustrd|Unstructured|Text|Information supplied to enable the matching/reconciliation of an entry with the items that the payment is intended to settle, such as commercial invoices in an accounts-receivable system, in an unstructured form||6|Description|  
|Stmt/Ntry/AddtlNtryInf|AdditionalEntryInformation|Text|Additional information about the entry||16|Transaction Information|  

 Elements in the **Ntry** node that are imported into [!INCLUDE[d365fin](includes/d365fin_md.md)] but not mapped to any fields are stored in the **Posting Exch. Column Def** table. Users can view these elements from the **Payment Reconciliation Journal**, **Payment Application**, and **Bank Acc. Reconciliation** windows by choosing the **Bank Statement Line Details** action. For more information, see [Reconcile Payments Using Automatic Application](receivables-how-reconcile-payments-auto-application.md).  
## <a name="see-also"></a>See Also  
[Setting Up Data Exchange](across-set-up-data-exchange.md)  
[Exchanging Data Electronically](across-data-exchange.md)  
[Set Up the Bank Data Conversion Service](bank-how-setup-bank-data-conversion-service.md)   
[Use XML Schemas to Prepare Data Exchange Definitions](across-how-to-use-xml-schemas-to-prepare-data-exchange-definitions.md)  
[Reconcile Payments Using Automatic Application](receivables-how-reconcile-payments-auto-application.md)  

