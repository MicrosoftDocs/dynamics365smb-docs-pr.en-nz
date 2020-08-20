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
ms.openlocfilehash: c2899cb79597ec84e170abb8d73240a24bc525e9
ms.sourcegitcommit: 007b331b6974983ee614db0406f00777da359ecb
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 08/10/2020
ms.locfileid: "3677270"
---
# <a name="create-check-installments"></a>Create Cheque Instalments
You can create cheque instalments for post-dated cheques. You can define the number of instalments that a payment will be divided into, the percent of interest, and the period in which the cheques will be created.  

## <a name="to-create-a-check-installment"></a>To create a cheque instalment  
1.  Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Post Dated Cheques-Purchases**, and then choose the relevant link.  
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
