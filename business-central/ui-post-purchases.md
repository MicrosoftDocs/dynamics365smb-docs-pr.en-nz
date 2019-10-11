---
title: Understanding How To Post Purchase Documents | Microsoft Docs
description: Learn about the different posting functions to post purchase documents, and how you can update posted documents.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.reviewer: edupont
ms.date: 10/01/2019
ms.author: sgroespe
ms.openlocfilehash: 0fccda42a69cd1d1d7129380518890fac5b8986c
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 10/01/2019
ms.locfileid: "2315100"
---
# <a name="posting-purchases"></a>Posting Purchases
In the **Posting group** on a purchase document, you can choose between the following posting functions:

* **Post**
* **Preview Posting**
* **Post and Print**
* **Test Report**
* **Post Batch**

When you have completed all the lines and entered all the information on the purchase order, you can post it, that is, create a receipt and an invoice.

When a purchase order is posted, the vendor's account, the general ledger, and the item ledger entries are updated.

For each purchase order, a purchase entry is created in the **G/L Entry** table. An entry is also created in the vendor's account in the **Vendor Ledger Entry** table and a G/L entry is created in the relevant payables account. In addition, posting the order may result in a GST entry and a G/L entry for the discount amount. Whether an entry for the discount is posted depends on the contents of the **Discount Posting** field on the **Purchases & Payables Setup** page.

For each purchase order line, an item ledger entry will be created in the **Item Ledger Entry** table (if the purchase lines contain item numbers) or a G/L entry will be created in the **G/L Entry** table (if the purchase lines contain a G/L account). In addition, purchase orders are always recorded in the **Purch. Recpt. Header** and **Purch. Inv. Header** tables.

Before you start to post, you can print a test report that contains all the information in the purchase order and indicates any errors there. To print the report, choose **Posting**, and then choose **Test Report**.

> [!IMPORTANT]  
>   When you post an order, you can create both a receipt and an invoice. These can be done simultaneously or independently. You can also create a partial receipt and a partial invoice by completing the **Qty. to Receive** and **Qty. to Invoice** fields on the individual purchase order lines before you post. Note that you cannot create an invoice for something that has not been received. That is, before you can invoice, you must have recorded a receipt, or you must choose to receive and invoice at the same time.

You can either post, or post and print. If you choose to post and print, a report is printed when the order is posted. You can also choose the **Post Batch** function, which lets you post several orders at the same time. For more information, see [Post Multiple Documents at the Same Time](ui-batch-posting.md).

When the posting is completed, the posted purchase lines are removed from the order. A message tells you when the posting is completed. After this, you will be able to see the posted entries in the various pages that contain posted entries, such as the **Vendor Ledger Entries**, **G/L Entries**, **Item Ledger Entries**, **Purchase Receipts**, and **Posted Purchase Invoices** pages.

You can edit certain fields on posted purchase documents, such as the **Payment Reference** field. For more information, see [Edit Posted Documents](across-edit-posted-document.md).

## <a name="see-also"></a>See Also
[Edit Posted Documents](across-edit-posted-document.md)  
[Post Multiple Documents at the Same Time](ui-batch-posting.md)  
[Purchasing](purchasing-manage-purchasing.md)  
[Posting Documents and Journals](ui-post-documents-journals.md)  
[Correct or Cancel Unpaid Purchase Invoices](purchasing-how-correct-cancel-unpaid-purchase-invoices.md)  
[Finding Pages and Information with Tell Me](ui-search.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
