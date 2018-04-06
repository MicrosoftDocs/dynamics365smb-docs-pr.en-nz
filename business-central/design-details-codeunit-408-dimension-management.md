---
title: Design Details - Codeunit 408 Dimension Management | Microsoft Docs
description: Codeunit 408 Dimension Management is a function library that handles common tasks that are related to dimensions, such as copying from one table to another or from one document to another.
services: project-madeira
documentationcenter: 
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
ms.openlocfilehash: 34d4314357aa590304885585016124100ead4ca3
ms.contentlocale: en-nz
ms.lasthandoff: 03/22/2018

---
# <a name="design-details-codeunit-408-dimension-management"></a><span data-ttu-id="b84be-103">Design Details: Codeunit 408 Dimension Management</span><span class="sxs-lookup"><span data-stu-id="b84be-103">Design Details: Codeunit 408 Dimension Management</span></span>
<span data-ttu-id="b84be-104">Codeunit 408 Dimension Management is a function library that handles common tasks that are related to dimensions, such as copying from one table to another or from one document to another.</span><span class="sxs-lookup"><span data-stu-id="b84be-104">Codeunit 408 Dimension Management is a function library that handles common tasks that are related to dimensions, such as copying from one table to another or from one document to another.</span></span> <span data-ttu-id="b84be-105">This topic lists the functions that are modified in Microsoft Dynamics NAV 2013 R2 and specifies what has to be done to the functions.</span><span class="sxs-lookup"><span data-stu-id="b84be-105">This topic lists the functions that are modified in Microsoft Dynamics NAV 2013 R2 and specifies what has to be done to the functions.</span></span> <span data-ttu-id="b84be-106">Many functions are deleted because there is no need for copying between dimension tables.</span><span class="sxs-lookup"><span data-stu-id="b84be-106">Many functions are deleted because there is no need for copying between dimension tables.</span></span>  

## <a name="modified-functions"></a><span data-ttu-id="b84be-107">Modified Functions</span><span class="sxs-lookup"><span data-stu-id="b84be-107">Modified Functions</span></span>  

|<span data-ttu-id="b84be-108">Function Name</span><span class="sxs-lookup"><span data-stu-id="b84be-108">Function Name</span></span>|<span data-ttu-id="b84be-109">Modification Description</span><span class="sxs-lookup"><span data-stu-id="b84be-109">Modification Description</span></span>|  
|-------------------|------------------------------|  
|<span data-ttu-id="b84be-110">CheckDimSetIDComb</span><span class="sxs-lookup"><span data-stu-id="b84be-110">CheckDimSetIDComb</span></span>|<span data-ttu-id="b84be-111">New function that substitutes the other check functions and takes a Dimension Set ID as an argument instead of a dimension table.</span><span class="sxs-lookup"><span data-stu-id="b84be-111">New function that substitutes the other check functions and takes a Dimension Set ID as an argument instead of a dimension table.</span></span>|  
|<span data-ttu-id="b84be-112">CheckDimSetIDComb</span><span class="sxs-lookup"><span data-stu-id="b84be-112">CheckDimSetIDComb</span></span><br /><br /> <span data-ttu-id="b84be-113">CheckDocDimComb</span><span class="sxs-lookup"><span data-stu-id="b84be-113">CheckDocDimComb</span></span><br /><br /> <span data-ttu-id="b84be-114">CheckServContractDimComb</span><span class="sxs-lookup"><span data-stu-id="b84be-114">CheckServContractDimComb</span></span><br /><br /> <span data-ttu-id="b84be-115">CheckDimBuffer</span><span class="sxs-lookup"><span data-stu-id="b84be-115">CheckDimBuffer</span></span><br /><br /> <span data-ttu-id="b84be-116">CheckDimComb</span><span class="sxs-lookup"><span data-stu-id="b84be-116">CheckDimComb</span></span><br /><br /> <span data-ttu-id="b84be-117">CheckDimValueComb</span><span class="sxs-lookup"><span data-stu-id="b84be-117">CheckDimValueComb</span></span>|<span data-ttu-id="b84be-118">Delete.</span><span class="sxs-lookup"><span data-stu-id="b84be-118">Delete.</span></span> <span data-ttu-id="b84be-119">All usage should be changed to CheckDimSetIDComb.</span><span class="sxs-lookup"><span data-stu-id="b84be-119">All usage should be changed to CheckDimSetIDComb.</span></span>|  
|<span data-ttu-id="b84be-120">GetDefaultDim</span><span class="sxs-lookup"><span data-stu-id="b84be-120">GetDefaultDim</span></span>|<span data-ttu-id="b84be-121">Modify to return an integer Dimension Set ID instead of a set of records.</span><span class="sxs-lookup"><span data-stu-id="b84be-121">Modify to return an integer Dimension Set ID instead of a set of records.</span></span>|  
|<span data-ttu-id="b84be-122">CopyJnlLineDimToICJnlDim</span><span class="sxs-lookup"><span data-stu-id="b84be-122">CopyJnlLineDimToICJnlDim</span></span><br /><br /> <span data-ttu-id="b84be-123">CopyICJnlDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="b84be-123">CopyICJnlDimToJnlLineDim</span></span><br /><br /> <span data-ttu-id="b84be-124">CopyDocDimtoICDocDim</span><span class="sxs-lookup"><span data-stu-id="b84be-124">CopyDocDimtoICDocDim</span></span><br /><br /> <span data-ttu-id="b84be-125">CopyICDocDimtoICDocDim</span><span class="sxs-lookup"><span data-stu-id="b84be-125">CopyICDocDimtoICDocDim</span></span>|<span data-ttu-id="b84be-126">Modify to work with DimSetID -> ICJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="b84be-126">Modify to work with DimSetID -> ICJnlLineDim</span></span>|  

