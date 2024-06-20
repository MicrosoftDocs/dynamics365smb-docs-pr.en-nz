---
title: Set Up a GST Statement
description: This topic tells you how to set up a GST Statement Template and GST Statement Names to meet changing tax authority requirements.
author: brentholtorf
ms.topic: conceptual
ms.devlang: al
ms.search.keywords: 'VAT, posting, tax, value-added tax'
ms.search.form: '317, 318, 320, 474'
ms.date: 06/16/2021
ms.author: bholtorf
ms.service: dynamics-365-business-central
ms.reviewer: bholtorf
---
# Set Up GST Statement Templates and GST Statement Names

Tax authorities can, and do, change their requirements for posting GST. GST Statement templates and GST statement names can help you prepare for upcoming changes and make a smooth transition to the new requirements. You can use GST statement templates to setup different Reports when choosing to print the statement. Each GST Statement Template can have multiple GST Statement names which in turn define the calculations, and you can create a new GST statement name when requirements change. For example, one name might calculate GST for this year based on the current requirements, and another might calculate GST based on requirements for next year. Names are also a way to keep a history of GST statement formats, for example, so that you can look back to see how you calculated GST in previous years.

## To define a GST statement

GST statements let you calculate your GST settlement amount for a certain period, for example, a quarter.

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **GST Statements**, and then choose the related link.  
2. Choose the **Name** field, and then choose **New** on the **GST Statement Names** page.
3. Fill in the required fields. Usually you want to have a setting for each GST Bus. Posting Group / GST Prod. Posting Group combination. For Row numbers it does make sense to use equvalent numbers or codes as in your official GST Statement [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

> [!Tip]
> You can filter the information that the statement will include, depending on what you choose in the **Type** field. **Account Totalling** is useful when you want the GST from a specific account.
**GST Entry Totalling** gets GST from the accounts assigned to the selections in the **Gen. Posting Type**, **GST Bus. Posting Group**, and/or the **GST Prod. Posting Group** fields. **Row Totalling** lets you enter a value or quick filter criteria in the **Row Totalling** field. For more information, see [Searching, filtering, and Sorting Data](ui-enter-criteria-filters.md). **Description** is often used to add a note to the statement. For example, you could use it as a heading when you've used row totalling.

## To preview the GST statement

After you define a GST statement, you can preview it to make sure it meets your needs.
> [!Tip]
> It is best practice to have one section in the VAT Statement using **Type** **GST Entry Totalling** and another section below using **Type** **Account Totalling** to reconcile the amounts based on the **GST Entry** table compared to the amount on the **G/L Accounts**. You can also use the **G/L - GST Reconciliation** Report for this purpose.

1. Choose **Preview**.
2. Enter a date filter to limit the statement to a specific period. For more information about how to customise the page to show the date filter, see [Searching, filtering, and Sorting Data](ui-enter-criteria-filters.md).
3. You can select various options to specify the type of GST entries to include in the statement.
4. On the lines where the **Type** field contains **GST Entry Totalling** you can see a list of GST entries by choosing the amount in the **Column Amount** field.
5. You can use personalisation to show more fields in the lines. For example the Unrealised Base Amount and Unrealised GST Amount, if you are using unrealised GST.

## See also

[Set Up Goods and Services Tax](finance-setup-vat.md)  
[Setting Up Unrealised Goods and Services Tax](finance-setup-unrealized-vat.md)  
[Report GST to a Tax Authority](finance-how-report-vat.md)  
[Work with GST on Sales and Purchases](finance-work-with-vat.md)  
[Local functionality in Business Central](about-localization.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]
