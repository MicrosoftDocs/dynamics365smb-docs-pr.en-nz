---
title: About Setting Up Value-Added Tax | Microsoft Docs
description: Make sure that you correctly calculate, post, and report on GST for sales and purchases.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: VAT, posting, tax, value-added tax
ms.date: 07/21/2020
ms.author: bholtorf
ms.openlocfilehash: bbaf458e39ec45dcbcb34bd50e38feb70fd8426b
ms.sourcegitcommit: bdb6d18d512aa76d8d4f477d73ccfb284b0047fc
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 07/21/2020
ms.locfileid: "3611683"
---
# <a name="set-up-value-added-tax"></a>Set Up Value-Added Tax

Consumers and businesses pay value-added tax (VAT) when they purchase goods or services. The amount of GST to pay can vary, depending on several factors. In [!INCLUDE[d365fin](includes/d365fin_md.md)], you set up VAT to specify the rates to use to calculate tax amounts based on the following:

* Who you sell to  
* Who you buy from  
* What you sell  
* What you buy  

You can set up GST calculations manually, but that can be tricky and time consuming. To make it easy, we provide an assisted setup guide named **VAT Setup** that will help you with the steps. We recommend that you use the assisted setup guide to set up GST.

> [!NOTE]  
> You can use the guide only if you have created a My Company, and have not posted transactions that include GST. Otherwise, it would be very easy to use different GST rates by mistake, and make GST-related reports inaccurate.  

If you want to set up GST calculations yourself, or just want to learn about each step, this topic contains descriptions of each step.

## <a name="to-use-the-vat-setup-assisted-setup-guide-to-set-up-vat-recommended"></a>To use the GST Setup assisted setup guide to set up GST (recommended)

We recommend that you use the VAT Setup assisted setup guide to set up VAT in [!INCLUDE[d365fin](includes/d365fin_md.md)].

To start the assisted setup guide, follow these steps:

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Assisted Setup**.  
2. Choose **Set up GST** and complete the steps.
3. When you have completed the assisted setup, visit the **GST Posting Setup** page and check if you have to fill in additional fields according to the local requirements in your version pf [!INCLUDE [prodshort](includes/prodshort.md)]. For more information, see [Local functionality in Business Central](about-localization.md)  

## <a name="to-set-up-vat-registration-numbers-for-your-country-or-region"></a>To set up GST registration numbers for your country or region

To help ensure that people enter valid GST registration numbers, you can define formats for the GST registration numbers that are used in the countries or regions in which you do business. [!INCLUDE[d365fin](includes/d365fin_md.md)] will display an error message when someone makes a mistake or uses a format that is incorrect for the country or region.

To setup GST registration numbers, follow these steps:

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Countries/Regions**.
2. Choose the country or region, and then choose the **GST Reg. No. Formats** action.
3. In the **Formats** field, define the format by entering one or more of the following characters:  

* **#** Requires a single-digit number.  
* **@** Requires a letter. This is not case-sensitive.  
* **?** Allows any character.  

    > [!Tip]
    > You can use other characters as long as they are always present in the country or region format. For example, if you need to include a period or a hyphen between sets of numbers, you can define the format as ##.####.### or @@-###-###.  

## <a name="to-set-up-vat-business-posting-groups"></a>To set up VAT business posting groups
VAT business posting groups should represent the markets in which you do business with customers and vendors, and define how to calculate and post VAT in each market. Examples of VAT business posting groups are **Domestic** and **European Union (EU)**.  

Use codes that are easy to remember and describe the business posting group, such as **EU**, **Non-EU**, or **Domestic**. The code must be unique. You can set up as many codes as you need, but you cannot have the same code more than once in a table.

To set up a GST business posting group, follow these steps:

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **GST Business Posting Group**, and then choose the related link.  
2. Fill in the fields as necessary.

You set up default GST business posting groups by linking them to general business posting groups. [!INCLUDE[d365fin](includes/d365fin_md.md)] automatically assigns the VAT business posting group when you assign the business posting group to a customer, vendor, or general ledger account.

## <a name="to-set-up-vat-product-posting-groups"></a>To set up GST product posting groups
GST product posting groups represent the items and resources you buy or sell, and determine how to calculate and post GST according to the type of item or resource that is being bought or sold.  
It is a good idea to use codes that are easy to remember and describe the rate, such as **NO-VAT** or **Zero**, **VAT10** or **Reduced** for 10% VAT, and **VAT25** or **Standard** for 25%.

To set up a GST business posting group, follow these steps:

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **GST Product Posting Groups**, and then choose the related link.  
2. Fill in the fields as necessary.

