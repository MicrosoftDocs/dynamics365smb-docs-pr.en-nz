---
title: Register New Customers by Creating a Customer Card (contains video)
description: Describes how to create a customer card to register information about each new customer or client you sell to.
author: brentholtorf
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 'client, customer, credit'
ms.search.form: '7, 21, 22, 33, 42, 43, 367, 368, 369, 461, 512, 785, 1330, 1380, 1381, 1382, 1627, 2107, 7177, 9080, 9081, 9084, 9301, 9305'
ms.date: 09/01/2022
ms.author: bholtorf
---
# <a name="register-new-customers"></a>Register New Customers

Customers are your source of income. You must register each customer you sell to as a customer card. Customer cards contain the information required to sell products to the customer. Learn more at [Invoice Sales](sales-how-invoice-sales.md) and [Register New Items](inventory-how-register-new-items.md).  

Before you can register new customers, you must set up various sales codes to choose from when you fill in customer cards. Learn more at [Setting Up Sales](sales-setup-sales.md).


> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3PZsM]

## <a name="adding-new-customers"></a>Adding new customers

You can add new customers manually by filling out the **Customer Card** page, or you can use templates that contain predefined information. For example, you can create a template for different types of customer profiles. Using templates saves time when adding new customers, and helps ensure the information is correct each time. 

If you create:
* Multiple templates for use with more than one type of customer, you can choose the suitable template when you add a customer.
* Only one template, it is used for all new customers. 

After you create a template, you can use the **Apply Template** action to apply it to one or more selected customers. To create a template, fill in the information to be reused on the **Customer Card** page, then save it as a template. Learn more in the [To save the customer card as a template](sales-how-register-new-customers.md#to-save-the-customer-card-as-a-template) section.

> [!TIP]
> It can be helpful to personalise the **Customer Template** page when you create a template. For example, you might want to add the **Credit Limit** field to a template. Learn more in the [Personalise your workspace](/dynamics365/business-central/ui-personalization-user#start-personalizing-by-using-the-personalization-mode) section.

You can also create a customer from a contact. Learn more in the [To create a customer, vendor, employee, or bank account from a contact](marketing-create-contact-companies.md#to-create-a-customer-vendor-employee-or-bank-account-from-a-contact) section.  

### <a name="to-create-a-new-customer-card"></a>To create a new customer card

[!INCLUDE[create_new_customer](includes/create_new_customer.md)]

The **Prices & Discounts** action provides options for managing special prices or discounts for a customer when an order meets certain criteria. Examples of such criteria might be when they're purchasing a certain item, ordering a minimum quantity, or buying before a date, such as when a campaign ends. Learn more at [Record Sales Price, Discount, and Payment Agreements](sales-how-record-sales-price-discount-payment-agreements.md).

The customer is now registered, and the customer card is ready to be used on sales documents.  

### <a name="to-save-the-customer-card-as-a-template"></a>To save the customer card as a template

You can use a customer card as a template when you create new customer cards.

1. On the **Customer Card** page, choose the **Save as Template** action. The **Customer Template** page opens showing the customer card as a template.
2. Fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. To reuse dimensions in templates, choose the **Dimensions** action. The **Dimension Templates** page opens showing any dimension codes set up for the customer.
4. Edit or enter dimension codes you want to apply to new customer cards created with this template.  
5. When you have completed the new customer template, choose **OK**.

The customer template is added to the list of customer templates, and you can use it to create new customer cards.

## <a name="deleting-customer-cards"></a>Deleting customer cards

If you have posted a transaction for a customer, you cannot delete the customer card because the ledger entries may be needed for auditing. To delete customer cards with ledger entries, contact your Microsoft partner to do so through code.  

## <a name="managing-credit-limits"></a>Managing credit limits

Credit limits, balance amounts, and payment terms make it possible for [!INCLUDE [prod_short](includes/prod_short.md)] to issue a credit and an overdue balance warning when you enter a sales order. Furthermore, reminder term and finance charge term elements enable you to invoice interest and/or extra fees.  

The **Credit Limit** field on a customer card specifies the maximum amount you allow the customer to exceed the payment balance before warnings are issued. Then, when you enter information in journals, quotes, orders, and invoices, [!INCLUDE [prod_short](includes/prod_short.md)] tests the sales header and individual sales lines to see if the credit limit has been exceeded.

You can post even if the credit limit has been exceeded. If the field is left blank, there will be no credit limit for this customer.  

You can choose not to have warnings tell you the customer's credit limit has been exceeded, and you can specify which types of warnings you want to see.

### <a name="to-specify-credit-limit-warnings"></a>To specify credit limit warnings

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales & Receivables Setup**, then choose the related link.

2. On the **General** FastTab, in the **Credit Warnings** field, choose the relevant option as described in the following table:

    |Option| Description|
    |------|------------|
    |**Both Warnings**| Both the **Credit Limit** and the **Balance Due** fields on the customer's card are checked, and a warning is shown if the customer exceeds its credit limit or has an overdue balance.|
    |**Credit Limit**|The value in the **Credit Limit** field on the customer's card is compared with the customer's balance, and a warning is shown if the customer's balance exceeds this amount.|
    |**Overdue Balance**|The **Balance Due** field on the customer's card is checked, and a warning is shown if the customer has an overdue balance.|
    |**No Warning**|No credit warnings are shown regarding the customer's status.|

## <a name="see-also"></a>See also

[Defining Payment Methods](finance-payment-methods.md)  
[Merge Duplicate Records](sales-how-merge-duplicate-records.md)  
[Create Number Series](ui-create-number-series.md)  
[Enable Partial Shipments with Shipping Advice](sales-how-send-partial-shipments.md)  
[Sales](sales-manage-sales.md)  
[Setting Up Sales](sales-setup-sales.md)  
[Use Online Maps to Find Locations and Directions](across-online-maps.md)  
[Work with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
