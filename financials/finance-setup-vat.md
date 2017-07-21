---
title: About Setting Up Value-Added Tax | Microsoft Docs
description: Make sure that you correctly calculate, post, and report on GST for sales and purchases.
services: project-madeira
documentationcenter: 
author: bholtorf
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: VAT, posting, tax, value-added tax
ms.date: 04/20/2017
ms.author: bholtorf
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: ce397b4a492a727211b49d7db2a231bea40d8c43
ms.contentlocale: en-nz
ms.lasthandoff: 07/07/2017


---

# <a name="setting-up-to-calculations-and-posting-methods-for-value-added-tax"></a>Setting Up to Calculations and Posting Methods for Value-Added Tax
Consumers and businesses pay value-added tax (VAT) when they purchase goods or services. The amount of GST to pay can vary, depending on several factors. In [!INCLUDE[d365fin](includes/d365fin_md.md)], you set up VAT to specify the rates to use to calculate tax amounts based on the following: 

* Who you sell to  
* Who you buy from  
* What you sell  
* What you buy  
  
You can set up GST calculations manually, but that can be tricky and time consuming. To make it easy, we provide an assisted setup guide named **VAT Setup** that will help you with the steps. We recommend that you use the assisted setup guide to set up GST.

> [!NOTE]  
>   You can use the guide only if you have created a My Company, and have not posted transactions that include GST. Otherwise, it would be very easy to use different GST rates by mistake, and make GST-related reports inaccurate.  
  
If you want to set up GST calculations yourself, or just want to learn about each step, this topic contains descriptions of each step. These include how to:  
  
* Set up GST business posting groups to define GST rates for the markets you do business in. You assign these to customers and vendors.  
* Set up GST product posting groups to define GST rates for the products and services you buy or sell.  
  
   > [!NOTE]  
>   The concepts behind GST business and product posting groups are similar to general posting groups. For more information, see [Posting Group Setups](finance-posting-groups.md).
* Combine GST business and product posting groups to create GST setups that calculate GST amounts on sales and purchases.  
* Assign GST product posting groups to the general ledger accounts you use for sales and purchases, and items, and resources.  

   > [!NOTE]  
>   To set up VAT for resources, you must enable the **Suite** user experience for your company. For more information, see [Customizing Your Dynamics 365 for Financials Experience](ui-experiences.md).
* Use reverse charge GST for trade between EU countries/regions  
* Understand GST rounding for documents  
* Set up clauses to explain the use of non-standard GST rates
* Verify VAT registration numbers

## <a name="use-the-vat-setup-assisted-setup-guide-to-set-up-vat-recommended"></a>Use the GST Setup assisted setup guide to set up GST (recommended)
We recommend that you use the VAT Setup assisted setup guide to set up VAT in [!INCLUDE[d365fin](includes/d365fin_md.md)]. 

To start the assisted setup guide, follow these steps:
1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Assisted Setup**.  
2. Choose **VAT Setup**.

## <a name="set-up-vat-business-posting-groups"></a>Set up GST business posting groups
GST business posting groups should represent the markets in which you do business with customers and vendors, and define how to calculate and post GST in each market. Examples of VAT business posting groups are **Domestic** and **European Union (EU)**.  

Use codes that are easy to remember and describe the business posting group, such as **EU**, **Non-EU**, or **Domestic**. The code must be unique. You can set up as many codes as you need, but you cannot have the same code more than once in a table.
  
To set up a GST business posting group, follow these steps:

1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **VAT Business Posting Group**, and then choose the related link.  
2. Fill in the fields as necessary.

You set up default GST business posting groups by linking them to general business posting groups. [!INCLUDE[d365fin](includes/d365fin_md.md)] automatically assigns the VAT business posting group when you assign the business posting group to a customer, vendor, or general ledger account. 

## <a name="set-up-vat-product-posting-groups"></a>Set up GST product posting groups
GST product posting groups represent the items and resources you buy or sell, and determine how to calculate and post GST according to the type of item or resource that is being bought or sold.  
It is a good idea to use codes that are easy to remember and describe the rate, such as **NO-VAT** or **Zero**, **VAT10** or **Reduced** for 10% VAT, and **VAT25** or **Standard** for 25%.

To set up a GST business posting group, follow these steps:

1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **VAT Product Posting Groups**, and then choose the related link.  
2. Fill in the fields as necessary.

## <a name="combine-vat-posting-groups-in-vat-posting-setups"></a>Combine GST posting groups in GST posting setups
[!INCLUDE[d365fin](includes/d365fin_md.md)] calculates VAT amounts on sales and purchases based on VAT posting setups, which are combinations of VAT business and product posting groups. For each combination, you can specify the GST percent, GST calculation type, and general ledger accounts for posting GST for sales, purchases, and reverse charges. You can also specify whether to recalculate GST when a payment discount is applied or received.  

