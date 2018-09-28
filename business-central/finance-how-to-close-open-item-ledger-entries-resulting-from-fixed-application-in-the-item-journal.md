---
title: How to Close Open Item Ledger Entries Resulting from Fixed Application in the Item Journal | Microsoft Docs
description: You can use the **Applies-from Entry** field in the **Item Journal** window to create a fixed application between an inbound transaction and the original outbound transaction. For example, to correct the outbound transaction or to process its return.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: f879688bd458714f354b2e98e58ce78686cf79d9
ms.contentlocale: en-nz
ms.lasthandoff: 03/22/2018

---
# <a name="close-open-item-ledger-entries-resulting-from-fixed-application-in-the-item-journal"></a>Close Open Item Ledger Entries Resulting from Fixed Application in the Item Journal
You can use the **Applies-from Entry** field in the **Item Journal** window to create a fixed application between an inbound transaction and the original outbound transaction. For example, to correct the outbound transaction or to process its return. For more information, see Applies-from Entry.  

> [!IMPORTANT]  
>  Fixed applications made in this manner only apply the cost, not the quantity. Accordingly, the posted positive item ledger entry will not close the applied outbound entry and will itself remain open. This also applies when you post a fixed application for a positive entry to a negative entry that has not been closed by a regular positive entry, then both the negative and the positive entries will remain open.  
>   
>  This also means that you cannot close an inventory period if such an entry exists.  

The following procedure shows how to close such entries by performing two corrective postings in the item journal.  

## <a name="to-close-open-item-ledger-entries-that-result-from-a-fixed-application-in-the-item-journal"></a>To close open item ledger entries that result from a fixed application in the item journal  

1.  Use the **Applies-from Entry** field to post a positive adjustment with the corresponding quantity. This closes the original negative entry with a fixed application.  
2.  Use the **Applies-to Entry** field to post a negative adjustment. This closes the original corrective positive entry with a fixed application.  

## <a name="see-also"></a>See Also  
[ Remove and Reapply Item Ledger Entries](finance-how-to-remove-and-reapply-item-entries.md)  
 [Process Sales Returns and Cancellations](sales-how-process-sales-returns-cancellations.md)   
 [Setting Up Inventory Valuation and Costing](finance-set-up-inventory-valuation-and-costing.md)   
 [Managing Inventory Costs](finance-manage-inventory-costs.md)   
 [Design Details: Costing Methods](design-details-costing-methods.md)

