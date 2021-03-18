---
title: Set Up Withholding Tax in the New Zealand version
description: Describes how to set things up for Withholding tax (WHT) in the New Zealand version.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 80071d6f1479455aa2db813a65d4d1f7aa4756e2
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "5383554"
---
# <a name="set-up-withholding-tax-in-the-new-zealand-version"></a><span data-ttu-id="b17b4-103">Set Up Withholding Tax in the New Zealand Version</span><span class="sxs-lookup"><span data-stu-id="b17b4-103">Set Up Withholding Tax in the New Zealand Version</span></span>

<span data-ttu-id="b17b4-104">Withholding tax (WHT) is the tax withheld by a company when it makes a payment to a vendor, in which the full amount owed to the vendor is reduced by the tax withheld.</span><span class="sxs-lookup"><span data-stu-id="b17b4-104">Withholding tax (WHT) is the tax withheld by a company when it makes a payment to a vendor, in which the full amount owed to the vendor is reduced by the tax withheld.</span></span> <span data-ttu-id="b17b4-105">The withheld tax is then remitted to tax authorities when the next Business Activity Statement (BAS) is submitted.</span><span class="sxs-lookup"><span data-stu-id="b17b4-105">The withheld tax is then remitted to tax authorities when the next Business Activity Statement (BAS) is submitted.</span></span>  

<span data-ttu-id="b17b4-106">If a supplier without a New Zealand Inland Revenue Department number (IRD) provides an invoice, a withholding tax amount must be withheld if the total amount of the invoice is more than the threshold amount.</span><span class="sxs-lookup"><span data-stu-id="b17b4-106">If a supplier without a New Zealand Inland Revenue Department number (IRD) provides an invoice, a withholding tax amount must be withheld if the total amount of the invoice is more than the threshold amount.</span></span>  

<span data-ttu-id="b17b4-107">To use withholding tax, you must set up the business posting groups and product posting groups for withholding tax so that the correct WHT calculations are made for each vendor.</span><span class="sxs-lookup"><span data-stu-id="b17b4-107">To use withholding tax, you must set up the business posting groups and product posting groups for withholding tax so that the correct WHT calculations are made for each vendor.</span></span>  

> [!NOTE]  
> <span data-ttu-id="b17b4-108">As a prerequisite, you need to set up source codes for WHT settlement on the **Source Code Setup** page.</span><span class="sxs-lookup"><span data-stu-id="b17b4-108">As a prerequisite, you need to set up source codes for WHT settlement on the **Source Code Setup** page.</span></span>  

<span data-ttu-id="b17b4-109">The following procedure describes how to set up product posting groups for WHT, but the same steps also apply to setting up business posting groups for WHT.</span><span class="sxs-lookup"><span data-stu-id="b17b4-109">The following procedure describes how to set up product posting groups for WHT, but the same steps also apply to setting up business posting groups for WHT.</span></span>  

[!INCLUDE [wht-posting-group-setup](../includes/AUNZ/wht-posting-group-setup.md)]

## <a name="see-also"></a><span data-ttu-id="b17b4-110">See Also</span><span class="sxs-lookup"><span data-stu-id="b17b4-110">See Also</span></span>

<span data-ttu-id="b17b4-111">[Set Up Revenue Types for Withholding Tax](how-to-set-up-revenue-types-for-withholding-tax.md) </span><span class="sxs-lookup"><span data-stu-id="b17b4-111">[Set Up Revenue Types for Withholding Tax](how-to-set-up-revenue-types-for-withholding-tax.md) </span></span>  
<span data-ttu-id="b17b4-112">[View Withholding Tax Entries](how-to-view-withholding-tax-entries.md) </span><span class="sxs-lookup"><span data-stu-id="b17b4-112">[View Withholding Tax Entries](how-to-view-withholding-tax-entries.md) </span></span>  
<span data-ttu-id="b17b4-113">[Calculate and Post Withholding Tax Settlements](how-to-calculate-and-post-withholding-tax-settlements.md) </span><span class="sxs-lookup"><span data-stu-id="b17b4-113">[Calculate and Post Withholding Tax Settlements](how-to-calculate-and-post-withholding-tax-settlements.md) </span></span>  
[<span data-ttu-id="b17b4-114">Withholding Tax</span><span class="sxs-lookup"><span data-stu-id="b17b4-114">Withholding Tax</span></span>](withholding-tax.md)   


[!INCLUDE[footer-include](../../includes/footer-banner.md)]