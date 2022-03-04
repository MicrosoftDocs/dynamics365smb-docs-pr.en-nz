---
title: Managing GST Rate changes
description: Learn how to use the GST Rate Change tool for Dynamics 365 Business Central for changing GST rates based on local legislation.
author: andregu
ms.topic: conceptual
ms.reviewer: edupont
ms.workload: na
ms.search.keywords: VAT, VAT rate, posting, tax, value-added tax
ms.search.form: 550,
ms.date: 06/16/2021
ms.author: andregu
ms.openlocfilehash: ce98367d08c399e8c1a93140bad6fbecd04dda95
ms.sourcegitcommit: ef80c461713fff1a75998766e7a4ed3a7c6121d0
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 02/15/2022
ms.locfileid: "8135409"
---
# <a name="managing-vat-rate-changes"></a>Managing GST Rate Changes

GST rates can change depending on local legislation. Any change in GST impacts your data in [!INCLUDE[prod_short](includes/prod_short.md)] whether or not the GST rate is lowered, raised, or removed. GST is connected to many entities in [!INCLUDE[prod_short](includes/prod_short.md)], such as customers, vendors, items, resources, item charges, and general ledger accounts. Changes in GST rates usually happen at a specific date, from which point you will need to have changed the GST setup, posting groups etc. to make sure new sales orders and purchase orders are created with the new GST rate.

## <a name="changing-vat-rates"></a>Changing GST rates

The optimal approach to manage a GST rate change is to fully post and close open orders and other documents before the GST rate switch date, to make sure these are not impacted by the change. This is the cleanest approach that allows you to start up new orders and documents with the new GST rate.

The following approach is suggested to manage a GST rate change

1. Fully post and close open orders, journals and other documents before the switch date. You can wait to after the switch date as long as you do not add new lines and make sure the effective date will be prior the switch date.  
2. Create the new GST setup.  
3. Make the GST switch on entities (relevant customers, vendors, items, and so on).  
4. At the GST rate switch date you create new documents that will use the new rate.  


> [!NOTE]  
> We are currently updating the GST Rate Change tool. The functionality mentioned below may not match the functionality in your environment. The update will take place before July 1st 2020 and will not be a regular monthly update. Instead, all environments will be updated automatically (hotfix). When this update is complete, this message will no longer appear.  

## <a name="the-vat-rate-change-tool"></a>The GST Rate Change tool

The GST Rate Change tool can assist with conversion of GST Rates on master data, journals and orders, to some extent. This is useful if you want to convert GST on master data more easily or if you have orders that you cannot close before the switch date and will be processed over a longer period of time, crossing the GST rate switch date. There are certain restrictions and limitations in the GST Rate Change tool that applies.

## <a name="understanding-the-vat-rate-conversion-process-and-limitations"></a>Understanding the GST rate conversion process and limitations

The GST Rate Change tool performs GST rate conversions for master data, journals, and orders in different ways. The selected master data and journals will be updated by the new general product posting group or GST product post group. If an order has been fully or partially shipped, the shipped items will keep the current general product posting group or GST product posting group. A new order line will be created for the unshipped items and updated to align current and new GST or general product posting groups. In addition, item charge assignments, configuration templates for items, reservations, and item tracking information will be updated accordingly. 

On order lines, the unit price will be updated for all lines of type Item and Resource, if using prices incl. GST for the item. For other line types it is possible to decide whether or not the unit price should be updated.

There are a few things that the tool does not convert:

* Sales or purchase orders and invoices where shipments have been posted. These documents are posted using the current GST rate.  
* Documents that have posted prepayment invoices. For example, you have made or received prepayments on invoices that have not been completed before you use the GST rate change tool. In this case, there will be a difference between the GST that is due and the GST that has been paid in the prepayments when the invoice is completed. The GST rate change tool will skip these documents and you will have to manually update them.  
* Sales or purchase orders with warehouse integration if they are partially shipped or received.  
* Drop shipments.
* Special orders. 
* Assembly orders.
* Service contracts.  
* Credit memos.
* Return orders.
* Prices on Items (master data)
* Prices on Sales Prices (master data)
* Business Posting Groups on Customers and Vendors.

