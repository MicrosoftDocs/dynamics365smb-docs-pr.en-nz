---
title: How to Set Up Vendors Without IRD Numbers for Calculating the Withholding Tax
description: Withholding Tax (WHT) is calculated for local vendors who do not have a New Zealand Inland Revenue Department number.
services: project-madeira
documentationcenter: 
author: bholtorf
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 06/20/2018
ms.author: bholtorf
ms.translationtype: HT
ms.sourcegitcommit: 046a42582dc66368fded90a4bb45add71a95d979
ms.openlocfilehash: 4098ace6d63e004fd1b90727f96700ad78779151
ms.contentlocale: en-nz
ms.lasthandoff: 07/02/2018

---
# <a name="set-up-vendors-without-ird-numbers-for-calculating-the-withholding-tax"></a>Set Up Vendors Without IRD numbers for Calculating the Withholding Tax
Withholding Tax (WHT) is calculated for local vendors who do not have a New Zealand Inland Revenue Department number (IRD), as required by tax law.  

## <a name="to-set-up-vendors-without-ird-for-calculating-the-withholding-tax"></a>To set up vendors without IRD for calculating the withholding tax  
1.  Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Vendors**, and then choose the related link.  
2.  Choose the required vendor, and then choose the **Edit** action.  
3.  In the **Vendor Card** window, on the **Registration** FastTab, make sure the **IRD No.** field and the **Foreign Vend** field must be empty.  
4.  Choose the **OK** button.  

    > [!NOTE]  
    >  The WHT percentage is automatically withheld in accordance with what was specified in the **WHT Posting Setup** window. The WHT certificate is produced for submission to the vendor. For more information, see [Withholding Tax](withholding-tax.md).  

## <a name="see-also"></a>See Also  
[Withholding Tax](withholding-tax.md)   
[Set Up Withholding Tax](how-to-set-up-withholding-tax.md)

