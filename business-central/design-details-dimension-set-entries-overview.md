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
ms.date: 04/01/2020
ms.author: sgroespe
ms.openlocfilehash: f35184a6a69ed0fa1ccd504525a19af6bd9c5955
ms.sourcegitcommit: 88e4b30eaf6fa32af0c1452ce2f85ff1111c75e2
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 04/01/2020
ms.locfileid: "3185532"
---
# <a name="dimension-set-entries-overview"></a><span data-ttu-id="808ae-103">Dimension Set Entries Overview</span><span class="sxs-lookup"><span data-stu-id="808ae-103">Dimension Set Entries Overview</span></span>
<span data-ttu-id="808ae-104">This topic describes how dimension set entries are stored and posted in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="808ae-104">This topic describes how dimension set entries are stored and posted in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  

## <a name="dimension-sets"></a><span data-ttu-id="808ae-105">Dimension Sets</span><span class="sxs-lookup"><span data-stu-id="808ae-105">Dimension Sets</span></span>  
<span data-ttu-id="808ae-106">A dimension set is a unique combination of dimension values.</span><span class="sxs-lookup"><span data-stu-id="808ae-106">A dimension set is a unique combination of dimension values.</span></span> <span data-ttu-id="808ae-107">It is stored as dimension set entries in the database.</span><span class="sxs-lookup"><span data-stu-id="808ae-107">It is stored as dimension set entries in the database.</span></span> <span data-ttu-id="808ae-108">Each dimension set entry represents a single dimension value.</span><span class="sxs-lookup"><span data-stu-id="808ae-108">Each dimension set entry represents a single dimension value.</span></span> <span data-ttu-id="808ae-109">The dimension set is identified by a common dimension set ID that is assigned to each dimension set entry that belongs to the dimension set.</span><span class="sxs-lookup"><span data-stu-id="808ae-109">The dimension set is identified by a common dimension set ID that is assigned to each dimension set entry that belongs to the dimension set.</span></span>  

<span data-ttu-id="808ae-110">The following example shows a dimension set that has three dimension set entries.</span><span class="sxs-lookup"><span data-stu-id="808ae-110">The following example shows a dimension set that has three dimension set entries.</span></span> <span data-ttu-id="808ae-111">The dimension set is identified by a dimension set ID, which is 108.</span><span class="sxs-lookup"><span data-stu-id="808ae-111">The dimension set is identified by a dimension set ID, which is 108.</span></span>  

|<span data-ttu-id="808ae-112">Dimension Set ID</span><span class="sxs-lookup"><span data-stu-id="808ae-112">Dimension Set ID</span></span>|<span data-ttu-id="808ae-113">Dimension Code</span><span class="sxs-lookup"><span data-stu-id="808ae-113">Dimension Code</span></span>|<span data-ttu-id="808ae-114">Dimension Value Code</span><span class="sxs-lookup"><span data-stu-id="808ae-114">Dimension Value Code</span></span>|<span data-ttu-id="808ae-115">Dimension Value Name</span><span class="sxs-lookup"><span data-stu-id="808ae-115">Dimension Value Name</span></span>|  
|----------------------|--------------------|--------------------------|--------------------------|  
|<span data-ttu-id="808ae-116">108</span><span class="sxs-lookup"><span data-stu-id="808ae-116">108</span></span>|<span data-ttu-id="808ae-117">AREA</span><span class="sxs-lookup"><span data-stu-id="808ae-117">AREA</span></span>|<span data-ttu-id="808ae-118">70</span><span class="sxs-lookup"><span data-stu-id="808ae-118">70</span></span>|<span data-ttu-id="808ae-119">America North</span><span class="sxs-lookup"><span data-stu-id="808ae-119">America North</span></span>|  
|<span data-ttu-id="808ae-120">108</span><span class="sxs-lookup"><span data-stu-id="808ae-120">108</span></span>|<span data-ttu-id="808ae-121">BUSINESSGROUP</span><span class="sxs-lookup"><span data-stu-id="808ae-121">BUSINESSGROUP</span></span>|<span data-ttu-id="808ae-122">HOME</span><span class="sxs-lookup"><span data-stu-id="808ae-122">HOME</span></span>|<span data-ttu-id="808ae-123">Home</span><span class="sxs-lookup"><span data-stu-id="808ae-123">Home</span></span>|  
|<span data-ttu-id="808ae-124">108</span><span class="sxs-lookup"><span data-stu-id="808ae-124">108</span></span>|<span data-ttu-id="808ae-125">DEPARTMENT</span><span class="sxs-lookup"><span data-stu-id="808ae-125">DEPARTMENT</span></span>|<span data-ttu-id="808ae-126">SALES</span><span class="sxs-lookup"><span data-stu-id="808ae-126">SALES</span></span>|<span data-ttu-id="808ae-127">Sales</span><span class="sxs-lookup"><span data-stu-id="808ae-127">Sales</span></span>|  

