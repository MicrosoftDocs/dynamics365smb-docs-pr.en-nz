---
title: Set up vendors without IRD for calculating withholding tax (NZ)
description: Withholding Tax (WHT) is calculated for local vendors who don't have a New Zealand Inland Revenue Department number.
author: brentholtorf
ms.topic: conceptual
ms.devlang: al
ms.search.keywords: null
ms.search.form: 28043
ms.date: 11/20/2023
ms.author: bholtorf
ms.service: dynamics-365-business-central
ms.reviewer: bholtorf
---
# <a name="set-up-vendors-without-ird-numbers-for-calculating-the-withholding-tax"></a>Set up vendors without IRD numbers for calculating the withholding tax

Withholding Tax (WHT) is calculated for local vendors who don't have a New Zealand Inland Revenue Department number (IRD), as required by tax law.  

## <a name="to-set-up-vendors-without-ird-for-calculating-the-withholding-tax"></a>To set up vendors without IRD for calculating the withholding tax

1.  Choose the ![Lightbulb that opens the Tell Me feature.](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Vendors**, and then choose the related link.  
2.  Choose the required vendor, and then choose the **Edit** action.  
3.  On the **Vendor Card** page, on the **Registration** FastTab, make sure the **IRD No. (Internal Revenue Department Number)** field and the **Foreign Vend** field must be empty.  
4.  Choose the **OK** button.  

> [!NOTE]  
> The WHT percentage is automatically withheld in accordance with what was specified on the **WHT Posting Setup** page. The WHT certificate is produced for submission to the vendor. For more information, see [Withholding Tax](withholding-tax.md).  

## <a name="see-also"></a>See also

[Withholding Tax](withholding-tax.md)   
[Set Up Withholding Tax](how-to-set-up-withholding-tax.md)


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
