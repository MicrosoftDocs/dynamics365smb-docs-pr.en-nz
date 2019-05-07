---
title: How to Set Up Goods and Service Tax Posting
description: Describes how to set up posting for goods and services tax (GST) in New Zealand.
services: project-madeira
documentationcenter: ''
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2019
ms.author: bholtorf
ms.openlocfilehash: d53b2d4a8a6078407c38424d928f6c6f32560117
ms.sourcegitcommit: bd78a5d990c9e83174da1409076c22df8b35eafd
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 03/31/2019
ms.locfileid: "931017"
---
# <a name="set-up-goods-and-service-tax-posting"></a>Set Up Goods and Service Tax Posting
Goods and services tax (GST) is the tax that is applied on most goods and services. The GST that is paid and received during a period is reported in the Business Activity Statement (BAS) that has to be submitted to the tax authority.  

To set up posting details for GST, you must define the posting groups, rate of GST, and the accounts to which GST is to be posted. You can set up this information for a particular combination business posting groups and product posting groups.  

## <a name="to-set-up-goods-and-sales-tax-posting"></a>To set up goods and sales tax posting  
1. Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **VAT Posting Setup**, and then choose the related link.  
2. Fill in the fields as described in the following table.  

    |Field|Description|  
    |---------------------------------|---------------------------------------|  
    |**GST Bus. Posting Group**|Specifies the GST business posting group code.|  
    |**GST Prod. Posting Group**|Specifies the GST product posting group code.|  
    |**GST Identifier**|Specifies the code that is used to group similar GST setups with similar attributes.<br /><br /> For example, you can group a number of GST posting setups that have a common GST percentage.|  
    |**GST %**|Specifies the GST rate.|  
    |**GST Calculation Type**|Specifies the method that is used to calculate the purchase or sale of items.|  
    |**Sales GST Account**|Specifies the number of the general ledger account to which you want to post the sales GST.<br /><br /> If you have selected the **Reverse Charge GST** option in the **GST Calculation Type** field, then do not enter a value in this field.|  
    |**Purchase GST Account**|Specifies the number of the general ledger account to which you want to post the purchase GST.|  
    |**Reverse Chrg. GST Acc.**|Specifies the number of the general ledger account to which you want to post the reverse charge GST.<br /><br /> You can enter a value in this field only if you have selected the **Reverse Charge GST** option in the **GST Calculation Type** field.|  

3.  Choose the **OK** button.  

## <a name="see-also"></a>See Also  
[Print Goods and Service Tax Settlement Reports](how-to-print-goods-and-service-tax-settlement-reports.md)
