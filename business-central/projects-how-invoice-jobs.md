---
title: Create a Job Sales Invoice to Invoice a Job| Microsoft Docs
description: Describes how to invoice customers for job expenses as a project progresses.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: project invoice
ms.date: 06/06/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: b526879c1b49a90ff0ddcb415ba19f9d0567f7fd
ms.contentlocale: en-nz
ms.lasthandoff: 03/22/2018

---
# <a name="invoice-jobs"></a>Invoice Jobs
During the project, job costs from resource usage, materials, and job-related purchases can accumulate. As the job progresses, these transactions get posted to the job journal. It is important that all costs get recorded in the job journal before you invoice the customer.

You can invoice the whole job from the **Job Task Lines** window or only invoice selected billable lines from the **Planning Lines** window. Invoicing can be done after the job is finished or at certain intervals during the job's progress based on an invoicing schedule.

> [!NOTE]  
>   If you select **Billable** in the **Job Line Type** field on the purchase documents for job-related purchases, then job planning lines that are ready to be invoiced to the customer are created. For more information, see [Manage Project Supplies](projects-how-manage-project-supplies.md).

## <a name="to-create-and-post-a-job-sales-invoice"></a>To create and post a job sales invoice
You can create an invoice for a job or for one or more job tasks for a customer when either the work to be invoiced is complete or the date for invoicing based on an invoicing schedule has been reached.

From the **Jobs** window, you can invoice a customer by selecting the job, and then choosing the **Create Job Sales Invoice** action. The following procedure shows how to use a batch job to invoice multiple jobs.  

1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Job Create Sales Invoice**, and then choose the related link.  
2. Fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. Set filters if you want to limit the jobs that the batch job will process.
4. Choose the **OK** button to create the invoices.  

## <a name="to-create-multiple-job-sales-invoices-from-job-planning-lines"></a>To create multiple job sales invoices from job planning lines
You can create an invoice from a job planning lines, and indicate at that time the quantity of the item, resource, or general ledger account that you want to invoice.

1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Jobs**, and then choose the related link.
2. Open a relevant job.
3. Select a job task for which the **Job Task Type** field contains **Posting**, and then choose the **Job Planning Lines** action.  
4. On a job planning line, in the **Qty. To Transfer to Invoice** field, enter the quantity of the item, resource, general ledger account type that you want to invoice.  
5. Choose the **Create Sales Invoice** action.
6. In the **Job Create Sales Invoice** window, enter the posting date and whether you want to create a new invoice or append this invoice to an existing one.
7. Choose the **OK** button.  

    On the job planning line, in the **Qty. Transferred to Invoice** field, you can see the quantity.
8. In the **Job Planning Lines** window, choose the **Sales Invoices/Credit Memos** action.

    The **Sales Invoice** window opens, showing the quantity that you have transferred to the invoice.  
9. Make any additional changes, and then choose the **Post** action.

> [!NOTE]  
>   The above procedure is similar for creating, reviewing, and posting a job-related sales credit memo.

## <a name="to-calculate-and-post-job-completion-entries"></a>To calculate and post job completion entries
When you have completed all activities for a job, including usage posting and invoicing, you must update the job to have a **Status** of **Completed**. Then, you must reverse any WIP that has been posted to the general ledger.

1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Jobs**, and then choose the related link.  
2. Select an open job, and then choose the **Edit** action.
3. In the **Status** field, select **Completed**.
4. Follow the assistance steps to calculate and post WIP. Alternatively, follows steps 5 and 6 to do so manually.  
5. Choose the **Calculate WIP** action.
6. In the **Job Calculate WIP** window, fill in the fields as necessary.  

     The job WIP entries created by running the batch job will have the **Job Complete** check box selected to show that they are completion entries.  
7. Choose the **Job Post WIP to G/L** action.
8. In the **Job Post WIP to G/L** window, fill in the fields as necessary.  

     The job WIP general ledger entries created by running the batch job will have the **Job Complete** check box selected to show they are completion entries.

## <a name="see-also"></a>See Also
[Managing Projects](projects-manage-projects.md)  
[Finance](finance.md)  
[Purchasing](purchasing-manage-purchasing.md)         
[Sales](sales-manage-sales.md)      
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

