---
title: Invoice Prepayments | Microsoft Docs
description: Prepayments are payments that are invoiced and posted to a sales or purchase prepayment order before final invoicing. You might require a deposit before you manufacture items to order, or you might require payment before you ship items to a customer. The prepayments functionality enables you to invoice and collect deposits required from customers or to remit deposits to vendors. Thus, you can ensure that all payments are posted against an invoice.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 08/07/2017
ms.author: sgroespe
ms.openlocfilehash: dbf1ea7104501fb4bee2fe62eed1039c3c441c16
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 04/29/2019
ms.locfileid: "1238778"
---
# <a name="invoicing-prepayments"></a>Invoicing Prepayments
Prepayments are payments that are invoiced and posted to a sales or purchase prepayment order before final invoicing. You might require a deposit before you manufacture items to order, or you might require payment before you ship items to a customer. The prepayments functionality enables you to invoice and collect deposits required from customers or to remit deposits to vendors. Thus, you can ensure that all payments are posted against an invoice.  

 Prepayment requirements can be defined for a customer or vendor for all items or selected items. After you complete the required setup, you can generate prepayment invoices from sales and purchase orders for the calculated prepayment amount. You can change the amounts on the invoice as needed. For example, you can specify a total amount for the entire order. You can also send additional prepayment invoices if, for example, additional items are added to the order. You can increase quantities or add new lines to an order after issuing a prepayment, and then you can post another prepayment invoice. If you want to delete a line for which a prepayment has already been invoiced, you must issue a prepayment credit memo before you can delete the line.  

 The following table describes a sequence of tasks, with links to the topics that describe them.

|**To**|**See**|  
|------------|-------------|  
|Set up prepayment posting groups and number series, and set up default prepayment percentages for customers, vendors, and items.|[Set Up Prepayments](finance-set-up-prepayments.md)|
|Create an order, adjust the prepayment amounts, and issue an invoice for prepayment amounts.|[Create Prepayment Invoices](finance-how-to-create-prepayment-invoices.md)|  
|Issue an additional prepayment invoice, either for additional items or for an additional deposit on the original order, or issue a prepayment credit memo.|[Correct Prepayments](finance-how-to-correct-prepayments.md)|  

## <a name="see-also"></a>See Also  
[Walkthrough: Setting Up and Invoicing Sales Prepayments](walkthrough-setting-up-and-invoicing-sales-prepayments.md)  
[Finance](finance.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
