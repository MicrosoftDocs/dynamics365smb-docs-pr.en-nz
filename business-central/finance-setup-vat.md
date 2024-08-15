---
title: Set up value-added tax
description: 'Make sure that you correctly calculate, post, and report on GST for sales and purchases. We recommend that you use the assisted setup guide to set up GST.'
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bholtorf
ms.topic: conceptual
ms.search.keywords: 'VAT, posting, tax, value-added tax'
ms.search.form: '10, 118, 391, 470, 471, 472, 575, 734, 747, 748, 1877,'
ms.date: 05/24/2024
ms.service: dynamics-365-business-central
ms.custom: bap-template
---

# <a name="set-up-calculations-and-posting-methods-for-value-added-tax"></a>Set up calculations and posting methods for goods and services tax

Consumers and businesses pay goods and services tax (GST) when they purchase goods or services. The amount of GST to pay can vary, depending on several factors. In [!INCLUDE[prod_short](includes/prod_short.md)], you set up GST to specify the rates used to calculate tax amounts based on the following parameters:

* Who you sell to  
* Who you buy from  
* What you sell  
* What you buy  

You can set up GST calculations manually, but that can be tricky and time-consuming. It's easy to use different GST rates by mistake and create inaccurate GST-related reports. To make GST set up easier, we recommend you use the **GST Setup** assisted setup guide.

However, if you want to set up the GST calculations yourself, or just want to learn about each step, this article contains descriptions of each step.  

[!INCLUDE [finance-vat](includes/finance-vat.md)]

## <a name="set-up-vat-using-the-assisted-setup-guide-recommended"></a>Set up GST using the assisted setup guide (recommended)

> [!NOTE]
> You can use the **GST Setup** guide only if you have created a *My Company* and haven't posted transactions that include GST. To learn more about a My Company, go to [Create new companies in [!INCLUDE[prod_short](includes/prod_short.md)]](about-new-company.md).

To start the assisted setup guide, follow these steps:

1. Choose the ![Lightbulb that opens the Tell Me feature 1.](media/ui-search/search_small.png "Tell me what you want to do") icon and enter **Assisted Setup**. 
2. Choose **Set up Goods and Services Tax (GST)** and complete the steps.
3. After you complete the assisted setup, go to the **GST Posting Setup** page to check whether you need to fill in more fields according to the local requirements in your version of [!INCLUDE [prod_short](includes/prod_short.md)]. Learn more at [Local functionality in Business Central](about-localization.md).  

### <a name="check-the-vat-posting-setup"></a>Check the GST posting setup

To support your fast start, [!INCLUDE [prod_short](includes/prod_short.md)] notifies you of missing general ledger (G/L) accounts in posting groups or posting setups, such as on the **GST Posting Setup** page. You can turn this type of notification on or off using the **G/L Account is missing in posting group or setup** notification in the **My Notifications** page. Just go to the **My settings** page, and then choose the **Change when I receive notifications** link.  

If you choose the notification, [!INCLUDE [prod_short](includes/prod_short.md)] creates posting setups based on the posting groups in the document or journal you're currently working on.  

At this point, you can just fill in the missing G/L accounts. But, when you further refine your setup later, you might realise your initial setup is wrong. [!INCLUDE [prod_short](includes/prod_short.md)] doesn't allow you to delete a GST posting setup and general posting setup after they're used to create entries. To prevent people from mistakenly using a setup that's no longer relevant for new postings, you can use the **Blocked** field on the **General Posting Setup** page.

## <a name="set-up-a-default-vat-date-for-documents-and-journals"></a>Set up a default GST date for documents and journals

GST reporting in [!INCLUDE [prod_short](includes/prod_short.md)] is based on the **GST Date** to include GST entries on GST reports in a GST period. The GST date can be changed on all documents and journals, but you must specify a default value for GST date.

> [!NOTE]
> After posting the document or journal, the **GST Date** will appear on **GST Entries** and **G/L Entries** as well as on the posted document if exists.

To set up a default value for a GST date, follow these steps:

1. Choose the ![Lightbulb that opens the Tell Me feature 1.](media/ui-search/search_small.png "Tell me what you want to do") icon and enter **General Ledger Setup**, and then choose the related link.  
2. On the **General** FastTab, in the **Default GST Date** field, choose either **Posting Date** or **Document Date**.
3. Close the page.  

> [!NOTE]
> By default, the **Default GST Date** is the **Posting Date**.

### <a name="enable-or-disable-the-vat-date-feature"></a>Enabling or disabling the GST Date feature

