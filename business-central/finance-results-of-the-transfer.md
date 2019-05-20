---
title: Results of the Transfer | Microsoft Docs
description: This topic describes what happens after you transfer general ledger entries to cost entries.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: general ledger, transfer, cost entries
ms.date: 04/01/2019
ms.author: sgroespe
redirect_url: finance-transfer-and-post-cost-entries
ms.openlocfilehash: 590c1501f9da2c7c343b5c2f3617df873fcd3b7a
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 04/29/2019
ms.locfileid: "1242507"
---
# <a name="results-of-transferring-general-ledger-entries-to-cost-entries"></a>Results of Transferring General Ledger Entries to Cost Entries
During the transfer of general ledger entries to cost entries, [!INCLUDE[d365fin](includes/d365fin_md.md)] creates connections in the entries in the **G/L Entry** table, the **Cost Entry** table, and the **Cost Register** table to make it possible to trace the connections between cost entries and general ledger entries.  

## <a name="general-ledger-entries"></a>General Ledger Entries  
For each general ledger entry that is transferred to cost accounting, [!INCLUDE[d365fin](includes/d365fin_md.md)] fills the cost **Entry No.** field.  

## <a name="cost-entries"></a>Cost Entries  
For each cost entry, [!INCLUDE[d365fin](includes/d365fin_md.md)] saves the entry number of the corresponding general ledger entry in the **G/L Entry No.** field in the **Cost Entry** table.  

For combined cost entries, [!INCLUDE[d365fin](includes/d365fin_md.md)] saves the entry number of the last general ledger entry, which is the entry with the highest entry number.  

The **G/L Account** field in the **Cost Entry** table contains the number of the general ledger account that the cost entry came from.  

For single cost entries, [!INCLUDE[d365fin](includes/d365fin_md.md)] transfers the posting text from the general ledger entry to the **Description** text field. For combined entries, the text field shows these entries are transferred as combined entries. For example, for a combined entry for the month of October in 2013, the text can be **Combined Entries, October 2013**.  

## <a name="cost-register"></a>Cost Register  
In the **Cost Register** table, [!INCLUDE[d365fin](includes/d365fin_md.md)] creates an entry with the source transfer from general ledger. The entry records the first and last entry numbers of the general ledger entries that are transferred, in addition to the first and last entry numbers of the cost entries that are created.  

## <a name="see-also"></a>See Also  
[Transferring and Posting Cost Entries](finance-transfer-and-post-cost-entries.md)   
