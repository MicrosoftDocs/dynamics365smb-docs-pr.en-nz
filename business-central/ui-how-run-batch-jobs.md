---
title: Run Batch Jobs and XMLports
description: You run batch jobs to process data and update information, for example, to do periodic accounting activities, or to do calculations.
author: SusanneWindfeldPedersen
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: task, process
ms.search.form: 672, 676, 682, 9020, 9022, 9026, 9027, 9030, 9000, 9004, 9005, 9018, 9006, 9007, 9010, 9016, 9017
ms.date: 04/01/2021
ms.author: solsen
ms.openlocfilehash: 7d06ebd368f42c142d7cb222ee378da79706132e
ms.sourcegitcommit: cdb57f14960f58b1d36a1b373fbf35dfed5fad9e
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 02/23/2022
ms.locfileid: "8335412"
---
# <a name="run-batch-jobs-and-xmlports"></a>Run Batch Jobs and XMLports

A batch job is a routine that processes data in batches, for example the **Adjust Exchange Rates** batch job. There are batch jobs that perform periodic accounting activities, such as closing the income statement at the end of a financial year. Many batch jobs do calculation work, such as calculation of finance charges, exchange rate adjustment, and calculation of unit prices.

A batch job is like a report, except the batch job uses the result of its work to update information directly, instead of printing the results.

You can schedule when a batch job runs. For more information, see [Use Job Queues to Schedule Tasks](admin-job-queues-schedule-tasks.md).

## <a name="to-run-a-batch-job"></a>To run a batch job
1. To open the request page for the relevant batch job, choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter the name of the batch job, and then choose the related link.
2. If there is an **Options** FastTab for the batch job, fill in the fields to determine what the batch job will do.
3. The page may contain one or more FastTab with filters, which you can use to limit the data included in the batch job. You can enter criteria in the suggested filters or add more filters.
4. Choose the **OK** button to start the batch job.

## <a name="see-also"></a>See Also
[Sorting, Searching, and Filtering Lists](ui-enter-criteria-filters.md)  
[Use Job Queues to Schedule Tasks](admin-job-queues-schedule-tasks.md)  
[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]