Some countries/regions require that businesses use a specific VAT date, but other countries/regions don't. Some countries/regions also require businesses to change the GST date in specific situations after they post documents, but other countries/regions don't allow changes to GST dates. To allow for different contexts, you can choose whether you want to use this functionality and, if so, to what degree.

To set up the level of GST date usage, follow these steps:

1. Choose the ![Lightbulb that opens the Tell Me feature 1.](media/ui-search/search_small.png "Tell me what you want to do") icon and enter **General Ledger Setup**, and then choose the related link.  
2. On the **General** FastTab, in the **GST Date Usage** field, specify the degree to which you want to use the GST date feature. You can choose one of the following options:

   | Type | Description |
   |--------------------|-----------------------------------------|
   | **Use full GST Date functionality** | Everything related to **GST Date** works by default, giving you the maximum **GST Date** functionality. You can set up the date, change it in documents, report based on it, and modify the date after posting as long as the period isn't closed or protected with allowed dates for posting. |
   | **Use but do not allow modifications** | Everything related to **GST Date** works by default with one exception. You can't modify the **GST Date** in **GST Entries**. |
   | **Not using GST Date functionality** | [!INCLUDE [prod_short](includes/prod_short.md)] hides and makes the **GST Date** fields unavailable on documents, journals, and entries. The **Default GST Date** is configured as the **Posting Date**. |

3. Close the page.

> [!IMPORTANT]
> Even if you choose the **Not using GST Date functionality** option, [!INCLUDE [prod_short](includes/prod_short.md)] will use the **GST Date** in the background. Because the **Default GST Date** is configured as the **Posting Date**, and you can't change it in this case, you'll get the same experience as without this feature. **GST Date** fields will be removed from all pages, but this field will still exist in tables and reports will work based on it.

### <a name="limiting-periods-for-posting-and-changing-the-vat-date"></a>Limiting periods for posting and changing the GST date

You can prevent people from posting or changing GST entries in specific date ranges. You set the restriction using two settings:

* Based on closed **GST Return Period**
* Based on the **Allow Posting From** and **Allow Posting To** fields.

#### <a name="to-limit-posting-based-on-vat-return-period"></a>To limit posting based on GST return period

