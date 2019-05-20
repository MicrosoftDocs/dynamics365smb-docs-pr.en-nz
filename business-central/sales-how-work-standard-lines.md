---
title: Setup Standard Lines for Recurring Sales and Purchases| Microsoft Docs
description: You can set up sales lines and purchase lines that you frequently make and then insert them on sales and purchase documents to quickly fill the lines with standard information.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: trade, sell, replenishment
ms.date: 04/24/2019
ms.author: sgroespe
ms.openlocfilehash: 83f6a24fc066faef49de456e18673f8059a9831d
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 04/29/2019
ms.locfileid: "1252280"
---
# <a name="create-recurring-sales-and-purchase-lines"></a>Create Recurring Sales and Purchase Lines
If you often need to create sales and purchase lines with similar information, you can set up standard lines that you can then insert on recurring sales and purchase documents, for example, for recurring replenishment orders.  

The following procedures show how to work with standard sales lines on a sales invoice. It works in a similar way for all other sales documents and for all purchase documents.  

## <a name="to-set-up-standard-sales-lines"></a>To set up standard sales lines  
1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Standard Sales Lines**, and then choose the related link.  
2. On the **Standard Sales Lines** page, choose the **New** action.  
3. On the **General** FastTab, fill the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  
4. On the **Lines** FastTab, enter information in the fields to prepare sales lines that reflect the standard lines that you expect to use as recurring lines on sales documents.  

> [!NOTE]
> You cannot define prices on standard sales lines because prices, discounts, etc. are calculated on the actual sales documents after you insert the standard sales lines.

## <a name="to-assign-standard-sales-lines-to-a-customer"></a>To assign standard sales lines to a customer
Assign one or more standard sales lines to a customer so that they are available to insert on sales documents for that customer.

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Customers**, and then choose the related link.
2. Open the card for a relevant customer.
3. Choose the **Recurring Sales Lines** action.
4. On the **Recurring Sales Lines** page, select codes for the recurring sales lines that you want to be able to insert on sales documents for the customer.
5. Fill in the additional fields to define when, how, and where the recurring sales lines are to be used.
6. In the four fields where you select how the lines are inserted on four document types, select one of the following options:

|Option|Description|
|-|-|
|**Manual**|You must manually look up and insert a recurring sales line that exists for the customer.|
|**Automatic**|If multiple recurring sales lines exist for the customer, you will get a notification from where you can pick which one to insert. If only one recurring sales line exists, it will be inserted automatically.|
|**Always Ask**|A notification appears and all existing recurring sales lines are shown so that you can select one.

## <a name="to-insert-recurring-sales-lines-on-a-sales-invoice"></a>To insert recurring sales lines on a sales invoice
If recurring sales lines exist for the customer, you can insert them on all types of sales documents, such as a sales invoice. If you have activated the notification in question, you will be informed if recurring sales lines exist.
1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Invoices**, and then choose the related link.
2. Open the sales invoice that you want to insert one or more standard sales lines on.
3. Choose the **Get Recurring Sales Lines** action.
4. On the **Recurring Sales Lines** page, choose the lookup button in the **Code** field, and then select a set of standard sales lines.

    > [!NOTE]
    > To use the recurring sales lines set together with the **Create Recurring Sales Invoices** batch job, you must also fill in the **Valid From Date** and **Valid To Date** fields on the **Recurring Sales Lines** page. For more information, see [To create multiple sales invoices based on standard sales lines](sales-how-work-standard-lines.md#to-create-multiple-sales-invoices-based-on-standard-sales-lines).

5. Choose the **OK** button to insert the standard sales lines on the invoice where you can reuse them as is or edit the information.

## <a name="to-create-multiple-sales-invoices-based-on-standard-sales-lines"></a>To create multiple sales invoices based on standard sales lines
You can use the **Create Recurring Sales Invoices** batch job to create sales invoices according to standard sales lines that are assigned to the customers and with posting dates within the valid-from and valid-to dates that you specify on the standard sales lines.

> [!NOTE]
> On the **Recurring Sales Lines** page, you can also specify a direct-debit payment method and a direct-debit mandate. The sales invoices that are created with the **Create Recurring Sales Inv.** batch job will then include information required to collect payment for the sales invoices with SEPA direct debit. For more information, see [Collect Payments with SEPA Direct Debit](finance-collect-payments-with-sepa-direct-debit.md).

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Create Recurring Sales Invoices**, and then choose the related link.
2. On the **Create Recurring Sales Invoices** page, fill in the fields as necessary.
3. In the **Code** filter field, enter the code for standard sales lines that are assigned to a customer that you want to create sales invoices for.
4. Choose the **OK** button.

Sales invoices are created for the customers with the specified standard customer sales code, and any specified direct-debit information, for posting on the specified date.

## <a name="see-also"></a>See Also  
[Sales](sales-manage-sales.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
