---
title: Updating Currency Exchange Rates| Microsoft Docs
description: To use multiple currencies in your business, you can set up a code for each currency and use an external exchange rate service, such as FloatRates.
services: project-madeira
documentationcenter: 
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: multiple currencies
ms.date: 10/01/2018
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 33b900f1ac9e295921e7f3d6ea72cc93939d8a1b
ms.openlocfilehash: 23940bd1e5fd29dc92e8285c08679135889701e9
ms.contentlocale: en-nz
ms.lasthandoff: 11/26/2018

---
# <a name="update-currency-exchange-rates"></a>Update Currency Exchange Rates
You must set up a code for each currency you use if you buy or sell in currencies other than your local currency, have receivables or payables in other currencies, or record G/L transactions in different currencies.  

As companies operate in increasingly more countries/regions, it becomes more important that they be able to review or report financials in more than one currency. The program supports use of multiple currencies. Within the program, your general ledger is set up using your local currency (LCY), and another currency is set up as an additional currency, with a current exchange rate assigned.  

 By designating a second currency as an additional reporting currency, [!INCLUDE[d365fin](includes/d365fin_md.md)] will automatically record amounts in both LCY and this additional reporting currency on each G/L entry and on other entries, such as GST entries. When G/L entry amounts are calculated in an additional reporting currency, the information on the **Currency Exchange Rates** page is used to find the relevant exchange rate.  

> [!WARNING]  
>  The Additional Reporting Currency functionality should NOT be used as a basis for financial statement translation. It is not a tool that can perform translation of foreign subsidiary financial statements as part of a company consolidation. The additional reporting currency functionality only provides the option of preparing reports in another currency, as if that currency was the company’s local currency.

## <a name="adjusting-exchange-rates"></a>Adjusting Exchange Rates  
Because exchange rates fluctuate constantly, additional currency equivalents in your system must be adjusted periodically. If these adjustments are not done, amounts that have been converted from foreign (or additional) currencies and posted to the general ledger in LCY may be misleading. In addition, daily entries posted before a daily exchange rate is entered into the program must be updated after the daily exchange rate information is entered. The Adjust Exchange Rates batch job is used to adjust the exchange rates of posted customer, vendor and bank account entries. It can also update additional reporting currency amounts on G/L entries.  

## <a name="displaying-reports-and-amounts-in-the-additional-reporting-currency"></a>Displaying Reports and Amounts in the Additional Reporting Currency  
Using an additional reporting currency can assist the reporting process for a company in the following cases:  

- Companies in non-EU countries/regions that have a high proportion of transactions with EU country/region companies. In this case, the non-EU company may also wish to report in euro to make its financial reports more usable for its EU trade partners.  

- Companies that also wish to display reports in a more internationally traded currency than their own local currency.  

Several reports in the General Ledger application area are based on G/L entries. To display the financial data in the report in the additional reporting currency, you simply select the **Show in Add.-Currency** field in the relevant G/L report page.  

## <a name="to-set-up-a-currency-exchange-rate-service"></a>To set up a currency exchange rate service
You can use an external service to keep your currency exchange rates up to date, such as FloatRates.

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Currency Exchange Rate Services**, and then choose the related link.
2. Choose the **New** action.
3. On the **Currency Exchange Rate Service** page, fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4. Choose the **Enabled** check box to enable the service.

## <a name="to-update-currency-exchange-rates-through-a-service"></a>To update currency exchange rates through a service
1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Currencies**, and then choose the related link.
2. Choose the **Update Exchange Rates** action.

The value in the **Exchange Rate** field on the **Currencies** page is updated with the latest currency exchange rate.

## <a name="see-also"></a>See Also
[Closing Years and Periods](year-close-years-periods.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

