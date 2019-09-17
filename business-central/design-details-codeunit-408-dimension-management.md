---
title: Design Details - Codeunit 408 Dimension Management | Microsoft Docs
description: Codeunit 408 Dimension Management is a function library that handles common tasks that are related to dimensions, such as copying from one table to another or from one document to another.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2019
ms.author: sgroespe
redirect_url: design-details-dimension-set-entries
ms.openlocfilehash: f725e5baea27b47399a50d041757fde83657673c
ms.sourcegitcommit: 1fa3d33db7bc71e3a27c826308a80ff24a436a72
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 08/30/2019
ms.locfileid: "1970986"
---
# <a name="design-details-codeunit-408-dimension-management"></a><span data-ttu-id="bb764-103">Design Details: Codeunit 408 Dimension Management</span><span class="sxs-lookup"><span data-stu-id="bb764-103">Design Details: Codeunit 408 Dimension Management</span></span>
<span data-ttu-id="bb764-104">Codeunit 408 Dimension Management is a function library that handles common tasks that are related to dimensions, such as copying from one table to another or from one document to another.</span><span class="sxs-lookup"><span data-stu-id="bb764-104">Codeunit 408 Dimension Management is a function library that handles common tasks that are related to dimensions, such as copying from one table to another or from one document to another.</span></span> <span data-ttu-id="bb764-105">This topic lists the functions that are modified in Microsoft Dynamics NAV 2013 R2 and specifies what has to be done to the functions.</span><span class="sxs-lookup"><span data-stu-id="bb764-105">This topic lists the functions that are modified in Microsoft Dynamics NAV 2013 R2 and specifies what has to be done to the functions.</span></span> <span data-ttu-id="bb764-106">Many functions are deleted because there is no need for copying between dimension tables.</span><span class="sxs-lookup"><span data-stu-id="bb764-106">Many functions are deleted because there is no need for copying between dimension tables.</span></span>  

## <a name="modified-functions"></a><span data-ttu-id="bb764-107">Modified Functions</span><span class="sxs-lookup"><span data-stu-id="bb764-107">Modified Functions</span></span>  

|<span data-ttu-id="bb764-108">Function Name</span><span class="sxs-lookup"><span data-stu-id="bb764-108">Function Name</span></span>|<span data-ttu-id="bb764-109">Modification Description</span><span class="sxs-lookup"><span data-stu-id="bb764-109">Modification Description</span></span>|  
|-------------------|------------------------------|  
|<span data-ttu-id="bb764-110">CheckDimSetIDComb</span><span class="sxs-lookup"><span data-stu-id="bb764-110">CheckDimSetIDComb</span></span>|<span data-ttu-id="bb764-111">New function that substitutes the other check functions and takes a Dimension Set ID as an argument instead of a dimension table.</span><span class="sxs-lookup"><span data-stu-id="bb764-111">New function that substitutes the other check functions and takes a Dimension Set ID as an argument instead of a dimension table.</span></span>|  
|<span data-ttu-id="bb764-112">CheckDimSetIDComb</span><span class="sxs-lookup"><span data-stu-id="bb764-112">CheckDimSetIDComb</span></span><br /><br /> <span data-ttu-id="bb764-113">CheckDocDimComb</span><span class="sxs-lookup"><span data-stu-id="bb764-113">CheckDocDimComb</span></span><br /><br /> <span data-ttu-id="bb764-114">CheckServContractDimComb</span><span class="sxs-lookup"><span data-stu-id="bb764-114">CheckServContractDimComb</span></span><br /><br /> <span data-ttu-id="bb764-115">CheckDimBuffer</span><span class="sxs-lookup"><span data-stu-id="bb764-115">CheckDimBuffer</span></span><br /><br /> <span data-ttu-id="bb764-116">CheckDimComb</span><span class="sxs-lookup"><span data-stu-id="bb764-116">CheckDimComb</span></span><br /><br /> <span data-ttu-id="bb764-117">CheckDimValueComb</span><span class="sxs-lookup"><span data-stu-id="bb764-117">CheckDimValueComb</span></span>|<span data-ttu-id="bb764-118">Delete.</span><span class="sxs-lookup"><span data-stu-id="bb764-118">Delete.</span></span> <span data-ttu-id="bb764-119">All usage should be changed to CheckDimSetIDComb.</span><span class="sxs-lookup"><span data-stu-id="bb764-119">All usage should be changed to CheckDimSetIDComb.</span></span>|  
|<span data-ttu-id="bb764-120">GetDefaultDim</span><span class="sxs-lookup"><span data-stu-id="bb764-120">GetDefaultDim</span></span>|<span data-ttu-id="bb764-121">Modify to return an integer Dimension Set ID instead of a set of records.</span><span class="sxs-lookup"><span data-stu-id="bb764-121">Modify to return an integer Dimension Set ID instead of a set of records.</span></span>|  
|<span data-ttu-id="bb764-122">CopyJnlLineDimToICJnlDim</span><span class="sxs-lookup"><span data-stu-id="bb764-122">CopyJnlLineDimToICJnlDim</span></span><br /><br /> <span data-ttu-id="bb764-123">CopyICJnlDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="bb764-123">CopyICJnlDimToJnlLineDim</span></span><br /><br /> <span data-ttu-id="bb764-124">CopyDocDimtoICDocDim</span><span class="sxs-lookup"><span data-stu-id="bb764-124">CopyDocDimtoICDocDim</span></span><br /><br /> <span data-ttu-id="bb764-125">CopyICDocDimtoICDocDim</span><span class="sxs-lookup"><span data-stu-id="bb764-125">CopyICDocDimtoICDocDim</span></span>|<span data-ttu-id="bb764-126">Modify to work with DimSetID -> ICJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="bb764-126">Modify to work with DimSetID -> ICJnlLineDim</span></span>|  

