---
title: Assign Item Charges to Sales and Purchases| Microsoft Docs
description: If you want your inventory items to carry added costs, such as freight, physical handling, insurance, and transportation that you incur when purchasing or selling items, you can use the Item Charges feature.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: transportation, added cost
ms.date: 06/06/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: 5a40482673c8b8110a6036046174a58f5d7be18f
ms.contentlocale: en-nz
ms.lasthandoff: 03/22/2018

---
# <a name="use-item-charges-to-account-for-additional-trade-costs"></a>Use Item Charges to Account for Additional Trade Costs
To ensure correct valuation, your inventory items must carry any added costs, such as freight, physical handling, insurance, and transportation that you incur when purchasing or selling the items. For purchases, the landed cost of a purchased item consists of the vendor's purchase price and all additional direct item charges that can be assigned to individual receipts or return shipments. For sales, knowing the cost of shipping sold items can be as vital to your company as knowing the landed cost of purchased items.

In addition to recording the added cost in you inventory value, you can use the Item Charges feature for the following:

- Identify the landed cost of an item for making more accurate decisions on how to optimise the distribution network.
- Break down the unit cost or unit price of an item for analysis purposes.
- include purchase allowances into the unit cost and sales allowances into the unit price.

Before you can assign item charges, you must set up item charge numbers for the different types of item charges, including to which G/L accounts costs related to sales, purchases, and inventory adjustments are posted to. An item charge number contains a combination of general product posting group, tax group code, GST product posting group, and item charge. When you enter the item charge number on a purchase or sales document, the relevant G/L account is retrieved based on the setup of the item charge number and the information on the document.

For both purchase and sales documents, you can assign an item charge in two ways:
- On the document where the items that the item charge relates to are listed. This you typically do for documents that are not yet fully posted.
- On a separate invoice by linking the item charge to a posted receipt or shipment where the items that the item charge relate to are listed.

> [!NOTE]  
>   You can assign item charges to orders, invoices, and credit memos, for both sales and purchases. The following procedures describe how to work with item charges for a purchase invoice. The steps are similar for all other purchase and sales documents.

## <a name="to-set-up-item-charge-numbers"></a>To set up item charge numbers
You use item charge numbers to distinguish between the different kinds of item charges that are used in your company.

1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Item Charges**, and then choose the related link.
2. In the **Item Charges** window, choose the **New** action to create a new line.
3. Fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="to-assign-an-item-charge-directly-to-the-purchase-invoice-for-the-item"></a>To assign an item charge directly to the purchase invoice for the item
If you know the item charge at the time when you post a purchase invoice for the item, follow this procedure.

1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Purchase Invoices**, and then choose the related link.
2. Create a new purchase invoice. For more information, see [Record Purchases](purchasing-how-record-purchases.md).
3. Make sure the purchase invoice has one or more lines of type Item.
4. On a new line, in the **Type** field, select **Charge (Item)**.
5. In the **Quantity** field, enter the units of the item charge that you have been invoiced for.
6. In the **Direct Unit Cost** field, enter the amount of the item charge.
7. Fill in the remaining fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

    In the following steps, you will perform the actual assignment. Until the item charge is fully assigned, the value in the **Qty. to Assign** field is in red font.
8. On the **Lines** tab, choose the **Item Charge Assignment** action.

    The **Item Charge Assignment** window opens showing one line for each line of type Item on the purchase invoice. To assign the item charge to one or more invoice lines, you can use a function that assigns and distributes it for you or you can manually fill in the **Qty. to Assign** field. The following steps describe how to use the Suggest Item Charge Assignment function.

9. In the **Item Charge Assignment** window, choose the **Suggest Item Charge Assignment** action.
10. If there are more than one invoice lines of type Item, choose one of the four distribution options.  

It the item charge is fully assigned, the value in the **Qty. to Assign** field on the purchase invoice is zero.

The item charge is now assigned to the purchase invoice. When you post the receipt of the purchase invoice, the items' inventory values are updated with the cost of the item charge.  

## <a name="to-assign-an-item-charge-from-a-separate-invoice-to-the-purchase-invoice-for-the-item"></a>To assign an item charge from a separate invoice to the purchase invoice for the item
If you received an invoice for the item charge after you posted the original purchase receipt, follow this procedure.
1. Repeat steps 1 through 8 in the "To assign an item charge directly to the purchase invoice for the item" section.
2. In the **Item Charge Assignment** window, choose the **Get Receipt Lines** action.
3. In the **Purch. Receipt Lines** window, select the posted purchase receipt for the item that you want to assign the item charge to, and then choose the **OK** button.
4. Choose the **Suggest Item Charge Assignment** action.

The item charge on the separate purchase invoice is now assigned to the item on the posted purchase receipt, thereby updating the item's inventory value with the cost of the item charge.

## <a name="see-also"></a>See Also
[Managing Payables](payables-manage-payables.md)  
[Record Purchases](purchasing-how-record-purchases.md)  
[Invoice Sales](sales-how-invoice-sales.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

