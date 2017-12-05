---
title: Design Details - Codeunit 408 Dimension Management | Microsoft Docs
description: Codeunit 408 Dimension Management is a function library that handles common tasks that are related to dimensions, such as copying from one table to another or from one document to another.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: ba26b354d235981bd7291f9ac6402779f554ac7a
ms.openlocfilehash: 32f67c058570f03d4aa1c84d9bb32289b1f07bec
ms.contentlocale: en-nz
ms.lasthandoff: 11/10/2017

---
# <a name="design-details-codeunit-408-dimension-management"></a><span data-ttu-id="6e335-103">Design Details: Codeunit 408 Dimension Management</span><span class="sxs-lookup"><span data-stu-id="6e335-103">Design Details: Codeunit 408 Dimension Management</span></span>
<span data-ttu-id="6e335-104">Codeunit 408 Dimension Management is a function library that handles common tasks that are related to dimensions, such as copying from one table to another or from one document to another.</span><span class="sxs-lookup"><span data-stu-id="6e335-104">Codeunit 408 Dimension Management is a function library that handles common tasks that are related to dimensions, such as copying from one table to another or from one document to another.</span></span> <span data-ttu-id="6e335-105">This topic lists the functions that are modified in Microsoft Dynamics NAV 2013 R2 and specifies what has to be done to the functions.</span><span class="sxs-lookup"><span data-stu-id="6e335-105">This topic lists the functions that are modified in Microsoft Dynamics NAV 2013 R2 and specifies what has to be done to the functions.</span></span> <span data-ttu-id="6e335-106">Many functions are deleted because there is no need for copying between dimension tables.</span><span class="sxs-lookup"><span data-stu-id="6e335-106">Many functions are deleted because there is no need for copying between dimension tables.</span></span>  

## <a name="modified-functions"></a><span data-ttu-id="6e335-107">Modified Functions</span><span class="sxs-lookup"><span data-stu-id="6e335-107">Modified Functions</span></span>  

|<span data-ttu-id="6e335-108">Function Name</span><span class="sxs-lookup"><span data-stu-id="6e335-108">Function Name</span></span>|<span data-ttu-id="6e335-109">Modification Description</span><span class="sxs-lookup"><span data-stu-id="6e335-109">Modification Description</span></span>|  
|-------------------|------------------------------|  
|<span data-ttu-id="6e335-110">CheckDimSetIDComb</span><span class="sxs-lookup"><span data-stu-id="6e335-110">CheckDimSetIDComb</span></span>|<span data-ttu-id="6e335-111">New function that substitutes the other check functions and takes a Dimension Set ID as an argument instead of a dimension table.</span><span class="sxs-lookup"><span data-stu-id="6e335-111">New function that substitutes the other check functions and takes a Dimension Set ID as an argument instead of a dimension table.</span></span>|  
|<span data-ttu-id="6e335-112">CheckDimSetIDComb</span><span class="sxs-lookup"><span data-stu-id="6e335-112">CheckDimSetIDComb</span></span><br /><br /> <span data-ttu-id="6e335-113">CheckDocDimComb</span><span class="sxs-lookup"><span data-stu-id="6e335-113">CheckDocDimComb</span></span><br /><br /> <span data-ttu-id="6e335-114">CheckServContractDimComb</span><span class="sxs-lookup"><span data-stu-id="6e335-114">CheckServContractDimComb</span></span><br /><br /> <span data-ttu-id="6e335-115">CheckDimBuffer</span><span class="sxs-lookup"><span data-stu-id="6e335-115">CheckDimBuffer</span></span><br /><br /> <span data-ttu-id="6e335-116">CheckDimComb</span><span class="sxs-lookup"><span data-stu-id="6e335-116">CheckDimComb</span></span><br /><br /> <span data-ttu-id="6e335-117">CheckDimValueComb</span><span class="sxs-lookup"><span data-stu-id="6e335-117">CheckDimValueComb</span></span>|<span data-ttu-id="6e335-118">Delete.</span><span class="sxs-lookup"><span data-stu-id="6e335-118">Delete.</span></span> <span data-ttu-id="6e335-119">All usage should be changed to CheckDimSetIDComb.</span><span class="sxs-lookup"><span data-stu-id="6e335-119">All usage should be changed to CheckDimSetIDComb.</span></span>|  
|<span data-ttu-id="6e335-120">GetDefaultDim</span><span class="sxs-lookup"><span data-stu-id="6e335-120">GetDefaultDim</span></span>|<span data-ttu-id="6e335-121">Modify to return an integer Dimension Set ID instead of a set of records.</span><span class="sxs-lookup"><span data-stu-id="6e335-121">Modify to return an integer Dimension Set ID instead of a set of records.</span></span>|  
|<span data-ttu-id="6e335-122">CopyJnlLineDimToICJnlDim</span><span class="sxs-lookup"><span data-stu-id="6e335-122">CopyJnlLineDimToICJnlDim</span></span><br /><br /> <span data-ttu-id="6e335-123">CopyICJnlDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="6e335-123">CopyICJnlDimToJnlLineDim</span></span><br /><br /> <span data-ttu-id="6e335-124">CopyDocDimtoICDocDim</span><span class="sxs-lookup"><span data-stu-id="6e335-124">CopyDocDimtoICDocDim</span></span><br /><br /> <span data-ttu-id="6e335-125">CopyICDocDimtoICDocDim</span><span class="sxs-lookup"><span data-stu-id="6e335-125">CopyICDocDimtoICDocDim</span></span>|<span data-ttu-id="6e335-126">Modify to work with DimSetID -> ICJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="6e335-126">Modify to work with DimSetID -> ICJnlLineDim</span></span>|  

