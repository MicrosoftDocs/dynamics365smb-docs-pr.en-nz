---
title: Set Up Goods and Services Tax
description: Make sure that you correctly calculate, post, and report on GST for sales and purchases. We recommend that you use the assisted setup guide to set up GST.
author: brentholtorf
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: VAT, posting, tax, value-added tax
ms.search.form: 10, 1877, 470, 471, 472
ms.date: 07/08/2022
ms.author: bholtorf
ms.openlocfilehash: 60943e508e382bbbaa46d92a102a96ad70fed432
ms.sourcegitcommit: f1e272485a0e675d337a694aba3e35a5daf43920
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 07/09/2022
ms.locfileid: "9130135"
---
# <a name="set-up-calculations-and-posting-methods-for-value-added-tax"></a>Set Up Calculations and Posting Methods for Goods and Services Tax

Consumers and businesses pay goods and services tax (GST) when they purchase goods or services. The amount of GST to pay can vary, depending on several factors. In [!INCLUDE[prod_short](includes/prod_short.md)], you set up GST to specify the rates to use to calculate tax amounts based on the following parameters:

* Who you sell to  
* Who you buy from  
* What you sell  
* What you buy  

You can set up GST calculations manually, but that can be tricky and time consuming. To make it easy, we provide an assisted setup guide named **GST Setup** that will help you with the steps. We recommend that you use the assisted setup guide to set up GST.

> [!NOTE]  
> You can use the guide only if you have created a My Company, and have not posted transactions that include GST. Otherwise, it would be very easy to use different GST rates by mistake, and make GST-related reports inaccurate.  

If you want to set up GST calculations yourself, or just want to learn about each step, this article contains descriptions of each step.  

[!INCLUDE [finance-vat](includes/finance-vat.md)]

## <a name="use-the-vat-setup-assisted-setup-guide-to-set-up-vat-recommended"></a>Use the GST Setup assisted setup guide to set up GST (recommended)

We recommend that you use the GST Setup assisted setup guide to set up GST in [!INCLUDE[prod_short](includes/prod_short.md)].

To start the assisted setup guide, follow these steps:

