---
title: Set Up Special Sales Prices and Discounts for Customers | Microsoft Docs
description: Describes how to define the alternate pricing and discount agreements that you want to apply to sales documents when selling to different customers.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: special price, alternate price, pricing
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 0873c45262dd9606ac187f5aab07b09677f6c1c8
ms.sourcegitcommit: adf1a87a677b8197c68bb28c44b7a58250d6fc51
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 01/21/2021
ms.locfileid: "5035622"
---
# <a name="record-special-sales-prices-and-discounts"></a>Record Special Sales Prices and Discounts

The different price and discount agreements that apply when selling to different customers must be defined so that the agreed rules and values are applied to sales documents that you create for the customers.

When you have recorded special prices and line discounts for sales and purchases, [!INCLUDE[prod_short](includes/prod_short.md)] ensures that your profit on item trade is always optimal by automatically calculating the best price on sales and purchase documents and on job and item journal lines. For more information, see [Best Price Calculation](sales-how-record-sales-price-discount-payment-agreements.md#best-price-calculation).

Concerning prices, you can have a special sales price inserted on sales lines if a certain combination of customer, item, minimum quantity, unit of measure, or starting/ending date exists. For more information, see the [To set up a sales price for a customer](#to-set-up-a-sales-price-for-a-customer) and [Best Price Calculation](#best-price-calculation) sections.  

Concerning discounts, you can set up and use two types of sales discounts:

| Discount Type | Description |
| --- | --- |
| **Sales Line Discount** |An amount discount that is inserted on sales lines if a certain combination of customer, item, minimum quantity, unit of measure, or starting/ending date exists. This works in the same way as for sales prices. |
| **Invoice Discount** |A percentage discount that is subtracted from the document total if the value amount of all lines on a sales document exceeds a certain minimum. |

Because sales prices and sales line discounts are based on a combination of item and customer, you can also perform this configuration from the item card of the item where the rules and values apply.

> [!NOTE]  
> If you do not want an item to ever be sold at a discounted price, simply leave discount fields on the item card empty, and do not include the item in any line discount setup.

## <a name="sales-invoice-discounts-and-service-charges"></a>Sales invoice discounts and service charges

When you use invoice discounts, the size of the invoice amount determines the size of the discount that is granted.  

On the **Cust. Invoice Discounts** page, you can also add a service charge to invoices over a certain amount.  

Before you can use invoice discounts with sales, you must specify certain information. You must decide the following:  

- Which customers will be granted this type of discount  
- Which discount percentages you will use  

If you want invoice discounts to be calculated automatically, you can specify this on the **Sales & Receivables Setup** page.  

For each customer, you can specify whether you will grant invoice discounts if the requirement is satisfied (that is, if the invoice amount is large enough). You can define the terms of the invoice discount in local currency for domestic customers and in foreign currency for foreign customers.  

You link discount percentages to specific invoice amounts in the **Cust. Invoice Discounts** page for each customer. You can enter any number of percentages. Each customer can have its own page, or you can link several customers to the same page.  

In addition to (or instead of) a discount percentage, you can link a service charge amount to a specific invoice amount.  

> [!TIP]  
> Before you start entering this information, it is a good idea to prepare an outline of the discount structure that you want to use. This makes it easier to see which customers can be linked to the same invoice discount page. The fewer pages you have to set up, the faster you can enter the basic information.

For training in discounts in sales, see [Set up discounts for your customers](/learn/modules/customer-discounts-dynamics-365-business-central/index) at Microsoft Learn.  

### <a name="calculating-invoice-discounts-on-sales"></a>Calculating Invoice Discounts on Sales

[!INCLUDE [sales-invoice-discounts](includes/sales-invoice-discounts.md)]

## <a name="to-set-up-a-sales-line-discount-for-a-customer"></a>To set up a sales line discount for a customer

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Customers**, and then choose the related link.
2. Open the relevant customer card, and then choose the **Line Discounts** action.

    On the **Sales Line Discounts** page, the **Sales Type** field is prefilled with **Customer**, and the **Sales Code** field is prefilled with the customer number.
3. Fill in the fields on the line as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)] Fill a line for each combination that will grant a sales line discount to the customer.

> [!Note]
> When you open the **Sales Prices** and **Sales Line Discounts** windows from a specific customer, the **Sales Type Filter** and **Sales Code Filter** fields are set for the customer and cannot be changed or removed, indicated by the grayed value in the **Sales Code Filter** field.
>
> To set up prices or line discounts for all customers, a customer price group, or a campaign, you must open the windows from an item card. Alternatively, for sales prices, use the **Sales Price Worksheet** page. For more information, see [To bulk update item prices](sales-how-record-sales-price-discount-payment-agreements.md#to-bulk-update-item-prices).  

## <a name="to-set-up-an-invoice-discount-for-a-customer"></a>To set up an invoice discount for a customer

When you have decided which customers are eligible for invoice discounts, enter the invoice discount code on the customer cards and set up the terms for each code.

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Customers**, and then choose the related link.
2. Open the customer card for a customer that will be eligible for invoice discounts.
3. In the **Invoice Disc. Code** field, select a code for the relevant invoice discount terms to use to calculate invoice discounts for the customer.

    > [!NOTE]  
    > Invoice discount codes are represented by existing customer cards. This enables you to quickly assign invoice discount terms to customers by picking the name of another customer who will have the same terms. To set up customer-specific invoice discount terms, set the **Invoice Disc. Code** field to the customer's customer code, and then proceed to the next step.

4. On the **Customer Card** page, choose the **Invoice Discounts** action. The **Cust. Invoice Discounts** page opens.
5. In the **Currency Code** field, enter the code for a currency that the invoice discount terms on the line applies to. Leave the field blank to set up invoice discount terms in NZD.
6. Optionally, in the **Minimum Amount** field, enter the minimum amount that an invoice must have to be eligible for the discount.
7. In the **Discount %** field, enter the invoice discount as a percentage of the invoice amount.
8. Repeat steps 5 through 7 for each currency that the customer will receive a different invoice discount for.

The invoice discount is now set up and assigned to the customer in question. When you select the customer code in the **Invoice Disc. Code** field on other customer cards, the same invoice discount is assigned to those customers.

## <a name="to-set-up-a-sales-price-for-a-customer"></a>To set up a sales price for a customer

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Customers**, and then choose the related link.
2. Open the relevant customer card, and then choose the **Prices** action.

    On the **Sales Prices** page, the **Sales Type** field is prefilled with **Customer**, and the **Sales Code** field is prefilled with the customer number.
3. Fill in the fields on the line as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)] Fill a line for each combination that will grant a special sales price to the customer.

