---
title: How to Adjust Settlement Exchange Rates for GST Entries
description: Describes how to settle GST entries according to the government exchange rate.
services: project-madeira
documentationcenter: 
author: bholtorf
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 10/01/2018
ms.author: bholtorf
ms.translationtype: HT
ms.sourcegitcommit: 046a42582dc66368fded90a4bb45add71a95d979
ms.openlocfilehash: 8e540abfeb1e842048802344d5efcef6e10d35e0
ms.contentlocale: en-nz
ms.lasthandoff: 07/02/2018

---
# <a name="adjust-settlement-exchange-rates-for-vat-entries"></a>Adjust Settlement Exchange Rates for GST Entries
You can use the **Adjust Settlement Exch. Rates** batch job to settle GST entries according to the government exchange rate as defined in the **Currency Exchange Rate** table.  

## <a name="to-adjust-settlement-exchange-rates-for-vat"></a>To adjust settlement exchange rates for GST  
1.  Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Adjust Settlement Exch. Rates**, and then choose the related link.  
2.  On the **Options** FastTab, fill in the fields as described in the following table.  

    |Field|Description|  
    |---------------------------------|---------------------------------------|  
    |**Settlement Period**|Specifies the start date of the settlement period.|  
    |**Ending Date**|Specifies the end date of the settlement period.|  
    |**Posting Description**|Specifies the posting description.|  
    |**Document No.**|Specifies the document number for which you want to settle GST entries.|  
    |**Posting Date**|Specifies the posting date of the document.|  
    |**Use Daily Settlement Exch. Rate**|Select if you want to use the daily settlement exchange rate.|  

3.  Choose the **OK** button.  

The GST entries are adjusted and you can view them in the **GST Register** report.

## <a name="see-also"></a>See Also
[New Zealand Local Functionality]new-zealand-local-functionality.md()
