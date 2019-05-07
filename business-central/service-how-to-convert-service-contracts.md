---
title: How to Convert Service Contracts | Microsoft Docs
description: Because the GST rate change tool cannot convert service contracts, these contracts must be converted manually. This topic describes several alternative methods that you can use for service contract conversion.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2019
ms.author: sgroespe
ms.openlocfilehash: 82c7e19c2c493df77094bd3b6e4d2e5835a278bb
ms.sourcegitcommit: bd78a5d990c9e83174da1409076c22df8b35eafd
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 03/31/2019
ms.locfileid: "913982"
---
# <a name="convert-service-contracts-that-include-vat-amounts"></a>Convert Service Contracts that Include GST Amounts
Because the GST rate change tool cannot convert service contracts, these contracts must be converted manually. This topic describes several alternative methods that you can use for service contract conversion.  

> [!NOTE]  
>  This topic provides a high-level workflow.  

 The following procedure describes how to correct an invoice for a prepaid service contract that has been created a year in advance.  

> [!NOTE]  
>  For this example, you must change your work date to 01.01.2017.  

### <a name="to-correct-an-invoice-for-a-prepaid-service-contract"></a>To correct an invoice for a prepaid service contract  
1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Contract Management**, and then choose the related link.  
2. Under **Lists**, choose **Service Contracts**.  
3. Create a new prepaid service contract. Enter a start date of **01.01.2017** and an invoice period year for customer **20000**.  
4. This contract must be signed. On the **Home** tab, in the **Process** group, choose **Sign Contract**.  
5. Create a service invoice.
6. The invoice is listed as an unposted service invoice. To view the service invoice, choose **Service**, choose **Contract Management**, and then choose **Service Invoices**.  
7. Post the service invoice.  

> [!NOTE]  
>  Do not change the unposted service invoice. Since the service ledger entries are created when the invoice is created, a change in the unposted invoice will not change the already created service ledger entries. However, the GST entries are created when the invoice is posted. This lets you change the general product posting group and the GSP product posting group on the unposted service invoice.  

### <a name="to-create-a-credit-memo-for-vat-difference"></a>To create a credit memo for GST difference  
The following procedure describes how to create a credit memo that only includes the GST difference for the already invoiced period starting on **01.07.2017**. In this example, the GST amount is only posted to the Financial Management module, not to the Service Management module. The GST entries that are linked to the service ledger entry will not be corrected.  

1. Create a new general ledger account for the GST difference. This account will be used for direct posting of the GST correction.  
2. Add a new line to the GST posting setup.  

### <a name="to-create-contract-expiration-dates-in-contract-lines"></a>To create contract expiration dates in contract lines  
The following procedure describes how to create new contracts by working with contract expiration dates in service contract lines.  

1. On the **Service Contract** page, set the contract expiration date to **30.06.2017**.  
2. Choose the **Create Credit Memo** action to automatically create a credit memo for July 2017 to December 2017.  
3. Because the contract has expired, you need to create a new contract for the period with the new GST rate for July 1, 2017 to December 31, 2017.  

### <a name="to-create-a-new-credit-memo"></a>To create a new credit memo  
The following procedure describes how to create a new credit memo using the **Get Prepaid Contract Entries** batch job. Entries that you do not want to correct from January 2017 to June 2017 will be deleted.  

1. Run the GST rate change tool on July 1, 2017. The general product posting group or the GST product posting group is changed. For more information, see [Work with GST on Sales and Purchases](finance-work-with-vat.md).  
2. After running the GST rate change tool, enter a contract expiration date for the service contract. You can now delete the service contract line and create a new line that is identical to the old one.  
3. Create a new invoice for the period of January 2017 to December 2012 using the new GST rate.  
4. To create another credit memo, on the **Service Credit Memos** page, choose **New** to create a new service credit memo.  
5. Choose the **Get Prepaid Contract Entries** action.  
6. After the conversion is complete, GST and service ledger entries will be correct.  

## <a name="see-also"></a>See Also  
[Work with Service Contracts and Service Contract Quotes](service-how-to-create-service-contracts-and-service-contract-quotes.md)  
[Finance](finance.md)  
[Report GST to Tax Authorities](finance-how-report-vat.md)  
[Work with GST on Sales and Purchases](finance-work-with-vat.md)  
