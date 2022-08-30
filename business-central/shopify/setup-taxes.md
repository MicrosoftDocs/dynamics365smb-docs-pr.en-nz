---
title: Set up taxes for Shopify connection
description: How to set up taxes in Shopify and Business Central.
ms.date: 05/27/2022
ms.topic: article
ms.service: dynamics365-business-central
author: AndreiPanko
ms.author: andreipa
ms.openlocfilehash: 0070d583752002cc34ebff74dee2906c289b7136
ms.sourcegitcommit: b353f06e0c91aa6e725d59600f90329774847ece
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 08/19/2022
ms.locfileid: "9317506"
---
# <a name="set-up-taxes-for-the-shopify-connection"></a>Set Up Taxes for the Shopify Connection

In this article, we'll investigate how various settings in Shopify impact the storefront prices and taxes that are displayed to the customer. We'll also look at how to configure [!INCLUDE[prod_short](../includes/prod_short.md)] to support the settings in Shopify. This article is not intended to be a comprehensive taxation guide. To learn more, contact your local tax authority or a tax professional.  

The article assumes that you are liable to pay taxes when selling goods locally or internationally.

## <a name="if-you-sell-domestically"></a>If you sell domestically 

Once you configure your Shopify to collect taxes in your domestic country or region, you can decide how you want to display prices on your storefront. You control this by enabling or disabling the **All prices include tax** toggle in the [**Taxes and Duties**](https://www.shopify.com/admin/settings/taxes) settings in your **Shopify admin**.

It is common to have this toggle enabled for such countries as Australia, Austria, Belgium, the Czech Republic, Denmark, Finland, France, Germany, Iceland, Italy, the Netherlands, New Zealand, Norway, Spain, Sweden, Switzerland, and the United Kingdom. In markets such as these, the price *100 EUR* defined in the product card already contains value-added tax (VAT) and that same price is displayed to the customer at storefront and at checkout.  

In the USA and Canada, customers expect to see product prices without taxes, which are added at checkout. So the **All prices include tax** field is usually not selected. In this case, the price *$100* defined in the product card represents the price without tax. At the checkout stage, taxes will be added on top of the price to tally the checkout total.

To support the scenario where **All prices include tax** is selected on the [!INCLUDE[prod_short](../includes/prod_short.md)] side, fill in the **Customer Template Code** field in the **Shopify shop card** page to access the template with following fields defined:  
<!--I changed that last part of the sentence above because it didn't track logically. Just wanted to let you know in case I introduced an inaccuracy.-->

1. **General Business Posting Group**, used for domestic customers.  
2. **VAT Business Posting Group**, used for domestic customers.  
3. **Prices including VAT** set to *yes*.  

Now define item prices in the **Item Card** or **Sales Price Lst** field, with or without tax. When exporting prices to Shopify, the system calculates the price to include domestic taxes then shows that price in the product card in Shopify.

> [!NOTE]
> If you configured the Shopify connector to create customers automatically, you may need more fields in your template, such as **Customer Posting Group**. If you use the default customer for imported orders, make sure the customer has the same fields populated. You still need to fill in the **Customer Template Code** as specified above, because the **Prices including tax**/**Prices including VAT** field in the created sales document doesn't depend on the customer, but on the **Customer Template** from the Shopify shop card or customer template per country.

## <a name="if-you-sell-internationally"></a>If you sell internationally

In this section, we'll explore settings for scenarios where you're required to collect taxes when selling to another country, such as other countries in the EU. 

Currently, the **Shopify connector** extension supports export of one price only. Shopify automatically applies local taxes, currencies, and rounding. The **All prices include tax** toggle results in the actions described in the following subsections.

### <a name="all-prices-include-tax-is-selected"></a>*All prices include tax* is selected

||Domestic sales|Foreign country where you're collecting taxes|Foreign country where you're not collecting taxes|
|------------------------|--------|--------|--------|
|Price displayed in the storefront|1200|1200|1200|
|Tax rate percentage|2.0|25|0|
|Price at checkout|1200|1200|1200|

Price for customer stays intact, regardless of their location, but your margin is affected due to tax rates differing per country.

### <a name="all-prices-include-tax-is-not-selected"></a>*All prices include tax* is not selected

||Domestic sales|Foreign country where you're collecting taxes|Foreign country where you're not collecting taxes|
|------------------------|--------|--------|--------|
|Price displayed in the storefront|1000|1000|1000|
|Tax rate percentage|2.0|25|0|
|Price at checkout|1200|1250|1000|

Shopify adds local taxes on top of the price defined on the product card based on where goods are shipped to.

## <a name="dynamic-tax-inclusive-pricing"></a>Dynamic tax-inclusive pricing

Because different countries have different requirements depending on if you're including tax in the shown price or not, you can switch on [dynamic tax-inclusive pricing](https://help.shopify.com/en/manual/markets/pricing/dynamic-tax-inclusive-pricing) in Shopify. This automates the tax inclusion function. 
<!--I added the last sentence to complete the thought. I hope that's okay.-->

Select **Include or exclude tax based on your customer's country** in the **Other Markets - Preferences** section of the [**Markets**](https://www.shopify.com/admin/settings/markets) settings in your **Shopify admin**.  

> [!NOTE]
> This setting doesn't affect the representation of prices in domestic markets, which is controlled by the **All prices include tax** toggle.

### <a name="all-prices-include-tax-is-selected"></a>*All prices include tax* is selected

||Domestic sales|Foreign country where tax is included in price|Foreign country where tax is excluded|
|------------------------|--------|--------|--------|
|Price displayed in the storefront|1200|1250|1000|
|Tax rate percentage|2.0|25|10|
|Price at checkout|1200|1250|1100|

The price for each customer changes depending on their location.

### <a name="all-prices-include-tax-is-not-selected"></a>*All prices include tax* is not selected

||Domestic sales|Foreign country where tax is included in price|Foreign country, where tax is excluded|
|------------------------|--------|--------|--------|
|Price displayed in the storefront|1000|1250|1000|
|Tax rate percentage|2.0|25|10|
|Price at checkout|1200|1250|1100|

> [!NOTE]
> The **All prices include tax** toggle doesn't change how prices are displayed to international customers.

## <a name="if-you-sell-to-eu-customers"></a>If you sell to EU customers

Different EU countries have different local tax rates. However, if you're located in the EU and sell to other EU countries, you can use your local tax rate in some cases.  

Check the **Collect VAT** box in the **European Union** section of the [**Taxes and Duties**](https://www.shopify.com/admin/settings/taxes) settings in your **Shopify admin**.

|Collect VAT|VAT rate|
|-|-|
|Micro-business exemption|Use your domestic tax rate for all sales inside the EU|
|One-stop shop or country-specific registration|Use the VAT rate of your customer's country|


### <a name="collect-vat-set-to-one-stop-shop-registration"></a>Collect VAT set to one-stop shop registration

In the following example, the **All prices include tax** toggle is enabled. The price on the product card is set to *1200*. 
        
|-|Domestic sales|Foreign country|
|------------------------|--------|--------|
|Price displayed in the storefront|1200|1250|
|Tax rate percentage|2.0|25|
|Price at checkout|1200|1250|       
        
### <a name="collect-vat-set-to-micro-business-exemption"></a>Collect VAT set to micro-business exemption

In the following example, the **All prices include tax** toggle is enabled. THe price on the product card is set to *1200*. 
        
|-|Domestic sales|Foreign country with local tax rate of 25 percent.|
|------------------------|--------|--------|
|Price displayed in the storefront|1200|1200|
|Tax rate percentage|2.0|2.0|
|Price at checkout|1200|1200|           
    
Shopify ignores the tax rate in the foreign country when calculating final prices and uses the domestic tax rate.

## <a name="importing-shopify-orders-sold-to-international-customers"></a>Importing Shopify orders sold to international customers

If you are collecting taxes from multiple countries, you most likely need to define a country-specific setting in [!INCLUDE[prod_short](../includes/prod_short.md)]. This is required because when a sales document gets created in [!INCLUDE[prod_short](../includes/prod_short.md)], the system calculates taxes instead of reusing ones imported from Shopify.

Country/region-specific settings are chosen in the **Shopify Customer Template** window.
<!--Should this be "window" or "page"? I haven't been seeing "window" is use elsewhere, but I don't know what the interface looks like for this action.--> There you can define **Default Customer No.** or **Customer Template No.**. In either case make sure the selected customer or template has the following fields defined:

1. **General Business Posting Group** (used for foreign customers).
2. **VAT Business Posting Group** (used for foreign customers).
3. **Prices including VAT** (aligned with setting on the Shopify side):
* Choose *Yes* if **All prices include tax** is enabled and **Include or exclude tax based on your customer's country** is disabled.
* Choose *No* if **All prices include tax** is disabled and **Include or exclude tax based on your customer's country** is disabled.
* Choose *Yes* if **Include or exclude tax based on your customer's country** is enabled and the country or region is listed in the [Tax-inclusive countries](https://help.shopify.com/en/manual/markets/pricing/dynamic-tax-inclusive-pricing#tax-inclusive-versus-tax-exclusive-countries-and-regions).
* Choose *No* if **Include or exclude tax based on your customer's country** is enabled and country/region is not listed in [Tax-inclusive countries](https://help.shopify.com/en/manual/markets/pricing/dynamic-tax-inclusive-pricing#tax-inclusive-versus-tax-exclusive-countries-and-regions).
<!--I changed "Set" to "Choose" since "Set" really isn't an instruction we use. if they're toggling, we then would say "Toggle" as in "Toggle *No* if...."-->
> 
[!Note]
> The setting of the **Prices including VAT** field comes from the template, not from the specific customer. That's why it's important to have the customer template defined.

## <a name="other-tax-remarks"></a>Other tax remarks

While the imported Shopify order contains information about taxes, the taxes get recalculated when you create the sales document. That recalculation means it's important the VAT/tax settings are correct in [!INCLUDE[prod_short](../includes/prod_short.md)].

- Multiple product tax or VAT rates. For example, some product categories are eligible for reduced tax rates. You can use the [tax override](https://help.shopify.com/en/manual/taxes/tax-overrides#create-a-manual-collection-for-products-that-need-a-tax-override) feature in Shopify. When items are imported and created in [!INCLUDE[prod_short](../includes/prod_short.md)], they use the tax setup as filled in on the item template code in the Shopify shop. Before importing orders with such items, you need to update the VAT product posting group.  

- Address-dependent tax rates. Use the **Tax Area Priority** field together with **Customer Templates** table to overwrite standard logic that fills in the **Tax Area Code** in the sales document. The **Tax Area Priority** field specifies the priority regarding where the function should take the information about the country or region and state or province. Then the corresponding record in the Shopify customer templates is identified, and the **Tax Area Code**, **Tax Liable**, and **VAT Bus. Posting Group** are used when a sales document is created.  

## <a name="see-also"></a>See Also

[Get Started with the Connector for Shopify](get-started.md)  
