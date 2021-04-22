---
title: General Journal Post Line Overview | Microsoft Docs
description: This topic introduces changes to Codeunit 12, **Gen. Jnl.-Post Line**, which is the major application object for general ledger posting and is the only place to insert general ledger, GST, and customer and vendor ledger entries.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: design, general ledger, post
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 6866e852899df3de3de2c4560c26ad981e46fda5
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 03/31/2021
ms.locfileid: "5777864"
---
# <a name="general-journal-post-line-overview"></a>General Journal Post Line Overview
Codeunit 12, **Gen. Jnl.-Post Line**, is the major application object for general ledger posting and is the only place to insert general ledger, GST, and customer and vendor ledger entries. This codeunit is also used for all Apply, Unapply and Reverse operations.  
  
While the codeunit has been improved in each release over the last ten years, its architecture remained essentially unchanged. The codeunit became very large, with approximately 7,600 code lines. With this release of [!INCLUDE[prod_short](includes/prod_short.md)], the architecture is changed and the codeunit has been made simpler and more maintainable. This documentation introduces the changes and provides information that you will need for upgrade.  
  
## <a name="old-architecture"></a>Old Architecture  
The old architecture had the following features:  
  
* There was extensive use of global variables, which increased the possibility of hidden errors due to use of variables with the wrong scope.  
* There were many long procedures (with more than 100 code lines) that also had high cyclomatic complexity (that is, a lot of CASE, REPEAT, IF nested statements), which made the code very difficult to read and maintain.  
* Several procedures that were only used locally and were only meant to be used locally were not marked as local.  
* Most procedures had no parameters and used global variables. Some used parameters and overrode global variables with locals.  
* Code patterns for searching the general ledger accounts and creating general ledger and GST entries was not standardised and varied from place to place. In addition, there was a lot of code duplication and broken symmetry between customer and vendor code.  
* A large part of the code in codeunit 12, approximately 30 percent, related to payment discount and tolerance calculations, although these features are not needed in many countries or regions.  
* Posting, Apply, Unapply, Reverse, Payment Discount and Tolerance, and Exchange Rate Adjustment were married together in codeunit 12 using a long list of global variables.  
  
### <a name="new-architecture"></a>New Architecture  
In [!INCLUDE[prod_short](includes/prod_short.md)], codeunit 12 has had the following improvements:  
  
* Codeunit 12 has been refactored into smaller procedures (all less than 100 code lines).  
* Standardised patterns for the search of general ledger accounts have been implemented by using helper functions from Posting Group tables.  
* A Posting Engine Framework has been implemented to manage the start and finish of transactions and to isolate the creation to general ledger and GST entries, the collection of GST adjustment, and the calculation of additional currency amounts.  
* Code duplication has been eliminated.  
* Many helper functions have been transferred to corresponding customer and vendor ledger entry tables.  
* The use of global variables has been minimised, so that each procedure uses parameters and encapsulates its own application logic.  
  
## <a name="see-also"></a>See Also  
[Design Details: Posting Interface Structure](design-details-posting-interface-structure.md)   
[Design Details: Posting Engine Structure](design-details-posting-engine-structure.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]