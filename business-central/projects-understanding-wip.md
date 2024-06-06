---
title: WIP Methods for Calculating and Recording Project Progress
description: 'Describes the different work in process (WIP) methods you can use to post, monitor, and calculate financial information for projects that are in progress.'
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bholtorf
ms.topic: conceptual
ms.search.keywords: 'work in process, work in progress, calculate project WIP'
ms.search.form: '1010,'
ms.date: 02/22/2024
ms.service: dynamics-365-business-central
ms.custom: bap-template
---
# <a name="understanding-wip-methods-in-project-management"></a>Understanding WIP Methods in Project Management

As a project progresses, materials, resources, and other expenses are consumed and must be posted to the project. Work in Process (WIP) is a feature that enables you to estimate the financial value of projects in the general ledger while the projects are ongoing. In many cases, you might post expenses for a project before invoicing a project. When only expenses have been posted, your financial statement will be inaccurate.

To track the value in the general ledger, you can calculate WIP and post the value to the general ledger. For more information, see [Monitor Project Progress and Performance](projects-how-monitor-progress-performance.md).

[!INCLUDE[prod_short](includes/prod_short.md)] supports the following methods of calculating and recording the value of work in process.

| WIP Method | Calculation Formula | Calculation Description |
| --- | --- | --- |
| Cost Value |Recognised Revenue = Billable Invoiced Price <br /><br />Budget Cost Ratio = Budget Total Costs / Budget Total Price <br /><br />Estimated Total Costs = Billable Total Price x Budget Cost Ratio <br /><br />Percentage of Completion = Usage Total Costs / Budget Total Costs <br /><br />Invoiced % = Billable Invoiced Price / Billable Total Price <br /><br />WIP Cost = (Percentage of Completion - Invoiced %) x Estimated Total Costs <br /><br />Recognised Costs = Usage Total Costs - WIP Cost|Cost value calculations start by calculating the value of what has been provided by taking a proportion of the estimated total costs based on percentage of completion. Invoiced costs are subtracted by taking a proportion of the estimated total costs based on the invoiced percentage.<br /><br />This calculation requires that the billable total price, budget total price, and budget total costs be correctly entered for the whole project. |
| Cost of Sales |Recognised Revenue = Billable Invoiced Price<br /><br /> Recognised Costs = Budget Total Cost x Invoiced Percentage<br /><br /> Invoiced % = Billable Invoiced Price / Billable Total Price<br /> (Invoiced % exists as a column on project task lines)<br /><br /> WIP Costs = Usage Total Costs – Recognised Costs |Cost of sales calculations begin by calculating the recognised costs. Costs are recognised proportionally based on budget total costs.<br /><br /> This calculation requires that the billable total price and budget total costs be correctly entered for the whole project. |
| Sales Value |Recognised Costs = Usage Total Costs<br /><br /> Recognised Revenue = Usage Total Price x Expected invoicing ratio<br /><br /> Cost Recovery % = Billable Total Price / Budget Total Price<br /><br /> WIP Sales = Recognised Sales - Billable Invoiced Price |Sales value calculations recognise revenue proportionally based on usage total costs and the expected cost recovery ratio.<br /><br /> This calculation requires that the billable total price and budget total price be correctly entered for the whole project. |
| Percentage of Completion |Recognised Costs = Usage Total Costs<br /><br /> Recognised Revenue = Billable Total Price x Percentage of Completion<br /><br /> Percentage of Completion = Usage Total Costs / Budget Total Costs<br /> (Captured in the **Cost Completion %** field on project task lines)<br /><br /> WIP Sales = Recognised Sales - Billable Invoiced Price |Percentage of completion calculations recognise revenue proportionally based on the percentage of completion, that is, usage total costs vs. budget costs.<br /><br /> This calculation requires that the billable total price and budget total costs be correctly entered for the whole project. |
| Completed Contract |WIP Amount = WIP Cost Amount = Usage (Total Cost)<br /><br /> WIP Sales Amount = Billable (Invoiced Price) |Completed contract does not recognise revenue and costs until the project is complete. You may want to do this when there is high uncertainty around the estimates of costs and revenue for the project.<br /><br /> All usage is posted to the WIP Costs account (asset) and all invoiced sales are posted to the WIP Invoiced Sales account (liability) until the project is complete. |

## <a name="see-also"></a>See also

[Project Management](projects-manage-projects.md)  
[Finance](finance.md)  
[Purchasing](purchasing-manage-purchasing.md)  
[Sales](sales-manage-sales.md)  
[Work with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]