## <a name="deleted-functions"></a><span data-ttu-id="bb764-127">Deleted Functions</span><span class="sxs-lookup"><span data-stu-id="bb764-127">Deleted Functions</span></span>  
 <span data-ttu-id="bb764-128">Functions that are deleted from codeunit 408 in connection with the Dimension Set Entries feature are listed below.</span><span class="sxs-lookup"><span data-stu-id="bb764-128">Functions that are deleted from codeunit 408 in connection with the Dimension Set Entries feature are listed below.</span></span>  

> [!CAUTION]  
>  <span data-ttu-id="bb764-129">During the upgrade of application code from Microsoft Dynamics NAV 2009 or earlier versions to Microsoft Dynamics NAV 2016, the following functions are not available in Microsoft Dynamics NAV 2016.</span><span class="sxs-lookup"><span data-stu-id="bb764-129">During the upgrade of application code from Microsoft Dynamics NAV 2009 or earlier versions to Microsoft Dynamics NAV 2016, the following functions are not available in Microsoft Dynamics NAV 2016.</span></span> <span data-ttu-id="bb764-130">If you have customisations that use one or more of the functions, you must upgrade that code accordingly.</span><span class="sxs-lookup"><span data-stu-id="bb764-130">If you have customizations that use one or more of the functions, you must upgrade that code accordingly.</span></span>

 <span data-ttu-id="bb764-131">InsertJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="bb764-131">InsertJnlLineDim</span></span>  

 <span data-ttu-id="bb764-132">UpdateJnlLineDefaultDim</span><span class="sxs-lookup"><span data-stu-id="bb764-132">UpdateJnlLineDefaultDim</span></span>  

 <span data-ttu-id="bb764-133">GetJnlLineDefaultDim</span><span class="sxs-lookup"><span data-stu-id="bb764-133">GetJnlLineDefaultDim</span></span>  

 <span data-ttu-id="bb764-134">GetPreviousDocDefaultDim</span><span class="sxs-lookup"><span data-stu-id="bb764-134">GetPreviousDocDefaultDim</span></span>  

 <span data-ttu-id="bb764-135">GetPreviousProdDocDefaultDim</span><span class="sxs-lookup"><span data-stu-id="bb764-135">GetPreviousProdDocDefaultDim</span></span>  

 <span data-ttu-id="bb764-136">InsertDocDim</span><span class="sxs-lookup"><span data-stu-id="bb764-136">InsertDocDim</span></span>  

 <span data-ttu-id="bb764-137">UpdateDocDefaultDim</span><span class="sxs-lookup"><span data-stu-id="bb764-137">UpdateDocDefaultDim</span></span>  

 <span data-ttu-id="bb764-138">ExtractDocDefaultDim</span><span class="sxs-lookup"><span data-stu-id="bb764-138">ExtractDocDefaultDim</span></span>  

 <span data-ttu-id="bb764-139">InsertProdDocDim</span><span class="sxs-lookup"><span data-stu-id="bb764-139">InsertProdDocDim</span></span>  

 <span data-ttu-id="bb764-140">UpdateProdDocDefaultDim</span><span class="sxs-lookup"><span data-stu-id="bb764-140">UpdateProdDocDefaultDim</span></span>  

 <span data-ttu-id="bb764-141">InsertServContractDim</span><span class="sxs-lookup"><span data-stu-id="bb764-141">InsertServContractDim</span></span>  

 <span data-ttu-id="bb764-142">UpdateServcontractDim</span><span class="sxs-lookup"><span data-stu-id="bb764-142">UpdateServcontractDim</span></span>  

 <span data-ttu-id="bb764-143">UpdateDefaultDimNewDimValue</span><span class="sxs-lookup"><span data-stu-id="bb764-143">UpdateDefaultDimNewDimValue</span></span>  

 <span data-ttu-id="bb764-144">GetDocDim</span><span class="sxs-lookup"><span data-stu-id="bb764-144">GetDocDim</span></span>  

 <span data-ttu-id="bb764-145">GetProdDocDim</span><span class="sxs-lookup"><span data-stu-id="bb764-145">GetProdDocDim</span></span>  

 <span data-ttu-id="bb764-146">TypeToTableID1</span><span class="sxs-lookup"><span data-stu-id="bb764-146">TypeToTableID1</span></span>  

 <span data-ttu-id="bb764-147">TypeToTableID2</span><span class="sxs-lookup"><span data-stu-id="bb764-147">TypeToTableID2</span></span>  

 <span data-ttu-id="bb764-148">TypeToTableID3</span><span class="sxs-lookup"><span data-stu-id="bb764-148">TypeToTableID3</span></span>  

 <span data-ttu-id="bb764-149">TypeToTableID4</span><span class="sxs-lookup"><span data-stu-id="bb764-149">TypeToTableID4</span></span>  

 <span data-ttu-id="bb764-150">TypeToTableID5</span><span class="sxs-lookup"><span data-stu-id="bb764-150">TypeToTableID5</span></span>  

 <span data-ttu-id="bb764-151">DeleteJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="bb764-151">DeleteJnlLineDim</span></span>  

 <span data-ttu-id="bb764-152">DeleteDocDim</span><span class="sxs-lookup"><span data-stu-id="bb764-152">DeleteDocDim</span></span>  

 <span data-ttu-id="bb764-153">DeletePostedDocDim</span><span class="sxs-lookup"><span data-stu-id="bb764-153">DeletePostedDocDim</span></span>  

 <span data-ttu-id="bb764-154">DeleteProdDocDim</span><span class="sxs-lookup"><span data-stu-id="bb764-154">DeleteProdDocDim</span></span>  

 <span data-ttu-id="bb764-155">DeleteServContractDim</span><span class="sxs-lookup"><span data-stu-id="bb764-155">DeleteServContractDim</span></span>  

 <span data-ttu-id="bb764-156">ShowJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="bb764-156">ShowJnlLineDim</span></span>  

 <span data-ttu-id="bb764-157">SaveJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="bb764-157">SaveJnlLineDim</span></span>  

 <span data-ttu-id="bb764-158">ShowJnlLineNewDim</span><span class="sxs-lookup"><span data-stu-id="bb764-158">ShowJnlLineNewDim</span></span>  

 <span data-ttu-id="bb764-159">SaveJnlLineNewDim</span><span class="sxs-lookup"><span data-stu-id="bb764-159">SaveJnlLineNewDim</span></span>  

 <span data-ttu-id="bb764-160">ShowDocDim</span><span class="sxs-lookup"><span data-stu-id="bb764-160">ShowDocDim</span></span>  

 <span data-ttu-id="bb764-161">SaveDocDim</span><span class="sxs-lookup"><span data-stu-id="bb764-161">SaveDocDim</span></span>  

 <span data-ttu-id="bb764-162">ShowProdDocDim</span><span class="sxs-lookup"><span data-stu-id="bb764-162">ShowProdDocDim</span></span>  

 <span data-ttu-id="bb764-163">SaveProdDocDim</span><span class="sxs-lookup"><span data-stu-id="bb764-163">SaveProdDocDim</span></span>  

 <span data-ttu-id="bb764-164">ShowTempDim</span><span class="sxs-lookup"><span data-stu-id="bb764-164">ShowTempDim</span></span>  

 <span data-ttu-id="bb764-165">SaveTempDim</span><span class="sxs-lookup"><span data-stu-id="bb764-165">SaveTempDim</span></span>  

 <span data-ttu-id="bb764-166">ShowTempNewDim</span><span class="sxs-lookup"><span data-stu-id="bb764-166">ShowTempNewDim</span></span>  

 <span data-ttu-id="bb764-167">SaveTempNewDim</span><span class="sxs-lookup"><span data-stu-id="bb764-167">SaveTempNewDim</span></span>  

 <span data-ttu-id="bb764-168">SaveServContractDim</span><span class="sxs-lookup"><span data-stu-id="bb764-168">SaveServContractDim</span></span>  

 <span data-ttu-id="bb764-169">MoveJnlLineDimToLedgEntryDim</span><span class="sxs-lookup"><span data-stu-id="bb764-169">MoveJnlLineDimToLedgEntryDim</span></span>  

 <span data-ttu-id="bb764-170">MoveDocDimToPostedDocDim</span><span class="sxs-lookup"><span data-stu-id="bb764-170">MoveDocDimToPostedDocDim</span></span>  

 <span data-ttu-id="bb764-171">MoveOneDocDimToPostedDocDim</span><span class="sxs-lookup"><span data-stu-id="bb764-171">MoveOneDocDimToPostedDocDim</span></span>  

 <span data-ttu-id="bb764-172">MoveLedgEntryDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="bb764-172">MoveLedgEntryDimToJnlLineDim</span></span>  

 <span data-ttu-id="bb764-173">MoveDimBufToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="bb764-173">MoveDimBufToJnlLineDim</span></span>  

 <span data-ttu-id="bb764-174">MoveDimBufToLedgEntryDim</span><span class="sxs-lookup"><span data-stu-id="bb764-174">MoveDimBufToLedgEntryDim</span></span>  

 <span data-ttu-id="bb764-175">MoveDimBufToPostedDocDim</span><span class="sxs-lookup"><span data-stu-id="bb764-175">MoveDimBufToPostedDocDim</span></span>  

 <span data-ttu-id="bb764-176">MoveDimBufToGLBudgetDim</span><span class="sxs-lookup"><span data-stu-id="bb764-176">MoveDimBufToGLBudgetDim</span></span>  

 <span data-ttu-id="bb764-177">CopyJnlLineDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="bb764-177">CopyJnlLineDimToJnlLineDim</span></span>  

 <span data-ttu-id="bb764-178">CopyLedgEntryDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="bb764-178">CopyLedgEntryDimToJnlLineDim</span></span>  

 <span data-ttu-id="bb764-179">CopyDocDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="bb764-179">CopyDocDimToDocDim</span></span>  

 <span data-ttu-id="bb764-180">CopyPostedDocDimToPostedDocDim</span><span class="sxs-lookup"><span data-stu-id="bb764-180">CopyPostedDocDimToPostedDocDim</span></span>  

 <span data-ttu-id="bb764-181">CopyDocDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="bb764-181">CopyDocDimToJnlLineDim</span></span>  

 <span data-ttu-id="bb764-182">CopyDimBufToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="bb764-182">CopyDimBufToJnlLineDim</span></span>  

 <span data-ttu-id="bb764-183">CopyDimBufToDocDim</span><span class="sxs-lookup"><span data-stu-id="bb764-183">CopyDimBufToDocDim</span></span>  

 <span data-ttu-id="bb764-184">CopySCDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="bb764-184">CopySCDimToDocDim</span></span>  

 <span data-ttu-id="bb764-185">MoveDocDimToLedgEntryDim</span><span class="sxs-lookup"><span data-stu-id="bb764-185">MoveDocDimToLedgEntryDim</span></span>  

 <span data-ttu-id="bb764-186">MoveDocDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="bb764-186">MoveDocDimToDocDim</span></span>  

 <span data-ttu-id="bb764-187">MoveDocDimArchvToDocDim</span><span class="sxs-lookup"><span data-stu-id="bb764-187">MoveDocDimArchvToDocDim</span></span>  

 <span data-ttu-id="bb764-188">MoveLedgEntryDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="bb764-188">MoveLedgEntryDimToDocDim</span></span>  

 <span data-ttu-id="bb764-189">MoveProdDocDimToProdDocDim</span><span class="sxs-lookup"><span data-stu-id="bb764-189">MoveProdDocDimToProdDocDim</span></span>  

 <span data-ttu-id="bb764-190">MoveJnlLineDimToProdDocDim</span><span class="sxs-lookup"><span data-stu-id="bb764-190">MoveJnlLineDimToProdDocDim</span></span>  

 <span data-ttu-id="bb764-191">MoveJnlLineDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="bb764-191">MoveJnlLineDimToDocDim</span></span>  

 <span data-ttu-id="bb764-192">MoveJnlLineDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="bb764-192">MoveJnlLineDimToJnlLineDim</span></span>  

 <span data-ttu-id="bb764-193">CopyLedgEntryDimToLedgEntryDim</span><span class="sxs-lookup"><span data-stu-id="bb764-193">CopyLedgEntryDimToLedgEntryDim</span></span>  

 <span data-ttu-id="bb764-194">MoveTempFromDimToTempToDim</span><span class="sxs-lookup"><span data-stu-id="bb764-194">MoveTempFromDimToTempToDim</span></span>  

 <span data-ttu-id="bb764-195">TransferTempToDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="bb764-195">TransferTempToDimToDocDim</span></span>  

 <span data-ttu-id="bb764-196">MoveJnlLineDimToBuf</span><span class="sxs-lookup"><span data-stu-id="bb764-196">MoveJnlLineDimToBuf</span></span>  

 <span data-ttu-id="bb764-197">CopyICJnlDimToICJnlDim</span><span class="sxs-lookup"><span data-stu-id="bb764-197">CopyICJnlDimToICJnlDim</span></span>  

 <span data-ttu-id="bb764-198">TestDimValue</span><span class="sxs-lookup"><span data-stu-id="bb764-198">TestDimValue</span></span>  

 <span data-ttu-id="bb764-199">TestNewDimValue</span><span class="sxs-lookup"><span data-stu-id="bb764-199">TestNewDimValue</span></span>  

 <span data-ttu-id="bb764-200">MoveDimBufToItemBudgetDim.</span><span class="sxs-lookup"><span data-stu-id="bb764-200">MoveDimBufToItemBudgetDim.</span></span> <span data-ttu-id="bb764-201">(Delete because the ItemBudgetDim Table is deleted.)</span><span class="sxs-lookup"><span data-stu-id="bb764-201">(Delete because the ItemBudgetDim Table is deleted.)</span></span>  

 <span data-ttu-id="bb764-202">GetServContractDim</span><span class="sxs-lookup"><span data-stu-id="bb764-202">GetServContractDim</span></span>  

 <span data-ttu-id="bb764-203">MoveTempDimToBuf</span><span class="sxs-lookup"><span data-stu-id="bb764-203">MoveTempDimToBuf</span></span>  

 <span data-ttu-id="bb764-204">UpdateSCInvLineDim</span><span class="sxs-lookup"><span data-stu-id="bb764-204">UpdateSCInvLineDim</span></span>  

 <span data-ttu-id="bb764-205">CopyJnlLineDimToBuffer</span><span class="sxs-lookup"><span data-stu-id="bb764-205">CopyJnlLineDimToBuffer</span></span>  

 <span data-ttu-id="bb764-206">UpdateDocDefaultDim2</span><span class="sxs-lookup"><span data-stu-id="bb764-206">UpdateDocDefaultDim2</span></span>  

