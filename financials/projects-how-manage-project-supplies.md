---
title: Purchase Items or Services for a Job and Manage Supplies| Microsoft Docs
description: Describes how to manage the supply and purchase of material and services to jobs.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: project management, material, purchase
ms.date: 06/06/2017
ms.author: sgroespe
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: 46cae53022ba5d65a370694c9818f52a7bf45525
ms.contentlocale: en-nz
ms.lasthandoff: 07/07/2017


---
# <a name="how-to-manage-job-supplies"></a>How to: Manage Job Supplies
Managing project supplies of items, services, and expenses is an integral and critical aspect of the execution of all jobs. You can use inventory quantities or make job-specific purchases using purchase orders or purchase invoices. For example, a service job on a computer requires a new disk. You create a purchase invoice to buy a new disk and record the job that it will be used on.

If the purchase process does not require that the physical transaction be recorded separately, then a purchase may be processed in the **Job G/L Journal** window. For more information, see [How to: Record Usage for Jobs](projects-how-record-job-usage.md).

## <a name="to-purchase-items-or-services-for-a-job"></a>To purchase items or services for a job
The following procedure shows how to use a purchase invoice to purchase products for a job. The same steps apply when using a purchase order.  

1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Purchase Invoices**, and then choose the related link.  
2. Choose the **New** action and fill in the fields as necessary. For more information, see [How to: Record Purchases](purchasing-how-record-purchases.md).
3. In the **Job No.** and **Job Task No.** fields, select the information of the job that you want to purchase items or services for. Use the **Choose Columns** function if the field is not visible. For more information, see [User Personalization](ui-user-personalization.md).

    The value that you select in the **Job Line Type** field defines whether a planning line is created when you post the usage of the item. If the field contains **Billable**, then job planning lines that are ready to be invoiced to the customer are created. For more information, see [How to: Invoice Jobs](projects-how-invoice-jobs.md).
4. Choose the **Post** action.

## <a name="to-view-the-value-of-purchases-for-a-job"></a>To view the value of purchases for a job
1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Jobs**, and then choose the related link.
2. Open a relevant job card.

    On the **Tasks** FastTab, the **Outstanding Orders** field shows the total outstanding amount, in local currency, of inventory items and services on purchase documents for the job task line.  

    The **Amt. Rec. Not Invoiced** field shows the value of items delivered on purchase documents, but not yet invoiced.  
3. Choose either of the fields to open the **Purchase Lines** window where you can review information about the related purchase document lines, including which items or services have been received.

## <a name="to-post-a-job-related-expense"></a>To post a job-related expense
If you incur extraordinary or one-time job expenses, you can use the **Job G/L Journal** window to post them directly to the relevant job account.

1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Job G/L Journals**, and then choose the related link.  
2. Create a new line and enter information about the expense, including information in the **Job No.** and **Job Task No** fields.  
3. When the journal is complete, choose the **Post** action.

## <a name="see-also"></a>See Also
[Project Management](projects-manage-projects.md)  
[Finance](finance.md)  
[Purchasing](purchasing-manage-purchasing.md)         
[Sales](sales-manage-sales.md)      
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

