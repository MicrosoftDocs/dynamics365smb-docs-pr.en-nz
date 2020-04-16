---
title: How to Create Cheque Instalments
description: Describes how to create cheque instalments for post-dated cheques.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2020
ms.author: bholtorf
ms.openlocfilehash: 8d90be494db24514e5827f5b71743a0b12c0af1c
ms.sourcegitcommit: 88e4b30eaf6fa32af0c1452ce2f85ff1111c75e2
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 04/01/2020
ms.locfileid: "3181062"
---
# <a name="create-check-installments"></a>Create Cheque Instalments
You can create cheque instalments for post-dated cheques. You can define the number of instalments that a payment will be divided into, the percent of interest, and the period in which the cheques will be created.  

## <a name="to-create-a-check-installment"></a>To create a cheque instalment  
1.  Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Post Dated Cheques-Purchases**, and then choose the relevant link.  
2.  Choose the relevant check, and then choose the **Edit** action.  
3.  On the **Post Dated checks-Purchase** page, choose the **Create check instalments** action.  
4.  On the **Options** FastTab, fill in the fields as described in the following table.  

5.  |Field|Description|  
    |---------------------------------|---------------------------------------|  
    |**No. of Instalments**|Specifies the number of instalments into which the post-dated cheque will be divided.|  
    |**Interest %**|Specifies the percent of interest.|  
    |**Period Length**|Specifies the period for which the instalments will be created. For example, if you want to divide the cheque into monthly instalments, enter **1M**.|  
    |**Start Document No.**|Specifies the starting number of the document. Based on the number of instalments specified, the consecutive numbers are allocated to the documents created.|  

6.  Choose the **OK** button.  

     The instalment cheques are created and displayed on the **Post Dated Cheques-Purchases** page.

## <a name="see-also"></a>See Also
[New Zealand Local Functionality](new-zealand-local-functionality.md)