## <a name="see-also"></a><span data-ttu-id="bb764-207">See Also</span><span class="sxs-lookup"><span data-stu-id="bb764-207">See Also</span></span>
 <span data-ttu-id="bb764-208">[Design Details: Dimension Set Entries](design-details-dimension-set-entries.md) </span><span class="sxs-lookup"><span data-stu-id="bb764-208">[Design Details: Dimension Set Entries](design-details-dimension-set-entries.md) </span></span>  
 <span data-ttu-id="bb764-209">[Design Details: Dimension Set Entries Overview](design-details-dimension-set-entries-overview.md) </span><span class="sxs-lookup"><span data-stu-id="bb764-209">[Design Details: Dimension Set Entries Overview](design-details-dimension-set-entries-overview.md) </span></span>  
 <span data-ttu-id="bb764-210">[Design Details: Searching for Dimension Combinations](design-details-searching-for-dimension-combinations.md) </span><span class="sxs-lookup"><span data-stu-id="bb764-210">[Design Details: Searching for Dimension Combinations](design-details-searching-for-dimension-combinations.md) </span></span>  
 [<span data-ttu-id="bb764-211">Design Details: Table Structure</span><span class="sxs-lookup"><span data-stu-id="bb764-211">Design Details: Table Structure</span></span>](design-details-table-structure.md)   
 
