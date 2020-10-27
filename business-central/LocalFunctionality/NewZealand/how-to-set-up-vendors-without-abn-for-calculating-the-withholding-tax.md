---
title: How to Set Up Vendors Without IRD Numbers for Calculating the Withholding Tax
description: Withholding Tax (WHT) is calculated for local vendors who do not have a New Zealand Inland Revenue Department number.
services: project-madeira
documentationcenter: ''
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: bholtorf
ms.openlocfilehash: 559471b63c72a4dcecdec28ff6ec54ef4369b1e3
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 10/01/2020
ms.locfileid: "3919824"
---
# <a name="set-up-vendors-without-ird-numbers-for-calculating-the-withholding-tax"></a>Set Up Vendors Without IRD numbers for Calculating the Withholding Tax
Withholding Tax (WHT) is calculated for local vendors who do not have a New Zealand Inland Revenue Department number (IRD), as required by tax law.  

## <a name="to-set-up-vendors-without-ird-for-calculating-the-withholding-tax"></a>To set up vendors without IRD for calculating the withholding tax  
1.  Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Vendors** , and then choose the related link.  
2.  Choose the required vendor, and then choose the **Edit** action.  
3.  On the **Vendor Card** page, on the **Registration** FastTab, make sure the **IRD No.** field and the **Foreign Vend** field must be empty.  
4.  Choose the **OK** button.  

    > [!NOTE]  
    >  The WHT percentage is automatically withheld in accordance with what was specified on the **WHT Posting Setup** page. The WHT certificate is produced for submission to the vendor. For more information, see [Withholding Tax](withholding-tax.md).  

## <a name="see-also"></a>See Also  
[Withholding Tax](withholding-tax.md)   
[Set Up Withholding Tax](how-to-set-up-withholding-tax.md)
