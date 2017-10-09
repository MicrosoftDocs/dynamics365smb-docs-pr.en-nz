---
title: Posting Group Setup| Microsoft Docs
description: Overview of the posting groups you can use to save time and avoid mistakes when you post transactions.
services: project-madeira
documentationcenter: 
author: bholtorf
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: posting setup, initialize
ms.date: 06/02/2017
ms.author: bholtorf
ms.translationtype: HT
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: add78070e838dcf8b0eb24dcc8b642d621a400b9
ms.contentlocale: en-nz
ms.lasthandoff: 09/22/2017

---
# <a name="setting-up-posting-groups"></a>Setting Up Posting Groups
Posting groups map entities like customers, vendors, items, resources, and sales and purchase documents to general ledger accounts. They save time and help avoid mistakes when you post transactions. The transaction values go to the accounts specified in the posting group for that particular entity. The only requirement is that you have a chart of accounts. For more information, see [Set Up the Chart of Accounts](finance-setup-chart-accounts.md).  

Posting groups are covered under three umbrellas:  

* General - Define who you sell to and buy from, and what you sell and what you buy. You can also combine groups to specify things like the income statement accounts to post to, or use groups to filter reports.  
* Specific - Use sales documents, for example, instead of posting directly to the general ledger. When you create entries in the customer ledger, corresponding entries are made in the general ledger.  
* Tax - Define the tax percentages and calculation types that apply to who you sell to and buy from, and what you sell and what you buy.

The following tables describe the posting groups under each umbrella.  

| General Posting Groups | Description |
| --- | --- |
| General Business Posting Groups |Assign this group to customers and vendors to specify who you sell to, and who you buy from. Set these up in the **Gen. Business Posting Groups** window. When you do, think about how many groups you'll need to break down sales and purchases. For example, group customers and vendors by geographical area, or by the type of business. |
| General Product Posting Groups |Assign this group to items and resources to specify what you sell, and what you buy. Set these up in the **Gen. Product Posting Groups** window. When you do, consider the number of groups you'll need to break down sales by product (items and resources) and purchases by items. For example, divide these groups by raw materials, retail, resources, capacity, and so on. |
| General Posting Setups |Combine business and product posting groups and choose the accounts to post to. For each combination of business and product posting groups, you can assign a set of general ledger accounts. For example, this means you can post the sale of the same item to different sales accounts in the general ledger because customers are assigned to different business posting groups. Set these up in the **General Posting Setup** window. |

| Specific Posting Groups | Description |
| --- | --- |
| Customer Posting Groups |Define the accounts to use when you post accounts receivable transactions. If you use inventory with receivables, the general business posting group assigned to your customer, and the general product posting group assigned to the inventory item determine the accounts the sales order lines post to. Set these up in the **Customer Posting Groups** window. |
| Vendor Posting Groups |Define where to post transactions for payables accounts, service charge accounts, and payment discount accounts. This is similar to customer posting groups. Set these up in the **Vendor Posting Groups** window. |
| Inventory Posting Groups |Define balance sheet inventory accounts. These also provide a good way to organise your inventory, so you can separate items by their posting group when you generate reports. Set these up in the **Inventory Posting Groups** window. |
| Bank Account Posting Groups |Define accounts for bank accounts. For example, this can simplify the processes of tracing transactions and reconciling bank accounts. Set these up in the **Bank Account Posting Groups** window. |
| Fixed Assets Posting Groups |Define accounts for different types of expenses and costs, such as acquisition costs, accumulated depreciation amounts, acquisition costs on disposal, accumulated depreciation on disposal, gains on disposal, losses on disposal, maintenance expenses, and depreciation expenses. Set these up in the **FA Posting Groups** window. |

| Tax Posting Group | Description |
| --- | --- |
| Tax Business Posting Groups |Determine how to calculate and post sales tax for customers and vendors. Set these up in the **Tax Business Posting Groups** window. When you do, think about how many groups you need. For example, this can depend on factors like local legislation, and whether you trade both domestically and internationally. |
| Tax Product Posting Groups |Indicate the tax calculations needed for the types of items or resources you buy or sell. |
| Tax Posting Setup |Combine tax business posting groups and tax product posting groups. When you fill in a general journal line, purchase line, or sales line, we'll look at the combination to identify the accounts to use. |

## <a name="example-of-linking-posting-groups"></a>Example of linking posting groups
Here's a scenario.  

These posting groups are chosen on the customer card:  

* General business posting group
* Customer posting group  

These posting groups are chosen on the item card:  

* General product posting group  
* Inventory posting group  

When you create a sales document, the sales header uses the customer card information, and the sales lines use the item card information.  

* The revenue posting (income statement) is determined by the combination of the general business posting group and the general product posting group.  
* The accounts receivable posting (balance sheet) is determined by the customer posting group.  
* The inventory posting (balance sheet) is determined by the inventory posting group.  
* The cost of goods sold posting (income statement) is determined by the combination of general business posting group and general product posting group.  

Your setup determines when posting happens. For example, the timing is affected by when you do periodic activities, such as posting inventory cost or adjusting cost item entries.

## <a name="copying-posting-setup-lines"></a>Copying posting setup lines
The more product and business posting groups you have, the more lines you see in the General Posting Setup window. This can mean a lot of data entry to set up the general posting setup for the company. While there may be many different combinations of business and product posting groups, different combinations may still post to the same general ledger accounts. To limit the amount of manual entry, copy the general ledger accounts from an existing line in the **General Posting Setup** window.

## <a name="see-also"></a>See also 
[The General Ledger and the Chart of Accounts](finance-general-ledger.md)  
[Setting Up Finance](finance-setup-finance.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

