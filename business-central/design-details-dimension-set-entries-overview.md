---
title: Dimension Set Entries Overview | Microsoft Docs
description: This topic describes how dimension set entries are stored and posted in Dynamcis 365.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: dimension
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 1113f371caf00b693144d0ea6f74aed49bbbc9df
ms.contentlocale: en-nz
ms.lasthandoff: 03/22/2018

---
# <a name="dimension-set-entries-overview"></a><span data-ttu-id="a9ccf-103">Dimension Set Entries Overview</span><span class="sxs-lookup"><span data-stu-id="a9ccf-103">Dimension Set Entries Overview</span></span>
<span data-ttu-id="a9ccf-104">This topic describes how dimension set entries are stored and posted in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="a9ccf-104">This topic describes how dimension set entries are stored and posted in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  
  
## <a name="dimension-sets"></a><span data-ttu-id="a9ccf-105">Dimension Sets</span><span class="sxs-lookup"><span data-stu-id="a9ccf-105">Dimension Sets</span></span>  
<span data-ttu-id="a9ccf-106">A dimension set is a unique combination of dimension values.</span><span class="sxs-lookup"><span data-stu-id="a9ccf-106">A dimension set is a unique combination of dimension values.</span></span> <span data-ttu-id="a9ccf-107">It is stored as dimension set entries in the database.</span><span class="sxs-lookup"><span data-stu-id="a9ccf-107">It is stored as dimension set entries in the database.</span></span> <span data-ttu-id="a9ccf-108">Each dimension set entry represents a single dimension value.</span><span class="sxs-lookup"><span data-stu-id="a9ccf-108">Each dimension set entry represents a single dimension value.</span></span> <span data-ttu-id="a9ccf-109">The dimension set is identified by a common dimension set ID that is assigned to each dimension set entry that belongs to the dimension set.</span><span class="sxs-lookup"><span data-stu-id="a9ccf-109">The dimension set is identified by a common dimension set ID that is assigned to each dimension set entry that belongs to the dimension set.</span></span>  
  
<span data-ttu-id="a9ccf-110">The following example shows a dimension set that has three dimension set entries.</span><span class="sxs-lookup"><span data-stu-id="a9ccf-110">The following example shows a dimension set that has three dimension set entries.</span></span> <span data-ttu-id="a9ccf-111">The dimension set is identified by a dimension set ID, which is 108.</span><span class="sxs-lookup"><span data-stu-id="a9ccf-111">The dimension set is identified by a dimension set ID, which is 108.</span></span>  
  
|<span data-ttu-id="a9ccf-112">Dimension Set ID</span><span class="sxs-lookup"><span data-stu-id="a9ccf-112">Dimension Set ID</span></span>|<span data-ttu-id="a9ccf-113">Dimension Code</span><span class="sxs-lookup"><span data-stu-id="a9ccf-113">Dimension Code</span></span>|<span data-ttu-id="a9ccf-114">Dimension Value Code</span><span class="sxs-lookup"><span data-stu-id="a9ccf-114">Dimension Value Code</span></span>|<span data-ttu-id="a9ccf-115">Dimension Value Name</span><span class="sxs-lookup"><span data-stu-id="a9ccf-115">Dimension Value Name</span></span>|  
|----------------------|--------------------|--------------------------|--------------------------|  
|<span data-ttu-id="a9ccf-116">108</span><span class="sxs-lookup"><span data-stu-id="a9ccf-116">108</span></span>|<span data-ttu-id="a9ccf-117">AREA</span><span class="sxs-lookup"><span data-stu-id="a9ccf-117">AREA</span></span>|<span data-ttu-id="a9ccf-118">70</span><span class="sxs-lookup"><span data-stu-id="a9ccf-118">70</span></span>|<span data-ttu-id="a9ccf-119">America North</span><span class="sxs-lookup"><span data-stu-id="a9ccf-119">America North</span></span>|  
|<span data-ttu-id="a9ccf-120">108</span><span class="sxs-lookup"><span data-stu-id="a9ccf-120">108</span></span>|<span data-ttu-id="a9ccf-121">BUSINESSGROUP</span><span class="sxs-lookup"><span data-stu-id="a9ccf-121">BUSINESSGROUP</span></span>|<span data-ttu-id="a9ccf-122">HOME</span><span class="sxs-lookup"><span data-stu-id="a9ccf-122">HOME</span></span>|<span data-ttu-id="a9ccf-123">Home</span><span class="sxs-lookup"><span data-stu-id="a9ccf-123">Home</span></span>|  
|<span data-ttu-id="a9ccf-124">108</span><span class="sxs-lookup"><span data-stu-id="a9ccf-124">108</span></span>|<span data-ttu-id="a9ccf-125">DEPARTMENT</span><span class="sxs-lookup"><span data-stu-id="a9ccf-125">DEPARTMENT</span></span>|<span data-ttu-id="a9ccf-126">SALES</span><span class="sxs-lookup"><span data-stu-id="a9ccf-126">SALES</span></span>|<span data-ttu-id="a9ccf-127">Sales</span><span class="sxs-lookup"><span data-stu-id="a9ccf-127">Sales</span></span>|  
  
