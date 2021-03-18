---
title: Add Attachments, Links, and Notes on Records| Microsoft Docs
description: Attach a hyperlink to a document or website to a specific record, such as a customer or document.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 6aa7018a43db8c663c209894e118518c3de2f7cf
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "5393914"
---
# <a name="manage-attachments-links-and-notes-on-cards-and-documents"></a><span data-ttu-id="49e77-103">Manage Attachments, Links, and Notes on Cards and Documents</span><span class="sxs-lookup"><span data-stu-id="49e77-103">Manage Attachments, Links, and Notes on Cards and Documents</span></span>

<span data-ttu-id="49e77-104">In the FactBox on most cards and documents, you can attach files, add links, and write notes.</span><span class="sxs-lookup"><span data-stu-id="49e77-104">In the FactBox on most cards and documents, you can attach files, add links, and write notes.</span></span> <span data-ttu-id="49e77-105">For links and notes, you can also do this on the list page by first selecting the related line.</span><span class="sxs-lookup"><span data-stu-id="49e77-105">For links and notes, you can also do this on the list page by first selecting the related line.</span></span>

<span data-ttu-id="49e77-106">To view or change any of these attached information types, you must first open the **Attachments** tab in the FactBox.</span><span class="sxs-lookup"><span data-stu-id="49e77-106">To view or change any of these attached information types, you must first open the **Attachments** tab in the FactBox.</span></span> <span data-ttu-id="49e77-107">The number behind the tab title indicates how many attached files, links, or notes exist for the card or document.</span><span class="sxs-lookup"><span data-stu-id="49e77-107">The number behind the tab title indicates how many attached files, links, or notes exist for the card or document.</span></span>

<span data-ttu-id="49e77-108">Attachments, links, and notes stay attached as the card or document is processed into other states, such as from an ongoing sales order to a posted sales invoice.</span><span class="sxs-lookup"><span data-stu-id="49e77-108">Attachments, links, and notes stay attached as the card or document is processed into other states, such as from an ongoing sales order to a posted sales invoice.</span></span> <span data-ttu-id="49e77-109">However, none of the attachment types are output from the system, for example, when printing or when saving to a file.</span><span class="sxs-lookup"><span data-stu-id="49e77-109">However, none of the attachment types are output from the system, for example, when printing or when saving to a file.</span></span>

> [!NOTE]
> <span data-ttu-id="49e77-110">When you partially ship and invoice a sales order or purchase order, the attachment will only be attached to the final invoice of that order.</span><span class="sxs-lookup"><span data-stu-id="49e77-110">When you partially ship and invoice a sales order or purchase order, the attachment will only be attached to the final invoice of that order.</span></span> <span data-ttu-id="49e77-111">Likewise, when you invoice using the Deferrals feature, the attachment is only attached to the G/L entries for the document but not for the deferral entries.</span><span class="sxs-lookup"><span data-stu-id="49e77-111">Likewise, when you invoice using the Deferrals feature, the attachment is only attached to the G/L entries for the document but not for the deferral entries.</span></span>

## <a name="to-attach-a-file-to-a-purchase-invoice"></a><span data-ttu-id="49e77-112">To attach a file to a purchase invoice</span><span class="sxs-lookup"><span data-stu-id="49e77-112">To attach a file to a purchase invoice</span></span>
<span data-ttu-id="49e77-113">You can attach any type of file, containing text, image, or video, to a card or document.</span><span class="sxs-lookup"><span data-stu-id="49e77-113">You can attach any type of file, containing text, image, or video, to a card or document.</span></span> <span data-ttu-id="49e77-114">This is useful, for example, when you want to store a vendor's invoice as a PDF file on the related purchase invoice in [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="49e77-114">This is useful, for example, when you want to store a vendor's invoice as a PDF file on the related purchase invoice in [!INCLUDE[prod_short](includes/prod_short.md)].</span></span>

