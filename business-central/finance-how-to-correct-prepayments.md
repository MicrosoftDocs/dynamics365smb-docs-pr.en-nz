---
title: How to Correct Prepayments | Microsoft Docs
description: You can make a correction to an order after you have posted a prepayment invoice for the order. You can add new lines to an order after issuing a prepayment, and then you can post another prepayment invoice, but you cannot delete a line from an order after a prepayment has been invoiced for the line.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 3dd124807d3d6ce3a775d18dcd88a8251b0feb30
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 10/01/2020
ms.locfileid: "3924194"
---
# <a name="correct-prepayments"></a>Correct Prepayments

You can make a correction to an order after you have posted a prepayment invoice for the order. You can add new lines to an order after issuing a prepayment, and then you can post another prepayment invoice, but you cannot delete a line from an order after a prepayment has been invoiced for the line.  

> [!TIP]
> If you have posted a prepayment invoice for a sales invoice that you then correct or cancel, you must correct or cancel the prepayment as well.

## <a name="to-correct-a-prepayment"></a>To correct a prepayment

The following procedure shows how to issue a prepayment credit memo to cancel all invoiced prepayments for a sales order.  

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders** , and then choose the related link.  
2. Open the relevant sales order.
3. Choose the **Prepayment** action, and then choose the **Post Prepayment Credit Memo** action or the **Post and Print Prepmt. Cr. Memo** action.  
4. On the **Sales Credit Memo** page, proceed to correct the relevant entries, as for any sales credit memo. For more information, see [Process Sales Returns or Cancellations](sales-how-process-sales-returns-cancellations.md).  

    > [!NOTE]  
    > To reduce the amount in the **Line Amount** field, you must first increase the prepayment percentage on the line so that the value in the **Prepmt. Line Amount** field is not decreased below the value in the **Prepmt. Amt. Inv.** field.

5. To make a prepayment invoice for any new lines in the sales credit memo, choose the **Prepayment** action, and then choose the **Post Prepayment Invoice** action or the **Post and Print Prepmt. Invoice** action.  
6. To issue an additional prepayment invoice, increase the prepayment amount on one or more lines and post the prepayment invoice. A new invoice will be created for the difference between the prepayment amounts invoiced and the new prepayment amounts.  

## <a name="see-also"></a>See Also

[Invoicing Prepayments](finance-invoice-prepayments.md)  
[Walkthrough: Setting Up and Invoicing Sales Prepayments](walkthrough-setting-up-and-invoicing-sales-prepayments.md)  
[Finance](finance.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  