## <a name="deleted-functions"></a><span data-ttu-id="6e335-127">Deleted Functions</span><span class="sxs-lookup"><span data-stu-id="6e335-127">Deleted Functions</span></span>  
 <span data-ttu-id="6e335-128">Functions that are deleted from codeunit 408 in connection with the Dimension Set Entries feature are listed below.</span><span class="sxs-lookup"><span data-stu-id="6e335-128">Functions that are deleted from codeunit 408 in connection with the Dimension Set Entries feature are listed below.</span></span>  

> [!CAUTION]  
>  <span data-ttu-id="6e335-129">During the upgrade of application code from Microsoft Dynamics NAV 2009 or earlier versions to Microsoft Dynamics NAV 2016, the following functions are not available in Microsoft Dynamics NAV 2016.</span><span class="sxs-lookup"><span data-stu-id="6e335-129">During the upgrade of application code from Microsoft Dynamics NAV 2009 or earlier versions to Microsoft Dynamics NAV 2016, the following functions are not available in Microsoft Dynamics NAV 2016.</span></span> <span data-ttu-id="6e335-130">If you have customisations that use one or more of the functions, you must upgrade that code accordingly.</span><span class="sxs-lookup"><span data-stu-id="6e335-130">If you have customizations that use one or more of the functions, you must upgrade that code accordingly.</span></span>

 <span data-ttu-id="6e335-131">InsertJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="6e335-131">InsertJnlLineDim</span></span>  

 <span data-ttu-id="6e335-132">UpdateJnlLineDefaultDim</span><span class="sxs-lookup"><span data-stu-id="6e335-132">UpdateJnlLineDefaultDim</span></span>  

 <span data-ttu-id="6e335-133">GetJnlLineDefaultDim</span><span class="sxs-lookup"><span data-stu-id="6e335-133">GetJnlLineDefaultDim</span></span>  

 <span data-ttu-id="6e335-134">GetPreviousDocDefaultDim</span><span class="sxs-lookup"><span data-stu-id="6e335-134">GetPreviousDocDefaultDim</span></span>  

 <span data-ttu-id="6e335-135">GetPreviousProdDocDefaultDim</span><span class="sxs-lookup"><span data-stu-id="6e335-135">GetPreviousProdDocDefaultDim</span></span>  

 <span data-ttu-id="6e335-136">InsertDocDim</span><span class="sxs-lookup"><span data-stu-id="6e335-136">InsertDocDim</span></span>  

 <span data-ttu-id="6e335-137">UpdateDocDefaultDim</span><span class="sxs-lookup"><span data-stu-id="6e335-137">UpdateDocDefaultDim</span></span>  

 <span data-ttu-id="6e335-138">ExtractDocDefaultDim</span><span class="sxs-lookup"><span data-stu-id="6e335-138">ExtractDocDefaultDim</span></span>  

 <span data-ttu-id="6e335-139">InsertProdDocDim</span><span class="sxs-lookup"><span data-stu-id="6e335-139">InsertProdDocDim</span></span>  

 <span data-ttu-id="6e335-140">UpdateProdDocDefaultDim</span><span class="sxs-lookup"><span data-stu-id="6e335-140">UpdateProdDocDefaultDim</span></span>  

 <span data-ttu-id="6e335-141">InsertServContractDim</span><span class="sxs-lookup"><span data-stu-id="6e335-141">InsertServContractDim</span></span>  

 <span data-ttu-id="6e335-142">UpdateServcontractDim</span><span class="sxs-lookup"><span data-stu-id="6e335-142">UpdateServcontractDim</span></span>  

 <span data-ttu-id="6e335-143">UpdateDefaultDimNewDimValue</span><span class="sxs-lookup"><span data-stu-id="6e335-143">UpdateDefaultDimNewDimValue</span></span>  

 <span data-ttu-id="6e335-144">GetDocDim</span><span class="sxs-lookup"><span data-stu-id="6e335-144">GetDocDim</span></span>  

 <span data-ttu-id="6e335-145">GetProdDocDim</span><span class="sxs-lookup"><span data-stu-id="6e335-145">GetProdDocDim</span></span>  

 <span data-ttu-id="6e335-146">TypeToTableID1</span><span class="sxs-lookup"><span data-stu-id="6e335-146">TypeToTableID1</span></span>  

 <span data-ttu-id="6e335-147">TypeToTableID2</span><span class="sxs-lookup"><span data-stu-id="6e335-147">TypeToTableID2</span></span>  

 <span data-ttu-id="6e335-148">TypeToTableID3</span><span class="sxs-lookup"><span data-stu-id="6e335-148">TypeToTableID3</span></span>  

 <span data-ttu-id="6e335-149">TypeToTableID4</span><span class="sxs-lookup"><span data-stu-id="6e335-149">TypeToTableID4</span></span>  

 <span data-ttu-id="6e335-150">TypeToTableID5</span><span class="sxs-lookup"><span data-stu-id="6e335-150">TypeToTableID5</span></span>  

 <span data-ttu-id="6e335-151">DeleteJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="6e335-151">DeleteJnlLineDim</span></span>  

 <span data-ttu-id="6e335-152">DeleteDocDim</span><span class="sxs-lookup"><span data-stu-id="6e335-152">DeleteDocDim</span></span>  

 <span data-ttu-id="6e335-153">DeletePostedDocDim</span><span class="sxs-lookup"><span data-stu-id="6e335-153">DeletePostedDocDim</span></span>  

 <span data-ttu-id="6e335-154">DeleteProdDocDim</span><span class="sxs-lookup"><span data-stu-id="6e335-154">DeleteProdDocDim</span></span>  

 <span data-ttu-id="6e335-155">DeleteServContractDim</span><span class="sxs-lookup"><span data-stu-id="6e335-155">DeleteServContractDim</span></span>  

 <span data-ttu-id="6e335-156">ShowJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="6e335-156">ShowJnlLineDim</span></span>  

 <span data-ttu-id="6e335-157">SaveJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="6e335-157">SaveJnlLineDim</span></span>  

 <span data-ttu-id="6e335-158">ShowJnlLineNewDim</span><span class="sxs-lookup"><span data-stu-id="6e335-158">ShowJnlLineNewDim</span></span>  

 <span data-ttu-id="6e335-159">SaveJnlLineNewDim</span><span class="sxs-lookup"><span data-stu-id="6e335-159">SaveJnlLineNewDim</span></span>  

 <span data-ttu-id="6e335-160">ShowDocDim</span><span class="sxs-lookup"><span data-stu-id="6e335-160">ShowDocDim</span></span>  

 <span data-ttu-id="6e335-161">SaveDocDim</span><span class="sxs-lookup"><span data-stu-id="6e335-161">SaveDocDim</span></span>  

 <span data-ttu-id="6e335-162">ShowProdDocDim</span><span class="sxs-lookup"><span data-stu-id="6e335-162">ShowProdDocDim</span></span>  

 <span data-ttu-id="6e335-163">SaveProdDocDim</span><span class="sxs-lookup"><span data-stu-id="6e335-163">SaveProdDocDim</span></span>  

 <span data-ttu-id="6e335-164">ShowTempDim</span><span class="sxs-lookup"><span data-stu-id="6e335-164">ShowTempDim</span></span>  

 <span data-ttu-id="6e335-165">SaveTempDim</span><span class="sxs-lookup"><span data-stu-id="6e335-165">SaveTempDim</span></span>  

 <span data-ttu-id="6e335-166">ShowTempNewDim</span><span class="sxs-lookup"><span data-stu-id="6e335-166">ShowTempNewDim</span></span>  

 <span data-ttu-id="6e335-167">SaveTempNewDim</span><span class="sxs-lookup"><span data-stu-id="6e335-167">SaveTempNewDim</span></span>  

 <span data-ttu-id="6e335-168">SaveServContractDim</span><span class="sxs-lookup"><span data-stu-id="6e335-168">SaveServContractDim</span></span>  

 <span data-ttu-id="6e335-169">MoveJnlLineDimToLedgEntryDim</span><span class="sxs-lookup"><span data-stu-id="6e335-169">MoveJnlLineDimToLedgEntryDim</span></span>  

 <span data-ttu-id="6e335-170">MoveDocDimToPostedDocDim</span><span class="sxs-lookup"><span data-stu-id="6e335-170">MoveDocDimToPostedDocDim</span></span>  

 <span data-ttu-id="6e335-171">MoveOneDocDimToPostedDocDim</span><span class="sxs-lookup"><span data-stu-id="6e335-171">MoveOneDocDimToPostedDocDim</span></span>  

 <span data-ttu-id="6e335-172">MoveLedgEntryDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="6e335-172">MoveLedgEntryDimToJnlLineDim</span></span>  

 <span data-ttu-id="6e335-173">MoveDimBufToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="6e335-173">MoveDimBufToJnlLineDim</span></span>  

 <span data-ttu-id="6e335-174">MoveDimBufToLedgEntryDim</span><span class="sxs-lookup"><span data-stu-id="6e335-174">MoveDimBufToLedgEntryDim</span></span>  

 <span data-ttu-id="6e335-175">MoveDimBufToPostedDocDim</span><span class="sxs-lookup"><span data-stu-id="6e335-175">MoveDimBufToPostedDocDim</span></span>  

 <span data-ttu-id="6e335-176">MoveDimBufToGLBudgetDim</span><span class="sxs-lookup"><span data-stu-id="6e335-176">MoveDimBufToGLBudgetDim</span></span>  

 <span data-ttu-id="6e335-177">CopyJnlLineDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="6e335-177">CopyJnlLineDimToJnlLineDim</span></span>  

 <span data-ttu-id="6e335-178">CopyLedgEntryDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="6e335-178">CopyLedgEntryDimToJnlLineDim</span></span>  

 <span data-ttu-id="6e335-179">CopyDocDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="6e335-179">CopyDocDimToDocDim</span></span>  

 <span data-ttu-id="6e335-180">CopyPostedDocDimToPostedDocDim</span><span class="sxs-lookup"><span data-stu-id="6e335-180">CopyPostedDocDimToPostedDocDim</span></span>  

 <span data-ttu-id="6e335-181">CopyDocDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="6e335-181">CopyDocDimToJnlLineDim</span></span>  

 <span data-ttu-id="6e335-182">CopyDimBufToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="6e335-182">CopyDimBufToJnlLineDim</span></span>  

 <span data-ttu-id="6e335-183">CopyDimBufToDocDim</span><span class="sxs-lookup"><span data-stu-id="6e335-183">CopyDimBufToDocDim</span></span>  

 <span data-ttu-id="6e335-184">CopySCDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="6e335-184">CopySCDimToDocDim</span></span>  

 <span data-ttu-id="6e335-185">MoveDocDimToLedgEntryDim</span><span class="sxs-lookup"><span data-stu-id="6e335-185">MoveDocDimToLedgEntryDim</span></span>  

 <span data-ttu-id="6e335-186">MoveDocDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="6e335-186">MoveDocDimToDocDim</span></span>  

 <span data-ttu-id="6e335-187">MoveDocDimArchvToDocDim</span><span class="sxs-lookup"><span data-stu-id="6e335-187">MoveDocDimArchvToDocDim</span></span>  

 <span data-ttu-id="6e335-188">MoveLedgEntryDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="6e335-188">MoveLedgEntryDimToDocDim</span></span>  

 <span data-ttu-id="6e335-189">MoveProdDocDimToProdDocDim</span><span class="sxs-lookup"><span data-stu-id="6e335-189">MoveProdDocDimToProdDocDim</span></span>  

 <span data-ttu-id="6e335-190">MoveJnlLineDimToProdDocDim</span><span class="sxs-lookup"><span data-stu-id="6e335-190">MoveJnlLineDimToProdDocDim</span></span>  

 <span data-ttu-id="6e335-191">MoveJnlLineDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="6e335-191">MoveJnlLineDimToDocDim</span></span>  

 <span data-ttu-id="6e335-192">MoveJnlLineDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="6e335-192">MoveJnlLineDimToJnlLineDim</span></span>  

 <span data-ttu-id="6e335-193">CopyLedgEntryDimToLedgEntryDim</span><span class="sxs-lookup"><span data-stu-id="6e335-193">CopyLedgEntryDimToLedgEntryDim</span></span>  

 <span data-ttu-id="6e335-194">MoveTempFromDimToTempToDim</span><span class="sxs-lookup"><span data-stu-id="6e335-194">MoveTempFromDimToTempToDim</span></span>  

 <span data-ttu-id="6e335-195">TransferTempToDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="6e335-195">TransferTempToDimToDocDim</span></span>  

 <span data-ttu-id="6e335-196">MoveJnlLineDimToBuf</span><span class="sxs-lookup"><span data-stu-id="6e335-196">MoveJnlLineDimToBuf</span></span>  

 <span data-ttu-id="6e335-197">CopyICJnlDimToICJnlDim</span><span class="sxs-lookup"><span data-stu-id="6e335-197">CopyICJnlDimToICJnlDim</span></span>  

 <span data-ttu-id="6e335-198">TestDimValue</span><span class="sxs-lookup"><span data-stu-id="6e335-198">TestDimValue</span></span>  

 <span data-ttu-id="6e335-199">TestNewDimValue</span><span class="sxs-lookup"><span data-stu-id="6e335-199">TestNewDimValue</span></span>  

 <span data-ttu-id="6e335-200">MoveDimBufToItemBudgetDim.</span><span class="sxs-lookup"><span data-stu-id="6e335-200">MoveDimBufToItemBudgetDim.</span></span> <span data-ttu-id="6e335-201">(Delete because the ItemBudgetDim Table is deleted.)</span><span class="sxs-lookup"><span data-stu-id="6e335-201">(Delete because the ItemBudgetDim Table is deleted.)</span></span>  

 <span data-ttu-id="6e335-202">GetServContractDim</span><span class="sxs-lookup"><span data-stu-id="6e335-202">GetServContractDim</span></span>  

 <span data-ttu-id="6e335-203">MoveTempDimToBuf</span><span class="sxs-lookup"><span data-stu-id="6e335-203">MoveTempDimToBuf</span></span>  

 <span data-ttu-id="6e335-204">UpdateSCInvLineDim</span><span class="sxs-lookup"><span data-stu-id="6e335-204">UpdateSCInvLineDim</span></span>  

 <span data-ttu-id="6e335-205">CopyJnlLineDimToBuffer</span><span class="sxs-lookup"><span data-stu-id="6e335-205">CopyJnlLineDimToBuffer</span></span>  

 <span data-ttu-id="6e335-206">UpdateDocDefaultDim2</span><span class="sxs-lookup"><span data-stu-id="6e335-206">UpdateDocDefaultDim2</span></span>  

