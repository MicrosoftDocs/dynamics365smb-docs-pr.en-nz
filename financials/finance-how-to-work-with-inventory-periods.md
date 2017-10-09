---
title: How to Work with Inventory Periods | Microsoft Docs
description: You can control the timeframe in which people can post post changes to inventory by defining inventory periods.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: inventory, periods
ms.date: 08/07/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 8f9c289f4fef06ef0b684dd7176630d29b2fc5d3
ms.contentlocale: en-nz
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-work-with-inventory-periods"></a>How to: Work with Inventory Periods
Inventory periods define a period of time in which you can post changes to inventory. An inventory period is defined by the date on which it ends, or the ending date. When you close an inventory period, you cannot post any changes to inventory, either expected or invoiced, before this ending date. You cannot post any new values to inventory before the ending date. If you have open item entries in the closed period, meaning positive quantities that have not yet been applied to outbound transactions, you can still apply outbound quantities to these entries, even if the period is closed.  

The following sections describe how to:  

* Create inventory periods.  
* Close inventory periods.  
* Reopen inventory periods.  

## <a name="to-create-an-inventory-period"></a>To create an inventory period  
1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Inventory Periods**, and then choose the related link.  
2. Create a new line.  
3. In the **Ending Date** field, enter the last date in the inventory period that you want to define. When the period is closed, you will not be able to post inventory changes before this date.  
4. Enter a descriptive name in the **Name** field. Choose the **OK** button.  

## <a name="closing-inventory-periods"></a>Closing Inventory Periods  
The **Closed** field indicates whether or not the inventory period is closed to inventory value changes. You cannot edit this field.  

You can close any inventory period, provided that the following is true:  

* There are no open outbound item ledger entries, meaning negative inventory, in that period.  
* The cost of all items has been adjusted using the **Adjust Cost – Item Entries** batch job.  

This means that all outbound transaction quantities, such as those from sales orders, outbound transfers, sales invoices, purchase returns, or purchase credit memos, must be applied to existing quantity in inventory.  

### <a name="to-close-an-inventory-period"></a>To close an inventory period  
1. Before closing an inventory period, run the **Adjust Cost – Item Entries** batch job to ensure that all cost adjustments are posted. On the **Actions** tab, in the **Functions** group, choose **Adjust Cost – Item Entries**.  

     Run the **Close Inventory Period – Test** report to determine if there are any open outbound item entries within the inventory period or any items whose cost has not yet been adjusted.  
2. Choose the **Close Inventory Period – Test** action.  

     Run the **Post Inventory Cost to G/L** batch job to ensure that all costs are posted to the general ledger.  
3. Choose the **Post Inventory to G/L** action.  
4. In the **Inventory Periods** window, select the inventory period you want to close.  
5. Choose the **Close Period** action. After the inventory period has been closed, you cannot post inventory changes before the ending date. The cost of all items must be adjusted with the **Adjust Cost – Item Entries** batch job before you close the inventory period.  
6. Choose the **Yes** button to confirm that you want to close the period, or choose **No** to cancel the closing.  
7. The inventory period is closed and a confirmation message is displayed when it is finished.  

## <a name="reopening-inventory-periods"></a>Reopening Inventory Periods  
After you have closed the inventory period, you cannot delete the inventory period. You can, however, reopen it, if you would like to allow posting before the ending date of the inventory period. Reopening a period also reopens all inventory periods with ending dates later than the period you reopen.  

### <a name="to-reopen-an-inventory-period"></a>To reopen an inventory period  
1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Inventory Periods**, and then choose the related link.  
2. Select the inventory period you want to reopen.  
3. Choose the **Reopen Period** period action. Confirm that you want to reopen the period.  
4. All inventory periods with ending dates later than the period you selected are reopened.  

## <a name="see-also"></a>See Also  
[Design Details: Inventory Periods](design-details-inventory-periods.md)  
[Finance](finance.md)  
[Inventory](inventory-manage-inventory.md)  
[Working with Financials](ui-work-product.md)

