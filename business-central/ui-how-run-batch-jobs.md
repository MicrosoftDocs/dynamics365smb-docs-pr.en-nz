---
title: Create and Run a Batch Job | Microsoft Docs
description: You run batch jobs to process data and update information, for example, to do periodic accounting activities, or to do calculations.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: task, process
ms.date: 04/01/2019
ms.author: solsen
ms.openlocfilehash: 0b9bf37f9054d767938b851e399a1b2c347f77c3
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 04/29/2019
ms.locfileid: "1249277"
---
# <a name="run-batch-jobs"></a>Run Batch Jobs
A batch job is a routine that processes data in batches, for example the **Adjust Exchange Rates** batch job. There are batch jobs that perform periodic accounting activities, such as closing the income statement at the end of a fiscal year. Many batch jobs do calculation work, such as calculation of finance charges, exchange rate adjustment, and calculation of unit prices.

A batch job is like a report, except the batch job uses the result of its work to update information directly, instead of printing the results.

## <a name="to-run-a-batch-job"></a>To run a batch job
1. To open the request page for the relevant batch job, choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter the name of the batch job, and then choose the related link.
2. If there is an **Options** FastTab for the batch job, fill in the fields to determine what the batch job will do.
3. The page may contain one or more FastTab with filters, which you can use to limit the data included in the batch job. You can enter criteria in the suggested filters or add more filters.
4. Choose the **OK** button to start the batch job.

## <a name="see-also"></a>See Also
[Sorting, Searching, and Filtering Lists](ui-enter-criteria-filters.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