## <a name="to-combine-vat-posting-groups-in-vat-posting-setups"></a>To combine GST posting groups in GST posting setups
[!INCLUDE[d365fin](includes/d365fin_md.md)] calculates VAT amounts on sales and purchases based on VAT posting setups, which are combinations of VAT business and product posting groups. For each combination, you can specify the GST percent, GST calculation type, and general ledger accounts for posting GST for sales, purchases, and reverse charges. You can also specify whether to recalculate GST when a payment discount is applied or received.  

Set up as many combinations as you need. If you want to group VAT posting setup combinations with similar attributes, you can define a **VAT Identifier** for each group, and assign the identifier to the group members.

To combine GST posting setups, follow these steps:

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **GST Posting Setup**, and then choose the related link.
2. Fill in the fields as necessary.

## <a name="to-assign-vat-posting-groups-by-default-to-multiple-entities"></a>To assign GST posting groups by default to multiple entities
If you want to apply the same VAT posting groups to multiple entities, you can set up [!INCLUDE[d365fin](includes/d365fin_md.md)] to do so by default. There are a couple of ways to do this:

* You can assign GST business posting groups to general business posting groups, or customer or vendor templates
* You can assign GST product posting groups on general product posting groups  

The GST business or product posting group is assigned when you choose a business or product posting group for a customer, vendor, item, or resource.

## <a name="assigning-vat-posting-groups-to-accounts-customers-vendors-items-and-resources"></a>Assigning GST Posting Groups to Accounts, Customers, Vendors, Items, and Resources
The following sections describe how to assign GST posting groups to individual entities.

### <a name="to-assign-vat-posting-groups-to-individual-general-ledger-accounts"></a>To assign GST posting groups to individual general ledger accounts
1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Chart of Accounts**, and then choose the related link.  
2. Open the **G/L Account** card for the account.  
3. On the **Posting** FastTab, in the **Gen. Posting Type** field, choose either **Sale** or **Purchase**.  
5. Choose the GST posting groups to use for the sales or purchase account.  

### <a name="to-assign-vat-business-posting-groups-to-customers-and-vendors"></a>To assign GST business posting groups to customers and vendors  
1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Customer** or **Vendor**, and then choose the related link.  
2. On the **Customer** or **Vendor** card, expand the **Invoicing** FastTab.  
3. Choose the GST business posting group.  

### <a name="to-assign-vat-product-posting-groups-to-individual-items-and-resources"></a>To assign GST product posting groups to individual items and resources  
1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Item** or **Resource**, and then choose the related link.  
2. Do one of the following:  

* On the **Item** card, expand the **Price & Posting** FastTab, and then choose **Show more** to display the **VAT Product Posting Group** field.  
* On the **Resource** card, expand the **Invoicing** FastTab.  
3. Choose the GST product posting group.  

## <a name="setting-up-clauses-to-explain-vat-exemption-or-non-standard-vat-rates"></a>Setting Up Clauses to Explain GST Exemption or Non-Standard GST Rates
You set up a GST clause to describe information about the type of GST that is being applied. The information may be required by government regulation. After you set up a GST clause, and associate it with a GST posting setup, the GST clause is displayed on printed sales documents that use the GST posting setup group.

If needed, you can also specify how to translate GST clauses to other languages. Then, when you create and print a sales document that contains a GST identifier, the document will include the translated GST clause. The language code specified on the customer card determines the language.

When non-standard GST rates are used in different types of documents, such as invoices or credit memos, companies are usually required to include an exemption text (GST clause) stating why a reduced GST or zero GST rate has been calculated. You can define different GST clauses to be included on business documents per the type of document, such as invoice or credit memo. You do this on the **GST Clauses by Doc. Type** page.

You can modify or delete a GST clause, and your modifications will be reflected in a generated report. However, [!INCLUDE[d365fin](includes/d365fin_md.md)] does not keep a history of the change. On the report, the GST clause descriptions are printed and displayed for all lines in the report alongside the GST amount and the GST base amount. If a GST clause has not been defined for any lines on the sales document, then the whole section is omitted when the report is printed.

### <a name="to-set-up-vat-clauses"></a>To set up GST clauses
1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **GST Clauses**, and then choose the related link.  
2. On the **VAT Clauses** page, create a new line.  
3. In the **Code** field, enter an identifier for the clause. You use this code to assign the clause to GST posting groups.  
4. In the **Description** field, enter the GST exemption text that you want to display on documents that can include GST. In the **Description 2** field, enter additional text, if needed. The text will be displayed on new document lines.
5. Choose the **Description by Document Type** action.
6. On the **GST Clauses by Doc. Type** page, fill in the fields to set up which GST exemption text to display for which document type.  
7. Optional: To assign the GST clause to a GST posting setup right away, choose **Setup**, and then choose the clause. If you want to wait, you can assign the clause later on the **GST Posting Setup** page.  
8. Optional: To specify how to translate the VAT clause, choose the **Translations** action.

