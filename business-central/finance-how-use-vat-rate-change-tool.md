---
title: Use the VAT Rate Change Tool | Microsoft Docs
description: Use the VAT Rate Change Tool
author: andregu
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: VAT, posting, tax, value-added tax
ms.date: 04/01/2020
ms.author: andregu
ms.openlocfilehash: 76c6f8902e9661f4f4dbbbf70487a53bf286edb2
ms.sourcegitcommit: 88e4b30eaf6fa32af0c1452ce2f85ff1111c75e2
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 04/01/2020
ms.locfileid: "3183180"
---
# <a name="use-the-vat-rate-change-tool"></a>Use the VAT Rate Change Tool

## <a name="understanding-the-vat-rate-conversion-process"></a>Understanding the GST Rate Conversion Process  
The GST rate change tool performs GST rate conversions for master data, journals, and orders in different ways. The selected master data and journals will be updated by the new general product posting group or GST product post group. If an order has been fully or partially shipped, the shipped items will keep the current general product posting group or GST product posting group. A new order line will be created for the unshipped items and updated to align current and new GST or general product posting groups. In addition, item charge assignments, reservations, and item tracking information will be updated accordingly.  

There are a few things that the tool does not convert:

* Sales or purchase orders and invoices where shipments have been posted. These documents are posted using the current GST rate.  
* Documents that have posted prepayment invoices. For example, you have made or received prepayments on invoices that have not been completed before you use the GST rate change tool. In this case, there will be a difference between the GST that is due and the GST that has been paid in the prepayments when the invoice is completed. The GST rate change tool will skip these documents and you will have to manually update them.  
* Drop shipments or special orders.  
* Sales or purchase orders with warehouse integration if they are partially shipped or received.  
* Service contracts.  

### <a name="to-prepare-vat-rate-change-conversions"></a>To prepare GST rate change conversions  
Before you set up the GST rate change tool, you must make the following preparations.

* If you have transactions that use different rates, then they must be separated into different groups either by creating new general ledger accounts for each rate or by using data filters to group transactions according to rate.  
* If you create new general ledger accounts, then you must create new general posting groups.  
* To reduce the number of documents that get converted, post as many documents as possible and reduce unposted documents to a minimum.  
* Back up data.

### <a name="to-set-up-the-vat-rate-change-tool"></a>To set up the GST rate change tool  
1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **GST Rate Change Setup**, and then choose the related link.  
2. On the **Master Data**, **Journals**, and **Documents** FastTabs, choose a posting group value from the option list for needed fields. For each group you can choose whether to convert VAT product posting groups or general product posting groups, or convert both values if they are available in the master data item. For some areas you can also set a filter to convert only a subset of values, for example, G/L accounts. 

### <a name="to-set-up-product-posting-group-conversion"></a>To set up product posting group conversion  
1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **GST Rate Change Setup**, and then choose the related link.  
2. On the **GST Rate Change Setup** page, choose either the **GST Prod. Posting Group Conv.** or **Gen Prod. Posting Group Conv.** action.  
3. In the **From Code** field, enter the current posting group.  
4. In the **To Code** field, enter the new posting group.  

### <a name="to-perform-vat-rate-change-conversion"></a>To perform GST rate change conversion  
You use the GST rate change tool to manage changes in the standard rate of GST. You perform GST and general posting group conversions to change GST rates and maintain accurate GST reporting. Depending on your setup, the following changes are made:  

* GST and general posting groups are converted.  
* Changes are implemented in general ledger accounts, customers, vendors, open documents, journal lines, and so on.  

> [!IMPORTANT]  
>  Before you perform GST rate change conversion, you can test the conversion. To do so, follow the steps below, but make sure to clear the **Perform Conversion** and **GST Rate Change Tool Completed** check boxes. During test conversion, the **Converted** field in the **GST Rate Change Log Entry** table is cleared and the **Converted Date** field in the **GST Rate Change Log Entry** table is blank. After the conversion is complete, choose **GST Rate Change Log Entries** to view the results of the test conversion. Verify each entry before you perform the conversion. In particular, verify transactions that use an old GST rate.     

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **GST Rate Change**, and then choose the **GST Rate Change Setup** link.  
2. Verify that you have already set up the GST product posting group conversion or general product posting group conversion.  
3. Choose the **Perform Conversion** check box.  

    > [!IMPORTANT]  
    >  Clear the **GST Rate Change Tool Completed** check box. The check box is automatically selected when the GST rate change conversion is completed.  

4. Choose the **Convert** action.  
5. After the conversion is complete, choose the **GST Rate Change Log Entries** action to view the results of the conversion.  

> [!IMPORTANT]  
>  After the conversion, the **Converted** field in the **GST Rate Change Log Entry** table is chosen and the **Converted Date** field in the **GST Rate Change Log Entry** table displays the conversion date.  
## <a name="see-also"></a>See Also  
[Set Up Value-Added Tax](finance-setup-vat.md)  
[Setting Up Unrealised Goods and Services Tax](finance-setup-unrealized-vat.md)      
[Report GST to a Tax Authority](finance-how-report-vat.md)  
[Work with GST on Sales and Purchases](finance-work-with-vat.md)  
[Local functionality in Business Central](about-localization.md)
