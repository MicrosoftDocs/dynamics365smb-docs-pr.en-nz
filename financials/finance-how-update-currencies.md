---
title: 'How to: Update Currency Exchange Rates | Microsoft Docs'
description: Working with multiple currencies
services: project-madeira
documentationcenter: 
author: edupont04
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: multiple currencies, Yahoo
ms.date: 03/24/2017
ms.author: edupont
ms.translationtype: Human Translation
ms.sourcegitcommit: a31be0f9d07e2abb591e26f6bae34c6f6e4dcda6
ms.openlocfilehash: b261da0f233ce78a9f14c2979c876be401ffedef
ms.contentlocale: en-nz
ms.lasthandoff: 05/04/2017


---
# <a name="how-to-update-currency-exchange-rates"></a>How to: Update Currency Exchange Rates
You must set up a code for each currency you use if you buy or sell in currencies other than your local currency, have receivables or payables in other currencies, or record G/L transactions in different currencies.  

**Note**: This functionality requires that your experience is set to **Suite**. For more information, see [Customizing Your [!INCLUDE[d365fin](includes/d365fin_md.md)] Experience](ui-experiences.md).

You can use an external service to keep your currency exchange rates up to date. The Yahoo Currency Exchange Rates service is preinstalled and ready to enable.

## <a name="to-set-up-a-currency-exchange-rate-service"></a>To set up a currency exchange rate service
1. In the top right corner, choose the **Search for Page or Report** icon ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon"), enter **Currency Exchange Rate Services**, and then choose the related link.
2. Choose the **New** action.
3. In the **Currency Exchange Rate Service** window, fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4. Choose the **Enabled** check box to enable the service.

## <a name="to-update-currency-exchange-rates-through-a-service"></a>To update currency exchange rates through a service
1. In the top right corner, choose the **Search for Page or Report** icon ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon"), enter **Currencies**, and then choose the related link.
2. Choose the **Update Exchange Rates** action.

The value in the **Exchange Rate** field in the **Currencies** window is updated with the latest currency exchange rate.

## <a name="see-also"></a>See Also
[Closing Years and Periods](year-close-years-periods.md)  
[Working With [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

