---
title: Available Fonts
description: Learn about the pre-installed fonts that you can use for your externally-facing reports.
author: SorenGP
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.search.form: 9020, 9022, 9026, 9027, 9030, 9000, 9004, 9005, 9018, 9006, 9007, 9010, 9016, 9017
ms.date: 11/30/2021
ms.author: edupont
ms.openlocfilehash: faa581a88a6c7503c34177db459345a24638a95a
ms.sourcegitcommit: cdb57f14960f58b1d36a1b373fbf35dfed5fad9e
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 02/23/2022
ms.locfileid: "8334980"
---
# <a name="available-fonts"></a>Available Fonts

The online version of [!INCLUDE[prod_short](includes/prod_short.md)] contains pre-installed fonts on the servers that can be used when generating reports. The following sections outline which fonts are available.

> [!NOTE]
> For security and legal reasons, you cannot upload custom fonts to the [!INCLUDE[prod_short](includes/prod_short.md)] environment.

## <a name="document-fonts"></a>Document Fonts

The following fonts are installed and available to use in both Word and RDLC report layouts:

* Arial
* Consolas
* Courier New
* Lucida Console
* Segoe Print
* Segoe Script
* Segoe UI
* Segoe UI Light
* Segoe UI Semilight
* Times New Roman

## <a name="fonts-for-checks"></a>Fonts for Cheques

Magnetic Ink Character Recognition (MICR) fonts are installed and available to use. Both the E-13B and the CMC-7 standards are supported.  

In addition to MICR fonts, special security fonts are available to generate text, names, amounts, and the currency symbols Dollar, Euro, Pound, and Yen, which are hard to tamper with once a cheque has been printed.  

For more information, see [Select a Cheque Layout](finance-how-define-check-layouts.md).  

## <a name="fonts-for-barcodes"></a>Fonts for Barcodes
Fonts to generate barcodes are installed and available to use in both Word and RDLC report layouts.

The following one-dimensional barcode symbologies are supported:
* Code 3 of 9 (Code 39)
* Code 128
* Code 93
* Codabar
* MSI
* Interleaved 2 of 5

The following two-dimensional barcode symbologies are supported:
* Aztec
* Data Matrix
* Maxicode
* PDF417
* QR

For more information, see [Barcode Fonts with Business Central Online](/dynamics365/business-central/dev-itpro/developer/devenv-report-barcode-fonts).

## <a name="see-also"></a>See Also

[Managing Report Layouts](ui-manage-report-layouts.md)  
[Select a Cheque Layout](finance-how-define-check-layouts.md)  
[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)
[Barcode Fonts with Business Central Online](/dynamics365/business-central/dev-itpro/developer/devenv-report-barcode-fonts)

[!INCLUDE[footer-include](includes/footer-banner.md)]
