---
title: Defining the Relationship Between Cost Types and General Ledger Accounts | Microsoft Docs
description: Learn how to define the relationship between the cost type and the general ledger account.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: cost types, general ledger
ms.date: 11/13/2018
ms.author: sgroespe
redirect_url: finance-transfer-and-post-cost-entries
ms.openlocfilehash: f80e9b6276d26adffb5e3208ffefbf98d7f7ff96
ms.sourcegitcommit: 1bcfaa99ea302e6b84b8361ca02730b135557fc1
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 03/08/2019
ms.locfileid: "821985"
---
# <a name="defining-the-relationship-between-cost-types-and-general-ledger-accounts"></a>Defining the Relationship Between Cost Types and General Ledger Accounts
The relationship between the cost type and the general ledger account is created in the cost type and in the general ledger account.  

* The **G/L Account Range** field in the **Cost Type** table establishes which general ledger accounts belong to a cost type.  
* The **Cost Type No.** field in the chart of accounts establishes which cost type a general ledger account belongs to.  

These two fields are filled automatically when you use the **Get Cost Types from Chart of Accounts** function.  

## <a name="relationship-between-general-ledger-accounts-and-cost-types"></a>Relationship Between General Ledger Accounts and Cost Types  
There is an n:1 relationship between general ledger accounts and cost types. Several general ledger accounts can belong to one cost type, but each general ledger account belongs to only one cost type. The following table describes the details in the relationship.  

|Relationship|**G/L Account Range**|**Cost Type No.**|  
|------------------|------------------------------------------------|-------------------------------------------|  
|One general ledger account for each cost type|One general ledger account|One cost type|  
|Several general ledger accounts for one cost type|General ledger account range, for example, 7110..7193 for each general ledger account|For each general ledger account in the range, there is only one cost type|  
|Cost types without corresponding general ledger accounts|<Empty>||  
|General ledger accounts whose entries will not be transferred||<Empty>|  

## <a name="cost-types-without-a-relationship-to-the-general-ledger"></a>Cost Types Without a Relationship to the General Ledger  
A cost type may not have a relationship to general ledger accounts if one of the following conditions is true:  

* Accounts for operational accounting, such as Calc. Interest and Depreciation, only take costs from the operational accounting.  
* Helping cost types, such as cost types 9901, 9902, and 9903 in the [!INCLUDE[d365fin](includes/d365fin_md.md)] database, are used as credit and debit accounts for allocations.  
* The helping account, 9920 in the [!INCLUDE[d365fin](includes/d365fin_md.md)] database, contains actual accruals that show the difference between costs and the expense from the general ledger.  

## <a name="see-also"></a>See Also  
[Accounting for Costs](finance-manage-cost-accounting.md)  
[Setting Up Cost Accounting](finance-set-up-cost-accounting.md)   
[About Cost Accounting](finance-about-cost-accounting.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
