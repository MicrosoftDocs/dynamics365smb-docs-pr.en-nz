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
ms.date: 10/01/2018
ms.author: bholtorf
ms.openlocfilehash: 681919badbe7f98e57a28bec89395f8588506d1e
ms.sourcegitcommit: 1bcfaa99ea302e6b84b8361ca02730b135557fc1
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 03/08/2019
ms.locfileid: "827044"
---
# <a name="set-up-vendors-without-ird-numbers-for-calculating-the-withholding-tax"></a>Set Up Vendors Without IRD numbers for Calculating the Withholding Tax
Withholding Tax (WHT) is calculated for local vendors who do not have a New Zealand Inland Revenue Department number (IRD), as required by tax law.  

## <a name="to-set-up-vendors-without-ird-for-calculating-the-withholding-tax"></a>To set up vendors without IRD for calculating the withholding tax  
1.  Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Vendors**, and then choose the related link.  
2.  Choose the required vendor, and then choose the **Edit** action.  
3.  On the **Vendor Card** page, on the **Registration** FastTab, make sure the **IRD No.** field and the **Foreign Vend** field must be empty.  
4.  Choose the **OK** button.  

    > [!NOTE]  
    >  The WHT percentage is automatically withheld in accordance with what was specified on the **WHT Posting Setup** page. The WHT certificate is produced for submission to the vendor. For more information, see [Withholding Tax](withholding-tax.md).  

## <a name="see-also"></a>See Also  
[Withholding Tax](withholding-tax.md)   
[Set Up Withholding Tax](how-to-set-up-withholding-tax.md)
