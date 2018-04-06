---
title: General Journal Post Line Overview | Microsoft Docs
description: This topic introduces changes to Codeunit 12, **Gen. Jnl.-Post Line**, which is the major application object for general ledger posting and is the only place to insert general ledger, GST, and customer and vendor ledger entries.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: design, general ledger, post
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 77fa52505dc586dc11ca89e53f6eec75042d3606
ms.contentlocale: en-nz
ms.lasthandoff: 03/22/2018

---
# <a name="general-journal-post-line-overview"></a><span data-ttu-id="eb5ca-103">General Journal Post Line Overview</span><span class="sxs-lookup"><span data-stu-id="eb5ca-103">General Journal Post Line Overview</span></span>
<span data-ttu-id="eb5ca-104">Codeunit 12, **Gen. Jnl.-Post Line**, is the major application object for general ledger posting and is the only place to insert general ledger, GST, and customer and vendor ledger entries.</span><span class="sxs-lookup"><span data-stu-id="eb5ca-104">Codeunit 12, **Gen. Jnl.-Post Line**, is the major application object for general ledger posting and is the only place to insert general ledger, VAT, and customer and vendor ledger entries.</span></span> <span data-ttu-id="eb5ca-105">This codeunit is also used for all Apply, Unapply and Reverse operations.</span><span class="sxs-lookup"><span data-stu-id="eb5ca-105">This codeunit is also used for all Apply, Unapply and Reverse operations.</span></span>  
  
<span data-ttu-id="eb5ca-106">While the codeunit has been improved in each release over the last ten years, its architecture remained essentially unchanged.</span><span class="sxs-lookup"><span data-stu-id="eb5ca-106">While the codeunit has been improved in each release over the last ten years, its architecture remained essentially unchanged.</span></span> <span data-ttu-id="eb5ca-107">The codeunit became very large, with approximately 7,600 code lines.</span><span class="sxs-lookup"><span data-stu-id="eb5ca-107">The codeunit became very large, with approximately 7,600 code lines.</span></span> <span data-ttu-id="eb5ca-108">With this release of [!INCLUDE[d365fin](includes/d365fin_md.md)], the architecture is changed and the codeunit has been made simpler and more maintainable.</span><span class="sxs-lookup"><span data-stu-id="eb5ca-108">With this release of [!INCLUDE[d365fin](includes/d365fin_md.md)], the architecture is changed and the codeunit has been made simpler and more maintainable.</span></span> <span data-ttu-id="eb5ca-109">This documentation introduces the changes and provides information that you will need for upgrade.</span><span class="sxs-lookup"><span data-stu-id="eb5ca-109">This documentation introduces the changes and provides information that you will need for upgrade.</span></span>  
  
## <a name="old-architecture"></a><span data-ttu-id="eb5ca-110">Old Architecture</span><span class="sxs-lookup"><span data-stu-id="eb5ca-110">Old Architecture</span></span>  
<span data-ttu-id="eb5ca-111">The old architecture had the following features:</span><span class="sxs-lookup"><span data-stu-id="eb5ca-111">The old architecture had the following features:</span></span>  
  
* <span data-ttu-id="eb5ca-112">There was extensive use of global variables, which increased the possibility of hidden errors due to use of variables with the wrong scope.</span><span class="sxs-lookup"><span data-stu-id="eb5ca-112">There was extensive use of global variables, which increased the possibility of hidden errors due to use of variables with the wrong scope.</span></span>  
* <span data-ttu-id="eb5ca-113">There were many long procedures (with more than 100 code lines) that also had high cyclomatic complexity (that is, a lot of CASE, REPEAT, IF nested statements), which made the code very difficult to read and maintain.</span><span class="sxs-lookup"><span data-stu-id="eb5ca-113">There were many long procedures (with more than 100 code lines) that also had high cyclomatic complexity (that is, a lot of CASE, REPEAT, IF nested statements), which made the code very difficult to read and maintain.</span></span>  
* <span data-ttu-id="eb5ca-114">Several procedures that were only used locally and were only meant to be used locally were not marked as local.</span><span class="sxs-lookup"><span data-stu-id="eb5ca-114">Several procedures that were only used locally and were only meant to be used locally were not marked as local.</span></span>  
* <span data-ttu-id="eb5ca-115">Most procedures had no parameters and used global variables.</span><span class="sxs-lookup"><span data-stu-id="eb5ca-115">Most procedures had no parameters and used global variables.</span></span> <span data-ttu-id="eb5ca-116">Some used parameters and overrode global variables with locals.</span><span class="sxs-lookup"><span data-stu-id="eb5ca-116">Some used parameters and overrode global variables with locals.</span></span>  
* <span data-ttu-id="eb5ca-117">Code patterns for searching the general ledger accounts and creating general ledger and GST entries was not standardised and varied from place to place.</span><span class="sxs-lookup"><span data-stu-id="eb5ca-117">Code patterns for searching the general ledger accounts and creating general ledger and VAT entries was not standardized and varied from place to place.</span></span> <span data-ttu-id="eb5ca-118">In addition, there was a lot of code duplication and broken symmetry between customer and vendor code.</span><span class="sxs-lookup"><span data-stu-id="eb5ca-118">In addition, there was a lot of code duplication and broken symmetry between customer and vendor code.</span></span>  
* <span data-ttu-id="eb5ca-119">A large part of the code in codeunit 12, approximately 30 percent, related to payment discount and tolerance calculations, although these features are not needed in many countries or regions.</span><span class="sxs-lookup"><span data-stu-id="eb5ca-119">A large part of the code in codeunit 12, approximately 30 percent, related to payment discount and tolerance calculations, although these features are not needed in many countries or regions.</span></span>  
* <span data-ttu-id="eb5ca-120">Posting, Apply, Unapply, Reverse, Payment Discount and Tolerance, and Exchange Rate Adjustment were married together in codeunit 12 using a long list of global variables.</span><span class="sxs-lookup"><span data-stu-id="eb5ca-120">Posting, Apply, Unapply, Reverse, Payment Discount and Tolerance, and Exchange Rate Adjustment were married together in codeunit 12 using a long list of global variables.</span></span>  
  