## <a name="deleted-functions"></a><span data-ttu-id="b84be-127">Deleted Functions</span><span class="sxs-lookup"><span data-stu-id="b84be-127">Deleted Functions</span></span>  
 <span data-ttu-id="b84be-128">Functions that are deleted from codeunit 408 in connection with the Dimension Set Entries feature are listed below.</span><span class="sxs-lookup"><span data-stu-id="b84be-128">Functions that are deleted from codeunit 408 in connection with the Dimension Set Entries feature are listed below.</span></span>  

> [!CAUTION]  
>  <span data-ttu-id="b84be-129">During the upgrade of application code from Microsoft Dynamics NAV 2009 or earlier versions to Microsoft Dynamics NAV 2016, the following functions are not available in Microsoft Dynamics NAV 2016.</span><span class="sxs-lookup"><span data-stu-id="b84be-129">During the upgrade of application code from Microsoft Dynamics NAV 2009 or earlier versions to Microsoft Dynamics NAV 2016, the following functions are not available in Microsoft Dynamics NAV 2016.</span></span> <span data-ttu-id="b84be-130">If you have customisations that use one or more of the functions, you must upgrade that code accordingly.</span><span class="sxs-lookup"><span data-stu-id="b84be-130">If you have customizations that use one or more of the functions, you must upgrade that code accordingly.</span></span>

 <span data-ttu-id="b84be-131">InsertJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="b84be-131">InsertJnlLineDim</span></span>  

 <span data-ttu-id="b84be-132">UpdateJnlLineDefaultDim</span><span class="sxs-lookup"><span data-stu-id="b84be-132">UpdateJnlLineDefaultDim</span></span>  

 <span data-ttu-id="b84be-133">GetJnlLineDefaultDim</span><span class="sxs-lookup"><span data-stu-id="b84be-133">GetJnlLineDefaultDim</span></span>  

 <span data-ttu-id="b84be-134">GetPreviousDocDefaultDim</span><span class="sxs-lookup"><span data-stu-id="b84be-134">GetPreviousDocDefaultDim</span></span>  

 <span data-ttu-id="b84be-135">GetPreviousProdDocDefaultDim</span><span class="sxs-lookup"><span data-stu-id="b84be-135">GetPreviousProdDocDefaultDim</span></span>  

 <span data-ttu-id="b84be-136">InsertDocDim</span><span class="sxs-lookup"><span data-stu-id="b84be-136">InsertDocDim</span></span>  

 <span data-ttu-id="b84be-137">UpdateDocDefaultDim</span><span class="sxs-lookup"><span data-stu-id="b84be-137">UpdateDocDefaultDim</span></span>  

 <span data-ttu-id="b84be-138">ExtractDocDefaultDim</span><span class="sxs-lookup"><span data-stu-id="b84be-138">ExtractDocDefaultDim</span></span>  

 <span data-ttu-id="b84be-139">InsertProdDocDim</span><span class="sxs-lookup"><span data-stu-id="b84be-139">InsertProdDocDim</span></span>  

 <span data-ttu-id="b84be-140">UpdateProdDocDefaultDim</span><span class="sxs-lookup"><span data-stu-id="b84be-140">UpdateProdDocDefaultDim</span></span>  

 <span data-ttu-id="b84be-141">InsertServContractDim</span><span class="sxs-lookup"><span data-stu-id="b84be-141">InsertServContractDim</span></span>  

 <span data-ttu-id="b84be-142">UpdateServcontractDim</span><span class="sxs-lookup"><span data-stu-id="b84be-142">UpdateServcontractDim</span></span>  

 <span data-ttu-id="b84be-143">UpdateDefaultDimNewDimValue</span><span class="sxs-lookup"><span data-stu-id="b84be-143">UpdateDefaultDimNewDimValue</span></span>  

 <span data-ttu-id="b84be-144">GetDocDim</span><span class="sxs-lookup"><span data-stu-id="b84be-144">GetDocDim</span></span>  

 <span data-ttu-id="b84be-145">GetProdDocDim</span><span class="sxs-lookup"><span data-stu-id="b84be-145">GetProdDocDim</span></span>  

 <span data-ttu-id="b84be-146">TypeToTableID1</span><span class="sxs-lookup"><span data-stu-id="b84be-146">TypeToTableID1</span></span>  

 <span data-ttu-id="b84be-147">TypeToTableID2</span><span class="sxs-lookup"><span data-stu-id="b84be-147">TypeToTableID2</span></span>  

 <span data-ttu-id="b84be-148">TypeToTableID3</span><span class="sxs-lookup"><span data-stu-id="b84be-148">TypeToTableID3</span></span>  

 <span data-ttu-id="b84be-149">TypeToTableID4</span><span class="sxs-lookup"><span data-stu-id="b84be-149">TypeToTableID4</span></span>  

 <span data-ttu-id="b84be-150">TypeToTableID5</span><span class="sxs-lookup"><span data-stu-id="b84be-150">TypeToTableID5</span></span>  

 <span data-ttu-id="b84be-151">DeleteJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="b84be-151">DeleteJnlLineDim</span></span>  

 <span data-ttu-id="b84be-152">DeleteDocDim</span><span class="sxs-lookup"><span data-stu-id="b84be-152">DeleteDocDim</span></span>  

 <span data-ttu-id="b84be-153">DeletePostedDocDim</span><span class="sxs-lookup"><span data-stu-id="b84be-153">DeletePostedDocDim</span></span>  

 <span data-ttu-id="b84be-154">DeleteProdDocDim</span><span class="sxs-lookup"><span data-stu-id="b84be-154">DeleteProdDocDim</span></span>  

 <span data-ttu-id="b84be-155">DeleteServContractDim</span><span class="sxs-lookup"><span data-stu-id="b84be-155">DeleteServContractDim</span></span>  

 <span data-ttu-id="b84be-156">ShowJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="b84be-156">ShowJnlLineDim</span></span>  

 <span data-ttu-id="b84be-157">SaveJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="b84be-157">SaveJnlLineDim</span></span>  

 <span data-ttu-id="b84be-158">ShowJnlLineNewDim</span><span class="sxs-lookup"><span data-stu-id="b84be-158">ShowJnlLineNewDim</span></span>  

 <span data-ttu-id="b84be-159">SaveJnlLineNewDim</span><span class="sxs-lookup"><span data-stu-id="b84be-159">SaveJnlLineNewDim</span></span>  

 <span data-ttu-id="b84be-160">ShowDocDim</span><span class="sxs-lookup"><span data-stu-id="b84be-160">ShowDocDim</span></span>  

 <span data-ttu-id="b84be-161">SaveDocDim</span><span class="sxs-lookup"><span data-stu-id="b84be-161">SaveDocDim</span></span>  

 <span data-ttu-id="b84be-162">ShowProdDocDim</span><span class="sxs-lookup"><span data-stu-id="b84be-162">ShowProdDocDim</span></span>  

 <span data-ttu-id="b84be-163">SaveProdDocDim</span><span class="sxs-lookup"><span data-stu-id="b84be-163">SaveProdDocDim</span></span>  

 <span data-ttu-id="b84be-164">ShowTempDim</span><span class="sxs-lookup"><span data-stu-id="b84be-164">ShowTempDim</span></span>  

 <span data-ttu-id="b84be-165">SaveTempDim</span><span class="sxs-lookup"><span data-stu-id="b84be-165">SaveTempDim</span></span>  

 <span data-ttu-id="b84be-166">ShowTempNewDim</span><span class="sxs-lookup"><span data-stu-id="b84be-166">ShowTempNewDim</span></span>  

 <span data-ttu-id="b84be-167">SaveTempNewDim</span><span class="sxs-lookup"><span data-stu-id="b84be-167">SaveTempNewDim</span></span>  

 <span data-ttu-id="b84be-168">SaveServContractDim</span><span class="sxs-lookup"><span data-stu-id="b84be-168">SaveServContractDim</span></span>  

 <span data-ttu-id="b84be-169">MoveJnlLineDimToLedgEntryDim</span><span class="sxs-lookup"><span data-stu-id="b84be-169">MoveJnlLineDimToLedgEntryDim</span></span>  

 <span data-ttu-id="b84be-170">MoveDocDimToPostedDocDim</span><span class="sxs-lookup"><span data-stu-id="b84be-170">MoveDocDimToPostedDocDim</span></span>  

 <span data-ttu-id="b84be-171">MoveOneDocDimToPostedDocDim</span><span class="sxs-lookup"><span data-stu-id="b84be-171">MoveOneDocDimToPostedDocDim</span></span>  

 <span data-ttu-id="b84be-172">MoveLedgEntryDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="b84be-172">MoveLedgEntryDimToJnlLineDim</span></span>  

 <span data-ttu-id="b84be-173">MoveDimBufToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="b84be-173">MoveDimBufToJnlLineDim</span></span>  

 <span data-ttu-id="b84be-174">MoveDimBufToLedgEntryDim</span><span class="sxs-lookup"><span data-stu-id="b84be-174">MoveDimBufToLedgEntryDim</span></span>  

 <span data-ttu-id="b84be-175">MoveDimBufToPostedDocDim</span><span class="sxs-lookup"><span data-stu-id="b84be-175">MoveDimBufToPostedDocDim</span></span>  

 <span data-ttu-id="b84be-176">MoveDimBufToGLBudgetDim</span><span class="sxs-lookup"><span data-stu-id="b84be-176">MoveDimBufToGLBudgetDim</span></span>  

 <span data-ttu-id="b84be-177">CopyJnlLineDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="b84be-177">CopyJnlLineDimToJnlLineDim</span></span>  

 <span data-ttu-id="b84be-178">CopyLedgEntryDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="b84be-178">CopyLedgEntryDimToJnlLineDim</span></span>  

 <span data-ttu-id="b84be-179">CopyDocDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="b84be-179">CopyDocDimToDocDim</span></span>  

 <span data-ttu-id="b84be-180">CopyPostedDocDimToPostedDocDim</span><span class="sxs-lookup"><span data-stu-id="b84be-180">CopyPostedDocDimToPostedDocDim</span></span>  

 <span data-ttu-id="b84be-181">CopyDocDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="b84be-181">CopyDocDimToJnlLineDim</span></span>  

 <span data-ttu-id="b84be-182">CopyDimBufToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="b84be-182">CopyDimBufToJnlLineDim</span></span>  

 <span data-ttu-id="b84be-183">CopyDimBufToDocDim</span><span class="sxs-lookup"><span data-stu-id="b84be-183">CopyDimBufToDocDim</span></span>  

 <span data-ttu-id="b84be-184">CopySCDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="b84be-184">CopySCDimToDocDim</span></span>  

 <span data-ttu-id="b84be-185">MoveDocDimToLedgEntryDim</span><span class="sxs-lookup"><span data-stu-id="b84be-185">MoveDocDimToLedgEntryDim</span></span>  

 <span data-ttu-id="b84be-186">MoveDocDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="b84be-186">MoveDocDimToDocDim</span></span>  

 <span data-ttu-id="b84be-187">MoveDocDimArchvToDocDim</span><span class="sxs-lookup"><span data-stu-id="b84be-187">MoveDocDimArchvToDocDim</span></span>  

 <span data-ttu-id="b84be-188">MoveLedgEntryDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="b84be-188">MoveLedgEntryDimToDocDim</span></span>  

 <span data-ttu-id="b84be-189">MoveProdDocDimToProdDocDim</span><span class="sxs-lookup"><span data-stu-id="b84be-189">MoveProdDocDimToProdDocDim</span></span>  

 <span data-ttu-id="b84be-190">MoveJnlLineDimToProdDocDim</span><span class="sxs-lookup"><span data-stu-id="b84be-190">MoveJnlLineDimToProdDocDim</span></span>  

 <span data-ttu-id="b84be-191">MoveJnlLineDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="b84be-191">MoveJnlLineDimToDocDim</span></span>  

 <span data-ttu-id="b84be-192">MoveJnlLineDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="b84be-192">MoveJnlLineDimToJnlLineDim</span></span>  

 <span data-ttu-id="b84be-193">CopyLedgEntryDimToLedgEntryDim</span><span class="sxs-lookup"><span data-stu-id="b84be-193">CopyLedgEntryDimToLedgEntryDim</span></span>  

 <span data-ttu-id="b84be-194">MoveTempFromDimToTempToDim</span><span class="sxs-lookup"><span data-stu-id="b84be-194">MoveTempFromDimToTempToDim</span></span>  

 <span data-ttu-id="b84be-195">TransferTempToDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="b84be-195">TransferTempToDimToDocDim</span></span>  

 <span data-ttu-id="b84be-196">MoveJnlLineDimToBuf</span><span class="sxs-lookup"><span data-stu-id="b84be-196">MoveJnlLineDimToBuf</span></span>  

 <span data-ttu-id="b84be-197">CopyICJnlDimToICJnlDim</span><span class="sxs-lookup"><span data-stu-id="b84be-197">CopyICJnlDimToICJnlDim</span></span>  

 <span data-ttu-id="b84be-198">TestDimValue</span><span class="sxs-lookup"><span data-stu-id="b84be-198">TestDimValue</span></span>  

 <span data-ttu-id="b84be-199">TestNewDimValue</span><span class="sxs-lookup"><span data-stu-id="b84be-199">TestNewDimValue</span></span>  

 <span data-ttu-id="b84be-200">MoveDimBufToItemBudgetDim.</span><span class="sxs-lookup"><span data-stu-id="b84be-200">MoveDimBufToItemBudgetDim.</span></span> <span data-ttu-id="b84be-201">(Delete because the ItemBudgetDim Table is deleted.)</span><span class="sxs-lookup"><span data-stu-id="b84be-201">(Delete because the ItemBudgetDim Table is deleted.)</span></span>  

 <span data-ttu-id="b84be-202">GetServContractDim</span><span class="sxs-lookup"><span data-stu-id="b84be-202">GetServContractDim</span></span>  

 <span data-ttu-id="b84be-203">MoveTempDimToBuf</span><span class="sxs-lookup"><span data-stu-id="b84be-203">MoveTempDimToBuf</span></span>  

 <span data-ttu-id="b84be-204">UpdateSCInvLineDim</span><span class="sxs-lookup"><span data-stu-id="b84be-204">UpdateSCInvLineDim</span></span>  

 <span data-ttu-id="b84be-205">CopyJnlLineDimToBuffer</span><span class="sxs-lookup"><span data-stu-id="b84be-205">CopyJnlLineDimToBuffer</span></span>  

 <span data-ttu-id="b84be-206">UpdateDocDefaultDim2</span><span class="sxs-lookup"><span data-stu-id="b84be-206">UpdateDocDefaultDim2</span></span>  

