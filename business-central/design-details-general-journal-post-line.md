---
title: Design Details - General Journal Post Line | Microsoft Docs
description: This topic provides insight into the concepts and principles that are used to redesign the general journal posting line feature in Business Central.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: design, general journal, posting, codeunit 12
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: e7e61b572b2a7a1538d58430cbbcbb19d7cda999
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "5390090"
---
# <a name="design-details-general-journal-post-line"></a><span data-ttu-id="57ff7-103">Design Details: General Journal Post Line</span><span class="sxs-lookup"><span data-stu-id="57ff7-103">Design Details: General Journal Post Line</span></span>
<span data-ttu-id="57ff7-104">This documentation provides detailed technical insight into the concepts and principles that are used to redesign the general journal posting line feature in [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="57ff7-104">This documentation provides detailed technical insight into the concepts and principles that are used to redesign the general journal posting line feature in [!INCLUDE[prod_short](includes/prod_short.md)].</span></span> <span data-ttu-id="57ff7-105">The redesign makes codeunit 12 simpler and more maintainable.</span><span class="sxs-lookup"><span data-stu-id="57ff7-105">The redesign makes codeunit 12 simpler and more maintainable.</span></span> <span data-ttu-id="57ff7-106">The documentation starts by describing conceptual overviews of the redesign.</span><span class="sxs-lookup"><span data-stu-id="57ff7-106">The documentation starts by describing conceptual overviews of the redesign.</span></span> <span data-ttu-id="57ff7-107">Then it explains the technical architecture to show the changes that result from the redesign.</span><span class="sxs-lookup"><span data-stu-id="57ff7-107">Then it explains the technical architecture to show the changes that result from the redesign.</span></span>  

## <a name="in-this-section"></a><span data-ttu-id="57ff7-108">In This Section</span><span class="sxs-lookup"><span data-stu-id="57ff7-108">In This Section</span></span>  
[<span data-ttu-id="57ff7-109">General Journal Post Line Overview</span><span class="sxs-lookup"><span data-stu-id="57ff7-109">General Journal Post Line Overview</span></span>](design-details-general-journal-post-line-overview.md)  
[<span data-ttu-id="57ff7-110">Design Details: Posting Interface Structure</span><span class="sxs-lookup"><span data-stu-id="57ff7-110">Design Details: Posting Interface Structure</span></span>](design-details-posting-interface-structure.md)  
[<span data-ttu-id="57ff7-111">Design Details: Posting Engine Structure</span><span class="sxs-lookup"><span data-stu-id="57ff7-111">Design Details: Posting Engine Structure</span></span>](design-details-posting-engine-structure.md)  
[<span data-ttu-id="57ff7-112">Codeunit 12 Changes: Mapping Global Variables for General Journal Post Line</span><span class="sxs-lookup"><span data-stu-id="57ff7-112">Codeunit 12 Changes: Mapping Global Variables for General Journal Post Line</span></span>](design-details-codeunit-12-changes-mapping-global-variables-for-general-journal-post-line.md)  
[<span data-ttu-id="57ff7-113">Codeunit 12 Changes: Changes in General Journal Post Procedures</span><span class="sxs-lookup"><span data-stu-id="57ff7-113">Codeunit 12 Changes: Changes in General Journal Post Procedures</span></span>](design-details-codeunit-12-changes-changes-in-general-journal-post-procedures.md)  

## <a name="see-also"></a><span data-ttu-id="57ff7-114">See Also</span><span class="sxs-lookup"><span data-stu-id="57ff7-114">See Also</span></span>  
[<span data-ttu-id="57ff7-115">Working with General Journals</span><span class="sxs-lookup"><span data-stu-id="57ff7-115">Working with General Journals</span></span>](ui-work-general-journals.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]