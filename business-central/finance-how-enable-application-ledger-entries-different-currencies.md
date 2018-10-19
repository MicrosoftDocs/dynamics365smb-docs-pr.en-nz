---
title: Apply Entries in Different Currencies| Microsoft Docs
description: You can apply ledger entries in multiple currencies, for example, if you sell in one currency and receive payment in another.
services: project-madeira
documentationcenter: 
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: multiple currencies, payment, reconcile
ms.date: 10/01/2018
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: f8216885adb734dde214570c65b5f6036caa37d2
ms.contentlocale: en-nz
ms.lasthandoff: 09/28/2018

---
# <a name="enable-application-of-ledger-entries-in-different-currencies"></a>Enable Application of Ledger Entries in Different Currencies
If you purchase from a vendor in one currency and submit payment in another currency, you can apply the payment to the purchase.

Likewise, if you sell to a customer in one currency and receive payment in another currency, you can apply the payment to the sales invoice.

The following procedure describes how to set this up for vendor ledger entries in the **Purchases & Payables Setup** window. The setup is similar for customer ledger entries in the **Sales & Receivables Setup** window.

## <a name="to-enable-application-of-vendor-ledger-entries-in-different-currencies"></a>To enable application of vendor ledger entries in different currencies
1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchases & Payables Setup**, and then choose the related link.
2. In the **Appln. between Currencies** field, select one of the following options.

| Option | Description |
| --- | --- |
| None |Application between currencies is not allowed. |
| EMU |Application between EMU currencies is allowed. |
| All |Application between all currencies is allowed. |

## <a name="to-set-up-gl-accounts-for-currency-application-rounding-differences"></a>To set up G/L accounts for currency application rounding differences  
If you apply entries in different currencies, you must set up the general ledger accounts to which you want to post rounding differences.  

> [!NOTE]  
>  You must set up the general ledger accounts before you complete the task. For more information, see [Understanding the General Ledger and the Chart of Accounts](finance-general-ledger.md).

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Customer Posting Groups**, and then choose the related link.  
2. In the **Debit Curr. Appln. Rndg. Acc.** and **Credit Curr. Appln. Rndg. Acc.** fields, enter the relevant general ledger accounts to post rounding differences.  
3. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Vendor Posting Groups**, and then choose the related link.  
4. In the **Debit Curr. Appln. Rndg. Acc.** and **Credit Curr. Appln. Rndg. Acc.** fields, enter the relevant general ledger accounts to post rounding differences.  

## <a name="see-also"></a>See Also
[Managing Payables](payables-manage-payables.md)  
[Managing Receivables](receivables-manage-receivables.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