1. Choose the ![Lightbulb that opens the TellF Me feature 1.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **General Ledger Setup**, and then choose the related link.  
2. On the **General** FastTab, in the **Control GST Period** field, specify the degree of GST Return Period control. The following table describes the options.

| Type | Description |
|--------------------|-----------------------------------------|
| **Block posting within closed and warn for released period** | Prevent people from posting a document or journal, or changing GST entries that have a GST date within a closed **GST Return Period**. [!INCLUDE [prod_short](includes/prod_short.md)] also shows a warning if your **GST Return Period** is open, but the status of **GST Return** is **Released** or **Submitted**. |
| **Block posting within closed period** | Prevent people from posting a document or journal, or changing GST entries that have a GST date within the closed **GST Return Period**. |
| **Warn when posting in closed period** | Show a warning, but don't block posting, if you want to post a document or journal that has a GST date within a closed **GST Return Period**. |
| **Disabled** | Take no action based on a closed **GST Return Period**. |

#### <a name="limit-posting-based-on-allow-fromto-period"></a>Limit posting based on Allow from/to period

> [!NOTE]
> As of Business Central version 23.1, this control is changed. In earlier versions, there was only one control on the **General Ledger Setup** page for both Posting Date and GST Date. Now, these controls are split, so control in the **General Ledger Setup** page is for the **Posting Date** only and control in the **GST Setup** page is for the **GST Date** only. There are also new date controls in the **User Setup** page.  

##### <a name="version-231-or-newer"></a>Version 23.1 or newer

> [!IMPORTANT]
> When you upgrade to a newversion, be aware that values are upgraded in the new **Allow GST Date From/To** in the **GST Setup** page based on the values in **Allow Posting From/To** in the **General Ledger Setup**. If you want to use different date controls, open the **GST Setup** page and make changes.  

You can set up limitations on the company or at specific user levels.

To limit all postings for the whole company:

1. Select the ![Lightbulb that opens the Tell Me feature 1.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **GST Setup**, and then select the related link.  
2. On the **GST Date** FastTab, in the **Allow GST Date From** field, specify the GST date from which you allow posting. Posting a document or journal with a GST date before this date isn't allowed.  
3. On the **GST Date** FastTab, in the **Allow GST Date To** field, specify the GST date until which you allow posting. Posting a document or journal with a GST date after this date isn't allowed. 

To limit postings for the specific user:  

1. Select the ![Lightbulb that opens the Tell Me feature 1.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **User Setup**, and then select the related link.  
2. In the **User ID** field, specify the user allowed to post in a specific period.  
3. In the **Allow GST Date From** field, specify the GST date from which you allow posting. Posting a document or journal with a GST date before this date isn't allowed. 
4. In the **Allow GST Date To** field, specify the GST date until which you allow posting. Posting a document or journal with a GST date after this date isn't allowed.  

##### <a name="versions-before-231"></a>Versions before 23.1

You can set up limitation on the company or specific user levels.

To limit all postings for the whole company:

1. Choose the ![Lightbulb that opens the Tell Me feature 1.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **General Ledger Setup**, and then choose the related link.  
2. On the **General** FastTab, in the **Allow Posting From** field, specify the GST date from which you allow posting. Posting a document or journal with a GST date before this date isn't allowed.  
3. On the **General** FastTab, in the **Allow Posting To** field, specify the GST date until which you allow posting. Posting a document or journal with a GST date after this date isn't allowed.

To limit postings for the specific user:

1. Choose the ![Lightbulb that opens the Tell Me feature 1.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **User Setup**, and then choose the related link.  
2. In the **User ID** field, specify the user allowed to post in specific period.  
3. In the **Allow Posting From** field, specify the GST date from which you allow posting. Posting a document or journal with a GST date before this date isn't allowed.
4. In the **Allow Posting To** field, specify the GST date until which you allow posting. Posting a document or journal with a GST date after this date isn't allowed.

## <a name="set-up-vat-registration-numbers-for-your-countryregion"></a>Set up GST registration numbers for your country/region

To help ensure people enter valid GST registration numbers, you can define formats for the GST registration numbers that are used in the countries/regions in which you do business. [!INCLUDE[prod_short](includes/prod_short.md)] displays an error message if someone makes a mistake or uses a format that is incorrect for the country/region.

To set up GST registration numbers, follow these steps:

1. Choose the ![Lightbulb that opens the Tell Me feature 2.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Countries/Regions**.
2. Choose the country or region, and then choose the **GST Reg. No. Formats** action.
3. In the **Formats** field, define the format by entering one or more of the following characters:  

* **#** Requires a single-digit number.  
* **@** Requires a letter. This format isn't case-sensitive.  
* **?** Allows any character.  

    > [!TIP]
    > You can use other characters as long as they are always present in the country or region format. So, if you need to include a period or a hyphen between sets of numbers, you can define the format as ##.####.### or @@-###-###.  

## <a name="set-up-vat-business-posting-groups"></a>Set up GST business posting groups

GST business posting groups should represent the markets in which you do business with customers and vendors, and define how to calculate and post GST in each market. Examples of GST business posting groups are **Domestic** and **European Union (EU)**.  

Use codes that are easy to remember and describe the business posting group, such as **EU**, **Non-EU**, or **Domestic**. Each code must be unique, meaning you can set up as many codes as you need, but you can't have the same code more than once in a table.

To set up a GST business posting group, follow these steps:

1. Choose the ![Lightbulb that opens the Tell Me feature 3.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **GST Business Posting Groups**, and then choose the related link.  
2. Fill in the fields as necessary.

You can set up default GST business posting groups by linking them to general business posting groups. [!INCLUDE[prod_short](includes/prod_short.md)] automatically assigns the GST business posting group when you assign the business posting group to a customer, vendor, or general ledger account.

## <a name="set-up-vat-product-posting-groups"></a>Set up GST product posting groups

GST product posting groups represent the items and resources you buy or sell, and determine how to calculate and post GST according to the type of item or resource.

It's a good idea to use codes that are easy to remember and describe the rate, such as **NO-VAT** or **Zero**, **VAT10** or **Reduced** for 10 percent VAT, and **VAT25** or **Standard** for 25 percent.

To set up a GST business posting group, follow these steps:

1. Choose the ![Lightbulb that opens the Tell Me feature 4.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **GST Product Posting Groups**, and then choose the related link.  
2. Fill in the fields as necessary.

## <a name="combine-vat-posting-groups-in-vat-posting-setups"></a>Combine GST posting groups in GST posting setups

[!INCLUDE[prod_short](includes/prod_short.md)] calculates GST amounts on sales and purchases based on VAT posting setups, which are combinations of GST business and product posting groups. For each combination, you can specify the GST percent, GST calculation type, and general ledger accounts for posting GST for sales, purchases, and reverse charges. You can also specify whether to recalculate GST when a payment discount is applied or received.  

Set up as many combinations as you need. To group GST posting setup combinations with similar attributes, define a **GST Identifier** for each group, and assign the identifier to the group members.  

> [!NOTE]
> A **GST Identifier** is a code you can use to group similar attributes. We recommend you use different GST identifiers for different GST percentages.  

To combine GST posting setups, follow these steps:

1. Choose the ![Lightbulb that opens the Tell Me feature 5.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **GST Posting Setup**, and then choose the related link.
2. Fill in the fields as necessary. [!INCLUDE [tooltip-inline-tip_md](includes/tooltip-inline-tip_md.md)]

## <a name="assign-vat-posting-groups-by-default-to-multiple-entities"></a>Assign GST posting groups by default to multiple entities

If you want to apply the same GST posting groups to multiple entities, you can set up [!INCLUDE[prod_short](includes/prod_short.md)] to do so by default.

* You can assign GST business posting groups to general business posting groups, or customer or vendor templates.
* You can assign GST product posting groups on general product posting groups.  

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
2. Do one of the following steps:  

    * On the **Item** card, expand the **Price & Posting** FastTab, and then choose **Show more** to display the **GST Product Posting Group** field.  
    * On the **Resource** card, expand the **Invoicing** FastTab.  
3. Choose the GST product posting group.  

## <a name="set-up-clauses-to-explain-vat-exemption-or-nonstandard-vat-rates"></a>Set up clauses to explain GST exemption or nonstandard GST rates

You set up a GST clause to describe information about the type of GST that is being applied. Government regulations might require this information. After you set up a GST clause and associate it with a GST posting setup, the GST clause displays on printed sales documents that use the GST posting group setup.

If needed, you can also specify how to translate GST clauses to other languages. When you create and print a sales document that contains a GST identifier, the document includes the translated GST clause. The language code specified on the customer card determines the language.

When you use nonstandard GST rates in different types of documents, such as invoices or credit memos, you might have to include an exemption text (GST clause). The exemption text states why you calculated a reduced GST or zero GST rate. You can define different GST clauses to include on business documents for each type of document on the **GST Clauses by Document Type** page.

You can modify or delete a GST clause, and your modifications are reflected in a generated report. However, [!INCLUDE[prod_short](includes/prod_short.md)] doesn't keep a history of the change. On the report, the GST clause descriptions are printed and displayed for all lines in the report alongside the GST amount and the GST base amount. If a GST clause isn't defined for any lines on the sales document, the whole section is omitted when you print the report.

### <a name="to-set-up-vat-clauses"></a>To set up GST clauses

1. Choose the ![Lightbulb that opens the Tell Me feature 9.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **GST Clauses**, and then choose the related link.  
2. On the **GST Clauses** page, create a new line.  
3. In the **Code** field, enter an identifier for the clause. You use this code to assign the clause to GST posting groups.  
4. In the **Description** field, enter the GST exemption text that you want to display on documents that can include GST. In the **Description 2** field, enter more text, if needed. The text is displayed on new document lines.
5. Choose the **Description by document type** action.
6. On the **GST Clauses by Document Type** page, fill in the fields to set up which GST exemption text to display for which document type.  
7. Optional: To assign the GST clause to a GST posting setup right away, choose **Setup**, and then choose the clause. If you want to wait, you can assign the clause later on the **GST Posting Setup** page.  
8. Optional: To specify how to translate the GST clause, choose the **Translations** action.

### <a name="to-assign-a-vat-clause-to-a-vat-posting-setup"></a>To assign a GST clause to a GST posting setup

1. Choose the ![Lightbulb that opens the Tell Me feature 10.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **GST Posting Setup**, and then choose the related link.  
2. In the **GST Clause** column, choose the clause to use for each GST posting setup it applies to.  

### <a name="to-specify-translations-for-vat-clauses"></a>To specify translations for GST clauses

1. Choose the ![Lightbulb that opens the Tell Me feature 11.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **GST Clauses**, and then choose the related link.  
2. Choose the **Translations** action.  
3. In the **Language Code** field, choose the language you're translating to.  
4. In the **Description** and **Description 2** fields, enter the translations of the descriptions. This text displays in the translated GST report documents.  

### <a name="to-specify-extended-text-for-vat-clauses"></a>To specify extended text for GST clauses

> [!NOTE]  
> If your country or region requires longer text for the GST clauses than the default version supports, you can specify the longer text for the GST clauses as *extended text* so that it prints on the sales and purchase reports.  

1. Choose the ![Lightbulb that opens the Tell Me feature 11.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **GST Clauses**, and then choose the related link.  
2. Choose the **Extended Texts** action.  
3. Choose the **New** action.  
4. Fill in the **Language Code** and **Description** fields.  
5. Optionally, select the **All Language Codes** field, or specify the relevant language in the **Language Code** field if you use language codes.  
6. Fill in the **Starting Date** and **Ending Date** fields if you want to limit the dates on which the extended text is used.  
7. In the **Text** lines, write the extended text for your GST clauses.  
8. Select the relevant fields for the document types where you want the extended text printed.  
9. Close the page.  

## <a name="create-a-vat-posting-setup-to-handle-import-vat"></a>Create a GST posting setup to handle Import GST

Use the *Import GST* feature when you need to post a document where the entire amount is GST. You use this feature if you receive an invoice from the tax authorities for GST for imported goods.  

To set up codes for import GST, follow these steps:  

1. Choose the ![Lightbulb that opens the Tell Me feature 12.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **GST Product Posting Groups**, and then choose the related link.  
2. On the GST Product Posting Groups page, set up a new GST product posting group for import GST.  
3. Choose the ![Lightbulb that opens the Tell Me feature 13.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **GST Posting Setup**, and then choose the related link.  
4. On the GST Posting Setup page, create a new line, or use an existing GST business posting groups in combination with the new GST product posting group for import GST.  
5. In the **GST Calculation Type** field, choose **Full GST**.  
6. In the **Purchase GST Account** field, enter the general ledger account to use for posting import GST. All other accounts are optional.  

## <a name="use-reverse-charge-vat-for-trade-between-eu-countriesregions"></a>Use reverse charge GST for trade between EU countries/regions

Some companies must use reverse charge VAT when trading with other companies. For example, this rule applies to purchases from EU countries/regions and sales to EU countries/regions.  

> [!NOTE]  
> This rule applies when trading with companies that are registered as VAT liable in another EU country/region. If you do business directly with consumers in other EU countries/regions, then you should contact your tax authority for applicable GST rules.  

> [!TIP]  
> You can verify that a company is registered as VAT liable in another EU country/region by using the EU VAT Registration Number Validation service. The service is available for free in [!INCLUDE[prod_short](includes/prod_short.md)]. For more information, see [Verify VAT registration numbers](finance-how-validate-vat-registration-number.md).

### <a name="sales-to-eu-countriesregions"></a>Sales to EU countries/regions

VAT isn't calculated on sales to VAT-liable companies in other EU countries/regions. You must report the value of these sales to EU countries/regions separately on your GST statement.  

To correctly calculate GST on sales to EU countries/regions, you should:  

* Set up a line for sales with the same information for purchases. If you set up lines on the **GST Posting Setup** page for purchases from EU countries/regions, you can also use these lines for sales.  
* Assign the GST business posting groups in the **GST Bus. Posting Group** field on the **Invoicing** FastTab of the customer card of each EU customer. You should also enter the customer's VAT registration number in the **VAT Registration No.** field on the **Foreign Trade** FastTab.  

When you post a sale to a customer in another EU country/region, [!INCLUDE [prod_short](includes/prod_short.md)] calculates the GST amount and creates a GST entry based on information about the reverse charge GST and the GST base. This amount is used to calculate the GST amount. No entries are posted to the GST accounts in the general ledger.

If you want to use combination of GST business posting group and GST product posting group for reporting as services in the periodic GST reports, mark the **EU Service** field.

> [!NOTE]  
> The **EU Service** field is only applicable for GST reports. The field isn't related to the **Service Declaration** or **Intrastat for Services** features.

## <a name="vat-rounding-for-documents"></a>GST rounding for documents

Amounts in documents that aren't posted are rounded and displayed to correspond with the final rounding of amounts that are posted. [!INCLUDE [prod_short](includes/prod_short.md)] calculates GST for a complete document. The GST calculation is based on the sum of all lines with the same GST identifier in the document.  

## <a name="set-up-vat-reporting"></a>Set up GST reporting

You must set up information about how the tax authorities in your country or region require you to submit GST reports. The following steps illustrate the most commonly used information. However, your country or region might require other steps. For more information, see the relevant article in the *Local functionality* section in the panel to the left.

[!INCLUDE [vat-report-setup](includes/vat-report-setup.md)]

## <a name="see-also"></a>See also

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

[!INCLUDE[footer-include](includes/footer-banner.md)]