1. Choose the ![Lightbulb that opens the Tell Me feature 1.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Assisted Setup**.  
2. Choose **Set up GST** and complete the steps.
3. When you have completed the assisted setup, visit the **GST Posting Setup** page and check if you have to fill in more fields according to the local requirements in your version of [!INCLUDE [prod_short](includes/prod_short.md)]. For more information, see [Local functionality in Business Central](about-localization.md)  

### <a name="check-the-vat-posting-setup"></a>Check the GST posting setup

To support you in getting started fast, [!INCLUDE [prod_short](includes/prod_short.md)] will show you notifications if you are missing general ledger (G/L) accounts in posting groups or posting setups, such as the **GST Posting Setup** page. You can switch this type of notification on or off using the *G/L accounts missing in posting group or setup* notification in the **My Notifications** page. Just go to the **My settings** page, and then choose the *Change when I receive notifications.* link.  

If you choose such a notification, [!INCLUDE [prod_short](includes/prod_short.md)] automatically creates those posting setups based on the posting groups in the document or journal you're currently working on.  

At this point, you might just fill in the missing G/L accounts. Then, later, when you further refine the setup, you might realise this setup was wrong. [!INCLUDE [prod_short](includes/prod_short.md)] does not allow the deletion of GST posting setup and general posting setup when there are entries created based on such configurations. Starting in 2022 release wave 1, you can use the **Blocked** field in the **GST Posting Setup** page to prevent users from mistakenly using a setup that is no longer relevant for new postings.

## <a name="set-up-vat-registration-numbers-for-your-country-or-region"></a>Set up GST registration numbers for your country or region

To help ensure that people enter valid GST registration numbers, you can define formats for the GST registration numbers that are used in the countries or regions in which you do business. [!INCLUDE[prod_short](includes/prod_short.md)] will display an error message when someone makes a mistake or uses a format that is incorrect for the country or region.

To set up GST registration numbers, follow these steps:

1. Choose the ![Lightbulb that opens the Tell Me feature 2.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Countries/Regions**.
2. Choose the country or region, and then choose the **GST Reg. No. Formats** action.
3. In the **Formats** field, define the format by entering one or more of the following characters:  

* **#** Requires a single-digit number.  
* **@** Requires a letter. This format is not case-sensitive.  
* **?** Allows any character.  

    > [!Tip]
    > You can use other characters as long as they are always present in the country or region format. For example, if you need to include a period or a hyphen between sets of numbers, you can define the format as ##.####.### or @@-###-###.  

## <a name="set-up-vat-business-posting-groups"></a>Set up GST business posting groups

GST business posting groups should represent the markets in which you do business with customers and vendors, and define how to calculate and post GST in each market. Examples of GST business posting groups are **Domestic** and **European Union (EU)**.  

Use codes that are easy to remember and describe the business posting group, such as **EU**, **Non-EU**, or **Domestic**. The code must be unique. You can set up as many codes as you need, but you cannot have the same code more than once in a table.

To set up a GST business posting group, follow these steps:

1. Choose the ![Lightbulb that opens the Tell Me feature 3.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **GST Business Posting Group**, and then choose the related link.  
2. Fill in the fields as necessary.

You set up default GST business posting groups by linking them to general business posting groups. [!INCLUDE[prod_short](includes/prod_short.md)] automatically assigns the GST business posting group when you assign the business posting group to a customer, vendor, or general ledger account.

## <a name="set-up-vat-product-posting-groups"></a>Set up GST product posting groups

GST product posting groups represent the items and resources you buy or sell, and determine how to calculate and post GST according to the type of item or resource that is being bought or sold.  
It is a good idea to use codes that are easy to remember and describe the rate, such as **NO-GST** or **Zero**, **GST10** or **Reduced** for 10% GST, and **GST25** or **Standard** for 25%.

To set up a GST business posting group, follow these steps:

1. Choose the ![Lightbulb that opens the Tell Me feature 4.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **GST Product Posting Groups**, and then choose the related link.  
2. Fill in the fields as necessary.

## <a name="combine-vat-posting-groups-in-vat-posting-setups"></a>Combine GST posting groups in GST posting setups

[!INCLUDE[prod_short](includes/prod_short.md)] calculates GST amounts on sales and purchases based on VAT posting setups, which are combinations of GST business and product posting groups. For each combination, you can specify the GST percent, GST calculation type, and general ledger accounts for posting GST for sales, purchases, and reverse charges. You can also specify whether to recalculate GST when a payment discount is applied or received.  

Set up as many combinations as you need. If you want to group GST posting setup combinations with similar attributes, you can define a **GST Identifier** for each group, and assign the identifier to the group members.

To combine GST posting setups, follow these steps:

1. Choose the ![Lightbulb that opens the Tell Me feature 5.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **GST Posting Setup**, and then choose the related link.
2. Fill in the fields as necessary. [!INCLUDE [tooltip-inline-tip_md](includes/tooltip-inline-tip_md.md)]

## <a name="assign-vat-posting-groups-by-default-to-multiple-entities"></a>Assign GST posting groups by default to multiple entities

If you want to apply the same GST posting groups to multiple entities, you can set up [!INCLUDE[prod_short](includes/prod_short.md)] to do so by default. There are a couple of ways to do this:

* You can assign GST business posting groups to general business posting groups, or customer or vendor templates
* You can assign GST product posting groups on general product posting groups  

The GST business or product posting group is assigned when you choose a business or product posting group for a customer, vendor, item, or resource.

## <a name="assign-vat-posting-groups-to-accounts-customers-vendors-items-and-resources"></a>Assign GST posting groups to accounts, customers, vendors, items, and resources

The following sections describe how to assign GST posting groups to individual entities.

### <a name="to-assign-vat-posting-groups-to-individual-general-ledger-accounts"></a>To assign GST posting groups to individual general ledger accounts

1. Choose the ![Lightbulb that opens the Tell Me feature 6.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Chart of Accounts**, and then choose the related link.  
2. Open the **G/L Account** card for the account.  
3. On the **Posting** FastTab, in the **Gen. Posting Type** field, choose either **Sale** or **Purchase**.  
4. Choose the GST posting groups to use for the sales or purchase account.  

### <a name="to-assign-vat-business-posting-groups-to-customers-and-vendors"></a>To assign GST business posting groups to customers and vendors

1. Choose the ![Lightbulb that opens the Tell Me feature 7.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Customer** or **Vendor**, and then choose the related link.  
2. On the **Customer** or **Vendor** card, expand the **Invoicing** FastTab.  
3. Choose the GST business posting group.  

### <a name="to-assign-vat-product-posting-groups-to-individual-items-and-resources"></a>To assign GST product posting groups to individual items and resources

1. Choose the ![Lightbulb that opens the Tell Me feature 8.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Item** or **Resource**, and then choose the related link.  
2. Do one of the following:  

    * On the **Item** card, expand the **Price & Posting** FastTab, and then choose **Show more** to display the **GST Product Posting Group** field.  
    * On the **Resource** card, expand the **Invoicing** FastTab.  
3. Choose the GST product posting group.  

## <a name="set-up-clauses-to-explain-vat-exemption-or-non-standard-vat-rates"></a>Set up clauses to explain GST exemption or non-standard GST rates

You set up a GST clause to describe information about the type of GST that is being applied. The information may be required by government regulation. After you set up a GST clause, and associate it with a GST posting setup, the GST clause is displayed on printed sales documents that use the GST posting setup group.

If needed, you can also specify how to translate GST clauses to other languages. Then, when you create and print a sales document that contains a GST identifier, the document will include the translated GST clause. The language code specified on the customer card determines the language.

When non-standard GST rates are used in different types of documents, such as invoices or credit memos, companies are usually required to include an exemption text (GST clause) stating why a reduced GST or zero GST rate has been calculated. You can define different GST clauses to be included on business documents per the type of document, such as invoice or credit memo. You do this on the **GST Clauses by Doc. Type** page.

You can modify or delete a GST clause, and your modifications will be reflected in a generated report. However, [!INCLUDE[prod_short](includes/prod_short.md)] does not keep a history of the change. On the report, the GST clause descriptions are printed and displayed for all lines in the report alongside the GST amount and the GST base amount. If a GST clause has not been defined for any lines on the sales document, then the whole section is omitted when the report is printed.

### <a name="to-set-up-vat-clauses"></a>To set up GST clauses

1. Choose the ![Lightbulb that opens the Tell Me feature 9.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **GST Clauses**, and then choose the related link.  
2. On the **GST Clauses** page, create a new line.  
3. In the **Code** field, enter an identifier for the clause. You use this code to assign the clause to GST posting groups.  
4. In the **Description** field, enter the GST exemption text that you want to display on documents that can include GST. In the **Description 2** field, enter more text, if needed. The text will be displayed on new document lines.
5. Choose the **Description by Document Type** action.
6. On the **GST Clauses by Doc. Type** page, fill in the fields to set up which GST exemption text to display for which document type.  
7. Optional: To assign the GST clause to a GST posting setup right away, choose **Setup**, and then choose the clause. If you want to wait, you can assign the clause later on the **GST Posting Setup** page.  
8. Optional: To specify how to translate the GST clause, choose the **Translations** action.

### <a name="to-assign-a-vat-clause-to-a-vat-posting-setup"></a>To assign a GST clause to a GST posting setup

1. Choose the ![Lightbulb that opens the Tell Me feature 10.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **GST Posting Setup**, and then choose the related link.  
2. In the **GST Clause** column, choose the clause to use for each GST posting setup it applies to.  

### <a name="to-specify-translations-for-vat-clauses"></a>To specify translations for GST clauses

1. Choose the ![Lightbulb that opens the Tell Me feature 11.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **GST Clauses**, and then choose the related link.  
2. Choose the **Translations** action.  
3. In the **Language Code** field, choose the language you are translating to.  
4. In the **Description** and **Description 2** fields, enter the translations of the descriptions. This text displays in the translated GST report documents.  

### <a name="to-specify-extended-text-for-vat-clauses"></a>To specify extended text for GST clauses

> [!NOTE]  
> If your country or region requires longer text for the GST clauses than the default version supports, you can specify the longer text for the GST clauses as *extended text* so that it prints on the sales and purchase reports.  

1. Choose the ![Lightbulb that opens the Tell Me feature 11.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **GST Clauses**, and then choose the related link.  
2. Choose the **Extended texts** action.  
3. Fill in the **Code** and **Description** fields.  
3. Choose the **New** action.  
4. Optionally, select the **All Language Codes** field, or specify the relevant language in the **Language Code** field if you use language codes.  
5. Fill in the **Starting Date** and **Ending Date** fields if you want to limit the dates on which the extended text is used.  
6. In the **Text** lines, write the extended text for your GST clauses.  
7. Select the relevant fields for the document types where you want the extended text printed.  
8. Close the page.  

## <a name="create-a-vat-posting-setup-to-handle-import-vat"></a>Create a GST posting setup to handle Import GST

You use the *Import GST* feature when you need to post a document where the entire amount is GST. You will use this if you receive an invoice from the tax authorities for GST for imported goods.  

To set up codes for import GST, follow these steps:  

1. Choose the ![Lightbulb that opens the Tell Me feature 12.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **GST Product Posting Groups**, and then choose the related link.  
2. On the GST Product Posting Groups page, set up a new GST product posting group for import GST.  
3. Choose the ![Lightbulb that opens the Tell Me feature 13.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **GST Posting Setup**, and then choose the related link.  
4. On the GST Posting Setup page, create a new line, or use an existing GST business posting groups in combination with the new GST product posting group for import GST.  
5. In the **GST Calculation Type** field, choose **Full GST**.  
6. In the **Purchase GST Account** field, enter the general ledger account to use for posting import GST. All other accounts are optional.  

## <a name="use-reverse-charge-vat-for-trade-between-eu-countries-or-regions"></a>Use reverse charge GST for trade between EU countries or regions

Some companies must use reverse charge VAT when trading with other companies. For example this rule applies to purchases from EU countries/regions and sales to EU countries/regions.  

> [!NOTE]  
> This rule applies when trading with companies that are registered as VAT liable in another EU country/region. If you do business directly with consumers in other EU countries/regions, then you should contact your tax authority for applicable GST rules.  

> [!TIP]  
> You can verify that a company is registered as VAT liable in another EU country by using the EU VAT Registration Number Validation service. The service is available for free in [!INCLUDE[prod_short](includes/prod_short.md)]. For more information, see [Verify VAT registration numbers](finance-how-validate-vat-registration-number.md).

### <a name="sales-to-eu-countries-or-regions"></a>Sales to EU countries or regions

GST is not calculated on sales to GST-liable companies in other EU countries/regions. You must report the value of these sales to EU countries/regions separately on your GST statement.  

To correctly calculate GST on sales to EU countries/regions, you should:  

* Set up a line for sales with the same information for purchases. If you have already set up lines on the GST Posting Setup page for purchases from EU countries/regions, then you can also use these lines for sales.  
* Assign the GST business posting groups in the **GST Bus. Posting Group** field on the **Invoicing** FastTab of the customer card of each EU customer. You should also enter the customer's VAT registration number in the **VAT Registration No.** field on the **Foreign Trade** FastTab.  

When you post a sale to a customer in another EU country/region, the GST amount is calculated, and a GST entry is created by using the information about the reverse charge GST and the GST base, which is the amount that is used to calculate the GST amount. No entries are posted to the GST accounts in the general ledger.

## <a name="vat-rounding-for-documents"></a>GST rounding for documents

Amounts in documents that are not yet posted are rounded and displayed to correspond with the final rounding of amounts that are actually posted. GST is calculated for a complete document, which means that GST is calculated based on the sum of all lines with the same GST identifier in the document.  

## <a name="set-up-vat-reporting"></a>Set up GST reporting

You must set up information about how the tax authorities in your country or region require you to submit GST reports. The following steps illustrate the most commonly used information. However, your country or region may require additional steps. For more information, see the relevant article in the *Local functionality* section in the panel to the left.

[!INCLUDE [vat-report-setup](includes/vat-report-setup.md)]

## <a name="see-also"></a>See Also

[Set Up GST Statement Templates and GST Statement Names](finance-how-setup-vat-statement.md)  
[Set Up Unrealised Goods and Services Tax](finance-setup-unrealized-vat.md)  
[Report GST to a Tax Authority](finance-how-report-vat.md)  
[Work with GST on Sales and Purchases](finance-work-with-vat.md)  
[Work with the GST Rate Change Tool](finance-how-use-vat-rate-change-tool.md)  
[Verify VAT registration numbers](finance-how-validate-vat-registration-number.md)  
[Local functionality in Business Central](about-localization.md)  
[VAT Reporting in the German version](LocalFunctionality/Germany/vat-reporting.md)  
[Belgian VAT](LocalFunctionality/Belgium/belgian-vat.md)  
[Italian VAT](LocalFunctionality/Italy/italian-vat.md)  
[Set Up Electronic VAT and ICP Declarations in the Dutch Version](LocalFunctionality/Netherlands/how-to-set-up-electronic-vat-and-icp-declarations.md)  
[VAT Reports in the Spanish Version](LocalFunctionality/Spain/vat-reports.md)  
[Set Up Goods and Services Tax Posting in the Australian Version](LocalFunctionality/Australia/how-to-set-up-goods-and-service-tax-posting.md)  
[VAT in the Czech Version](LocalFunctionality/Czech/finance-vat.md)  
[VAT Reporting in the Norwegian Version](LocalFunctionality/Norway/norwegian-vat-reporting.md)  
[Reporting Goods/Services Tax and Harmonized Sales Tax in Canada](LocalFunctionality/Canada/sales-tax-goods-services.md)  

## <a name="see-related-training-at-microsoft-learn"></a>See Related Training at [Microsoft Learn](/learn/paths/process-vat-dynamics-365-business-central/)


[!INCLUDE[footer-include](includes/footer-banner.md)]