### <a name="to-assign-a-vat-clause-to-a-vat-posting-setup"></a>To assign a GST clause to a GST posting setup
1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **GST Posting Setup**, and then choose the related link.  
2. In the **VAT Clause** column, choose the clause to use for each VAT posting setup it applies to.  

### <a name="to-specify-translations-for-vat-clauses"></a>To specify translations for GST clauses
1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **GST Clauses**, and then choose the related link.  
2. Choose the **Translations** action.  
3. In the **Language Code** field, choose the language you are translating to.  
4. In the **Description** and **Description 2** fields, enter the translations of the descriptions. This text displays in the translated GST report documents.  

## <a name="to-create-a-vat-posting-setup-to-handle-import-vat"></a>To create a GST posting setup to handle Import GST
You use the Import GST feature when you need to post a document where the entire amount is GST. You will use this if you receive an invoice from the tax authorities for GST for imported goods.  

To set up codes for import GST, follow these steps:  
1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **GST Product Posting Groups**, and then choose the related link.  
2. On the GST Product Posting Groups page, set up a new GST product posting group for import GST.  
3. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **GST Posting Setup**, and then choose the related link.  
4. On the GST Posting Setup page, create a new line, or use an existing GST business posting groups in combination with the new GST product posting group for import GST.  
5. In the **VAT Calculation Type** field, choose **Full VAT**.  
6. In the **Purchase VAT Account** field, enter the general ledger account to use for posting import VAT. All other accounts are optional.  


## <a name="using-reverse-charge-vat-for-trade-between-eu-countries-or-regions"></a>Using Reverse Charge GST for Trade between EU Countries or Regions
Some companies must use reverse charge GST when trading with other companies. For example this rule applies to purchases from EU countries/regions and sales to EU countries/regions.  

> [!NOTE]  
> This rule applies when trading with companies that are registered as GST liable in another EU country/region. If you do business directly with consumers in other EU countries/regions, then you should contact your tax authority for applicable GST rules.  

> [!TIP]  
> You can verify that a company is registered as VAT liable in another EU country by using the EU VAT Registration Number Validation service. The service is available for free in [!INCLUDE[d365fin](includes/d365fin_md.md)]. For more information, see the section titled _Verify VAT registration numbers_ in this topic.

### <a name="sales-to-eu-countries-or-regions"></a>Sales to EU Countries or Regions
GST is not calculated on sales to GST-liable companies in other EU countries/regions. You must report the value of these sales to EU countries/regions separately on your GST statement.  

To correctly calculate GST on sales to EU countries/regions, you should:  

* Set up a line for sales with the same information for purchases. If you have already set up lines on the GST Posting Setup page for purchases from EU countries/regions, then you can also use these lines for sales.  
* Assign the GST business posting groups in the **GST Bus. Posting Group** field on the **Invoicing** FastTab of the customer card of each EU customer. You should also enter the customer's GST Registration Number in the **GST Registration No.** field on the **Foreign Trade** FastTab.  

When you post a sale to a customer in another EU country/region, the GST amount is calculated, and a GST entry is created by using the information about the reverse charge GST and the GST base, which is the amount that is used to calculate the GST amount. No entries are posted to the GST accounts in the general ledger.

## <a name="understanding-vat-rounding-for-documents"></a>Understanding GST Rounding for Documents
Amounts in documents that are not yet posted are rounded and displayed to correspond with the final rounding of amounts that are actually posted. GST is calculated for a complete document, which means that GST is calculated based on the sum of all lines with the same GST identifier in the document.




## <a name="see-also"></a>See Also
[Setting up GST Statement Templates and GST Statement Names](finance-how-setup-vat-statement.md)   
[Setting Up Unrealised Goods and Services Tax](finance-setup-unrealized-vat.md)      
[Report GST to a Tax Authority](finance-how-report-vat.md)      
[Work with GST on Sales and Purchases](finance-work-with-vat.md)    
[Work with the VAT Rate Change Tool](finance-how-use-vat-rate-change-tool.md)    
[Verify VAT Registration numbers](finance-how-validate-vat-registration-number.md)  
[Local functionality in Business Central](about-localization.md)  

## <a name="see-related-training-at-microsoft-learn"></a>See Related Training at [Microsoft Learn](/learn/paths/process-vat-dynamics-365-business-central/)