### <a name="new-architecture"></a><span data-ttu-id="eb5ca-121">New Architecture</span><span class="sxs-lookup"><span data-stu-id="eb5ca-121">New Architecture</span></span>  
<span data-ttu-id="eb5ca-122">In [!INCLUDE[d365fin](includes/d365fin_md.md)], codeunit 12 has had the following improvements:</span><span class="sxs-lookup"><span data-stu-id="eb5ca-122">In [!INCLUDE[d365fin](includes/d365fin_md.md)], codeunit 12 has had the following improvements:</span></span>  
  
* <span data-ttu-id="eb5ca-123">Codeunit 12 has been refactored into smaller procedures (all less than 100 code lines).</span><span class="sxs-lookup"><span data-stu-id="eb5ca-123">Codeunit 12 has been refactored into smaller procedures (all less than 100 code lines).</span></span>  
* <span data-ttu-id="eb5ca-124">Standardised patterns for the search of general ledger accounts have been implemented by using helper functions from Posting Group tables.</span><span class="sxs-lookup"><span data-stu-id="eb5ca-124">Standardized patterns for the search of general ledger accounts have been implemented by using helper functions from Posting Group tables.</span></span>  
* <span data-ttu-id="eb5ca-125">A Posting Engine Framework has been implemented to manage the start and finish of transactions and to isolate the creation to general ledger and GST entries, the collection of GST adjustment, and the calculation of additional currency amounts.</span><span class="sxs-lookup"><span data-stu-id="eb5ca-125">A Posting Engine Framework has been implemented to manage the start and finish of transactions and to isolate the creation to general ledger and VAT entries, the collection of VAT adjustment, and the calculation of additional currency amounts.</span></span>  
* <span data-ttu-id="eb5ca-126">Code duplication has been eliminated.</span><span class="sxs-lookup"><span data-stu-id="eb5ca-126">Code duplication has been eliminated.</span></span>  
* <span data-ttu-id="eb5ca-127">Many helper functions have been transferred to corresponding customer and vendor ledger entry tables.</span><span class="sxs-lookup"><span data-stu-id="eb5ca-127">Many helper functions have been transferred to corresponding customer and vendor ledger entry tables.</span></span>  
* <span data-ttu-id="eb5ca-128">The use of global variables has been minimised, so that each procedure uses parameters and encapsulates its own application logic.</span><span class="sxs-lookup"><span data-stu-id="eb5ca-128">The use of global variables has been minimized, so that each procedure uses parameters and encapsulates its own application logic.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="eb5ca-129">See Also</span><span class="sxs-lookup"><span data-stu-id="eb5ca-129">See Also</span></span>  
<span data-ttu-id="eb5ca-130">[Design Details: Posting Interface Structure](design-details-posting-interface-structure.md) </span><span class="sxs-lookup"><span data-stu-id="eb5ca-130">[Design Details: Posting Interface Structure](design-details-posting-interface-structure.md) </span></span>  
[<span data-ttu-id="eb5ca-131">Design Details: Posting Engine Structure</span><span class="sxs-lookup"><span data-stu-id="eb5ca-131">Design Details: Posting Engine Structure</span></span>](design-details-posting-engine-structure.md)

