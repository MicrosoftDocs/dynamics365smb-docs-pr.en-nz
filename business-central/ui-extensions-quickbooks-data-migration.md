---
title: Using the QuickBooks Migration Extension | Microsoft Docs
description: Describes how to use the extension to import customers, vendors, items, and accounts from QuickBooks Desktop to Business Central.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: app, add-in, manifest, customize, import, implement
ms.date: 10/01/2018
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: add32e82465610830b68a979e238103bfa10d438
ms.openlocfilehash: e5cb755b6a15070410c42328ccf08b784928f3ca
ms.contentlocale: en-nz
ms.lasthandoff: 11/29/2018

---

# <a name="the-quickbooks-data-migration-extension"></a>The QuickBooks Data Migration Extension
This extension makes it easy to migrate customers, vendors, items, and accounts from QuickBooks to [!INCLUDE[d365fin](includes/d365fin_md.md)]. If your business uses QuickBooks today, you can export the relevant information and then open an assisted setup guide to upload the data to [!INCLUDE[d365fin](includes/d365fin_md.md)].  
For more information, see [Importing Business Data from Other Finance Systems](across-import-data-configuration-packages.md).

## <a name="data-from-quickbooks-desktop"></a>Data from QuickBooks Desktop
 
You can import the following data from QuickBooks Online to Business Central:

- Customers  
- Vendors  
- Items  
- Chart of Accounts  
- Beginning Balance transactions in General Ledger  
- On-hand Quantities for Inventory Items  
- Open documents for customers and vendors, such as invoices, credit memos and payments  

We migrate only full amounts on sales and purchase documents. We do not update partially paid amounts. For example, if a customer has paid 300 of a total of 500 dollars on a sales invoice, we migrate the full 500. If you have received partial payments, you must update these manually, either before or after you migrate data. We recommend that you apply outstanding transactions before you migrate, just to make things easier afterward.

> [!NOTE]
> We do not migrate purchase orders or sales orders.

## <a name="before-you-start"></a>Before You Start
An important part of the migration process is to specify the accounts to migrate transactions to. It's a good idea to plan this mapping before you migrate data. For example, the accounts where you post transactions for:

- The sale of items or services to customers  
- The purchase of items or services from vendors  
- Adjustments in the general ledger  

Business Central requires that general ledger accounts have account numbers assigned to them. Make sure that account numbers are assigned to your accounts in QuickBooks.
If transactions in QuickBooks have tax amounts, you must set up a tax account for your tax jurisdictions in Business Central before you can post transactions.

In order to get your data out of the QuickBooks desktop application you will need to download the Microsoft Data Exporter Tool.  The instructions for the tool are in the Data Migration Wizard in [!INCLUDE[d365fin](includes/d365fin_md.md)]. The tool will connect to your QuickBooks application and export the applicable data to a .zip file.  

> [!NOTE]
> Currently the data exporter tool only works with QuickBooks 2017 and 2018.

## <a name="finding-the-quickbooks-data-migration-extension"></a>Finding the QuickBooks Data Migration Extension
The QuickBooks Data Migration extension is installed and ready to go as an integrated part of the Data Migration assisted setup guide. If you are ready to get started now, and have exported your data from QuickBooks, choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Assisted Setup**, and then choose the related link. Choose **Migrate business data**, and then follow the steps in the guide.  

## <a name="what-do-i-do-after-i-migrate-data"></a>What do I do after I migrate Data?
After you migrate data, transactions have the status Unposted, so you can review them and make adjustments. To review the transactions, go to the page where you would normally find them. For example, to review unposted sales invoices, go to the Sales Invoices page. To review payment journals, go to the Payment Journals page.
There are a few things in particular that you should do: If the transactions in QuickBooks had markup or discount amounts, you must manually add the amounts to the related transactions in Business Central before you post them.
If you are using value added tax (VAT), you may need to add a business posting group and a product posting group to the posting setup so that you can post VAT amounts.
Verify the beginning balances for accounts in the general ledger. QuickBooks does not store the current balance for all accounts, so you might need to correct beginning balances.

## <a name="see-also"></a>See Also
[Importing Business Data from Other Finance Systems](across-import-data-configuration-packages.md)  
[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions ](ui-extensions.md)  

