---
title: How to Verify GST Registration Numbers | Microsoft Docs
description: You can use an EU web service to verify that VAT registration numbers that you enter on customer, vendor, or contact cards are valid.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/10/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 7180c7823055dba52a398584ed2f4c2952d08492
ms.contentlocale: en-nz
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-verify-vat-registration-numbers"></a>How to: Verify VAT Registration Numbers
You can use an EU web service to verify that VAT registration numbers that you enter on customer, vendor, or contact cards are valid.  

 When you modify the **GST Registration No.** field on a card where the value in the **Country/Region Code** field is an EU country/region, then the new GST Registration number. and your user ID are logged in the **GST Registration Log** window. You verify a GST Registration number by choosing the **Verify Registration No.** button in the **GST Registration Log** window. A new line is created every time you use the verification function. If the number could be verified, the **Status** field contains **Valid**. If the number could not be verified, the **Status** field contains **Invalid**, and you must then change the number in the **GST Registration No.** field on the card and start the verification function again.  

 The URL of the default web service is set up in the **GST Reg. No. Validation URL** field in the **General Ledger Setup** window.  

 In the **GST Registration No. Format** table, you can change for each country/region the different formats of GST Registration number that users are allowed to enter in the **GST Registration No.** field.  

> [!WARNING]  
>  This web service uses the http protocol, which means that data transferred through the service is not encrypted.  

> [!NOTE]  
>  You may experience downtime for this service for which Microsoft is not responsible, as the service is part of a broad EU network of national GST registers.  

## <a name="to-verify-a-vat-registration-number-from-a-customer-card"></a>To verify a GST registration number from a customer card  
The following describes how to verify a GST Registration number for a customer. The steps are similar for a vendor and a contact.   
1.  Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Customers**, and then choose the related link.  

2.  Open the card of a customer where you want to verify the GST registration number.  

    > [!NOTE]  
    >  The **Country/Region Code** field on the customer card must contain an EU country/region.  
3.  On the **Invoicing** FastTab, choose the DrillDown button next to the **GST Registration No.** field.  

    The **GST Registration Log** window opens showing one line where the **Status** field contains **Not Verified**.  
4.  Choose the **Verify Registration No.** action.  

     A new line is created where the **Status** field contains either **Valid** or **Invalid**.  
5.  If the **Status** field contains **Invalid**, change the number in the **GST Registration No.** field on the card, and then repeat steps 3 through 4.  

## <a name="see-also"></a>See Also  
[Finance](finance.md)  
[How to: Register New Customers](sales-how-register-new-customers.md)  
[How to: Register New Vendors](purchasing-how-register-new-vendors.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

