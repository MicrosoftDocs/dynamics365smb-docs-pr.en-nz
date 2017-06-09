---
title: 'How to: Find Posted Documents without Incoming Document Records| Microsoft Docs'
description: 'How to: Find Posted Documents without Incoming Document Records'
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: electronic document, e-invoice, incoming document, OCR, ecommerce, document exchange, import invoice
ms.date: 05/12/2016
ms.author: sgroespe
ms.translationtype: Human Translation
ms.sourcegitcommit: a31be0f9d07e2abb591e26f6bae34c6f6e4dcda6
ms.openlocfilehash: e0925bde31e7079ca9f3d0f7acb16d4dd75c1987
ms.contentlocale: en-nz
ms.lasthandoff: 05/04/2017


---
# <a name="how-to-find-posted-documents-without-incoming-document-records"></a>How to: Find Posted Documents without Incoming Document Records
From the **Chart of Accounts** and **General Ledger Entries** windows, you can use a search function to find general ledger entries for posted purchase and sales documents that do not have incoming document records and then centrally link to existing records or create new ones with attached document files.

## <a name="to-find-posted-documents-without-incoming-document-records"></a>To find posted documents without incoming document records
1. In the top right corner, choose the **Search for Page or Report** icon ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon"), enter **Chart of Accounts**, and then choose the related link.
2. Select a line for a G/L account for whose general ledger entries you want to see posted purchase and sales documents without incoming document records, and then choose the **Posted Documents without Incoming Document** action.
3. Alternatively, choose the **Ledger Entries** action.
4. In the **General Ledger Entries** window, choose the **Posted Documents without Incoming Documents** action.

The **Posted Documents without Incoming Document** window opens showing posted purchase and sales documents without incoming document records represented by general ledger entries on the G/L account that you opened the window for. The window can show a maximum of 1000 lines. By default, the **Date Filter** field therefore contains a filter that limits the lines to entries with posting dates from the beginning of the accounting period to the work date.

## <a name="to-connect-found-documents-to-existing-incoming-document-records"></a>To connect found documents to existing incoming document records
1. In the **Posted Documents without Incoming Document** window, select the line for a posted document that you want to connect to an existing incoming document record, and then choose the **Select Incoming Document** action.
2. In the **Incoming Documents** window, select the incoming document record that you want to connect to posted document found, and then choose the **OK** button.
3. In the **Posted Documents without Incoming Document** window, the selected incoming document record is now connected to the posted document, as you can see in the **Incoming Document Files** FactBox.

If a relevant incoming document record does not exist in the **Incoming Documents** window, then you can create it. For more information, see [How to: Create Incoming Document Records](across-how-create-income-document-records.md).

## <a name="see-also"></a>See Also
[Process Incoming Documents](across-process-income-documents.md)  
[Incoming Documents](across-income-documents.md)  
[Purchasing](purchasing-manage-purchasing.md)  
[Working With [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

