---
title: How to Set Up Multiple Interest Rates
description: You can calculate finance charges with multiple interest rates for a specific period. The interest calculation is similar for all financial charges, with variation only in the rate of interest for a specific period.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 96098ca669dd5001f334cf464d8e3a37de5dbf03
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "5387290"
---
# <a name="set-up-multiple-interest-rates"></a>Set Up Multiple Interest Rates
Multiple interest rates are used for different periods for delayed payments in trade transactions. For example, a government specifies the maximum interest to be levied for a consumer. This interest rate can be changed twice a year on 01 January and 01 July. The interest rate between businesses (B2B) is agreed by the parties and there is no limit to that customer group. The announced rate is usually four percent more than the normal bank interest.

When you create finance charge terms and reminder terms, for delayed payment penalty, you can specify multiple interest rates so that the penalty fee is calculated from different interest rates in different periods. For more information, see [Collect Outstanding Balances](receivables-collect-outstanding-balances.md).

## <a name="to-set-up-multiple-interest-rates"></a>To set up multiple interest rates  
1.  Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Finance Charge Terms**, and then choose the related link.  
2.  On the **Finance Charge Terms** page, select the required finance term, and then choose the **Interest Rates** action.  
3.  Fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4.  Choose the **OK** button.  
5.  Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Reminder Terms**, and then choose the related link.  
6.  On the **Reminder Terms** page, select the required reminder term, and then choose the **Levels** action.  
7.  On the **Reminder Levels** page, select the **Calculate Interest** field.  

When you issue a finance charge memo, the memo shows the finance charges with multiple interest rates for a specific time period. The memo also contains the contact details of the customer, the company issuing the memo, the additional amount, and the total amount. The opening entry on the memo is displayed in bold. The finance charges are calculated with multiple interest rates for a specific time period and are printed after the opening entry of the memo.  

## <a name="see-also"></a>See Also  
[Collect Outstanding Balances](receivables-collect-outstanding-balances.md)  
[Setting Up Finance](finance-setup-finance.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]