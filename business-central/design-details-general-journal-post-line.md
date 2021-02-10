---
title: Design Details - General Journal Post Line | Microsoft Docs
description: This topic provides insight into the concepts and principles that are used to redesign the general journal posting line feature in Business Central.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: design, general journal, posting, codeunit 12
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 56cf606151f687cf48138b3e14758d7febc47db6
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 12/17/2020
ms.locfileid: "4751596"
---
# <a name="design-details-general-journal-post-line"></a><span data-ttu-id="ab971-103">Design Details: General Journal Post Line</span><span class="sxs-lookup"><span data-stu-id="ab971-103">Design Details: General Journal Post Line</span></span>
<span data-ttu-id="ab971-104">This documentation provides detailed technical insight into the concepts and principles that are used to redesign the general journal posting line feature in [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="ab971-104">This documentation provides detailed technical insight into the concepts and principles that are used to redesign the general journal posting line feature in [!INCLUDE[prod_short](includes/prod_short.md)].</span></span> <span data-ttu-id="ab971-105">The redesign makes codeunit 12 simpler and more maintainable.</span><span class="sxs-lookup"><span data-stu-id="ab971-105">The redesign makes codeunit 12 simpler and more maintainable.</span></span> <span data-ttu-id="ab971-106">The documentation starts by describing conceptual overviews of the redesign.</span><span class="sxs-lookup"><span data-stu-id="ab971-106">The documentation starts by describing conceptual overviews of the redesign.</span></span> <span data-ttu-id="ab971-107">Then it explains the technical architecture to show the changes that result from the redesign.</span><span class="sxs-lookup"><span data-stu-id="ab971-107">Then it explains the technical architecture to show the changes that result from the redesign.</span></span>  

## <a name="in-this-section"></a><span data-ttu-id="ab971-108">In This Section</span><span class="sxs-lookup"><span data-stu-id="ab971-108">In This Section</span></span>  
[<span data-ttu-id="ab971-109">General Journal Post Line Overview</span><span class="sxs-lookup"><span data-stu-id="ab971-109">General Journal Post Line Overview</span></span>](design-details-general-journal-post-line-overview.md)  
[<span data-ttu-id="ab971-110">Design Details: Posting Interface Structure</span><span class="sxs-lookup"><span data-stu-id="ab971-110">Design Details: Posting Interface Structure</span></span>](design-details-posting-interface-structure.md)  
[<span data-ttu-id="ab971-111">Design Details: Posting Engine Structure</span><span class="sxs-lookup"><span data-stu-id="ab971-111">Design Details: Posting Engine Structure</span></span>](design-details-posting-engine-structure.md)  
[<span data-ttu-id="ab971-112">Codeunit 12 Changes: Mapping Global Variables for General Journal Post Line</span><span class="sxs-lookup"><span data-stu-id="ab971-112">Codeunit 12 Changes: Mapping Global Variables for General Journal Post Line</span></span>](design-details-codeunit-12-changes-mapping-global-variables-for-general-journal-post-line.md)  
[<span data-ttu-id="ab971-113">Codeunit 12 Changes: Changes in General Journal Post Procedures</span><span class="sxs-lookup"><span data-stu-id="ab971-113">Codeunit 12 Changes: Changes in General Journal Post Procedures</span></span>](design-details-codeunit-12-changes-changes-in-general-journal-post-procedures.md)  

## <a name="see-also"></a><span data-ttu-id="ab971-114">See Also</span><span class="sxs-lookup"><span data-stu-id="ab971-114">See Also</span></span>  
[<span data-ttu-id="ab971-115">Working with General Journals</span><span class="sxs-lookup"><span data-stu-id="ab971-115">Working with General Journals</span></span>](ui-work-general-journals.md)
