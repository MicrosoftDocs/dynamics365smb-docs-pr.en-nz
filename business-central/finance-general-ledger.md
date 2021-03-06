---
title: Learn About General Ledger and COA| Microsoft Docs
description: Describes the general ledger, the chart of accounts, and account categories.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: analysis, history, track
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: dbeb9f9cbe0eff61b28dc4d371a1f8d9031ea1b4
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 12/17/2020
ms.locfileid: "4747057"
---
# <a name="understanding-the-general-ledger-and-the-coa"></a>Understanding the General Ledger and the COA

The general ledger stores your financial data, and the chart of accounts shows the accounts that all general ledger entries are posted to. [!INCLUDE[prod_short](includes/prod_short.md)] includes a standard chart of accounts that is ready to support your business.

## <a name="general-ledger-setup-and-general-posting-setup"></a>General Ledger Setup and General Posting Setup

The setup of the general ledger is at the core of financial processes because it defines how you post data.  

On the **General Ledger Setup** page, you specify how to handle certain accounting issues in your company, such as:  

* Invoice rounding details  
* Address formats  
* Financial reporting  

Similarly, on the **General Posting Setup** page, you specify how you want to set up combinations of general business and general product posting groups. Posting groups map entities like customers, vendors, items, resources, and sales and purchase documents to general ledger accounts. You fill in a line for each combination of business posting group and product posting group. For more information, see [Posting Group Setups](finance-posting-groups.md).  

> [!TIP]
> The **General Ledger Setup** page includes generic fields and fields that are particular to your country or region. If you are not sure of the meaning of a field, we suggest you work with your accountant to determine whether it is of relevance to your organisation.  

## <a name="the-chart-of-accounts"></a>The Chart of Accounts

The chart of accounts shows all general ledger accounts. From the chart of accounts, you can do things like:  

* View reports that show general ledger entries and balances.  
* Close your income statement.  
* Open the G/L account card to add or change settings.  
* See a list of posting groups that post to that account.
* View separate debit and credit balances for a single account  

You can add, change, or delete general ledger accounts. However, to prevent discrepancies, you can't delete a general ledger account if it's data is used in the chart of accounts.  

## <a name="account-categories"></a>Account Categories

You can personalise the structure of your financial statements by mapping general ledger accounts to account categories.  

The **G/L Account Categories** page shows your categories and subcategories, and the G/L accounts that are assigned to them. You can create new subcategories and assign those categories to existing accounts.  

You create a category group by indenting other subcategories under a line on the **G/L Account Categories** page. This makes it easy for you to get an overview, because each grouping shows a total balance. For example, you can create subcategories for different types of assets, and then create category groups for fixed assets versus current assets.  

You can specify whether the accounts in each subcategory must be included in specific types of reports. The account categories help define the layout of your financial statements.  

For example, the default balance statement has a subcategory for Cash under Current Assets. If you want the balance statement consider petty cash and chequing, you can:  

1. Add two new subcategories. One for petty cash, and one for your current account.  
2. Specify the additional report definition **Cash Accounts** for these subcategories.  
3. Indent them under the **Cash** subcategory.  

The next time you generate account schedules your balance statement will show a total balance for cash and two lines with balances for petty cash and the current account.  

## <a name="see-also"></a>See Also

[Finance](finance.md)  
[Setting Up or Changing the Chart of Accounts](finance-setup-chart-accounts.md)  
[Business Intelligence](bi.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]