Set up as many combinations as you need. If you want to group VAT posting setup combinations with similar attributes, you can define a **VAT Identifier** for each group, and assign the identifier to the group members.

To combine GST posting setups, follow these steps:

1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **VAT Posting Setup**, and then choose the related link.
2. Fill in the fields as necessary.

## <a name="assign-vat-posting-groups-by-default-to-multiple-entities"></a>Assign GST posting groups by default to multiple entities
If you want to apply the same VAT posting groups to multiple entities, you can set up [!INCLUDE[d365fin](includes/d365fin_md.md)] to do so by default. There are a couple of ways to do this:

* You can assign GST business posting groups to general business posting groups, or customer or vendor templates 
* You can assign GST product posting groups on general product posting groups  

The GST business or product posting group is assigned when you choose a business or product posting group for a customer, vendor, item, or resource.

## <a name="assign-vat-posting-groups-to-individual-accounts-customers-vendors-items-and-resources"></a>Assign GST posting groups to individual accounts, customers, vendors, items, and resources
The following sections describe how to assign GST posting groups to individual entities.

### <a name="to-assign-vat-posting-groups-to-individual-general-ledger-accounts"></a>To assign GST posting groups to individual general ledger accounts 
1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Chart of Accounts**, and then choose the related link.  
2. Open the **G/L Account** card for the account.
3. On the **Posting** FastTab, in the **Gen. Posting Type** field, choose either **Sale** or **Purchase**.  
5. Choose the GST posting groups to use for the sales or purchase account.  

### <a name="to-assign-vat-business-posting-groups-to-customers-and-vendors"></a>To assign GST business posting groups to customers and vendors  
1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Customer** or **Vendor**, and then choose the related link.  
2. On the **Customer** or **Vendor** card, expand the **Invoicing** FastTab.  
3. Choose the GST business posting group.  

### <a name="to-assign-vat-product-posting-groups-to-individual-items-and-resources"></a>To assign GST product posting groups to individual items and resources  
1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Item** or **Resource**, and then choose the related link.  
2. Do one of the following:
* On the **Item** card, expand the **Price & Posting** FastTab, and then choose **Show more** to display the **VAT Product Posting Group** field.  
* On the **Resource** card, expand the **Invoicing** FastTab.  
3. Choose the GST product posting group.

## <a name="set-up-clauses-to-explain-the-use-of-non-standard-vat-rates"></a>Set up clauses to explain the use of non-standard GST rates
You set up a GST clause to describe information about the type of GST that is being applied. The information may be required by government regulation. After you set up a GST clause, and associate it with a GST posting setup, the GST clause is displayed on printed sales documents that use the GST posting setup group. 

If needed, you can also specify how to translate GST clauses to other languages. Then, when you create and print a sales document that contains a GST identifier, the document will include the translated GST clause. The language code specified on the Customer card determines the language.
  
### <a name="to-set-up-vat-clauses"></a>To set up GST clauses
1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **VAT Clauses**, and then choose the related link.  
2. On the **VAT Clauses** page, create a new line.  
3. In the **Code** field, enter an identifier for the clause. You use this code to assign the clause to GST posting groups.  
4. In the **Description** field, enter the text that you want to display on documents that can include VAT. In the **Description 2** field, enter additional text, if needed. The text displays on new lines.  
5. Optional: To assign the VAT clause to a VAT posting setup right away, choose **Setup**, and then choosing the clause. If you want to wait, you can assign the clause later on the GST Posting Setup page.  
6. Optional: To specify how to translate the VAT clause, choose the **Translations** action.

### <a name="to-assign-a-vat-clause-to-a-vat-posting-setup"></a>To assign a GST clause to a GST posting setup
1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **VAT Posting Setup**, and then choose the related link.  
2. In the **VAT Clause** column, choose the clause to use for each VAT posting setup it applies to.  

### <a name="to-specify-translations-for-vat-clauses"></a>To specify translations for GST clauses
1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **VAT Clauses**, and then choose the related link.  
2. Choose the **Translations** action.  
3. In the **Language Code** field, choose the language you are translating to.  
4. In the **Description** and **Description 2** fields, enter the translations of the descriptions. This text displays in the translated GST report documents.  
  
## <a name="create-a-vat-posting-setup-to-handle-import-vat"></a>Create a GST posting setup to handle Import GST
You use the Import GST feature when you need to post a document where the entire amount is GST. You will use this if you receive an invoice from the tax authorities for GST for imported goods.  
  