### <a name="to-prepare-vat-rate-change-conversions"></a>To prepare GST rate change conversions

Before you set up the GST rate change tool, you must make the following preparations.

* If you have transactions that use different rates, then they must be separated into different groups either by creating new general ledger accounts for each rate or by using data filters to group transactions according to rate.  
* If you create new general ledger accounts, then you must create new general posting groups.  
* To reduce the number of documents that get converted, post as many documents as possible and reduce unposted documents to a minimum.  
* Back up data.

### <a name="to-set-up-the-vat-rate-change-tool"></a>To set up the GST rate change tool

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **GST Rate Change Setup**, and then choose the related link.  
2. On the **Master Data**, **Journals**, and **Documents** FastTabs, choose a posting group value from the option list for needed fields. For each group you can choose whether to convert GST product posting groups or general product posting groups, or convert both values if they are available in the master data item. For some areas you can also set a filter to convert only a subset of values, for example, G/L accounts. 
3. On the **Prices Incl. GST** FastTab, choose which line types on orders for which you want to update unit prices. Unit prices on lines of type Item and Resource will always be updated.

### <a name="to-set-up-product-posting-group-conversion"></a>To set up product posting group conversion

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **GST Rate Change Setup**, and then choose the related link.  
2. On the **GST Rate Change Setup** page, choose either the **GST Prod. Posting Group Conv.** or **Gen Prod. Posting Group Conv.** action.  
3. In the **From Code** field, enter the current posting group.  
4. In the **To Code** field, enter the new posting group.  

### <a name="to-perform-vat-rate-change-conversion"></a>To perform GST rate change conversion

You use the GST rate change tool to manage changes in the standard rate of GST. You perform GST and general posting group conversions to change GST rates and maintain accurate GST reporting. Depending on your setup, the following changes are made:  

* GST and general posting groups are converted.  
* Changes are implemented in general ledger accounts, customers, vendors, open documents, journal lines, and so on.  

> [!IMPORTANT]  
> Before you perform GST rate change conversion, you can test the conversion. To do so, follow the steps below, but make sure to clear the **Perform Conversion** and **GST Rate Change Tool Completed** check boxes. During test conversion, the **Converted** field in the **GST Rate Change Log Entry** table is cleared and the **Converted Date** field in the **GST Rate Change Log Entry** table is blank. After the conversion is complete, choose **GST Rate Change Log Entries** to view the results of the test conversion. Verify each entry before you perform the conversion. In particular, verify transactions that use an old GST rate.

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **GST Rate Change**, and then choose the **GST Rate Change Setup** link.  
2. Verify that you have already set up the GST product posting group conversion or general product posting group conversion.  
3. Choose the **Perform Conversion** check box.  

    > [!IMPORTANT]  
    >  Clear the **GST Rate Change Tool Completed** check box. The check box is automatically selected when the GST rate change conversion is completed.  

4. Choose the **Convert** action.  
5. After the conversion is complete, choose the **GST Rate Change Log Entries** action to view the results of the conversion.  

> [!IMPORTANT]  
> After the conversion, the **Converted** field in the **GST Rate Change Log Entry** table is chosen and the **Converted Date** field in the **GST Rate Change Log Entry** table displays the conversion date.  

## <a name="see-also"></a>See Also

[Set Up Goods and Services Tax](finance-setup-vat.md)  
[Setting Up Unrealised Goods and Services Tax](finance-setup-unrealized-vat.md)  
[Report GST to a Tax Authority](finance-how-report-vat.md)  
[Work with GST on Sales and Purchases](finance-work-with-vat.md)  
[Local functionality in Business Central](about-localization.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]