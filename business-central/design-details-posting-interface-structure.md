---
title: Design Details - Posting Interface Structure | Microsoft Docs
description: This topic provides an overview of the global procedures in the posting interface structure.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: posting, interface, design
ms.date: 06/08/2021
ms.author: edupont
ms.openlocfilehash: 529a0e42d814f0754e62fcc4b93b793d44b8daa7
ms.sourcegitcommit: 0953171d39e1232a7c126142d68cac858234a20e
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 06/09/2021
ms.locfileid: "6215844"
---
# <a name="design-details-posting-interface-structure"></a><span data-ttu-id="641a8-103">Design Details: Posting Interface Structure</span><span class="sxs-lookup"><span data-stu-id="641a8-103">Design Details: Posting Interface Structure</span></span>
<span data-ttu-id="641a8-104">In the [!INCLUDE[prod_short](includes/prod_short.md)] posting interface structure, there are several global procedures that use the same structure:</span><span class="sxs-lookup"><span data-stu-id="641a8-104">In the [!INCLUDE[prod_short](includes/prod_short.md)] posting interface structure, there are several global procedures that use the same structure:</span></span>  
  
* <span data-ttu-id="641a8-105">RunWithCheck and RunWithoutCheck call procedure Code – generic posting interface for Gen.</span><span class="sxs-lookup"><span data-stu-id="641a8-105">RunWithCheck and RunWithoutCheck call procedure Code – generic posting interface for Gen.</span></span> <span data-ttu-id="641a8-106">Jnl Line.</span><span class="sxs-lookup"><span data-stu-id="641a8-106">Jnl Line.</span></span>  
* <span data-ttu-id="641a8-107">CustPostApplyCustLedgEntry – post customer application, called from codeunit 226 CustEntry-Apply Posted Entries.</span><span class="sxs-lookup"><span data-stu-id="641a8-107">CustPostApplyCustLedgEntry – post customer application, called from codeunit 226 CustEntry-Apply Posted Entries.</span></span>  
* <span data-ttu-id="641a8-108">VendPostApplyVendLedgEntry – post vendor application, called from codeunit 227 VendEntry-Apply Posted Entries.</span><span class="sxs-lookup"><span data-stu-id="641a8-108">VendPostApplyVendLedgEntry – post vendor application, called from codeunit 227 VendEntry-Apply Posted Entries.</span></span>  
* <span data-ttu-id="641a8-109">UnapplyCustLedgEntry – post unapply of customer application, called from codeunit 226 CustEntry-Apply Posted Entries</span><span class="sxs-lookup"><span data-stu-id="641a8-109">UnapplyCustLedgEntry – post unapply of customer application, called from codeunit 226 CustEntry-Apply Posted Entries</span></span>  
* <span data-ttu-id="641a8-110">UnapplyVendLedgEntry – post unapply of vendor application, called from codeunit 227 VendEntry-Apply Posted Entries</span><span class="sxs-lookup"><span data-stu-id="641a8-110">UnapplyVendLedgEntry – post unapply of vendor application, called from codeunit 227 VendEntry-Apply Posted Entries</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="641a8-111">See Also</span><span class="sxs-lookup"><span data-stu-id="641a8-111">See Also</span></span>  
[<span data-ttu-id="641a8-112">Design Details: Posting Engine Structure</span><span class="sxs-lookup"><span data-stu-id="641a8-112">Design Details: Posting Engine Structure</span></span>](design-details-posting-engine-structure.md)

[!INCLUDE[footer-include](includes/footer-banner.md)]