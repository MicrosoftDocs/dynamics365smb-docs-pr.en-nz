---
title: Electronic Funds Transfer (EFT)
description: You can pay vendors using the electronic funds transfer (EFT) system in New Zealand.
services: project-madeira
documentationcenter: ''
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2019
ms.author: bholtorf
ms.openlocfilehash: c4da6d27f50044bb61301ea6c1e1d0950f71de75
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 10/01/2019
ms.locfileid: "2300111"
---
# <a name="electronic-funds-transfer-eft"></a>Electronic Funds Transfer (EFT)
You can pay vendors using the electronic funds transfer (EFT) system in New Zealand.  

## <a name="setting-up-electronic-funds-transfer-in-included365finincludesd365fin_mdmd"></a>Setting up Electronic Funds Transfer in [!INCLUDE[d365fin](../../includes/d365fin_md.md)]  
[!INCLUDE[d365fin](../../includes/d365fin_md.md)] can export EFT files that you can then upload to your bank’s website for additional processing. To submit EFT files, you must set up the following information:  

* You must add EFT information to the bank account or bank accounts that you will use to pay vendors electronically. The EFT-specific fields are in the **Transfer** FastTab on the **Bank Account** page.  
* For those vendors that you want to pay electronically, you must select the **EFT Payment** check box and specify the vendor bank account in the **EFT Vendor Bank Account Code** field on the **Vendor** page.  

When you have set up bank accounts and vendors, you can create EFT file that are based on entries in the payment journal. When you create an EFT file, an entry is made in the **EFT Register** table. On the EFT Register page you can drill down to see the vendor ledger entries for the EFT file. On the Payment Journal page,you can also import existing EFT register entries to the payment journal by using the **Transfer EFT Register** batch job.

## <a name="see-also"></a>See Also  
[Export Payments to a Bank File](../../payables-how-export-payments-bank-file.md)  
[New Zealand Local Functionality](new-zealand-local-functionality.md)