## <a name="see-also"></a><span data-ttu-id="b84be-207">See Also</span><span class="sxs-lookup"><span data-stu-id="b84be-207">See Also</span></span>
 <span data-ttu-id="b84be-208">[Design Details: Dimension Set Entries](design-details-dimension-set-entries.md) </span><span class="sxs-lookup"><span data-stu-id="b84be-208">[Design Details: Dimension Set Entries](design-details-dimension-set-entries.md) </span></span>  
 <span data-ttu-id="b84be-209">[Design Details: Dimension Set Entries Overview](design-details-dimension-set-entries-overview.md) </span><span class="sxs-lookup"><span data-stu-id="b84be-209">[Design Details: Dimension Set Entries Overview](design-details-dimension-set-entries-overview.md) </span></span>  
 <span data-ttu-id="b84be-210">[Design Details: Searching for Dimension Combinations](design-details-searching-for-dimension-combinations.md) </span><span class="sxs-lookup"><span data-stu-id="b84be-210">[Design Details: Searching for Dimension Combinations](design-details-searching-for-dimension-combinations.md) </span></span>  
 <span data-ttu-id="b84be-211">[Design Details: Table Structure](design-details-table-structure.md) </span><span class="sxs-lookup"><span data-stu-id="b84be-211">[Design Details: Table Structure](design-details-table-structure.md) </span></span>  
 [<span data-ttu-id="b84be-212">Design Details: Code Examples of Changed Patterns in Modifications</span><span class="sxs-lookup"><span data-stu-id="b84be-212">Design Details: Code Examples of Changed Patterns in Modifications</span></span>](design-details-code-examples-of-changed-patterns-in-modifications.md)