> [!NOTE]
> <span data-ttu-id="49e77-115">Files attached with the Incoming Documents feature are not included on the **Attachments** tab. For more information, see [Incoming Documents](across-income-documents.md).</span><span class="sxs-lookup"><span data-stu-id="49e77-115">Files attached with the Incoming Documents feature are not included on the **Attachments** tab. For more information, see [Incoming Documents](across-income-documents.md).</span></span>

<span data-ttu-id="49e77-116">The following procedure is based on a purchase invoice.</span><span class="sxs-lookup"><span data-stu-id="49e77-116">The following procedure is based on a purchase invoice.</span></span> <span data-ttu-id="49e77-117">The steps are similar for all other supported documents and cards.</span><span class="sxs-lookup"><span data-stu-id="49e77-117">The steps are similar for all other supported documents and cards.</span></span>

1. <span data-ttu-id="49e77-118">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchase Invoices**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="49e77-118">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchase Invoices**, and then choose the related link.</span></span>
2. <span data-ttu-id="49e77-119">Open the sales order that you want to attach a file to.</span><span class="sxs-lookup"><span data-stu-id="49e77-119">Open the sales order that you want to attach a file to.</span></span>
3. <span data-ttu-id="49e77-120">In the FactBox, open the **Attachments** tab.</span><span class="sxs-lookup"><span data-stu-id="49e77-120">In the FactBox, open the **Attachments** tab.</span></span>
4. <span data-ttu-id="49e77-121">Choose the value behind the **Documents** field, such as "0".</span><span class="sxs-lookup"><span data-stu-id="49e77-121">Choose the value behind the **Documents** field, such as "0".</span></span>
5. <span data-ttu-id="49e77-122">On the **Attached Documents** page, in the **Attachment** field, choose the **Select File** action.</span><span class="sxs-lookup"><span data-stu-id="49e77-122">On the **Attached Documents** page, in the **Attachment** field, choose the **Select File** action.</span></span>
5. <span data-ttu-id="49e77-123">Select a file from any location, and then choose the **Open** button.</span><span class="sxs-lookup"><span data-stu-id="49e77-123">Select a file from any location, and then choose the **Open** button.</span></span>

<span data-ttu-id="49e77-124">The file is now attached to the purchase invoice.</span><span class="sxs-lookup"><span data-stu-id="49e77-124">The file is now attached to the purchase invoice.</span></span>

## <a name="to-view-an-attached-file"></a><span data-ttu-id="49e77-125">To view an attached file</span><span class="sxs-lookup"><span data-stu-id="49e77-125">To view an attached file</span></span>
1. <span data-ttu-id="49e77-126">In the FactBox, open the **Attachments** tab.</span><span class="sxs-lookup"><span data-stu-id="49e77-126">In the FactBox, open the **Attachments** tab.</span></span>
2. <span data-ttu-id="49e77-127">Choose the value behind the **Documents** field, such as "1".</span><span class="sxs-lookup"><span data-stu-id="49e77-127">Choose the value behind the **Documents** field, such as "1".</span></span>
3. <span data-ttu-id="49e77-128">On the **Attached Documents** page, choose the **Preview** action.</span><span class="sxs-lookup"><span data-stu-id="49e77-128">On the **Attached Documents** page, choose the **Preview** action.</span></span>
4. <span data-ttu-id="49e77-129">Open the downloaded file.</span><span class="sxs-lookup"><span data-stu-id="49e77-129">Open the downloaded file.</span></span>

