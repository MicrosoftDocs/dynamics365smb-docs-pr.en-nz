---
title: Set Up Currencies
description: 'You must set up each currency if you buy or sell in currencies other than your local currency (LCY), or if you record G/L transactions in different currencies.'
author: edupont04
ms.topic: conceptual
ms.search.keywords: multiple currencies
ms.search.form: '5, 118'
ms.date: 03/15/2022
ms.author: edupont
---
# <a name="set-up-currencies"></a><a name="set-up-currencies"></a><a name="set-up-currencies"></a>Set Up Currencies

[!INCLUDE [finance-currencies-def](includes/finance-currencies-def.md)]

Use an external service to get the latest currency exchange rates into the **Currencies** list. For more information, see [To set up a currency exchange rate service](finance-how-update-currencies.md#to-set-up-a-currency-exchange-rate-service).  

[!INCLUDE [finance-currencies-lcy](includes/finance-currencies-lcy-note.md)]

## <a name="currencies"></a><a name="currencies"></a><a name="currencies"></a><a name="curr"></a>Currencies

The following table describes the fields in the **Currencies** list.

|Field|Description|  
|---------------------------------|---------------------------------------|  
|**Code**|The identifier for the currency.|
|**Description**|A free text description of the currency.|
|**ISO Code**|The international three letter code to the currency defined in ISO 4217.|
|**ISO Numeric code**|The international numeric reference to the currency defined in ISO 4217.|
|**Exchange Rate Date**|The latest actual exchange rate date.|
|**EMU Currency**|Specifies if the currency is an EMU (Economic and Monetary Union) currency, such as EUR.|
|**Realised Gains Account**|The account where the actual gain will be posted when you receive payments for receivables or register the actual currency rate on payments to payables. For an example of a receivable currency transaction, see the example below this table. |
|**Realised Losses Account**|The account where the actual loss will be posted when you receive payments for receivables or register the actual currency rate on payments to payables. For an example of a receivable currency transaction, see the example below this table. |
|**Unrealised Gains Account**|The account where the theoretical gain will be posted when you perform a currency adjustment.|
|**Unrealised Losses Account**|The account where the theoretical loss will be posted when you perform a currency adjustment.|
|**Amount Rounding Precision**|Some currencies have other formats for invoice amounts than are defined in the **General Ledger Setup** page. If you change the amount rounding precision for a currency, all invoice amounts in that currency will be rounded with the updated precision.|
|**Amount Decimal Places**|Some currencies have other formats for invoice amounts than are defined in the **General Ledger Setup** page. If you change the amount decimal places for a currency, all invoice amounts in the currency will be rounded with the updated decimals|
|**Invoice Rounding Type**|Specifies the method to use if the amounts must be rounded. The options are **Nearest**, **Up**, and **Down**.|
|**Unit-Amount Rounding Precision**|Some currencies have other formats for unit amounts than are defined in the **General Ledger Setup** page. if you change the unit amount rounding precision for a currency, all unit amounts in the currency will be rounded with the updated precision.|
|**Unit-Amount Decimal Places**|Some currencies have other formats for unit amounts than are defined in the **General Ledger Setup** page. If you change the unit amount decimal places for a currency, all unit amounts in the currency will be rounded with the updated decimals.|
|**Application Rounding Precision**|Specifies the size of the interval that is allowed as a rounding difference when you apply entries in different currencies to one another.|
|**Conversion LCY Rounding. Debit Account**|Specifies conversion information that must also contain a debit account if you want to insert correction lines for rounding differences in the general journals using the **Insert Conv. LCY Rndg. Lines** action.|
|**Conversion LCY Rounding Credit Account**|Specifies conversion information that must also contain a credit account if you wish to insert correction lines for rounding differences in the general journals using the **Insert Conv. LCY Rndg. Lines** action.|
|**Last Date Adjusted**|The date of the last currency adjustment.|
|**Last Date Modified**|The date of the change to the setup of the currency.|
|**Payment Tolerance %**|The maximum payment tolerance % set for this currency. For more information, see [Payment Tolerance and Payment Discount Tolerance](finance-payment-tolerance-and-payment-discount-tolerance.md). |
|**Max. Payment Tolerance Amount**|The maximum payment tolerance amount set for this currency. For more information, see [Payment Tolerance and Payment Discount Tolerance](finance-payment-tolerance-and-payment-discount-tolerance.md). |
|**Currency Factor**|Specifies the relationship between the currency and the local currency using the actual currency rate.|
|**Realised G/L Gains Account**|Specifies the G/L account that is used to post exchange rate gains for currency adjustments between the local currency (LCY) and the additional reporting currency. The exchange rate gains are calculated when the Adjust Exchange Rates batch job is run to adjust general ledger accounts. This field might not be visible by default. It can be retrieved by personalising the page.|
|**Realised G/L Losses Account**|Specifies the G/L account that is used to post exchange rate losses for currency adjustments between the local currency (LCY) and the additional reporting currency. The exchange rate gains are calculated when the Adjust Exchange Rates batch job is run to adjust general ledger accounts. This field might not be visible by default. It can be retrieved by personalising the page.|
|**Residual Gains Account**|Specifies the G/L account that is used to post residual gain amounts (rounding differences) when an additional reporting currency is used in the general ledger application area. This field might not be visible by default. It can be retrieved by personalising the page.|
|**Residual Losses Account**|Specifies the G/L account that is used to post residual loss amounts (rounding differences) when an additional reporting currency is used in the general ledger application area. This field might not be visible by default. It can be retrieved by personalising the page.|
|**Max. GST Difference Allowed**|The maximum amount allowed for GST differences in this currency. For more information, see [Correcting GST amounts manually on sales and purchase documents](finance-work-with-vat.md#correcting-vat-amounts-manually-on-sales-and-purchase-documents). This field might not be visible by default. It can be retrieved by personalising the page.|
|**GST Rounding Type**|Specifies the rounding method for correcting GST amounts manually in sales and purchase documents. This field might not be visible by default. It can be retrieved by personalising the page.|

### <a name="available-currency-functions"></a><a name="available-currency-functions"></a><a name="available-currency-functions"></a>Available currency functions

The following table outlines key actions on the **Currencies** page.  

|Menu|Action|Description|
|-------------|--------------|------------------------------|
|**Process**|**Suggest Accounts**|Use accounts from the other currencies. The most frequently used accounts will be inserted.|
||**Change Payment Tolerance**|Change either or both the maximum payment tolerance and the payment tolerance percentage, and filter by currency. For more information, see [Payment Tolerance and Payment Discount Tolerance](finance-payment-tolerance-and-payment-discount-tolerance.md)|
||**Exchange Rates**|View updated exchange rates for the currencies that you use.|
||**Adjust Exchange Rates**|Adjust general ledger, customer, vendor, and bank account entries to reflect a more updated balance if the exchange rate has changed since the entries were posted.|
||**Exchange Rate Adjustment Register**|View the results of running the **Adjust Exchange Rates** batch job. One line is created for each currency or each combination of currency and posting group that is included in the adjustment.|
|**Exchange Rate Service**|**Exchange Rate Services**|View or edit the setup of the services that are set up to fetch updated currency exchange rates when you choose the **Update Exchange Rates** action.|
||**Update Exchange Rates**|Get the latest currency exchange rates from a service provider.|
|**Reports**|**Foreign Currency Balance**|View the balances for all customers and vendors in both foreign currencies and in local currency (LCY). The report displays two LCY balances. One is the foreign currency balance converted to LCY by using the exchange rate at the time of the transaction. The other is the foreign currency balance converted to LCY by using the exchange rate of the work date.|

## <a name="lcy-and-other-currencies"></a><a name="lcy-and-other-currencies"></a><a name="lcy-and-other-currencies"></a>LCY and other currencies

[!INCLUDE [finance-currencies-lcy-def](includes/finance-currencies-lcy-def.md)]

## <a name="rounding-currencies"></a><a name="rounding-currencies"></a><a name="rounding-currencies"></a>Rounding currencies

To manage currencies that do not use decimals and to avoid unnecessary decimals in foreign currency, you can use two different rounding features:

- Unit-amount rounding  

- Amount rounding  

These features can operate independently or in combination. In addition, the features can operate in connection with invoice rounding.

As opposed to the invoice rounding features, the amount rounding and unit-amount rounding features affect only amounts in foreign currency-not the corresponding amounts in LCY. These two features will not result in any postings to general ledger accounts. Consequently, no general ledger account needs to be specified on posting groups or elsewhere.

### <a name="unit-amount-rounding"></a><a name="unit-amount-rounding"></a><a name="unit-amount-rounding"></a>Unit-amount rounding

The unit-amount rounding feature controls how sales prices for items and resources in foreign currencies are rounded on sales and purchase lines. You must specify the rules for each currency separately, in the **Unit-Amount Rounding Precision** field in the **Currencies** list.

The unit-amount rounding feature is used automatically every time you enter an item or resource number on a sales line. If the invoice is for a customer with a currency code, the item or resource price is converted into the customer's currency. The price is rounded according to the unit-amount rounding precision for the currency.

### <a name="amount-rounding"></a><a name="amount-rounding"></a><a name="amount-rounding"></a>Amount rounding

The amount rounding feature controls how amounts in foreign currencies are rounded on general journal lines, sales lines, and purchase lines. You must specify the rules for each currency separately, in the **Amount Rounding Precision** field in the **Currencies** list.

Amounts in foreign currencies are rounded when you fill in and post general journal lines, sales lines, and purchase lines.

## <a name="exchange-rates"></a><a name="exchange-rates"></a><a name="exchange-rates"></a>Exchange rates

You can register exchange rates for each foreign currency and specify from which dates the exchange rates are valid. For example, you can enter daily exchange rates, monthly exchange rates, or quarterly exchange rates for each foreign currency.

You can retain historical exchange rates in the **Currency Exchange Rates** page for reference purposes. When you need to update exchange rates, you can use the **Update Exchange Rates** button to get the latest exchange rates from an external service provider.

## <a name="general-ledger-accounts"></a><a name="general-ledger-accounts"></a><a name="general-ledger-accounts"></a>General ledger accounts

You cannot link currency codes to general ledger accounts because amounts on general ledger accounts are in LCY. If you have a bank loan in NZD and place deposits in a bank account in SEK, you can keep track of these accounts by setting up bank accounts in NZD and SEK. With posting groups, you can link the accounts to the relevant general ledger accounts. In the general ledger, the value of the amounts is shown in LCY.

You can enter a currency code on a general journal line and post the line to a general ledger account. The relevant exchange rate is used to convert the amount to LCY before it is posted to the general ledger account.  

## <a name="example-of-a-receivable-currency-transaction"></a><a name="example-of-a-receivable-currency-transaction"></a><a name="example-of-a-receivable-currency-transaction"></a>Example of a receivable currency transaction

[!INCLUDE [finance-currencies-example](includes/finance-currencies-example.md)]

## <a name="see-related-microsoft-training"></a><a name="see-related-microsoft-training"></a><a name="see-related-microsoft-training"></a>See related [Microsoft training](/training/modules/currencies-exchange-rates-dynamics-365-business-central/)

## <a name="see-also"></a><a name="see-also"></a><a name="see-also"></a>See also

[Update Currency Exchange Rates](finance-how-update-currencies.md)  
[Set Up an Additional Reporting Currency](finance-how-setup-additional-currencies.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]
