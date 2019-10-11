---
title: Make Payments with Bank Data Conversion Service or SEPA Credit Transfer | Microsoft Docs
description: Process payments to your vendors by exporting a file together with the payment information from the journal lines.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2019
ms.author: sgroespe
ms.openlocfilehash: c1089a48cee57f6e42e48d995ed9c9ae7fd8fd80
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 10/01/2019
ms.locfileid: "2302128"
---
# <a name="making-payments-with-bank-data-conversion-service-or-sepa-credit-transfer"></a>Making Payments with Bank Data Conversion Service or SEPA Credit Transfer
On the **Payment Journal** page, you can process payments to your vendors by exporting a file together with the payment information from the journal lines. You can then upload the file to your electronic bank where the related money transfers are processed. [!INCLUDE[d365fin](includes/d365fin_md.md)] supports the SEPA Credit Transfer format, but in your country/region, other formats for electronic payments may be available.

In the generic version of [!INCLUDE[d365fin](includes/d365fin_md.md)], a global provider of services to convert bank data to any file format that your bank requires is set up and connected. In North American versions, the same service can be used to send payment files as electronic funds transfer (EFT), however with a slightly different process. See step 6 in [To export payments to a bank file](finance-make-payments-with-bank-data-conversion-service-or-sepa-credit-transfer.md#to-export-payments-to-a-bank-file).   

 To enable SEPA credit transfers, you must first set up a bank account, a vendor, and the general journal batch that the payment journal is based on. You then prepare payments to vendors by automatically filling the **Payment Journal** page with due payments with specified posting dates.  

> [!NOTE]  
>  When you have verified that the payments are successfully processed by the bank, you can proceed to post the payment journal lines.  

## <a name="setting-up-the-bank-data-conversion-service"></a>Setting Up the Bank Data Conversion Service.
Activate the Bank Data Conversion Service feature to have any bank statement file converted to a format that you can import or to have your exported payment files converted to the format that your bank requires. For more information, see [Set Up the Bank Data Conversion Service](bank-how-setup-bank-statement-service.md).

## <a name="setting-up-sepa-credit-transfer"></a>Setting Up SEPA Credit Transfer
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

The direct-debit mandate is automatically inserted in the **Direct Debit Mandate ID** field when you create a sales invoice for the customer that you selected in step 2. For more information, see [Create Recurring Sales and Purchase Lines](sales-how-work-standard-lines.md).   

## <a name="preparing-the-payment-journal"></a>Preparing the Payment Journal
Fill the payment journal with lines for due payments to vendors, with the option to insert posting dates based on the due date of the related purchase documents. For more information, see [Managing Payables](payables-manage-payables.md).

## <a name="exporting-payments-to-a-bank-file"></a>Exporting Payments to a Bank File
When you are ready to make payments to your vendors, or reimbursements to your employees, you can export a file with the payment information on the lines on the **Payment Journal** page. You can then upload the file to your bank to process the related money transfers.

In the generic version of [!INCLUDE[d365fin](includes/d365fin_md.md)], the Bank Data Conversion service is set up and connected. In North American versions, the same service can be used to send payment files as electronic funds transfer (EFT), however with a slightly different process. See step 6 in [To export payments to a bank file](finance-make-payments-with-bank-data-conversion-service-or-sepa-credit-transfer.md#to-export-payments-to-a-bank-file).

> [!NOTE]  
>   Before you can export payment files from the payment journal, you must specify the electronic format for the involved bank account, and you must enable the bank data conversion service. For more information, see [Set Up Bank Accounts](bank-how-setup-bank-accounts.md) and [Set Up the Bank Data Conversion Service](bank-how-setup-bank-data-conversion-service.md). In addition, you must select the **Allow Payment Export** check box on the **General Journal Batches** page. For more information, see [Working with General Journals](ui-work-general-journals.md).  

You use the **Credit Transfer Registers** page to view the payment files that have been exported from the payment journal. From this page, you can also re-export payment files in case of technical errors or file changes. Note, however, that exported EFT files are not shown in this page and cannot be re-exported.  

### <a name="to-export-payments-to-a-bank-file"></a>To export payments to a bank file
The following describes how to pay a vendor by cheque. The steps are similar to refund a customer by cheque.

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Payment Journals**, and then choose the related link.
2. Fill in the payment journal lines. For more information, see [Record Payments and Refunds](payables-how-post-payments-refunds.md).

> [!NOTE]  
>   If you are using EFT, you must select either **Electronic Payment** or **Electronic Payment–IAT** in the **Bank Payment Type** field. Different file export services and their formats require different setup values in the **Bank Account Card** and **Vendor Bank Account Card** pages. You will be informed about wrong or missing setup values as you try to export the file.

3. When you have completed all payment journal lines, choose the **Export** action.
4. On the **Export Electronic Payments** page, fill in the fields as necessary.

    Any error messages will be shown in the **Payment File Errors** FactBox where you can also choose an error message to see detailed information. You must resolve all errors before the payment file can be exported.

    > [!TIP]  
    >   When you use the bank data conversion service, a common error message states that the bank account number does not have the length that your bank requires. To avoid or resolve the error, you must remove the value in the **IBAN** field on the **Bank Account Card** page and then, in the **Bank Account No.** field, enter a bank account number in the format that your bank requires.

5. On the **Save As** page, specify the location that the file is exported to, and then choose **Save**.

    > [!NOTE]  
    >   If you are using EFT, save the resulting vendor remittance form as a Word document or select to have it emailed directly to the vendor. The payments are now added to the **Generate EFT File** page from where you can generate multiple payment orders together to save transmission cost. For more information, see the following steps.
6. On the **Payment Journal** page, choose the **Generate EFT File** action.

    On the **Generate EFT File** page, all payments set up for EFT that you have exported from the payment journal for a specified bank account but not yet generated are listed on the **Lines** FastTab.
7. Choose the **Generate EFT File** action to export one file for all the EFT payments.
8. On the **Save As** page, specify the location that the file is exported to, and then choose **Save**.

The bank payment file is exported to the location that you specify, and you can proceed to upload it to your electronic bank account and make the actual payments. Then you can post the exported payment journal lines.

### <a name="to-plan-when-to-post-exported-payments"></a>To plan when to post exported payments
If you do not want to post a payment journal line for an exported payment, for example because you are waiting for confirmation that the transaction has been processed by the bank, you can just delete the journal line. When you later create a payment journal line to pay the remaining amount on the invoice, the **Total Exported Amount** field shows how much of the payment amount has already been exported. Also, you can find detailed information about the exported total by choosing the **Credit Transfer Reg. Entries** button to see details about exported payment files.

If you follow a process where you do not post payments until you have confirmation that they have been processed in the bank, you can control this in two ways.

* In a payment journal with suggested payment lines, you can sort on either the **Exported to Payment File** column or the **Total Exported Amount** and then delete payment suggestions for open invoices for which payments have already been made and you do not want to make payments for.
* On the **Suggest Vendor Payments** page, where you specify which payments to insert in the payment journal, you can select the **Skip Exported Payments** check box if you do not want to insert journal lines for payments that have already been exported.

To see information about exported payments, choose the **Payment Export History** action.

### <a name="to-re-export-payments-to-a-bank-file"></a>To re-export payments to a bank file
You can re-export payment files from the **Credit Transfer Registers** page. Before you delete or post payment journal lines, you can also re-export the payment file from the **Payment Journal** page by simply exporting it again. If you have deleted or posted the payment journal lines after exporting them, you can re-export the same payment file from the **Credit Transfer Registers** page. Select the line for the batch of credit transfers that you want to re-export, and then use the **Reexport Payments to File** action.

> [!NOTE]  
>   Exported EFT files are not shown on the **Credit Transfer Registers** page and cannot be re-exported.

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Credit Transfer Registers**, and then choose the related link.
2. Select a payment export that you want to re-export, and then choose the **Reexport Payment to File** action.

## <a name="posting-the-payments"></a>Posting the Payments
When the electronic payment is successfully processed by the bank, post the payments. For more information, see [Making Payments](payables-make-payments.md).

## <a name="see-also"></a>See Also  
[Set Up the Bank Data Conversion Service](bank-how-setup-bank-statement-service.md)  
[Set Up SEPA Credit Transfer](finance-how-to-set-up-sepa-credit-transfer.md)  
[Managing Payables](payables-manage-payables.md)   
[Working with General Journals](ui-work-general-journals.md)  
[Collect Payments with SEPA Direct Debit](finance-collect-payments-with-sepa-direct-debit.md)   