## <a name="to-save-a-document-as-a-pdf-attachment"></a><span data-ttu-id="49e77-130">To save a document as a PDF attachment</span><span class="sxs-lookup"><span data-stu-id="49e77-130">To save a document as a PDF attachment</span></span>
<span data-ttu-id="49e77-131">Whenever you need to save a document as a file, you can use the **Attach as PDF** action to capture the current document content as a PDF file attached to the FactBox of the document.</span><span class="sxs-lookup"><span data-stu-id="49e77-131">Whenever you need to save a document as a file, you can use the **Attach as PDF** action to capture the current document content as a PDF file attached to the FactBox of the document.</span></span> <span data-ttu-id="49e77-132">This is useful, for example, when documents follow multiple steps in a process, such as a sales process or an approval workflow, and you want to refer to a printout of the previous step.</span><span class="sxs-lookup"><span data-stu-id="49e77-132">This is useful, for example, when documents follow multiple steps in a process, such as a sales process or an approval workflow, and you want to refer to a printout of the previous step.</span></span>

<span data-ttu-id="49e77-133">The following procedure is based on a sales order.</span><span class="sxs-lookup"><span data-stu-id="49e77-133">The following procedure is based on a sales order.</span></span> <span data-ttu-id="49e77-134">The steps are similar for all supported documents.</span><span class="sxs-lookup"><span data-stu-id="49e77-134">The steps are similar for all supported documents.</span></span>

1. <span data-ttu-id="49e77-135">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="49e77-135">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.</span></span>
2. <span data-ttu-id="49e77-136">Select a sales order, and then choose the **Attach as PDF** action.</span><span class="sxs-lookup"><span data-stu-id="49e77-136">Select a sales order, and then choose the **Attach as PDF** action.</span></span>

<span data-ttu-id="49e77-137">A PDF file with the current content of the sales order is added to the **Attachments** tab in the FactBox.</span><span class="sxs-lookup"><span data-stu-id="49e77-137">A PDF file with the current content of the sales order is added to the **Attachments** tab in the FactBox.</span></span>

## <a name="to-add-a-link-from-an-item-card"></a><span data-ttu-id="49e77-138">To add a link from an item card</span><span class="sxs-lookup"><span data-stu-id="49e77-138">To add a link from an item card</span></span>
<span data-ttu-id="49e77-139">You can add a link from a card or document to any URL or path.</span><span class="sxs-lookup"><span data-stu-id="49e77-139">You can add a link from a card or document to any URL or path.</span></span> <span data-ttu-id="49e77-140">This is useful, for example, when you want to link an item card with the supplier's item catalogue.</span><span class="sxs-lookup"><span data-stu-id="49e77-140">This is useful, for example, when you want to link an item card with the supplier's item catalog.</span></span>

<span data-ttu-id="49e77-141">The following procedure is based on an item card.</span><span class="sxs-lookup"><span data-stu-id="49e77-141">The following procedure is based on an item card.</span></span> <span data-ttu-id="49e77-142">The steps are similar for all other supported cards and documents.</span><span class="sxs-lookup"><span data-stu-id="49e77-142">The steps are similar for all other supported cards and documents.</span></span>

1. <span data-ttu-id="49e77-143">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="49e77-143">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span></span>
2. <span data-ttu-id="49e77-144">Select the item that you want to add a link from, and then choose the **Attachments** tab in the FactBox.</span><span class="sxs-lookup"><span data-stu-id="49e77-144">Select the item that you want to add a link from, and then choose the **Attachments** tab in the FactBox.</span></span>
3. <span data-ttu-id="49e77-145">In the **Links**, choose the **+** icon.</span><span class="sxs-lookup"><span data-stu-id="49e77-145">In the **Links**, choose the **+** icon.</span></span>
4. <span data-ttu-id="49e77-146">In the **Link Address** field, enter the link.</span><span class="sxs-lookup"><span data-stu-id="49e77-146">In the **Link Address** field, enter the link.</span></span>

    <span data-ttu-id="49e77-147">The link must be a valid internet or intranet URL.</span><span class="sxs-lookup"><span data-stu-id="49e77-147">The link must be a valid internet or intranet URL.</span></span>

5. <span data-ttu-id="49e77-148">In the **Description** field, enter any information about the link.</span><span class="sxs-lookup"><span data-stu-id="49e77-148">In the **Description** field, enter any information about the link.</span></span>  
6. <span data-ttu-id="49e77-149">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="49e77-149">Choose the **OK** button.</span></span>

