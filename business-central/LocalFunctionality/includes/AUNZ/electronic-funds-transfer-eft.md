---
author: edupont04
ms.service: dynamics365-business-central
ms.topic: include
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 60d8b8d7843c0b5844a7d37a084a8fbd63627f51
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 12/17/2020
ms.locfileid: "4747439"
---
## <a name="setting-up-electronic-funds-transfer"></a>Setting up Electronic Funds Transfer

[!INCLUDE[prod_short](../../../includes/prod_short.md)] can export EFT files that you can then upload to your bank's website for additional processing. To submit EFT files, you must set up the following information:  

* You must add EFT information to the bank account or bank accounts that you will use to pay vendors electronically. The EFT-specific fields are on the **Bank Account** page.  
* For those vendors that you want to pay electronically, you must select the **EFT Payment** check box and specify the vendor bank account in the **EFT Vendor Bank Account Code** field on the **Vendor** page.  

When you have set up bank accounts and vendors, you can create EFT files that are based on entries in the payment journal. When you create an EFT file, an entry is made in the **EFT Register** table. On the **EFT Register** page, you can drill down to see the vendor ledger entries for the EFT file. On the **Payment Journal** page, you can also import existing EFT register entries to the payment journal by using the **Transfer EFT Register** batch job.

> [!NOTE]  
> Electronic Funds Transfer (EFT) uses posted and nonposted payments as the basis to calculate withholding tax amounts for applied invoices. Payments that are not applied to an invoice can only be exported to an EFT file if the **Skip WHT** check box is selected. During export of the EFT file, the payment journal lines are not deleted and cannot be deleted as long as they have a reference to an EFT register. To remove the link between the EFT register and payment journal lines, choose the **Cancel Export** action either on the **EFT Register** page or the **Payment Journal** page.       
