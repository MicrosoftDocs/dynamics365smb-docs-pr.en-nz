---
title: Create a vendor card to register a new vendor (contains video)
description: Learn how to create a vendor card to register a new vendor or supplier and save vendor cards as a template.
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bholtorf
ms.topic: conceptual
ms.search.keywords: supplier
ms.search.form: '26, 27, 34, 461, 786, 1379, 1385, 1386, 1628'
ms.date: 05/07/2024
ms.service: dynamics-365-business-central
ms.custom: bap-template
---
# <a name="register-new-vendors"></a>Register new vendors

Vendors provide the products you sell. Each vendor you purchase from must be registered with a vendor card.

Before you register new vendors, you must set up various purchase codes to select from when you fill in vendor cards. After all the required master data is created, you can add unique characteristics for a vendor, such as prioritise the vendor for payment purposes or list items that the vendor and other vendors supply. Another group of setup tasks for vendors is to record your agreements concerning discounts, prices, and payment methods. Learn more at [Setting Up Purchasing](purchasing-setup-purchasing.md).

Vendor cards hold the information required to buy products from each vendor. Learn more at [Record Purchases](purchasing-how-record-purchases.md) and [Register New Items](inventory-how-register-new-items.md).
<br /><br />  

> [!Video https://www.microsoft.com/videoplayer/embed/RE3PZtd?rel=0]

## <a name="adding-new-vendors"></a>Adding new vendors

You can add new vendors manually, by filling out the **Vendor Card** page, or you can use templates that contain predefined information. For example, you can create templates for different types of vendor profiles. Using templates saves time when adding new vendors, and helps ensure the information is correct each time.

> [!NOTE]  
> If vendor templates exist for different vendor types, when you begin to create a new vendor card you'll see a page from which you can select the appropriate template. If only one vendor template exists, then new vendor cards always use that template.

After you create a template, you can use the **Apply Template** action to apply it to one or more selected vendors. To create a template, fill in the information you want to reuse on the **Vendor Card** page, then save it as a template. Learn more in the [To save the Vendor Card Page as a template](purchasing-how-register-new-vendors.md#to-save-the-vendor-card-as-a-template) section.

> [!TIP]
> It can be helpful to personalise the **Vendor Template** page when you create a template. For example if want to add a field that is not already displayed on the page. Learn more in the [Personalise your workspace](/dynamics365/business-central/ui-personalization-user#start-personalizing-by-using-the-personalization-mode) section.

You can also create a vendor from a contact. Learn more in the [Creating a customer, vendor, employee, or bank account from a contact](marketing-create-contact-companies.md#to-create-a-customer-vendor-employee-or-bank-account-from-a-contact) section.

Remit-to addresses are used when you print cheques to pay your vendors, and vendors can have multiple remit-to addresses for payments. For example, a vendor might supply an item from a subsidiary company, but wants to receive payment at their headquarters. [!INCLUDE [prod_short](includes/prod_short.md)] lets you set up multiple mailing addresses for each vendor, and you can choose the correct location to send payments to on an invoice-by-invoice basis.

You specify remit-to addresses on Vendor Card pages, and on the Shipping & Payments FastTab on purchase orders and invoices. When you create payment journal lines using the Pay Vendor or Create Payment actions on the Vendors list page or Vendor Card page, or the Apply Entries action on a payment journal, the remit-to code on the vendor ledger entry is assigned. You can overwrite this value.

### <a name="to-create-a-new-vendor"></a>To create a new vendor

[!INCLUDE[create_new_vendor](includes/create_new_vendor.md)]

> [!TIP]  
> If you do not know the invoicing address to be used for every invoice from a vendor, do not fill in the **No.** field on the **General** FastTab. Instead, choose the pay-to vendor number after you have set up a purchase quote, order, or invoice header.

The vendor is now registered, and the vendor card is ready to use on purchase documents.

If you want to use this vendor card as a template when you create new vendor cards, you can save it as a vendor template. Learn more in the [To save the vendor card as a template](#to-save-the-vendor-card-as-a-template) section.

### <a name="deleting-and-editing-vendor-information"></a>Deleting and editing vendor information

You can edit the information on vendor cards at any time. However, if you have posted a transaction for a vendor, you cannot delete the card because the ledger entries may be needed for auditing. To delete vendor cards with ledger entries, contact your Microsoft partner to do so through code.

> [!TIP]
> You can change the International Bank Account Number (IBAN) on a vendor bank account without the change affecting your historical credit transfer register entries. Credit transfer register entries store the *Recipient IBAN* and the *Recipient Bank Account No.* specified in the **Vendor Bank Account** and **Recipient Name** fields from the **Vendor Card** page when the entries were created.

> [!TIP]
> You can add alternative addresses on vendor cards by choosing the **Order Addresses** action.

## <a name="to-save-the-vendor-card-as-a-template"></a>To save the vendor card as a template

1. On the **Vendor Card** page, choose the **Save as Template** action. The **Vendor Template** page opens showing the vendor card as a template.
2. Fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. To reuse dimensions in templates, choose the **Dimensions** action. The **Dimension Templates** page opens showing any dimension codes set up for the vendor.
4. Edit or enter dimension codes to apply to new vendor cards created using the template.
5. When you have completed the new vendor template, choose **OK**.  
   The vendor template is added to the list of vendor templates, so you can use it to create new vendor cards.

## <a name="see-also"></a>See also

[Merge Duplicate Records](sales-how-merge-duplicate-records.md)  
[Create Number Series](ui-create-number-series.md)  
[Set Up Vendor Bank Account](purchasing-how-set-up-vendors-bank-accounts.md)  
[Set Up Purchasers](purchasing-how-setup-purchasers.md)  
[Purchasing](purchasing-manage-purchasing.md)  
[Record Purchases](purchasing-how-record-purchases.md)  
[Use Online Maps to Find Locations and Directions](across-online-maps.md)  
[Work with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