<span data-ttu-id="49e77-150">The link is now attached to the item card.</span><span class="sxs-lookup"><span data-stu-id="49e77-150">The link is now attached to the item card.</span></span>  

## <a name="to-write-a-note-on-a-sales-order"></a><span data-ttu-id="49e77-151">To write a note on a sales order</span><span class="sxs-lookup"><span data-stu-id="49e77-151">To write a note on a sales order</span></span>
<span data-ttu-id="49e77-152">You can write a note on a document or card, for example, to communicate special instructions to other users of the document or card.</span><span class="sxs-lookup"><span data-stu-id="49e77-152">You can write a note on a document or card, for example, to communicate special instructions to other users of the document or card.</span></span> <span data-ttu-id="49e77-153">You can include file links and URLs in notes.</span><span class="sxs-lookup"><span data-stu-id="49e77-153">You can include file links and URLs in notes.</span></span>

> [!NOTE]
> <span data-ttu-id="49e77-154">Notes on the **Attachments** tab are not related to internal notes functionality, which is mainly used to communicate between workflow users.</span><span class="sxs-lookup"><span data-stu-id="49e77-154">Notes on the **Attachments** tab are not related to internal notes functionality, which is mainly used to communicate between workflow users.</span></span> <span data-ttu-id="49e77-155">For more information, see [Setting Up Workflow Notifications](across-setting-up-workflow-notifications.md).</span><span class="sxs-lookup"><span data-stu-id="49e77-155">For more information, see [Setting Up Workflow Notifications](across-setting-up-workflow-notifications.md).</span></span>

<span data-ttu-id="49e77-156">The following procedure is based on a sales order.</span><span class="sxs-lookup"><span data-stu-id="49e77-156">The following procedure is based on a sales order.</span></span> <span data-ttu-id="49e77-157">The steps are similar for all other supported documents and cards.</span><span class="sxs-lookup"><span data-stu-id="49e77-157">The steps are similar for all other supported documents and cards.</span></span>

1. <span data-ttu-id="49e77-158">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="49e77-158">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.</span></span>
2. <span data-ttu-id="49e77-159">Select the sales order that you want to write a note on, and then choose the **Attachments** tab in the FactBox.</span><span class="sxs-lookup"><span data-stu-id="49e77-159">Select the sales order that you want to write a note on, and then choose the **Attachments** tab in the FactBox.</span></span>
3. <span data-ttu-id="49e77-160">In the **Notes** section, choose the **+** icon.</span><span class="sxs-lookup"><span data-stu-id="49e77-160">In the **Notes** section, choose the **+** icon.</span></span>
4. <span data-ttu-id="49e77-161">In the **Note** field, write any text, such as "This is an urgent order.".</span><span class="sxs-lookup"><span data-stu-id="49e77-161">In the **Note** field, write any text, such as "This is an urgent order.".</span></span>
5. <span data-ttu-id="49e77-162">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="49e77-162">Choose the **OK** button.</span></span>

<span data-ttu-id="49e77-163">The note is now attached to the sales order.</span><span class="sxs-lookup"><span data-stu-id="49e77-163">The note is now attached to the sales order.</span></span>

## <a name="see-also"></a><span data-ttu-id="49e77-164">See Also</span><span class="sxs-lookup"><span data-stu-id="49e77-164">See Also</span></span>  
<span data-ttu-id="49e77-165">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="49e77-165">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="49e77-166">Incoming Documents</span><span class="sxs-lookup"><span data-stu-id="49e77-166">Incoming Documents</span></span>](across-income-documents.md)  
[<span data-ttu-id="49e77-167">Setting Up Workflow Notifications</span><span class="sxs-lookup"><span data-stu-id="49e77-167">Setting Up Workflow Notifications</span></span>](across-setting-up-workflow-notifications.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]