To set up codes for import GST, follow these steps:  
1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **VAT Product Posting Groups**, and then choose the related link.  
2. On the GST Product Posting Groups page, set up a new GST product posting group for import GST.  
3. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **VAT Posting Setup**, and then choose the related link.  
4. On the GST Posting Setup page, create a new line, or use an existing GST business posting groups in combination with the new GST product posting group for import GST.  
5. In the **VAT Calculation Type** field, choose **Full VAT**.  
6. In the **Purchase VAT Account** field, enter the general ledger account to use for posting import VAT. All other accounts are optional.  
  
## <a name="verify-vat-registration-numbers"></a>Verify VAT registration numbers
It is important that the VAT registration numbers you have for customers, vendors, and contacts are valid. For example, companies sometimes change their tax liability status, and in some countries tax authorities might ask you to provide reports, such as the EC Sales List report, that list the GST registration numbers you use when you do business. 
  
The European Commission provides the VIES VAT Number Validation service on its website, which is public and free. [!INCLUDE[d365fin](includes/d365fin_md.md)] can save you a step and let you use the VIES service to validate and track VAT numbers for customers, vendors, and contacts straight from the customer, vendor, and contact cards. The service in [!INCLUDE[d365fin](includes/d365fin_md.md)] is named **EU VAT Reg. No. Validation Service**. The service is available on the **Service Connections** page, and you can start using it right away. The service connection is free, and signup is not required.

When you use our service connection, we record a history of VAT numbers and verifications for each customer, vendor, or contact, in the **VAT Registration Log**, so you can easily track them. The log is specific to each customer. For example, the log is useful for proving that you have verified that the current GST number is correct. When you verify a VAT number, the **Request Identifier** column in the log will reflect that you have taken action. 

You can view the VAT Registration log on the Customer, Vendor, or Contact cards, on the **Invoicing** FastTab, by choosing the lookup button in the **VAT Registration No.** field.  

Our service can also save you time when you create a customer or vendor. If you know the customer's VAT number, you can enter it in the **VAT Registration No.** field on the Customer or Vendor cards, and we will fill out the customer name for you. Some countries also provide company addresses in a structured format. In those countries, we fill in the address too.  

> [!NOTE]  
> There are a couple of things to note about the VIES VAT Number Validation service:

* The service uses the http protocol, which means that data transferred through the service is not encrypted.  
* You may experience downtime for this service for which Microsoft is not responsible. The service is part of a broad EU network of national VAT registers.

## <a name="using-reverse-charge-vat-for-trade-between-eu-countries-or-regions"></a>Using reverse charge VAT for trade between EU countries or regions
Some companies must use reverse charge GST when trading with other companies. For example this rule applies to purchases from EU countries/regions and sales to EU countries/regions.  
  
> [!NOTE]  
> This rule applies when trading with companies that are registered as GST liable in another EU country/region. If you do business directly with consumers in other EU countries/regions, then you should contact your tax authority for applicable GST rules.  
  
> [!TIP]  
> You can verify that a company is registered as VAT liable in another EU country by using the EU VAT Registration Number Validation service. The service is available for free in [!INCLUDE[d365fin](includes/d365fin_md.md)]. For more information, see the section titled _Verify VAT registration numbers_ in this topic.

### <a name="sales-to-eu-countries-or-regions"></a>Sales to EU countries or regions
GST is not calculated on sales to GST-liable companies in other EU countries/regions. You must report the value of these sales to EU countries/regions separately on your GST statement.  

To correctly calculate GST on sales to EU countries/regions, you should:  
  
* Set up a line for sales with the same information for purchases. If you have already set up lines on the GST Posting Setup page for purchases from EU countries/regions, then you can also use these lines for sales.  
* Assign the GST business posting groups in the **GST Bus. Posting Group** field on the **Invoicing** FastTab of the customer card of each EU customer. You should also enter the customer's VAT registration number in the **VAT Registration No.** field on the **Foreign Trade** FastTab.  

When you post a sale to a customer in another EU country/region, the GST amount is calculated, and a GST entry is created by using the information about the reverse charge GST and the GST base, which is the amount that is used to calculate the GST amount. No entries are posted to the GST accounts in the general ledger.

## <a name="understanding-vat-rounding-for-documents"></a>Understanding GST rounding for documents
Amounts in documents that are not yet posted are rounded and displayed to correspond with the final rounding of amounts that are actually posted. GST is calculated for a complete document, which means that GST is calculated based on the sum of all lines with the same GST identifier in the document.

## <a name="see-also"></a>See Also  
[Setting Up Unrealized Value Added Tax](finance-setup-unrealized-vat.md)
