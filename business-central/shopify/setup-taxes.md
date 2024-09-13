---
title: Set up taxes for Shopify connection
description: How to set up taxes in Shopify and Business Central.
ms.date: 05/29/2024
ms.topic: article
ms.service: dynamics-365-business-central
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bholtorf
ms.custom: bap-template
---

# Set up taxes for the Shopify connection

In this article, we'll investigate how various settings in Shopify affect the storefront prices and taxes that display to customers. We'll also cover how to configure [!INCLUDE[prod_short](../includes/prod_short.md)] to support the settings in Shopify. This article is not intended to be a comprehensive taxation guide. To learn more, contact your local tax authority or a tax professional.  

The article assumes that you are liable to pay taxes when you sell goods locally or internationally.

## If you sell domestically

After you configure your Shopify to collect taxes in your domestic country or region, you can decide how to display prices on your storefront.

You specify whether to include tax in prices by turning on or off the **All prices include tax** toggle in the [**Taxes and Duties**](https://www.shopify.com/admin/settings/taxes) settings in your **Shopify admin**.

The toggle is typically enabled for the following countries/regions:

* Australia
* Austria
* Belgium
* Czech Republic
* Denmark
* Finland
* France
* Germany
* Iceland
* Italy
* Netherlands
* New Zealand
* Norway
* Spain
* Sweden
* Switzerland
* United Kingdom

In markets such as these, a price of 100 EUR defined on the product card already contains goods and services tax (GST). The price, including VAT, is displayed to the customer in the storefront and at checkout.  

In the USA and Canada, customers don't expect to see prices with taxes because the final tax depends on where products ship to. Tax is added at checkout, so the **All prices include tax** toggle is usually turned off. In this case, a price of $100 defined on the product card is the price without tax. At checkout, taxes are added to the price.

To support the scenario where **All prices include tax** is selected, in [!INCLUDE[prod_short](../includes/prod_short.md)], fill in the following fields on the **Shopify shop card** page:  

1. Turn on the **Prices including GST** toggle.  
2. In the **GST Business Posting Group** field, specify the posting group you use for domestic customers.  

Now define item prices in the **Item Card** or **Sales Price List** fields, with or without tax. When exporting prices to Shopify, [!INCLUDE [prod_short](../includes/prod_short.md)] includes domestic taxes in the calculated price and shows that price for the product in Shopify.

> [!NOTE]
> These settings affect the export of prices. When you import orders from Shopify, the setting for the **Prices including VAT** field comes from the **Customer Template** on the Shopify shop card, or the customer template per country/region. Even if you use the default customer for imported orders, you must fill in the **Customer Template Code**.

## If you sell internationally

This section explores settings for scenarios where you're required to collect taxes when selling to another country/region, such as other countries/regions in the EU.

Currently, the Shopify connector only lets you export one price. Shopify automatically applies local taxes, currencies, and rounding. The **All prices include tax** toggle results in the actions described in the following subsections.

### All prices include tax is selected

|-|Domestic sales|Foreign country/region where you're collecting taxes|Foreign country/region where you're not collecting taxes|
|------------------------|--------|--------|--------|
|Price displayed in the storefront|1200|1200|1200|
|Tax rate percentage|2.0|25|0|
|Price at checkout|1200|1200|1200|

The price for the customer stays intact, regardless of their location, but your margin is affected due to differing tax rates per country/region.

### All prices include tax is not selected

|-|Domestic sales|Foreign country where you're collecting taxes|Foreign country where you're not collecting taxes|
|------------------------|--------|--------|--------|
|Price displayed in the storefront|1000|1000|1000|
|Tax rate percentage|2.0|25|0|
|Price at checkout|1200|1250|1000|

Shopify adds local taxes to the price defined on the product card based on where goods are shipped to.

## Dynamic tax-inclusive pricing

Countries/regions have different requirements for including tax in prices. If you want prices to automatically include tax, you can turn on [Dynamic tax-inclusive pricing](https://help.shopify.com/en/manual/markets/pricing/dynamic-tax-inclusive-pricing) in Shopify.

In your **Shopify admin**, select **Include or exclude tax based on your customer's country** in the **Other Markets - Preferences** section of the [**Markets**](https://www.shopify.com/admin/settings/markets) settings.  

> [!NOTE]
> This setting doesn't affect prices in domestic markets, which is controlled by the **All prices include tax** toggle.

### All prices include tax is selected

|-|Domestic sales|Foreign country/region where tax is included in price|Foreign country/region where tax is excluded|
|------------------------|---------------|---------------|--------|
|Price displayed in the storefront|1200|1250|1000|
|Tax rate percentage|2.0|25|10|
|Price at checkout|1200|1250|1100|

The price for each customer changes, depending on their location.

### All prices include tax is not selected

|-|Domestic sales|Foreign country/region where tax is included in price|Foreign country/region, where tax is excluded|
|------------------------|--------|--------|--------|
|Price displayed in the storefront|1000|1250|1000|
|Tax rate percentage|2.0|25|10|
|Price at checkout|1200|1250|1100|

> [!NOTE]
> The **All prices include tax** toggle doesn't change how prices display to international customers.

## If you sell to EU customers

Different EU countries/regions have different local tax rates. However, if you're located in the EU and sell to other EU countries/regions, you can use your local tax rate in some cases.  

In your **Shopify admin**, check the **Collect GST** checkbox in the **European Union** section of the [**Taxes and Duties**](https://www.shopify.com/admin/settings/taxes) settings.

|Collect VAT|VAT rate|
|-|-|
|Micro-business exemption|Use your domestic tax rate for all sales inside the EU|
|One-stop shop or specific country/region registration|Use the VAT rate of your customer's country/region|

### Collect VAT set to one-stop shop registration

In the following example, the **All prices include tax** toggle is turned on. The price on the product card is set to *1200*.

|-|Domestic sales|Foreign country/region|
|------------------------|--------|--------|
|Price displayed in the storefront|1200|1250|
|Tax rate percentage|2.0|25|
|Price at checkout|1200|1250|

Shopify uses the tax rate in the foreign country/region when it calculates final prices.

### Collect VAT set to micro-business exemption

In the following example, the **All prices include tax** toggle is turned on. The price on the product card is set to *1200*.

|-|Domestic sales|Foreign country/region with local tax rate of 25 percent.|
|------------------------|--------|--------|
|Price displayed in the storefront|1200|1200|
|Tax rate percentage|2.0|2.0|
|Price at checkout|1200|1200|

Shopify uses the domestic tax rate and ignores the tax rate in the foreign country/region when it calculates final prices.

## Importing Shopify orders sold to international customers

If you're collecting taxes from multiple countries/regions, you must define a specific country/regional setting in [!INCLUDE[prod_short](../includes/prod_short.md)]. There's a reason why this setting is required. When a sales document is created in [!INCLUDE[prod_short](../includes/prod_short.md)], [!INCLUDE [prod_short](../includes/prod_short.md)] calculates taxes instead of reusing the taxes imported from Shopify.

You specify country/region-specific settings on the **Shopify Customer Template** page. You can define the **Default Customer No.** or **Customer Template No.**. In either case, ensure the customer or template has the following fields filled in:

1. **General Business Posting Group** (used for foreign customers).
2. **VAT Business Posting Group** (used for foreign customers).
3. **Prices including VAT** (aligned with setting on the Shopify side):

* Choose **Yes** if **All prices include tax** is enabled and **Include or exclude tax based on your customer's country** is disabled.
* Choose **No** if **All prices include tax** is disabled and **Include or exclude tax based on your customer's country** is disabled.
* Choose **Yes** if **Include or exclude tax based on your customer's country** is enabled and the country or region is listed in the [Tax-inclusive countries/regions](https://help.shopify.com/en/manual/markets/pricing/dynamic-tax-inclusive-pricing#tax-inclusive-versus-tax-exclusive-countries-and-regions).
* Choose **No** if **Include or exclude tax based on your customer's country** is enabled and the country/region isn't listed in [Tax-inclusive countries/regions](https://help.shopify.com/en/manual/markets/pricing/dynamic-tax-inclusive-pricing#tax-inclusive-versus-tax-exclusive-countries-and-regions).

> [!NOTE]
> The setting of the **Prices including VAT** field comes from the template, not from the specific customer. It's important to define the customer template.

## Other tax remarks

While the imported Shopify order contains information about taxes, the taxes get recalculated when you create the sales document. That recalculation means it's important that GST/tax settings are correct in [!INCLUDE[prod_short](../includes/prod_short.md)].

* Multiple product tax or VAT rates. For example, some product categories are eligible for reduced tax rates. You can use the [tax override](https://help.shopify.com/en/manual/taxes/tax-overrides#create-a-manual-collection-for-products-that-need-a-tax-override) feature in Shopify. When you import and create items [!INCLUDE[prod_short](../includes/prod_short.md)], they use the tax setup specified on the item template code in the Shopify shop. Before you import orders with such items, update the GST product posting group.  
* Address-dependent tax rates. Use the **Tax Area Priority** field together with **Customer Templates** table to overwrite standard logic that fills in the **Tax Area Code** in the sales document. The **Tax Area Priority** field specifies the priority regarding where the function should take the information about the country or region and state or province. Then the corresponding record in the Shopify customer templates is identified, and the **Tax Area Code**, **Tax Liable**, and **VAT Bus. Posting Group** are used when a sales document is created.  

## See Also

[Get Started with the Connector for Shopify](get-started.md)  
