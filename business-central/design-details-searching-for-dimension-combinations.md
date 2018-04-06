---
title: Design Details - Searching for Dimension Combinations | Microsoft Docs
description: When you close a window after you edit a set of dimensions, Business Central evaluates whether the edited set of dimensions exists. If the set does not exist, a new set is created and the dimension combination ID is returned.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 416fe8425d2b21f1f1f72b2f159bb6a863bc1d8b
ms.contentlocale: en-nz
ms.lasthandoff: 03/22/2018

---
# <a name="design-details-searching-for-dimension-combinations"></a><span data-ttu-id="997cb-104">Design Details: Searching for Dimension Combinations</span><span class="sxs-lookup"><span data-stu-id="997cb-104">Design Details: Searching for Dimension Combinations</span></span>
<span data-ttu-id="997cb-105">When you close a window after you edit a set of dimensions, [!INCLUDE[d365fin](includes/d365fin_md.md)] evaluates whether the edited set of dimensions exists.</span><span class="sxs-lookup"><span data-stu-id="997cb-105">When you close a window after you edit a set of dimensions, [!INCLUDE[d365fin](includes/d365fin_md.md)] evaluates whether the edited set of dimensions exists.</span></span> <span data-ttu-id="997cb-106">If the set does not exist, a new set is created and the dimension combination ID is returned.</span><span class="sxs-lookup"><span data-stu-id="997cb-106">If the set does not exist, a new set is created and the dimension combination ID is returned.</span></span>  

## <a name="building-search-tree"></a><span data-ttu-id="997cb-107">Building Search Tree</span><span class="sxs-lookup"><span data-stu-id="997cb-107">Building Search Tree</span></span>  
 <span data-ttu-id="997cb-108">Table 481 **Dimension Set Tree Node** is used when [!INCLUDE[d365fin](includes/d365fin_md.md)] evaluates whether a set of dimensions already exists in table 480 **Dimension Set Entry** table.</span><span class="sxs-lookup"><span data-stu-id="997cb-108">Table 481 **Dimension Set Tree Node** is used when [!INCLUDE[d365fin](includes/d365fin_md.md)] evaluates whether a set of dimensions already exists in table 480 **Dimension Set Entry** table.</span></span> <span data-ttu-id="997cb-109">The evaluation is performed by recursively traversing the search tree starting at the top level numbered 0.</span><span class="sxs-lookup"><span data-stu-id="997cb-109">The evaluation is performed by recursively traversing the search tree starting at the top level numbered 0.</span></span> <span data-ttu-id="997cb-110">The top level 0 represents a dimension set with no dimension set entries.</span><span class="sxs-lookup"><span data-stu-id="997cb-110">The top level 0 represents a dimension set with no dimension set entries.</span></span> <span data-ttu-id="997cb-111">The children of this dimension set represent dimension sets with only one dimension set entry.</span><span class="sxs-lookup"><span data-stu-id="997cb-111">The children of this dimension set represent dimension sets with only one dimension set entry.</span></span> <span data-ttu-id="997cb-112">The children of these dimension sets represent dimension sets with two children, and so on.</span><span class="sxs-lookup"><span data-stu-id="997cb-112">The children of these dimension sets represent dimension sets with two children, and so on.</span></span>  

### <a name="example-1"></a><span data-ttu-id="997cb-113">Example 1</span><span class="sxs-lookup"><span data-stu-id="997cb-113">Example 1</span></span>  
 <span data-ttu-id="997cb-114">The following diagram represents a search tree with six dimension sets.</span><span class="sxs-lookup"><span data-stu-id="997cb-114">The following diagram represents a search tree with six dimension sets.</span></span> <span data-ttu-id="997cb-115">Only the distinguishing dimension set entry is displayed in the diagram.</span><span class="sxs-lookup"><span data-stu-id="997cb-115">Only the distinguishing dimension set entry is displayed in the diagram.</span></span>  

 <span data-ttu-id="997cb-116">![Dimension tree structure](media/nav2013_dimension_tree.png "NAV2013_Dimension_Tree")</span><span class="sxs-lookup"><span data-stu-id="997cb-116">![Dimension tree structure](media/nav2013_dimension_tree.png "NAV2013_Dimension_Tree")</span></span>  

 <span data-ttu-id="997cb-117">The following table describes a complete list of dimension set entries that make up each dimension set.</span><span class="sxs-lookup"><span data-stu-id="997cb-117">The following table describes a complete list of dimension set entries that make up each dimension set.</span></span>  

