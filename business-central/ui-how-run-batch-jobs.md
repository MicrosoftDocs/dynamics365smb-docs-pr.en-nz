---
title: Create and Run a Batch Job | Microsoft Docs
description: You run batch jobs to process data and update information, for example, to do periodic accounting activities, or to do calculations.
services: project-madeira
documentationcenter: 
author: SusanneWindfeldPedersen
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: task, process
ms.date: 10/01/2018
ms.author: solsen
ms.translationtype: HT
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: 9a6435120d122db894bcd6c953da5ab8ea78420b
ms.contentlocale: en-nz
ms.lasthandoff: 09/28/2018

---
# <a name="run-batch-jobs"></a>Run Batch Jobs
A batch job is a routine that processes data in batches, for example the **Adjust Exchange Rates** batch job. There are batch jobs that perform periodic accounting activities, such as closing the income statement at the end of a fiscal year. Many batch jobs do calculation work, such as calculation of finance charges, exchange rate adjustment, and calculation of unit prices.

A batch job is like a report, except the batch job uses the result of its work to update information directly, instead of printing the results.

## <a name="to-run-a-batch-job"></a>To run a batch job
1. To open the request window for the relevant batch job, choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter the name of the batch job, and then choose the related link.
2. If there is an **Options** FastTab for the batch job, fill in the fields to determine what the batch job will do.
3. The window may contain one or more FastTab with filters, which you can use to limit the data included in the batch job. You can enter criteria in the suggested filters or add more filters.
4. Choose the **OK** button to start the batch job.

## <a name="see-also"></a>See Also
[Searching, Filtering, and Sorting Data](ui-enter-criteria-filters.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

