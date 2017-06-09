---
title: Dimensions| Microsoft Docs
description: Using dimensions to analyse data.
services: project-madeira
documentationcenter: 
author: bholtorf
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: analysis, history, track
ms.date: 03/24/2017
ms.author: bholtorf
ms.translationtype: Human Translation
ms.sourcegitcommit: a31be0f9d07e2abb591e26f6bae34c6f6e4dcda6
ms.openlocfilehash: 7552ee2b3398c203a7f3295f3203c83914fbb15f
ms.contentlocale: en-nz
ms.lasthandoff: 05/04/2017


---
# <a name="dimensions"></a>Dimensions
To make it simpler to perform analysis on documents such as sales orders, you can use dimensions. Dimensions are attributes and values that categorise entries so you can track and analyse them. For example, dimensions can indicate the project or department an entry came from.  

For example, instead of setting up separate general ledger accounts for each department and project, you can use dimensions. This gives a rich opportunity for analysis, without creating a complicated chart of accounts.  

Another example is to set up a dimension called *Department*, and use this dimension when you post sales documents. This will let you use business intelligence tools to see which department sold which items.
The more dimensions you use, the more detailed reports you can base your business decisions on. For example, a single sales entry can include multiple dimension information, such as:  

* The account the item sale was posted to  
* Where the item was sold
* Who sold it
* The kind of customer who bought it  

You can create as many dimensions with as many values as you want.  

**Note**: This functionality requires that your experience is set to **Suite**. For more information, see [Customizing Your [!INCLUDE[d365fin](includes/d365fin_md.md)] Experience](ui-experiences.md).

## <a name="using-dimensions"></a>Using Dimensions
In a document such as a sales order, you can add dimension information for both an individual document line and the document itself. For example, in the **Sales Order** window, you can enter dimension values for the first two shortcut dimensions on the individual sales lines, and you can add more dimension information if you choose the **Dimensions** button.  

If you work in a journal instead, you can add dimension information to an entry in the same way, if you have set up shortcut dimensions as fields directly on journal lines.  

You can set up default dimensions for accounts or account types, so that dimensions and dimension values are filled in automatically.  

## <a name="dimension-sets"></a>Dimension Sets
A dimension set is a unique combination of dimension values. It is stored as dimension set entries in the database. Each dimension set entry represents a single dimension value. The dimension set is identified by a common dimension set ID that is assigned to each dimension set entry that belongs to the dimension set.  

When you create a journal line, document header, or document line, you can specify a combination of dimension values. Instead of explicitly storing each dimension value in the database, a dimension set ID is assigned to the journal line, document header, or document line to specify the dimension set.  

## <a name="see-also"></a>See Also
[Finance](finance.md)  
[Setting Up Dimensions](finance-setup-dimensions.md)  
[Working With [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

