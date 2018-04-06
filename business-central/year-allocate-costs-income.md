---
title: Overview of Tasks to Allocate Costs and Income | Microsoft Docs
description: Outlines the tasks to allocate an entry in a general journal to several different accounts when you post the journal.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 06/07/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 31f8d40d5a8cf8d190f4a6cb655f09ca72f3e070
ms.contentlocale: en-nz
ms.lasthandoff: 03/22/2018

---
# <a name="allocate-costs-and-income"></a>Allocate Costs and Income
You can allocate an entry in a general journal to several different accounts when you post the journal. The allocation can be made by three different methods:

* Quantity
* Percentage (%)
* Amount

The allocation features can be used with recurring general journals and in fixed assets journals.
<!--You can also distribute the cost or revenue of a line to an intercompany partner when you post a sales or purchase document. When you post the document, a line will be posted in your general journal, and a corresponding line will be created in the intercompany outbox.-->

The following procedures describe how to prepare to allocate costs in a recurring general journal by defining allocation keys. When allocation keys are defined, you complete and post the journal like any other recurring general journal. For more information, see [Working with General Journals](ui-work-general-journals.md).

## <a name="to-set-up-allocation-keys"></a>To set up allocation keys
You can allocate an entry in a recurring general journal to several different accounts when you post the journal. The allocation can be made by quantity, percentage, or amount.
1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Recurring General Journal**, and then choose the related link.
2. Choose the **Batch Name** field to open the **General Journal Batches** window.
3. You can either modify allocations on an existing batch in the list or create a new batch with allocations.
   * To create a new batch, choose the **New** action, and go to the next step.
   * To change the allocations of an existing journal, select the journal and go to step 7.    
4. In the **Name** field, enter a name for the batch, such as CLEANING. In the **Description** field, enter a description, such as Cleaning Expenses Journal.
5. When you are done, close the window. A new, empty recurring journal opens.
6. Fill in the fields on the line.
7. Choose the **Allocations** action.
8. Add a line for each allocation. You must fill in either the **Allocation %**, **Allocation Quantity**, or **Amount** field. You must also fill in the **Account No.** field and, if you are allocating the transaction among global dimensions, the global dimension fields.
9. If you enter a percentage on a line, the amount in the **Amount** field is calculated automatically. These amounts have the opposite sign from the total amount in the **Amount** field in the recurring journal.
10. After entering the allocations lines, choose **OK** to return to the **Recurring General Journal** window. The **Allocated Amt. (NZD)** field is filled in and matches the **Amount** field.
11. Post the journal.

## <a name="to-change-an-allocation-key-that-has-already-been-set-up"></a>To change an allocation key that has already been set up
1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Recurring General Journal**, and then choose the related link.
2. In the **Recurring General Journal** window, select the journal with the allocation.
3. Choose the line with the allocation, and then choose **Allocations** action.
4. Change the relevant fields, and then choose the **OK** button.

## <a name="see-also"></a>See Also
[Closing Years and Periods](year-close-years-periods.md)  
[Working with General Journals](ui-work-general-journals.md)    
[Posting Documents and Journals](ui-post-documents-journals.md)    
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

