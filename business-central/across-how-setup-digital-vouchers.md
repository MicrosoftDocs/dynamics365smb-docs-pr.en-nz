---
title: Set up digital vouchers
description: This article explains how to set up and use enforced digital vouchers in Microsoft Dynamics 365 Business Central.
author: altotovi
ms.author: altotovi
ms.reviewer: null
ms.service: dynamics365-business-central
ms.topic: how-to
ms.search.keywords: 'digital voucher, voucher, attachment, setup'
ms.search.form: '5579, 5582, 5587'
ms.date: 11/17/2023
ms.custom: bap-template
---

# Set up digital vouchers

Administrators can use digital voucher functionality to require that documents are attached to specific transactions when they're posted. Therefore, this functionality allows for a source-driven approach and provides a better audit trail. Different types of enforcement can be configured for this purpose, depending on the documents or journal types.

The term *digital voucher* refers to a digital or electronic form of a traditional voucher in accounting. A voucher is a document that's used to support and authorise financial transactions. In accounting, a voucher typically serves as evidence of an expenditure or a receipt of funds. The voucher might include details such as the date of the transaction, a description, the amount, and any authorisation signatures.

> [!IMPORTANT]
> In some countries and regions, you might be restricted from configuring some options, because specific setups might be mandated by legal requirements. If you encounter these restrictions, look for a detailed explanation on the documentation page for your country or region.

## Enable digital vouchers

Follow these steps to enable digital voucher functionality.

1. Select the ![Lightbulb that opens the Tell Me feature 3.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Digital Voucher Setup**, and then select the related link.
2. Select the **Enabled** checkbox.

## Set up digital vouchers

You can use different setups for the following documents and journals.

| Entry type | Description |
|------------|-------------|
| Sales Document | Specifies postings that are completed from sales documents. |
| Purchase Document | Specifies postings that are completed from purchase documents. |
| General Journal | Specifies postings that are completed from the general journal for all account types except those that are related to the customer and vendor. If you select one of those account types, you change control of the posting process. If you select **Customer** as the account type, the system checks your setup that's related to the sales journal. If you select **Vendor** as the account type, the system checks your setup that's related to the purchase journal. |
| Sales Journal | Specifies the postings that are completed from the sales journal and the general journal where **Customer** is selected as the account type. |
| Purchase Journal | Specifies the postings that are completed from the purchase journal and the general journal where **Vendor** is selected as the account type. |

Follow these steps to define how your organisation uses enforced digital vouchers.

1. Select the ![Lightbulb that opens the Tell Me feature 3.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Digital Voucher Entry Setup**, and then select the related link. Alternatively, on the **Digital Voucher Setup** page, select **Entry Setup**.
2. In the **Entry Type** column, select an option.
3. In the **Cheque Type** column, select an enforcement option. If you select **None**, you can post the selected type of entry without a digital voucher. If you select **Attachment**, the entry must include an attachment. If you select **Attachment or Note**, you can include an attachment or a note for the entry. 
4. Select the **Generate Automatically** checkbox to generate the digital voucher automatically. For example, if you don't want to manually add a sales invoice to your transaction, select this checkbox. Then, you just have to post the document. The system automatically creates the document, based on your report layout, and attaches it to the transaction.
5. Select the **Skip If Manually Added** checkbox if you don't want to add an automatically generated digital voucher if the user has already added a manual attachment.

### Use source codes for setup

To use enforcement for journals, but not for all transaction types, connect the specific source code to identify the entry type in the general journal, sales journal, or purchase journal.

Follow these steps to set up specific source codes for digital vouchers.

1. On the **Digital Voucher Entry Setup** page, select **Source Codes**.
2. On the **Voucher Entry Source Codes** page, select the source codes that you want to configure.
3. Close the page.

## Use the functionality

Open a purchase or sales document, and enter information in the required fields. Before you post the document, you must follow these steps to attach a digital voucher.

1. In the **Incoming Document Files** FactBox, select **Attach File**.
2. Drag a file directly onto the **Insert File** page, or browse to the file from this page.

The document is attached to the **Incoming Document Files** FactBox. For each line, you can find the document name and type.

If you accidentally attach the wrong voucher, follow these steps to delete it before you post the document.

1. In the **Incoming Document Files** FactBox from the document line, select **Incoming Document**.
2. On the **Incoming document** page, select **Delete**.

> [!NOTE]
> If attachment of a digital voucher is configured as mandatory, and you try to post documents or journals without attaching a voucher, the system prevents you from posting. You receive the following error message: "Not possible to post without attaching the digital voucher."

### Find attached vouchers in transactions

You can find the attached voucher from the posted document or from the **General Ledger Entries** page by looking in the **Incoming Document Files** FactBox.

You can't delete an attached document after posting is completed. However, you can add more attachments after posting is completed.

## See also

[Financial Management](finance.md)  
[Work with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)

[!INCLUDE[footer-include](includes/footer-banner.md)]