## <a name="dimension-set-entries"></a><span data-ttu-id="808ae-128">Dimension Set Entries</span><span class="sxs-lookup"><span data-stu-id="808ae-128">Dimension Set Entries</span></span>  
<span data-ttu-id="808ae-129">Dimension sets are stored in the **Dimension Set Entry** table as dimension set entries with the same dimension set ID.</span><span class="sxs-lookup"><span data-stu-id="808ae-129">Dimension sets are stored in the **Dimension Set Entry** table as dimension set entries with the same dimension set ID.</span></span>  

<span data-ttu-id="808ae-130">![Flow of dimension set entries](media/dimensionentrynav7.png "Flow of dimension set entries")</span><span class="sxs-lookup"><span data-stu-id="808ae-130">![Flow of dimension set entries](media/dimensionentrynav7.png "Flow of dimension set entries")</span></span>  

<span data-ttu-id="808ae-131">When you create a new journal line, document header, or document line, you can specify a combination of dimension values.</span><span class="sxs-lookup"><span data-stu-id="808ae-131">When you create a new journal line, document header, or document line, you can specify a combination of dimension values.</span></span> <span data-ttu-id="808ae-132">Instead of explicitly storing each dimension value in the database, a dimension set ID is assigned to the journal line, document header, or document line to specify the dimension set.</span><span class="sxs-lookup"><span data-stu-id="808ae-132">Instead of explicitly storing each dimension value in the database, a dimension set ID is assigned to the journal line, document header, or document line to specify the dimension set.</span></span>  

<span data-ttu-id="808ae-133">When you edit and close the **Edit Dimension Set Entries** page, a check is performed to see whether the combination of dimension values exists as a dimension set in the table.</span><span class="sxs-lookup"><span data-stu-id="808ae-133">When you edit and close the **Edit Dimension Set Entries** page, a check is performed to see whether the combination of dimension values exists as a dimension set in the table.</span></span> <span data-ttu-id="808ae-134">If the combination occurs in the table, then the corresponding dimension set ID is assigned to the journal line, document header, or document line.</span><span class="sxs-lookup"><span data-stu-id="808ae-134">If the combination occurs in the table, then the corresponding dimension set ID is assigned to the journal line, document header, or document line.</span></span> <span data-ttu-id="808ae-135">Otherwise, a new dimension set is added to the table, and the new dimension set ID is assigned to the journal line, document header, or document line.</span><span class="sxs-lookup"><span data-stu-id="808ae-135">Otherwise, a new dimension set is added to the table, and the new dimension set ID is assigned to the journal line, document header, or document line.</span></span>

## <a name="codeunit-408-dimension-management"></a><span data-ttu-id="808ae-136">Codeunit 408 Dimension Management</span><span class="sxs-lookup"><span data-stu-id="808ae-136">Codeunit 408 Dimension Management</span></span>
<span data-ttu-id="808ae-137">Codeunit 408, Dimension Management, is a function library that handles common tasks that are related to dimensions, such as copying from one table to another or from one document to another.</span><span class="sxs-lookup"><span data-stu-id="808ae-137">Codeunit 408, Dimension Management, is a function library that handles common tasks that are related to dimensions, such as copying from one table to another or from one document to another.</span></span>

## <a name="performance-improvement"></a><span data-ttu-id="808ae-138">Performance Improvement</span><span class="sxs-lookup"><span data-stu-id="808ae-138">Performance Improvement</span></span>  
<span data-ttu-id="808ae-139">By storing dimension sets once in the database, database space is preserved and overall performance is improved.</span><span class="sxs-lookup"><span data-stu-id="808ae-139">By storing dimension sets once in the database, database space is preserved and overall performance is improved.</span></span>  

## <a name="see-also"></a><span data-ttu-id="808ae-140">See Also</span><span class="sxs-lookup"><span data-stu-id="808ae-140">See Also</span></span>  
<span data-ttu-id="808ae-141">[Design Details: Searching for Dimension Combinations](design-details-searching-for-dimension-combinations.md) </span><span class="sxs-lookup"><span data-stu-id="808ae-141">[Design Details: Searching for Dimension Combinations](design-details-searching-for-dimension-combinations.md) </span></span>  
<span data-ttu-id="808ae-142">[Design Details: Table Structure](design-details-table-structure.md) </span><span class="sxs-lookup"><span data-stu-id="808ae-142">[Design Details: Table Structure](design-details-table-structure.md) </span></span>  
[<span data-ttu-id="808ae-143">Design Details: Dimension Set Entries</span><span class="sxs-lookup"><span data-stu-id="808ae-143">Design Details: Dimension Set Entries</span></span>](design-details-dimension-set-entries.md)   