## <a name="dimension-set-entries"></a><span data-ttu-id="a9ccf-128">Dimension Set Entries</span><span class="sxs-lookup"><span data-stu-id="a9ccf-128">Dimension Set Entries</span></span>  
<span data-ttu-id="a9ccf-129">Dimension sets are stored in the **Dimension Set Entry** table as dimension set entries with the same dimension set ID.</span><span class="sxs-lookup"><span data-stu-id="a9ccf-129">Dimension sets are stored in the **Dimension Set Entry** table as dimension set entries with the same dimension set ID.</span></span>  
  
<span data-ttu-id="a9ccf-130">![Dimension Entry overview](media/dimensionentrynav7.png "DimensionEntryNAV7")</span><span class="sxs-lookup"><span data-stu-id="a9ccf-130">![Dimension Entry overview](media/dimensionentrynav7.png "DimensionEntryNAV7")</span></span>  
  
<span data-ttu-id="a9ccf-131">When you create a new journal line, document header, or document line, you can specify a combination of dimension values.</span><span class="sxs-lookup"><span data-stu-id="a9ccf-131">When you create a new journal line, document header, or document line, you can specify a combination of dimension values.</span></span> <span data-ttu-id="a9ccf-132">Instead of explicitly storing each dimension value in the database, a dimension set ID is assigned to the journal line, document header, or document line to specify the dimension set.</span><span class="sxs-lookup"><span data-stu-id="a9ccf-132">Instead of explicitly storing each dimension value in the database, a dimension set ID is assigned to the journal line, document header, or document line to specify the dimension set.</span></span>  
  
<span data-ttu-id="a9ccf-133">When you edit and close the **Edit Dimension Set Entries** window, a check is performed to see whether the combination of dimension values exists as a dimension set in the table.</span><span class="sxs-lookup"><span data-stu-id="a9ccf-133">When you edit and close the **Edit Dimension Set Entries** window, a check is performed to see whether the combination of dimension values exists as a dimension set in the table.</span></span> <span data-ttu-id="a9ccf-134">If the combination occurs in the table, then the corresponding dimension set ID is assigned to the journal line, document header, or document line.</span><span class="sxs-lookup"><span data-stu-id="a9ccf-134">If the combination occurs in the table, then the corresponding dimension set ID is assigned to the journal line, document header, or document line.</span></span> <span data-ttu-id="a9ccf-135">Otherwise, a new dimension set is added to the table, and the new dimension set ID is assigned to the journal line, document header, or document line.</span><span class="sxs-lookup"><span data-stu-id="a9ccf-135">Otherwise, a new dimension set is added to the table, and the new dimension set ID is assigned to the journal line, document header, or document line.</span></span>  
  
## <a name="performance-improvement"></a><span data-ttu-id="a9ccf-136">Performance Improvement</span><span class="sxs-lookup"><span data-stu-id="a9ccf-136">Performance Improvement</span></span>  
<span data-ttu-id="a9ccf-137">By storing dimension sets once in the database, database space is preserved, and overall performance is improved.</span><span class="sxs-lookup"><span data-stu-id="a9ccf-137">By storing dimension sets once in the database, database space is preserved, and overall performance is improved.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="a9ccf-138">See Also</span><span class="sxs-lookup"><span data-stu-id="a9ccf-138">See Also</span></span>  
<span data-ttu-id="a9ccf-139">[Design Details: Searching for Dimension Combinations](design-details-searching-for-dimension-combinations.md) </span><span class="sxs-lookup"><span data-stu-id="a9ccf-139">[Design Details: Searching for Dimension Combinations](design-details-searching-for-dimension-combinations.md) </span></span>  
<span data-ttu-id="a9ccf-140">[Design Details: Table Structure](design-details-table-structure.md) </span><span class="sxs-lookup"><span data-stu-id="a9ccf-140">[Design Details: Table Structure](design-details-table-structure.md) </span></span>  
<span data-ttu-id="a9ccf-141">[Design Details: Codeunit 408 Dimension Management](design-details-codeunit-408-dimension-management.md) </span><span class="sxs-lookup"><span data-stu-id="a9ccf-141">[Design Details: Codeunit 408 Dimension Management](design-details-codeunit-408-dimension-management.md) </span></span>  
<span data-ttu-id="a9ccf-142">[Design Details: Code Examples of Changed Patterns in Modifications](design-details-code-examples-of-changed-patterns-in-modifications.md) </span><span class="sxs-lookup"><span data-stu-id="a9ccf-142">[Design Details: Code Examples of Changed Patterns in Modifications](design-details-code-examples-of-changed-patterns-in-modifications.md) </span></span>  
[<span data-ttu-id="a9ccf-143">Design Details: Dimension Set Entries</span><span class="sxs-lookup"><span data-stu-id="a9ccf-143">Design Details: Dimension Set Entries</span></span>](design-details-dimension-set-entries.md)   
