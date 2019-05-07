---
title: Set up SEPA credit transfer | Microsoft Docs
description: Learn how to set up SEPA credit transfer in Business Central .
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: sepa, credit, transfer, payment,
ms.date: 04/01/2019
ms.author: sgroespe
redirect_url: finance-make-payments-with-bank-data-conversion-service-or-sepa-credit-transfer
ms.openlocfilehash: 56f200d00345bfe18d8fcccbee6493785fe6a034
ms.sourcegitcommit: bd78a5d990c9e83174da1409076c22df8b35eafd
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 03/31/2019
ms.locfileid: "929474"
---
# <a name="set-up-sepa-credit-transfer"></a>Set Up SEPA Credit Transfer
From the **Payment Journal** page, you can export payments to a file for upload to your electronic bank for processing of the related money transfers. [!INCLUDE[d365fin](includes/d365fin_md.md)] supports the SEPA Credit Transfer format, but in your country/region, other formats for electronic payments may be available.  

To enable export of a bank file formats that are not supported out of the box in [!INCLUDE[d365fin](includes/d365fin_md.md)] , you can set up a data exchange definition by using the data exchange framework. For more information, see [Set Up Data Exchange Definitions](across-how-to-set-up-data-exchange-definitions.md).  

Before you can process payment electronically by exporting payment files in the SEPA Credit Transfer format, you must perform the following setup steps:  

* Set up the bank account in question to handle the SEPA Credit Transfer format  
* Set up vendor cards to process payments by exporting files in the SEPA Credit Transfer format  
* Set up the related general journal batch to enable payment export from the **Payment Journal** page  
* Connect the data exchange definition for one or more payment types with the relevant payment method or methods  

### <a name="to-set-up-a-bank-account-for-sepa-credit-transfer"></a>To set up a bank account for SEPA Credit Transfer  
1. In the **Search** box, enter **Bank Accounts**, and then choose the related link.  
2. Open the card of the bank account from which you will export payment files in the SEPA Credit Transfer format.  
3. On the **Transfer** FastTab, in the **Payment Export Format** field, choose **SEPADD**.  
4. In the **SEPA CT Msg. ID No. Series** field, choose a number series from which numbers are assigned to SEPA credit transfer entries.  
5. Make sure the **IBAN** field is filled.  

    > [!NOTE]  
    >  The **Currency Code** field must be set to **EUR**, because SEPA credit transfers can only be made in the EURO currency.  

### <a name="to-set-up-a-vendor-card-for-sepa-credit-transfer"></a>To set up a vendor card for SEPA Credit Transfer  
1. In the **Search** box, enter **Vendors**, and then choose the related link.  
2. Open the card of the vendor whom you will pay electronically by export payment files in the SEPA Credit Transfer format.  
3. On the **Payment** FastTab, in the **Payment Method Code** field, choose **BANK**.  
4. In the **Preferred Bank Account** field, choose the bank to which the money will be transferred when it is processed by your electronic bank.  

     The value in the **Preferred Bank Account** field is copied to the **Recipient Bank Account** field on the **Payment Journal** page.  

### <a name="to-set-the-payment-journal-up-to-export-payment-files"></a>To set the payment journal up to export payment files  
1. In the **Search** box, enter **Payment Journals**, and then choose the related link.  
2. Open the payment journal that you use to process payments by exporting files in the SEPA Credit Transfer format.  
3. In the **Batch Name** field, choose the drop\-down button.  
4. On the **General Journal Batches** page, on the **Home** tab, in the **Manage** group, choose **Edit List**.  
5. On the line for the payment journal that you will use to export payments, select the **Allow Payment Export** check box.  

### <a name="to-connect-the-data-exchange-definition-for-one-or-more-payment-types-with-the-relevant-payment-method-or-methods"></a>To connect the data exchange definition for one or more payment types with the relevant payment method or methods  
1. In the **Search** box, enter **Payment Methods**, and then choose the related link.  
2. On the **Payment Methods** page, select the payment method that is used to export payments from, and then choose the **Pmt. Export Line Definition** field.  
3. On the **Pmt. Export Line Definitions** page, select the code that you specified in the **Code** field on the **Line Definitions** FastTab in step 4 in the “To describe the formatting of lines and columns in the file” section in the [Set Up Data Exchange Definitions](across-how-to-set-up-data-exchange-definitions.md) procedure.  

## <a name="see-also"></a>See Also  
[Collect Payments with SEPA Direct Debit](finance-collect-payments-with-sepa-direct-debit.md)  
[Set Up Data Exchange Definitions](across-how-to-set-up-data-exchange-definitions.md)  
[Create Recurring Sales and Purchase Lines](sales-how-work-standard-lines.md)  
[Exchanging Data Electronically](across-data-exchange.md)  
