---
title: 'How to: Manage Many Incoming Document Records| Microsoft Docs'
description: 'How to: Create Incoming Document Records'
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
ms.openlocfilehash: 821efd8c95d05fc5d93c79dd75942f61daa91683
ms.contentlocale: en-nz
ms.lasthandoff: 05/04/2017


---
# <a name="how-to-manage-many-incoming-document-records"></a>How to: Manage Many Incoming Document Records
As you create or process incoming document records, the number of lines in the **Incoming Documents** window may grow to an extent where you lose overview. Therefore, you can set incoming document records to Processed to remove them from the default view. When you choose the **Show All** action, you can view both processed and unprocessed records.

**Note**: You cannot edit information, attach files, or perform other processes on incoming document records that are set to Processed. You must first set it to Unprocessed.

The **Processed** check box is automatically selected on incoming document records that have been processed, but you can also select or deselect the check box manually. Depending on your business process, an incoming document record may be processed when a related document has been created for it or a file has been attached.

**Note**: When you open the **Incoming Documents** window with the **My Incoming Documents** action on the Role Centre, only unprocessed incoming document records are shown by default. This is referred to in this topic as "the default view".

## <a name="to-remove-incoming-document-records-from-the-default-view"></a>To remove incoming document records from the default view
1. In the **Incoming Documents** window, select one or more lines for incoming document records that you want to remove from the default view.
2. Choose the **Set to Processed** action.

The incoming document records are removed from the default view, and the **Processed** check box is selected on the lines.

**Note**: You can also perform this action for the individual record in the **Incoming Document Card** window.

## <a name="to-view-all-incoming-document-records"></a>To view all incoming document records
1. In the **Incoming Documents** window, choose the **Show All** action.

All incoming document records are displayed, including those where the **Processed** check box is not selected.

## <a name="to-add-incoming-document-records-to-the-default-view"></a>To add incoming document records to the default view
1. In the **Incoming Documents** window, choose the **Show All** action.
2. Select one or more lines for incoming document records that you want to appear in the default view.
3. Choose the **Set to Unprocessed** action.  

**Note**: You can also perform this action for the individual record in the **Incoming Document Card** window.

## <a name="see-also"></a>See Also
[Process Incoming Documents](across-process-income-documents.md)  
[Incoming Documents](across-income-documents.md)  
[Purchasing](purchasing-manage-purchasing.md)  
[Working With [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