## <a name="see-also"></a><span data-ttu-id="6e335-207">See Also</span><span class="sxs-lookup"><span data-stu-id="6e335-207">See Also</span></span>
 <span data-ttu-id="6e335-208">[Design Details: Dimension Set Entries](design-details-dimension-set-entries.md) </span><span class="sxs-lookup"><span data-stu-id="6e335-208">[Design Details: Dimension Set Entries](design-details-dimension-set-entries.md) </span></span>  
 <span data-ttu-id="6e335-209">[Design Details: Dimension Set Entries Overview](design-details-dimension-set-entries-overview.md) </span><span class="sxs-lookup"><span data-stu-id="6e335-209">[Design Details: Dimension Set Entries Overview](design-details-dimension-set-entries-overview.md) </span></span>  
 <span data-ttu-id="6e335-210">[Design Details: Searching for Dimension Combinations](design-details-searching-for-dimension-combinations.md) </span><span class="sxs-lookup"><span data-stu-id="6e335-210">[Design Details: Searching for Dimension Combinations](design-details-searching-for-dimension-combinations.md) </span></span>  
 <span data-ttu-id="6e335-211">[Design Details: Table Structure](design-details-table-structure.md) </span><span class="sxs-lookup"><span data-stu-id="6e335-211">[Design Details: Table Structure](design-details-table-structure.md) </span></span>  
 [<span data-ttu-id="6e335-212">Design Details: Code Examples of Changed Patterns in Modifications</span><span class="sxs-lookup"><span data-stu-id="6e335-212">Design Details: Code Examples of Changed Patterns in Modifications</span></span>](design-details-code-examples-of-changed-patterns-in-modifications.md)

