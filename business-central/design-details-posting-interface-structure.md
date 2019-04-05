---
title: Design Details - Posting Interface Structure | Microsoft Docs
description: This topic provides an overview of the global procedures in the posting interface structure.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: posting, interface, design
ms.date: 10/01/2018
ms.author: sgroespe
ms.openlocfilehash: 236cbcc45ccca23905dcb79a491236c80b2bdebf
ms.sourcegitcommit: 1bcfaa99ea302e6b84b8361ca02730b135557fc1
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 03/08/2019
ms.locfileid: "822366"
---
# <a name="design-details-posting-interface-structure"></a><span data-ttu-id="a0297-103">Design Details: Posting Interface Structure</span><span class="sxs-lookup"><span data-stu-id="a0297-103">Design Details: Posting Interface Structure</span></span>
<span data-ttu-id="a0297-104">In the [!INCLUDE[d365fin](includes/d365fin_md.md)] posting interface structure, there are several global procedures that use the same structure:</span><span class="sxs-lookup"><span data-stu-id="a0297-104">In the [!INCLUDE[d365fin](includes/d365fin_md.md)] posting interface structure, there are several global procedures that use the same structure:</span></span>  
  
* <span data-ttu-id="a0297-105">RunWithCheck and RunWithoutCheck call procedure Code – generic posting interface for Gen. Jnl Line.</span><span class="sxs-lookup"><span data-stu-id="a0297-105">RunWithCheck and RunWithoutCheck call procedure Code – generic posting interface for Gen. Jnl Line.</span></span>  
* <span data-ttu-id="a0297-106">CustPostApplyCustLedgEntry – post customer application, called from codeunit 226 CustEntry-Apply Posted Entries.</span><span class="sxs-lookup"><span data-stu-id="a0297-106">CustPostApplyCustLedgEntry – post customer application, called from codeunit 226 CustEntry-Apply Posted Entries.</span></span>  
* <span data-ttu-id="a0297-107">VendPostApplyVendLedgEntry – post vendor application, called from codeunit 227 VendEntry-Apply Posted Entries.</span><span class="sxs-lookup"><span data-stu-id="a0297-107">VendPostApplyVendLedgEntry – post vendor application, called from codeunit 227 VendEntry-Apply Posted Entries.</span></span>  
* <span data-ttu-id="a0297-108">UnapplyCustLedgEntry – post unapply of customer application, called from codeunit 226 CustEntry-Apply Posted Entries</span><span class="sxs-lookup"><span data-stu-id="a0297-108">UnapplyCustLedgEntry – post unapply of customer application, called from codeunit 226 CustEntry-Apply Posted Entries</span></span>  
* <span data-ttu-id="a0297-109">UnapplyVendLedgEntry – post unapply of vendor application, called from codeunit 227 VendEntry-Apply Posted Entries</span><span class="sxs-lookup"><span data-stu-id="a0297-109">UnapplyVendLedgEntry – post unapply of vendor application, called from codeunit 227 VendEntry-Apply Posted Entries</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="a0297-110">See Also</span><span class="sxs-lookup"><span data-stu-id="a0297-110">See Also</span></span>  
[<span data-ttu-id="a0297-111">Design Details: Posting Engine Structure</span><span class="sxs-lookup"><span data-stu-id="a0297-111">Design Details: Posting Engine Structure</span></span>](design-details-posting-engine-structure.md)