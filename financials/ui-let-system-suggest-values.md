---
title: Setting Up Suggested Field Values | Microsoft Docs
description: To avoid manual calculations and complete tasks quickly and accurately, you can set up automatic data entry so that Finance and Operations, Business edition fills in selected fields.
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 08/15/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: e9134b3d5fc62fb510b27db5fcbaa71e54b2b97a
ms.contentlocale: en-nz
ms.lasthandoff: 03/22/2018

---
# <a name="letting-included365finincludesd365finmdmd-suggest-values"></a>Letting [!INCLUDE[d365fin](includes/d365fin_md.md)] Suggest Values
[!INCLUDE[d365fin](includes/d365fin_md.md)] can help you complete tasks quicker and more correctly by prefilling fields or complete lines with data that you would otherwise have to calculate and enter yourself. Although such automatic data entry is always correct, you can change it afterwards if you want to.

Functionality that enters field values for you is typically offered for tasks where you enter large volumes of transactional data and want to avoid errors and save time. This topic contains a selection of such functionality. More sections will be added in future updates of [!INCLUDE[d365fin](includes/d365fin_md.md)].

## <a name="the-suggest-balancing-amount-check-box-in-the-general-journal-batches-window"></a>The **Suggest Balancing Amount** check box in the **General Journal Batches** window
When, for example, you are entering general journal lines for multiple expenses that must all be posted to the same bank account, then each time you enter a new journal line for an expense, you can have the **Amount** field on the bank account line automatically updated to the amount that balances the expenses. For more information about working with general journals, see [Working with General Journals](ui-work-general-journals.md).

### <a name="to-have-the-amount-field-on-balancing-general-journal-lines-filled-automatically"></a>To have the **Amount** field on balancing general journal lines filled automatically
1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **General Journals**, and then choose the related link.
2. On the line for your preferred general journal batch, choose the **Suggest Balancing Amount** check box.
3. Open the general journal and proceed to register and post transactions using the described functionality for automatic entry of a field value.       

For information about how to set up a personal general journal batch, for example, for expense handling, see [Working with General Journals](ui-work-general-journals.md).

## <a name="the-automatically-fill-date-received-field-in-the-payment-registration-window"></a>The **Automatically Fill Date Received** field in the **Payment Registration** window
The **Payment Registration** window shows outstanding incoming payments as lines that represent sales documents where an amount is due for payment. For more information about applying customer payments, see [Reconcile Customer Payments Manually From a List of Unpaid Sales Documents](receivables-how-reconcile-customer-payments-list-unpaid-sales-documents.md).

You main actions in the window are to fill in the **Payment Made** check box and the **Date Received** field. You can set [!INCLUDE[d365fin](includes/d365fin_md.md)] up to automatically enter work date in the **Date Received** field when you select the **Payment Made** check box.

### <a name="to-have-the-date-received-field-in-the-payment-registration-window-filled-automatically"></a>To have the **Date Received** field in the **Payment Registration** window filled automatically
1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Payment Registration Setup**, and then choose the related link.
2. Select the **Automatically Fill Date Received** check box.
3. Open the **Payment Registration** window and proceed to process incoming customer payments using the described functionality for automatic entry of a field value.

## <a name="see-also"></a>See Also
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  
[Finance](finance.md)

