---
author: edupont04
ms.service: dynamics365-business-central
ms.topic: include
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: d93cd845c8f2d25915b2b983d287cd7b9e6fcd15
ms.sourcegitcommit: 428f180604e5afcf94fa0e92a0615f58c88e13cd
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 10/02/2020
ms.locfileid: "3959632"
---
## <a name="setting-up-electronic-funds-transfer"></a>Setting up Electronic Funds Transfer

[!INCLUDE[d365fin](../../../includes/d365fin_md.md)] can export EFT files that you can then upload to your bank's website for additional processing. To submit EFT files, you must set up the following information:  

* You must add EFT information to the bank account or bank accounts that you will use to pay vendors electronically. The EFT-specific fields are on the **Bank Account** page.  
* For those vendors that you want to pay electronically, you must select the **EFT Payment** check box and specify the vendor bank account in the **EFT Vendor Bank Account Code** field on the **Vendor** page.  

When you have set up bank accounts and vendors, you can create EFT files that are based on entries in the payment journal. When you create an EFT file, an entry is made in the **EFT Register** table. On the **EFT Register** page, you can drill down to see the vendor ledger entries for the EFT file. On the **Payment Journal** page, you can also import existing EFT register entries to the payment journal by using the **Transfer EFT Register** batch job.

> [!NOTE]  
> Electronic Funds Transfer (EFT) uses posted and nonposted payments as the basis to calculate withholding tax amounts for applied invoices. Payments that are not applied to an invoice can only be exported to an EFT file if the **Skip WHT** check box is selected. During export of the EFT file, the payment journal lines are not deleted and cannot be deleted as long as they have a reference to an EFT register. To remove the link between the EFT register and payment journal lines, choose the **Cancel Export** action either on the **EFT Register** page or the **Payment Journal** page.       