|<span data-ttu-id="997cb-118">Dimension Sets</span><span class="sxs-lookup"><span data-stu-id="997cb-118">Dimension Sets</span></span>|<span data-ttu-id="997cb-119">Dimension Set Entries</span><span class="sxs-lookup"><span data-stu-id="997cb-119">Dimension Set Entries</span></span>|  
|--------------------|---------------------------|  
|<span data-ttu-id="997cb-120">Set 0</span><span class="sxs-lookup"><span data-stu-id="997cb-120">Set 0</span></span>|<span data-ttu-id="997cb-121">None</span><span class="sxs-lookup"><span data-stu-id="997cb-121">None</span></span>|  
|<span data-ttu-id="997cb-122">Set 1</span><span class="sxs-lookup"><span data-stu-id="997cb-122">Set 1</span></span>|<span data-ttu-id="997cb-123">AREA 30</span><span class="sxs-lookup"><span data-stu-id="997cb-123">AREA 30</span></span>|  
|<span data-ttu-id="997cb-124">Set 2</span><span class="sxs-lookup"><span data-stu-id="997cb-124">Set 2</span></span>|<span data-ttu-id="997cb-125">AREA 30, DEPT ADM</span><span class="sxs-lookup"><span data-stu-id="997cb-125">AREA 30, DEPT ADM</span></span>|  
|<span data-ttu-id="997cb-126">Set 3</span><span class="sxs-lookup"><span data-stu-id="997cb-126">Set 3</span></span>|<span data-ttu-id="997cb-127">AREA 30, DEPT PROD</span><span class="sxs-lookup"><span data-stu-id="997cb-127">AREA 30, DEPT PROD</span></span>|  
|<span data-ttu-id="997cb-128">Set 4</span><span class="sxs-lookup"><span data-stu-id="997cb-128">Set 4</span></span>|<span data-ttu-id="997cb-129">AREA 30, DEPT ADM, PROJ VW</span><span class="sxs-lookup"><span data-stu-id="997cb-129">AREA 30, DEPT ADM, PROJ VW</span></span>|  
|<span data-ttu-id="997cb-130">Set 5</span><span class="sxs-lookup"><span data-stu-id="997cb-130">Set 5</span></span>|<span data-ttu-id="997cb-131">AREA 40</span><span class="sxs-lookup"><span data-stu-id="997cb-131">AREA 40</span></span>|  
|<span data-ttu-id="997cb-132">Set 6</span><span class="sxs-lookup"><span data-stu-id="997cb-132">Set 6</span></span>|<span data-ttu-id="997cb-133">AREA 40, PROJ VW</span><span class="sxs-lookup"><span data-stu-id="997cb-133">AREA 40, PROJ VW</span></span>|  

