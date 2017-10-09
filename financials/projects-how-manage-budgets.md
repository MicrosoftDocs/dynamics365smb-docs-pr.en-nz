---
title: Set Up and Manage a Budget for a Job| Microsoft Docs
description: Describes how to plan resources and forecast and control the costs of a project by setting up a budget for each job.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: project budget, forecast
ms.date: 06/06/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: 0e480c67ddb2acd5e98799c98cb1cd9d972889df
ms.contentlocale: en-nz
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-manage-job-budgets"></a>How to: Manage Job Budgets
You can set up a budget for each job. The budget is used to plan the resources that you allocate to a job. The budget can be either general with few entries or it can contain more entries that are divided into activity levels. You can then compare the budgeted amounts with the actual usage as recorded in the job journal. By monitoring differences between actual usage and budgeted usage, you can control an ongoing project and improve the quality of future jobs by reducing the risk of underestimating costs.

The following procedure describes how to estimate budgeted costs during planning. For information about recording budgeted versus actual job prices and costs, see [How to: Record Usage for Jobs](projects-how-record-job-usage.md).  

## <a name="JobBudgetCosts"></a> To estimate the budgeted costs for a job
When a customer wants to know the price of a job that will be invoiced based on usage, you must have to determine the budgeted costs for the job. You use the **Job Task Lines** window to do this.

1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Jobs**, and then choose the related link.  
2. Open a relevant job.
3. Select a task line of type Posting, and then choose the **Job Planning Lines** action.
4. On a new line, fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]   

For the **Line Type** field, refer to the following information.  

| Line Type | Description |
| --- | --- |
| **Both Budget and Billable** |The cost and price amounts entered on the planning line are the budgeted costs for the particular planning line. The price amount will be invoiced. |
| **Budget** |The customer is not charged for usage. Usage is not transferred to an invoice, but will still be used in the calculation of WIP. |
| **Billable** |The customer is charged for usage. Usage is transferred to the invoice, based on the quantity specified in the Qty. to Transfer to Invoice field. |

> [!NOTE]  
>   The **Planning Date** field for the planning line contains the date when usage related to the planning line is expected to be completed. It is also the date when the planning line may be transferred to a sales invoice and posted.  

> [!NOTE]  
>   When you fill in the **Quantity** field, all total price and total cost information will be calculated and filled in for that planning line. You can edit them at any time.

In the **Job Card** window, you can now see a summary of the total budgeted costs, budgeted price, billable cost and billable price for each task.

For information about recording budgeted versus actual job prices and costs, see [How to: Record Usage for Jobs](projects-how-record-job-usage.md).

## <a name="see-also"></a>See Also
[Project Management](projects-manage-projects.md)  
[Finance](finance.md)  
[Purchasing](purchasing-manage-purchasing.md)         
[Sales](sales-manage-sales.md)      
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

