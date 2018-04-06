---
title: Design Details - Active versus Historic Item Tracking Entries | Microsoft Docs
description: When parts of a document line quantity are posted, only that particular quantity is transferred to the item ledger entries and its item tracking numbers. However, you will want to access all relevant item tracking information directly from the active document line. That is, not only will you want to see the entries that are related to the remaining quantity, you will also want information about the units that have been posted. When you view or modify the **Item Tracking Lines** window, the collective contents of the **Tracking Specification** table (T336) and **Reservation Entry** table (T337) are presented in a temporary version of T336. This ensures that historic and active item tracking data is accessed as one.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 0b0d49b4f9b9e77b311628c2d88b4891b32f8276
ms.contentlocale: en-nz
ms.lasthandoff: 03/22/2018

---
# <a name="design-details-active-versus-historic-item-tracking-entries"></a>Design Details: Active versus Historic Item Tracking Entries
When parts of a document line quantity are posted, only that particular quantity is transferred to the item ledger entries and its item tracking numbers. However, you will want to access all relevant item tracking information directly from the active document line. That is, not only will you want to see the entries that are related to the remaining quantity, you will also want information about the units that have been posted. When you view or modify the **Item Tracking Lines** window, the collective contents of the **Tracking Specification** table (T336) and **Reservation Entry** table (T337) are presented in a temporary version of T336. This ensures that historic and active item tracking data is accessed as one.  

 The following table shows how T336 and T337 are used in a purchase scenario. The bold figures represent values that the user manually enters in the **Item Tracking Lines** window.  

 Step 1: Create a purchase order line of seven pieces with item tracking numbers.  

||**Quantity (Base)**|**Qty. to Handle**|**Qty. to Invoice (Base)**|**Quantity Handled (Base)**|**Quantity Invoiced (Base)**|  
|-|----------------------------------------------|--------------------------------------------|------------------------------------------------------|-------------------------------------------------------|--------------------------------------------------------|  
|**T337**|Deferred Company Fund Installment (7)|0|0|0|0|  
|**T336**|0|0|0|0|0|  

 Step 2: Receive four pieces.  

||**Quantity (Base)**|**Qty. to Handle**|**Qty. to Invoice (Base)**|**Quantity Handled (Base)**|**Quantity Invoiced (Base)**|  
|-|----------------------------------------------|--------------------------------------------|------------------------------------------------------|-------------------------------------------------------|--------------------------------------------------------|  
|**Item Tracking Lines** window|Deferred Company Fund Installment (7)|**4**|**0**|0|0|  
|**T337**|2A-2B GST Net Amt. (3)|0|0|0|0|  
|**T336**|Total Amounts Withheld From All Payments (4)|0|0|Total Amounts Withheld From All Payments (4)|0|  

 Step 3: Receive two pieces and invoice two pieces.  

||**Quantity (Base)**|**Qty. to Handle**|**Qty. to Invoice (Base)**|**Quantity Handled (Base)**|**Quantity Invoiced (Base)**|  
|-|----------------------------------------------|--------------------------------------------|------------------------------------------------------|-------------------------------------------------------|--------------------------------------------------------|  
|**Item Tracking Lines** window|Deferred Company Fund Installment (7)|**2**|**2**|Total Amounts Withheld From All Payments (4)|0|  
|**T337**|1|0|0|0|0|  
|**T336**|6|0|0|6|2|  

 Step 4: Receive one piece.  

||**Quantity (Base)**|**Qty. to Handle**|**Qty. to Invoice (Base)**|**Quantity Handled (Base)**|**Quantity Invoiced (Base)**|  
|-|----------------------------------------------|--------------------------------------------|------------------------------------------------------|-------------------------------------------------------|--------------------------------------------------------|  
|**Item Tracking Lines** window|Deferred Company Fund Installment (7)|**1**|**0**|6|2|  
|**T336**|Deferred Company Fund Installment (7)|0|0|Deferred Company Fund Installment (7)|2|  

 Invoice 5 pieces.  

||**Quantity (Base)**|**Qty. to Handle**|**Qty. to Invoice (Base)**|**Quantity Handled (Base)**|**Quantity Invoiced (Base)**|  
|-|----------------------------------------------|--------------------------------------------|------------------------------------------------------|-------------------------------------------------------|--------------------------------------------------------|  
|**Item Tracking Lines** window|Deferred Company Fund Installment (7)|0|**5**|Deferred Company Fund Installment (7)|2|  
|**T336**|Deferred Company Fund Installment (7)|0|0|Deferred Company Fund Installment (7)|Deferred Company Fund Installment (7)|  

## <a name="see-also"></a>See Also  
 [Design Details: Item Tracking](design-details-item-tracking.md)   
 [Design Details: Item Tracking Lines Window](design-details-item-tracking-lines-window.md)

