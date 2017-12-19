---
title: Make Payments with Bank Data Conversion Service or SEPA Credit Transfer | Microsoft Docs
description: Process payments to your vendors by exporting a file together with the payment information from the journal lines.
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 11/17/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: aa56764b5f3210229ad21eae6891fb201462209c
ms.openlocfilehash: 0760b5480b3c2de9bc370526bd87da2c9a492d92
ms.contentlocale: en-nz
ms.lasthandoff: 12/14/2017

---
# <a name="making-payments-with-bank-data-conversion-service-or-sepa-credit-transfer"></a>Making Payments with Bank Data Conversion Service or SEPA Credit Transfer
In the **Payment Journal** window, you can process payments to your vendors by exporting a file together with the payment information from the journal lines. You can then upload the file to your electronic bank where the related money transfers are processed. [!INCLUDE[d365fin](includes/d365fin_md.md)] supports the SEPA Credit Transfer format, but in your country/region, other formats for electronic payments may be available.   

 To enable SEPA credit transfers, you must first set up a bank account, a vendor, and the general journal batch that the payment journal is based on. You then prepare payments to vendors by automatically filling the **Payment Journal** window with due payments with specified posting dates.  

> [!NOTE]  
>  When you have verified that the payments are successfully processed by the bank, you can proceed to post the payment journal lines.  

 The following table describes a sequence of tasks, with links to the topics that describe them.   

|**To**|**See**|  
|------------|-------------|  
|Activate the Bank Data Conversion Service feature to have any bank statement file converted to a format that you can import or to have your exported payment files converted to the format that your bank requires.|[How to: Set Up the Bank Data Conversion Service](bank-how-setup-bank-statement-service.md)|  
|Set up a bank account, a vendor, and a payment journal for SEPA credit transfer.|[How to: Set Up SEPA Credit Transfer](finance-how-to-set-up-sepa-credit-transfer.md)|  
|Fill the payment journal with lines for due payments to vendors, with the option to insert posting dates based on the due date of the related purchase documents.|[Managing Payables](payables-manage-payables.md)|  
|Export payment journal lines to a file in the SEPA Credit Transfer format.|[How to: Export Payments to a Bank File](payables-how-export-payments-bank-file.md)|  
|When the electronic payment is successfully processed by the bank, post the payments.|[Working with General Journals](ui-work-general-journals.md)|  

## <a name="see-also"></a>See Also  
[How to: Set Up the Bank Data Conversion Service](bank-how-setup-bank-statement-service.md)  
[How to: Set Up SEPA Credit Transfer](finance-how-to-set-up-sepa-credit-transfer.md)  
[Managing Payables](payables-manage-payables.md)   
[Working with General Journals](ui-work-general-journals.md)  
[Collecting Payments with SEPA Direct Debit](finance-collect-payments-with-sepa-direct-debit.md)   

