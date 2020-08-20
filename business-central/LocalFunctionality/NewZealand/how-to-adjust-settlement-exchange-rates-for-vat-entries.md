---
title: How to Adjust Settlement Exchange Rates for GST Entries
description: Describes how to settle GST entries according to the government exchange rate.
services: project-madeira
documentationcenter: ''
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2020
ms.author: bholtorf
ms.openlocfilehash: 1c58fe065754b76f811a8964db5ec48ecf302542
ms.sourcegitcommit: 007b331b6974983ee614db0406f00777da359ecb
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 08/10/2020
ms.locfileid: "3677275"
---
# <a name="adjust-settlement-exchange-rates-for-vat-entries"></a>Adjust Settlement Exchange Rates for GST Entries
You can use the **Adjust Settlement Exch. Rates** batch job to settle GST entries according to the government exchange rate as defined in the **Currency Exchange Rate** table.  

## <a name="to-adjust-settlement-exchange-rates-for-vat"></a>To adjust settlement exchange rates for GST  
1.  Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Adjust Settlement Exch. Rates**, and then choose the related link.  
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
[New Zealand Local Functionality](new-zealand-local-functionality.md)