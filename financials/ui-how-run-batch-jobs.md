---
title: Create and Run a Batch Job | Microsoft Docs
description: You run batch jobs to process data and update information, for example, to do periodic accounting activities, or to do calculations.
services: project-madeira
documentationcenter: 
author: SusanneWindfeldPedersen
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: task, process
ms.date: 03/29/2017
ms.author: solsen
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: 6844d5fe3efba5349eef166161c5956116bc7fc0
ms.contentlocale: en-nz
ms.lasthandoff: 07/07/2017


---
# <a name="how-to-run-batch-jobs"></a>How to: Run Batch Jobs
A batch job is a routine that processes data in batches, for example the **Adjust Exchange Rates** batch job. There are batch jobs that perform periodic accounting activities, such as closing the income statement at the end of a fiscal year. Many batch jobs do calculation work, such as calculation of finance charges, exchange rate adjustment, and calculation of unit prices.

A batch job is like a report, except the batch job uses the result of its work to update information directly, instead of printing the results.

## <a name="to-run-a-batch-job"></a>To run a batch job
1. To open the request window for the relevant batch job, choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter the name of the batch job, and then choose the related link.
2. If there is an **Options** FastTab for the batch job, fill in the fields to determine what the batch job will do.
3. The window may contain one or more FastTab with filters, which you can use to limit the data included in the batch job. You can enter criteria in the suggested filters or add more filters.
4. Choose the **OK** button to start the batch job.

## <a name="see-also"></a>See Also
[Entering Criteria in Filters](ui-enter-criteria-filters.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

