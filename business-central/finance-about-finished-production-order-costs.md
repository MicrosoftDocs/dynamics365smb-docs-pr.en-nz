---
title: About Finished Production Order Costs
description: Finishing the production order is key to completing the costing lifecycle of a production item. Final costs are calculated in Adjust Cost Item Entries batch job.
author: SorenGP
ms.topic: conceptual
ms.search.form: 99000867
ms.date: 06/16/2021
ms.author: edupont
ms.openlocfilehash: dd9010e055e5e24cafb87846b8eed98f54d83474
ms.sourcegitcommit: ef80c461713fff1a75998766e7a4ed3a7c6121d0
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 02/15/2022
ms.locfileid: "8147846"
---
# <a name="about-finished-production-order-costs"></a>About Finished Production Order Costs

Finishing the production order is an important task in completing the costing lifecycle of the item that is being produced. Final costs, including variances in a standard cost environment, actuals in a FIFO, Average, or LIFO cost environment, are calculated using the **Adjust Cost - Item Entries** batch job, which allows for financial reconciliation of the costs of item production. For a production order to be considered for cost adjustment, the status must be **Finished**. It is therefore critical that upon completion, the status of a production order is changed to **Finished**.  

## <a name="example"></a>Example

In a standard cost environment, when you consume material to produce an item, stated simply, the cost of the item plus labour and overhead go into WIP. When the item is produced, WIP is reduced by the amount of the standard cost of the item. Typically, these costs do not net to zero. So that these costs can net to zero, you must run the **Adjust Cost - Item Entries** batch job, noting that only production orders with the status of **Finished** will be considered for adjustment.  

## <a name="see-also"></a>See Also

[Managing Inventory Costs](finance-manage-inventory-costs.md)  
[Manufacturing](production-manage-manufacturing.md)  
[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]