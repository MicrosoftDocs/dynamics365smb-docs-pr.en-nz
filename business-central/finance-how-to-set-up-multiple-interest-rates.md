---
title: How to Set Up Multiple Interest Rates
description: You can calculate finance charges with multiple interest rates for a specific period. The interest calculation is similar for all financial charges, with variation only in the rate of interest for a specific period.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 12/21/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 0af01fe46f6b7df1149825c35a9fc0cc19482403
ms.contentlocale: en-nz
ms.lasthandoff: 03/22/2018

---
# <a name="set-up-multiple-interest-rates"></a>Set Up Multiple Interest Rates
Multiple interest rates are used for different periods for delayed payments in trade transactions. For example, a government specifies the maximum interest to be levied for a consumer. This interest rate can be changed twice a year on 01 January and 01 July. The interest rate between businesses (B2B) is agreed by the parties and there is no limit to that customer group. The announced rate is usually four percent more than the normal bank interest.

When you create finance charge terms and reminder terms, for delayed payment penalty, you can specify multiple interest rates so that the penalty fee is calculated from different interest rates in different periods. For more information, see [Collect Outstanding Balances](receivables-collect-outstanding-balances.md).

## <a name="to-set-up-multiple-interest-rates"></a>To set up multiple interest rates  
1.  Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Finance Charge Terms**, and then choose the related link.  
2.  In the **Finance Charge Terms** window, select the required finance term, and then choose the **Interest Rates** action.  
3.  Fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4.  Choose the **OK** button.  
5.  Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Reminder Terms**, and then choose the related link.  
6.  In the **Reminder Terms** window, select the required reminder term, and then choose the **Levels** action.  
7.  In the **Reminder Levels** window, select the **Calculate Interest** field.  

When you issue a finance charge memo, the memo shows the finance charges with multiple interest rates for a specific time period. The memo also contains the contact details of the customer, the company issuing the memo, the additional amount, and the total amount. The opening entry on the memo is displayed in bold. The finance charges are calculated with multiple interest rates for a specific time period and are printed after the opening entry of the memo.  

## <a name="see-also"></a>See Also  
[Collect Outstanding Balances](receivables-collect-outstanding-balances.md)  
[Setting Up Finance](finance-setup-finance.md)

