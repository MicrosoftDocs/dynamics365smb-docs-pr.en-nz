---
title: Set Up Incoming Documents| Microsoft Docs
description: Use the Incoming Documents feature to create electronic documents, manage OCR tasks, import invoices, and convert image files.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: electronic document, e-invoice, incoming document, OCR, ecommerce, document exchange, import invoice
ms.date: 04/01/2019
ms.author: sgroespe
ms.openlocfilehash: 7e99f4b33767a1bdea7b942d1b183edbacc829ac
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 04/29/2019
ms.locfileid: "1241524"
---
# <a name="set-up-incoming-documents"></a><span data-ttu-id="fc475-103">Set Up Incoming Documents</span><span class="sxs-lookup"><span data-stu-id="fc475-103">Set Up Incoming Documents</span></span>
<span data-ttu-id="fc475-104">If you create general journal lines from incoming document records, you must specify on the **Incoming Documents Setup** page which journal template and batch to use.</span><span class="sxs-lookup"><span data-stu-id="fc475-104">If you create general journal lines from incoming document records, you must specify on the **Incoming Documents Setup** page which journal template and batch to use.</span></span>

<span data-ttu-id="fc475-105">If you do not want users to create invoices or general journal lines from incoming document records unless the documents are first approved, you must set up approvers on the **Incoming Document Approvers** page.</span><span class="sxs-lookup"><span data-stu-id="fc475-105">If you do not want users to create invoices or general journal lines from incoming document records unless the documents are first approved, you must set up approvers on the **Incoming Document Approvers** page.</span></span>

<span data-ttu-id="fc475-106">To turn PDF and image files into electronic documents that you can convert to, for example, purchase invoices inside [!INCLUDE[d365fin](includes/d365fin_md.md)], you must first set up the OCR feature and enable the service.</span><span class="sxs-lookup"><span data-stu-id="fc475-106">To turn PDF and image files into electronic documents that you can convert to, for example, purchase invoices inside [!INCLUDE[d365fin](includes/d365fin_md.md)], you must first set up the OCR feature and enable the service.</span></span>

<span data-ttu-id="fc475-107">When the Incoming Documents feature is set up, you can use different functions to review expense receipts, manage OCR tasks, and convert incoming document files, manually or automatically, to the relevant documents or journal lines.</span><span class="sxs-lookup"><span data-stu-id="fc475-107">When the Incoming Documents feature is set up, you can use different functions to review expense receipts, manage OCR tasks, and convert incoming document files, manually or automatically, to the relevant documents or journal lines.</span></span> <span data-ttu-id="fc475-108">The external files can be attached at any process stage, including to posted documents and to the resulting vendor, customer, and general ledger entries.</span><span class="sxs-lookup"><span data-stu-id="fc475-108">The external files can be attached at any process stage, including to posted documents and to the resulting vendor, customer, and general ledger entries.</span></span> <span data-ttu-id="fc475-109">For more information, see [Processing Incoming Documents](across-process-income-documents.md).</span><span class="sxs-lookup"><span data-stu-id="fc475-109">For more information, see [Processing Incoming Documents](across-process-income-documents.md).</span></span>

## <a name="to-set-up-the-incoming-documents-feature"></a><span data-ttu-id="fc475-110">To set up the Incoming Documents feature</span><span class="sxs-lookup"><span data-stu-id="fc475-110">To set up the Incoming Documents feature</span></span>
1. <span data-ttu-id="fc475-111">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Incoming Document Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="fc475-111">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Incoming Document Setup**, and then choose the related link.</span></span>
2. <span data-ttu-id="fc475-112">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="fc475-112">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="to-set-up-approvers-of-incoming-document-records"></a><span data-ttu-id="fc475-113">To set up approvers of incoming document records</span><span class="sxs-lookup"><span data-stu-id="fc475-113">To set up approvers of incoming document records</span></span>
1. <span data-ttu-id="fc475-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Incoming Document Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="fc475-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Incoming Document Setup**, and then choose the related link.</span></span>  
2. <span data-ttu-id="fc475-115">On the **Incoming Documents Setup** page, choose the **Approvers** action.</span><span class="sxs-lookup"><span data-stu-id="fc475-115">On the **Incoming Documents Setup** page, choose the **Approvers** action.</span></span>

    <span data-ttu-id="fc475-116">The **Incoming Document Approvers** page shows all users that are set up in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="fc475-116">The **Incoming Document Approvers** page shows all users that are set up in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  
3. <span data-ttu-id="fc475-117">Select one or more users that can approve an incoming document before a related document or journal line can be created.</span><span class="sxs-lookup"><span data-stu-id="fc475-117">Select one or more users that can approve an incoming document before a related document or journal line can be created.</span></span>

<span data-ttu-id="fc475-118">When approvers have been set up on the **Incoming Document Approvers** page, only those users can approve an incoming document if the **Require Approval To Create** check box on the **Incoming Documents Setup** page is selected.</span><span class="sxs-lookup"><span data-stu-id="fc475-118">When approvers have been set up on the **Incoming Document Approvers** page, only those users can approve an incoming document if the **Require Approval To Create** check box on the **Incoming Documents Setup** page is selected.</span></span>

> [!NOTE]  
>   <span data-ttu-id="fc475-119">This approval setup is not related to approval workflows.</span><span class="sxs-lookup"><span data-stu-id="fc475-119">This approval setup is not related to approval workflows.</span></span> <span data-ttu-id="fc475-120">For more information, see [Use Approval Workflows](across-how-use-approval-workflows.md).</span><span class="sxs-lookup"><span data-stu-id="fc475-120">For more information, see [Use Approval Workflows](across-how-use-approval-workflows.md).</span></span>

## <a name="to-set-up-an-ocr-service"></a><span data-ttu-id="fc475-121">To set up an OCR service</span><span class="sxs-lookup"><span data-stu-id="fc475-121">To set up an OCR service</span></span>
1. <span data-ttu-id="fc475-122">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **OCR Service Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="fc475-122">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **OCR Service Setup**, and then choose the related link.</span></span>
2. <span data-ttu-id="fc475-123">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="fc475-123">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

> [!NOTE]  
> <span data-ttu-id="fc475-124">You login data is automatically encrypted.</span><span class="sxs-lookup"><span data-stu-id="fc475-124">You login data is automatically encrypted.</span></span>

## <a name="see-also"></a><span data-ttu-id="fc475-125">See Also</span><span class="sxs-lookup"><span data-stu-id="fc475-125">See Also</span></span>
[<span data-ttu-id="fc475-126">Process Incoming Documents</span><span class="sxs-lookup"><span data-stu-id="fc475-126">Process Incoming Documents</span></span>](across-process-income-documents.md)  
[<span data-ttu-id="fc475-127">Incoming Documents</span><span class="sxs-lookup"><span data-stu-id="fc475-127">Incoming Documents</span></span>](across-income-documents.md)  
[<span data-ttu-id="fc475-128">Purchasing</span><span class="sxs-lookup"><span data-stu-id="fc475-128">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="fc475-129">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="fc475-129">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
