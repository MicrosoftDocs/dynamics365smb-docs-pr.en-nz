---
title: Sales Tax in Canada| Microsoft Docs
description: Learn about local sales tax and goods and services tax in Canada.
services: project-madeira
documentationcenter: 
author: edupont04
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: sales tax, local
ms.date: 06/02/2017
ms.author: edupont
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: 571b11f4f18ffd194bdfe1d1d412bca87df4b868
ms.contentlocale: en-nz
ms.lasthandoff: 07/07/2017


---
# <a name="reporting-sales-tax-and-goodsservices-tax-in-canada"></a>Reporting Sales Tax and Goods/Services Tax in Canada
In Canada, when a vendor does not have a business presence in the province in which purchases are made, the vendor will charge the Goods and Services Tax (GST) or Harmonised Sales Tax (HST) only. However, if the province has a Provincial Sales Tax (PST), then the purchaser must still calculate the PST and pay it directly to the province. When a Provincial Tax Area Code is selected, [!INCLUDE[d365fin](includes/d365fin_md.md)] uses it to calculate the PST and post it so that there is a tax liability in both the general ledger and the tax entry records. Therefore, the tax area code selected here should be one where only the PST is included, not the GST.  

For more information about sales tax, see [Sales Tax and Tax Groups in the US and Canada](us-finance-sales-tax.md).  

## <a name="submitting-the-gsthst-file"></a>Submitting the GST/HST File
The tax information in purchase documents is used to generate a GST/HST online file transfer that you must provide to the tax authorities. This file includes goods and services tax (GST) and harmonised sales tax (HST). The file is created in a .tax file format, which can be transferred online.  

## <a name="see-also"></a>See Also
[Finance](finance.md)  
[Setting Up Finance](finance-setup-finance.md)  
[Sales Tax and Tax Groups in the US and Canada](us-finance-sales-tax.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