### <a name="example-2"></a><span data-ttu-id="997cb-134">Example 2</span><span class="sxs-lookup"><span data-stu-id="997cb-134">Example 2</span></span>  
 <span data-ttu-id="997cb-135">This example shows how [!INCLUDE[d365fin](includes/d365fin_md.md)] evaluates whether a dimension set that consists of the dimension set entries AREA 40, DEPT PROD exists.</span><span class="sxs-lookup"><span data-stu-id="997cb-135">This example shows how [!INCLUDE[d365fin](includes/d365fin_md.md)] evaluates whether a dimension set that consists of the dimension set entries AREA 40, DEPT PROD exists.</span></span>  

 <span data-ttu-id="997cb-136">First, [!INCLUDE[d365fin](includes/d365fin_md.md)] also updates the **Dimension Set Tree Node** table to make sure that the search tree looks like the following diagram.</span><span class="sxs-lookup"><span data-stu-id="997cb-136">First, [!INCLUDE[d365fin](includes/d365fin_md.md)] also updates the **Dimension Set Tree Node** table to make sure that the search tree looks like the following diagram.</span></span> <span data-ttu-id="997cb-137">Thus dimension set 7 becomes a child of the dimension set 5.</span><span class="sxs-lookup"><span data-stu-id="997cb-137">Thus dimension set 7 becomes a child of the dimension set 5.</span></span>  

 <span data-ttu-id="997cb-138">![NAV2013&#95;Dimension&#95;Tree&#95;Example 2](media/nav2013_dimension_tree_example2.png "NAV2013_Dimension_Tree_Example2")</span><span class="sxs-lookup"><span data-stu-id="997cb-138">![NAV2013&#95;Dimension&#95;Tree&#95;Example 2](media/nav2013_dimension_tree_example2.png "NAV2013_Dimension_Tree_Example2")</span></span>  

### <a name="finding-dimension-set-id"></a><span data-ttu-id="997cb-139">Finding Dimension Set ID</span><span class="sxs-lookup"><span data-stu-id="997cb-139">Finding Dimension Set ID</span></span>  
 <span data-ttu-id="997cb-140">At a conceptual level, **Parent ID**, **Dimension**, and **Dimension Value**, in the search tree, are combined and used as the primary key because [!INCLUDE[d365fin](includes/d365fin_md.md)] traverses the tree in the same order as the dimension entries.</span><span class="sxs-lookup"><span data-stu-id="997cb-140">At a conceptual level, **Parent ID**, **Dimension**, and **Dimension Value**, in the search tree, are combined and used as the primary key because [!INCLUDE[d365fin](includes/d365fin_md.md)] traverses the tree in the same order as the dimension entries.</span></span> <span data-ttu-id="997cb-141">The GET function (record) is used to search for dimension set ID.</span><span class="sxs-lookup"><span data-stu-id="997cb-141">The GET function (record) is used to search for dimension set ID.</span></span> <span data-ttu-id="997cb-142">The following code example shows how to find the dimension set ID when there are three dimension values.</span><span class="sxs-lookup"><span data-stu-id="997cb-142">The following code example shows how to find the dimension set ID when there are three dimension values.</span></span>  

```  
DimSet."Parent ID" := 0;  // 'root'  
IF UserDim.FINDSET THEN  
  REPEAT  
      DimSet.GET(DimSet."Parent ID",UserDim.DimCode,UserDim.DimValueCode);  
  UNTIL UserDim.NEXT = 0;  
EXIT(DimSet.ID);  

```  

 <span data-ttu-id="997cb-143">However, to preserve the ability of [!INCLUDE[d365fin](includes/d365fin_md.md)] to rename a dimension and dimension value, table 348 **Dimension Value** is extended with an integer field of **Dimension Value ID**.</span><span class="sxs-lookup"><span data-stu-id="997cb-143">However, to preserve the ability of [!INCLUDE[d365fin](includes/d365fin_md.md)] to rename a dimension and dimension value, table 348 **Dimension Value** is extended with an integer field of **Dimension Value ID**.</span></span> <span data-ttu-id="997cb-144">This table converts the field pair **Dimension** and **Dimension Value** to an integer value.</span><span class="sxs-lookup"><span data-stu-id="997cb-144">This table converts the field pair **Dimension** and **Dimension Value** to an integer value.</span></span> <span data-ttu-id="997cb-145">When you rename the dimension and dimension value, the integer value is not changed.</span><span class="sxs-lookup"><span data-stu-id="997cb-145">When you rename the dimension and dimension value, the integer value is not changed.</span></span>  

```  
DimSet."Parent ID" := 0;  // 'root'  
IF UserDim.FINDSET THEN  
  REPEAT  
      DimSet.GET(DimSet.ParentID,UserDim."Dimension Value ID");  
  UNTIL UserDim.NEXT = 0;  
EXIT(DimSet.ID);  

```  

## <a name="see-also"></a><span data-ttu-id="997cb-146">See Also</span><span class="sxs-lookup"><span data-stu-id="997cb-146">See Also</span></span>  
 <span data-ttu-id="997cb-147">[GET Function (Record)](/dynamics-nav/GET-Function--Record-)  </span><span class="sxs-lookup"><span data-stu-id="997cb-147">[GET Function (Record)](/dynamics-nav/GET-Function--Record-)  </span></span>  
 <span data-ttu-id="997cb-148">[Design Details: Dimension Set Entries](design-details-dimension-set-entries.md) </span><span class="sxs-lookup"><span data-stu-id="997cb-148">[Design Details: Dimension Set Entries](design-details-dimension-set-entries.md) </span></span>  
 <span data-ttu-id="997cb-149">[Dimension Set Entries Overview](design-details-dimension-set-entries-overview.md) </span><span class="sxs-lookup"><span data-stu-id="997cb-149">[Dimension Set Entries Overview](design-details-dimension-set-entries-overview.md) </span></span>  
 <span data-ttu-id="997cb-150">[Design Details: Table Structure](design-details-table-structure.md) </span><span class="sxs-lookup"><span data-stu-id="997cb-150">[Design Details: Table Structure](design-details-table-structure.md) </span></span>  
 <span data-ttu-id="997cb-151">[Design Details: Codeunit 408 Dimension Management](design-details-codeunit-408-dimension-management.md) </span><span class="sxs-lookup"><span data-stu-id="997cb-151">[Design Details: Codeunit 408 Dimension Management](design-details-codeunit-408-dimension-management.md) </span></span>  
 [<span data-ttu-id="997cb-152">Design Details: Code Examples of Changed Patterns in Modifications</span><span class="sxs-lookup"><span data-stu-id="997cb-152">Design Details: Code Examples of Changed Patterns in Modifications</span></span>](design-details-code-examples-of-changed-patterns-in-modifications.md)
