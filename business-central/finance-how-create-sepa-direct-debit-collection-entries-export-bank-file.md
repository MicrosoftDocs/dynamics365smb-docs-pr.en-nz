---
title: Export SEPA Direct Debit Collection Entries| Microsoft Docs
description: "Create a direct-debit collection, which holds information about the customer’s bank account, the affected sales invoices, and the direct-debit mandate."
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 10/01/2018
ms.author: sgroespe
redirect_url: finance-collect-payments-with-sepa-direct-debit
ms.translationtype: HT
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: d05a12251046b0c911387cda1d5a7a7c9a026d6b
ms.contentlocale: en-nz
ms.lasthandoff: 09/28/2018

---
# <a name="create-sepa-direct-debit-collection-entries-and-export-to-a-bank-file"></a>Create SEPA Direct Debit Collection Entries and Export to a Bank File
To instruct the bank to transfer the payment amount from the customer’s bank account to your company’s account, you create a direct-debit collection, which holds information about the customer’s bank account, the affected sales invoices, and the direct-debit mandate. From the resulting direct-debit collection entry, you then export an XML file that you send or upload to your electronic bank for processing. Any payments that could not be processed by the bank will be communicated to you by your bank, and you must then manually reject the direct debit-collection entries in question.  

> [!NOTE]  
>  To collect payments using SEPA Direct Debit, the currency on the sales invoice must be EURO.  

### <a name="to-create-a-direct-debit-collection"></a>To create a direct-debit collection  

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Direct Debit Collections**, and then choose the related link.  
2. In the **Direct Debit Collections** window, on the **Home** tab, in the **New** group, choose **Create Direct Debit Collection**.  
3. In the **Create Direct Debit Collection** window, fill in the fields as described in the following table.  

    |Field|Description|  
    |---------------------------------|---------------------------------------|  
    |**From Due Date**|Specify the earliest payment due date on sales invoices that you want to create a direct-debit collection for.|  
    |**To Due Date**|Specify the latest payment due date on sales invoices that you want to create a direct-debit collection for.|  
    |**Partner Type**|Specify if the direct-debit collection is made for customers of type **Company** or **Person**.|  
    |**Only Customers With Valid Mandate**|Specify if a direct-debit collection is created for customers who have a valid direct-debit mandate. **Note:**  A direct-debit collection is created even if the **Direct Debit Mandate ID** field is not filled on the sales invoice.|  
    |**Only Invoices With Valid Mandate**|Specify if a direct-debit collection is only created for sales invoices if a valid direct-debit mandate is selected in the **Direct Debit Mandate ID** field on the sales invoice.|  
    |**Bank Account No.**|Specify which of your company’s bank accounts the collected payment will be transferred to from the customer’s bank account.|  
    |**Bank Account Name**|Specifies the name of the bank account that you select in the **Bank Account No.** field. This field is filled automatically.|  

4. Choose the **OK** button.  

     A direct-debit collection is added to the **Direct Debit Collections** window, and one or more direct-debit collection entries are created.  

### <a name="to-export-a-direct-debit-collection-entry-to-a-bank-file"></a>To export a direct-debit collection entry to a bank file  
1. In the **Direct Debit Collections** window, on the **Home** tab, in the **Process** group, choose **Direct Debit Collect. Entries**.  
2. In the **Direct Debit Collect. Entries** window, select the entry that you want to export, and then, on the **Home** tab, in the **Process** group, choose **Create Direct Debit** File.  
3. Save the export file to the location from where you send or upload it to your electronic bank.  

     In the **Direct Debit Collect. Entries** window, the **Direct Debit Collection Status** field is changed to File Created. In the **SEPA Direct Debit Mandates** window, the **Debit Counter** field is updated with one count.  

If the exported file cannot be processed, for example because the customer is insolvent, you can reject the direct-debit collection entry. If the exported file is successfully processed by the bank, the due payments of the involved sales invoices are automatically collected from the involved customers. In that case you can close the collection.  

### <a name="to-reject-a-direct-debit-collection-entry"></a>To reject a direct-debit collection entry  

* In the **Direct Debit Collect. Entries** window, select the entry that was not successfully processed, and then, on the **Home** tab, in the **Process** group, choose **Reject Entry**.  

     The value in the **Status** field in the **Direct Debit Collect. Entries** window is changed to **Rejected**.  

### <a name="to-close-a-direct-debit-collection"></a>To close a direct-debit collection  
*  In the **Direct Debit Collect. Entries** window, select the entry that was successfully processed, and then, on the **Home** tab, in the **Process** group, choose **Close Collection**.  

     The related direct-debit collection is closed.  

You can now proceed to post receipts of payment for the involved sales invoices. You can do this as you typically post payment receipts, such as in the **Payment Registration** window, or you can post the related payment receipts directly from the **Direct Debit Collect. Entries** window. For more information, see [Post SEPA Direct Debit Payment Receipts](finance-how-to-post-sepa-direct-debit-payment-receipts.md).  

## <a name="see-also"></a>See Also  
[Set Up SEPA Direct Debit](finance-how-to-set-up-sepa-direct-debit.md)  
[Post SEPA Direct Debit Payment Receipts](finance-how-to-post-sepa-direct-debit-payment-receipts.md)  
[Collecting Payments with SEPA Direct Debit](finance-collect-payments-with-sepa-direct-debit.md)  

