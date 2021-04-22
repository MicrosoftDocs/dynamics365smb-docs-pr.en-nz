---
author: edupont04
ms.service: dynamics365-business-central
ms.topic: include
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: b71effff749b4190008ea321acaa65e069d7ea3e
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 03/31/2021
ms.locfileid: "5774358"
---
You can create cheque instalments for post-dated cheques. You can define the number of instalments that a payment will be divided into, the percent of interest, and the period in which the cheques will be created.  

## <a name="to-create-a-check-installment"></a>To create a cheque instalment  
1.  Choose the ![Lightbulb that opens the Tell Me feature](../../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Post Dated Cheques-Purchases**, and then choose the relevant link.  
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