## <a name="to-copy-sales-prices"></a>To copy sales prices

If you want to copy sales prices, such as an individual customer's sales prices to use for a customer price group, you must run the **Suggest Sales Price on Wksh.** batch job, which you launch from the **Sales Price Worksheet** page.  

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Price Worksheet**, and then choose the related link.  
2. Choose the **Suggest Sales Price on Wksh.** action.  
3. On the **Sales Prices** FastTab, fill in the **Sales Type** and **Sales Code** fields with the original sales prices you want to copy.  
4. In the top section of the request page, fill in the **Sales Type** and **Sales Code** fields with the type and name you want the sales prices copied to.  
5. If you want the batch job to create new prices, select the **Create New Prices** check box.  
6. Choose the **OK** button to fill in the lines on the **Sales Price Worksheet** page with the suggested new prices, indicating that they are valid for the selected sales type.  

> [!NOTE]  
> This batch job only creates suggestions and it does not implement the suggested changes. If you are satisfied with the suggestions and want to implement them, that is insert them on the **Sales Prices** page, choose the **Implement Price Changes** action on the **Sales Price Worksheet** page.

## <a name="to-bulk-update-item-prices"></a>To bulk update item prices

If you want to bulk update item prices, such as increase all item prices by some percentage, you must run the **Suggest Item Price on Wksh.** batch job. You can find a link to the batch job on the **Sales Price Worksheet** page.  

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Price Worksheet**, and then choose the related link.  
2. Choose the **Suggest Item Price on Wksh.** action.  
3. On the **Item** FastTab, fill in the **No.** or **Inventory Posting Group** or other fields with the original item prices you want to update.  
4. In the top section of the request page, fill in the **Sales Type** and **Sales Code** with the type and name you want the sales prices copied to.
5. If you want the batch job to automatically adjust suggested item prices, enter adjustment in **Adjustment Factor** field. For example, you would enter 1.15 in **Adjustment Factor** for 15% increase in item price.  
6. If you want the batch job to create new prices, select the **Create New Prices** field.  
7. Choose the **OK** button to fill in the lines on the **Sales Price Worksheet** page with the suggested new prices, indicating that they are valid for the selected **Item**.  

> [!NOTE]
> This batch job only creates suggestions and it does not implement the suggested changes. If you are satisfied with the suggestions and want to implement them, that is insert them in the **Sales Prices** table, you can use the **Implement Price Changes** batch job, which is found on the **Actions** tab, in the **Functions** group, on the **Sales Price Worksheet** page.

## <a name="best-price-calculation"></a>Best Price Calculation

When you have recorded special prices and line discounts for sales and purchases, [!INCLUDE[prod_short](includes/prod_short.md)] ensures that your profit on item trade is always optimal by automatically calculating the best price on sales and purchase documents and on job and item journal lines.

The best price is the lowest permissible price with the highest permissible line discount on a given date. [!INCLUDE[prod_short](includes/prod_short.md)] automatically calculates this when it inserts the unit price and the line discount percentage for items on new document and journal lines.

> [!NOTE]  
> The following describes how the best price is calculated for sales. The calculation is the same for purchases.

1. [!INCLUDE[prod_short](includes/prod_short.md)] checks the combination of the bill-to customer and the item and then calculates the applicable unit price and line discount percentage, using the following criteria:

    - Does the customer have a price/discount agreement, or does the customer belong to a group that does?
    - Is the item or the item discount group on the line included in any of these price/discount agreements?
    - Is the order date (or the posting date for the invoice and credit memo) within the starting and ending date of the price/discount agreement?
    - Is a unit of measure code specified? If so, [!INCLUDE[prod_short](includes/prod_short.md)] checks for prices/discounts with the same unit of measure code, and prices/discounts with no unit of measure code.

2. [!INCLUDE[prod_short](includes/prod_short.md)] checks if any price/discount agreements apply to information on the document or journal line, and then inserts the applicable unit price and line discount percentage, using the following criteria:

    - Is there a minimum quantity requirement in the price/discount agreement that is fulfilled?
    - Is there a currency requirement in the price/discount agreement that is fulfilled? If so, the lowest price and the highest line discount for that currency are inserted, even if local currency would provide a better price. If there is no price/discount agreement for the specified currency code, [!INCLUDE[prod_short](includes/prod_short.md)] inserts the lowest price and the highest line discount in your local currency.

If no special price can be calculated for the item on the line, then either the last direct cost or the unit price from the item card is inserted.

## <a name="see-related-training-at-microsoft-learn"></a>See Related Training at [Microsoft Learn](/learn/modules/manage-sales-prices-dynamics-365-business-central/index)

## <a name="see-also"></a>See Also

[Setting Up Sales](sales-setup-sales.md)  
[Sales](sales-manage-sales.md)  
[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]