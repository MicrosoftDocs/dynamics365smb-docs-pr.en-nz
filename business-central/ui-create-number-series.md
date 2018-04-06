---
title: Create Number Series | Microsoft Docs
description: Learn how to set up number series that assign unique ID codes to accounts and documents in Business Central .
documentationcenter: 
author: SusanneWindfeldPedersen
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: numbers, numbering
ms.date: 06/02/2017
ms.author: solsen
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 151e585b0a809b1b537b52089fce297f222a60dc
ms.contentlocale: en-nz
ms.lasthandoff: 03/22/2018

---
# <a name="create-number-series"></a>Create Number Series
For each company that you set up, you need to assign unique identification codes to things such as general ledger accounts, customer and vendor accounts, invoices, and other documents. Numbering is important not only for identification. A well-designed numbering system also makes the company more manageable and easy to analyse, and can reduce the number of errors that occur in data entry.

> [!NOTE]  
>   We recommend that you use the same number series codes as you see listed in the **No. Series List** window in the CRONUS demonstration company. Codes such as *P-INV+* might not make immediate sense to you, but [!INCLUDE[d365fin](includes/d365fin_md.md)] has a number of default settings that depend on these number series codes.

You create a numbering system by setting up one or more codes for each type of master data or document. For example, you can set up one code for numbering customers, another code for numbering sales invoices, and another code for numbering documents in general journals. After you have set up a code, you set must set up at least one number series line. The number series line contains information such as the first and last number in the series and the starting date. You can set up more than one number series line per number series code, with a different starting date for each line. The series will be used consecutively, starting each series on the respective starting date.

You typically set up your number series to automatically insert the next consecutive number on new cards or documents that you create. However, you can also set a number series up to allow that you manually enter the new number. You specify this with the **Manual Nos.** check box.

If you want to use more than one number series code for one type of master data - for example, if you want to use different number series for different categories of items - you can use number series relationships.

## <a name="to-create-a-new-number-series"></a>To create a new number series
1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **No. Series**, and then choose the related link.
2. Choose the **New** action.
3. On the new line, fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

**TIP**: To allow manual entry of a number on new cards or documents, deselect the **Default Nos.** check box and select the **Manual Nos.** check box.

Now when you create a new card or document that is set up to use the number series in question, you can manually fill in the **No.** field with any value.  

## <a name="to-set-up-where-a-number-series-is-used"></a>To set up where a number series is used
The following procedure shows how to set number series up for the Sales area. The steps are similar for other areas.
1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sales & Receivables**, and then choose the related link.
2. In the **Sales & Receivables** window, on the **Number Series** FastTab, select the desired number series for each sales card or document.

The selected number will now be used to fill in the **No.** field on the card or document in question, according to the settings you made on the number series line.

## <a name="to-create-relationships-between-number-series"></a>To create relationships between number series
If you have set up more than one number series code for the same kind of basic information or transactions, you can create relationships between the codes. This feature can assist you in deciding among the codes when you use a number.

1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **No. Series**, and then choose the related link.
2. Select the line with the number series you want to create relationships for and then choose **Relationships**.
3. In the **Series Code** field, enter the code for the number series that you want to relate to the series you selected in step 2.
4. Add a line for each code that you want to relate to the selected number series.
5. Close the window.

Now when you set up something that requires a number, you can use the relationships you created to select among the related number series.

## <a name="see-also"></a>See Also
[Setting Up [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

