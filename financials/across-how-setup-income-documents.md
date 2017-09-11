---
title: Set Up Incoming Documents| Microsoft Docs
description: Use the Incoming Documents feature to create electronic documents, manage OCR tasks, import invoices, and convert image files.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: electronic document, e-invoice, incoming document, OCR, ecommerce, document exchange, import invoice
ms.date: 06/02/2017
ms.author: sgroespe
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: 69cb1037da2f3873ecb9a3f498ce5fadfeabac1d
ms.contentlocale: en-nz
ms.lasthandoff: 09/11/2017

---
# <a name="how-to-set-up-incoming-documents"></a><span data-ttu-id="6192f-103">How to: Set Up Incoming Documents</span><span class="sxs-lookup"><span data-stu-id="6192f-103">How to: Set Up Incoming Documents</span></span>
<span data-ttu-id="6192f-104">If you create general journal lines from incoming document records, you must specify in the **Incoming Documents Setup** window which journal template and batch to use.</span><span class="sxs-lookup"><span data-stu-id="6192f-104">If you create general journal lines from incoming document records, you must specify in the **Incoming Documents Setup** window which journal template and batch to use.</span></span>

<span data-ttu-id="6192f-105">If you do not want users to create invoices or general journal lines from incoming document records unless the documents are first approved, you must set up approvers in the **Incoming Document Approvers** window.</span><span class="sxs-lookup"><span data-stu-id="6192f-105">If you do not want users to create invoices or general journal lines from incoming document records unless the documents are first approved, you must set up approvers in the **Incoming Document Approvers** window.</span></span>

<span data-ttu-id="6192f-106">To turn PDF and image files into electronic documents that you can convert to, for example, purchase invoices inside [!INCLUDE[d365fin](includes/d365fin_md.md)], you must first set up the OCR feature and enable the service.</span><span class="sxs-lookup"><span data-stu-id="6192f-106">To turn PDF and image files into electronic documents that you can convert to, for example, purchase invoices inside [!INCLUDE[d365fin](includes/d365fin_md.md)], you must first set up the OCR feature and enable the service.</span></span>

<span data-ttu-id="6192f-107">When the Incoming Documents feature is set up, you can use different functions to review expense receipts, manage OCR tasks, and convert incoming document files, manually or automatically, to the relevant documents or journal lines.</span><span class="sxs-lookup"><span data-stu-id="6192f-107">When the Incoming Documents feature is set up, you can use different functions to review expense receipts, manage OCR tasks, and convert incoming document files, manually or automatically, to the relevant documents or journal lines.</span></span> <span data-ttu-id="6192f-108">The external files can be attached at any process stage, including to posted documents and to the resulting vendor, customer, and general ledger entries.</span><span class="sxs-lookup"><span data-stu-id="6192f-108">The external files can be attached at any process stage, including to posted documents and to the resulting vendor, customer, and general ledger entries.</span></span> <span data-ttu-id="6192f-109">For more information, see [Processing Incoming Documents](across-process-income-documents.md).</span><span class="sxs-lookup"><span data-stu-id="6192f-109">For more information, see [Processing Incoming Documents](across-process-income-documents.md).</span></span>

## <a name="to-set-up-the-incoming-documents-feature"></a><span data-ttu-id="6192f-110">To set up the Incoming Documents feature</span><span class="sxs-lookup"><span data-stu-id="6192f-110">To set up the Incoming Documents feature</span></span>
1. <span data-ttu-id="6192f-111">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Incoming Document Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="6192f-111">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Incoming Document Setup**, and then choose the related link.</span></span>
2. <span data-ttu-id="6192f-112">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="6192f-112">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="to-set-up-approvers-of-incoming-document-records"></a><span data-ttu-id="6192f-113">To set up approvers of incoming document records</span><span class="sxs-lookup"><span data-stu-id="6192f-113">To set up approvers of incoming document records</span></span>
1. <span data-ttu-id="6192f-114">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Incoming Document Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="6192f-114">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Incoming Document Setup**, and then choose the related link.</span></span>  
2. <span data-ttu-id="6192f-115">In the **Incoming Documents Setup** window, choose the **Approvers** action.</span><span class="sxs-lookup"><span data-stu-id="6192f-115">In the **Incoming Documents Setup** window, choose the **Approvers** action.</span></span>

    <span data-ttu-id="6192f-116">The **Incoming Document Approvers** window shows all users that are set up in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="6192f-116">The **Incoming Document Approvers** window shows all users that are set up in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  
3. <span data-ttu-id="6192f-117">Select one or more users that can approve an incoming document before a related document or journal line can be created.</span><span class="sxs-lookup"><span data-stu-id="6192f-117">Select one or more users that can approve an incoming document before a related document or journal line can be created.</span></span>

<span data-ttu-id="6192f-118">When approvers have been set up in the **Incoming Document Approvers** window, only those users can approve an incoming document if the **Require Approval To Create** check box in the **Incoming Documents Setup** window is selected.</span><span class="sxs-lookup"><span data-stu-id="6192f-118">When approvers have been set up in the **Incoming Document Approvers** window, only those users can approve an incoming document if the **Require Approval To Create** check box in the **Incoming Documents Setup** window is selected.</span></span>

> [!NOTE]  
>   <span data-ttu-id="6192f-119">This approval setup is not related to approval workflows.</span><span class="sxs-lookup"><span data-stu-id="6192f-119">This approval setup is not related to approval workflows.</span></span> <span data-ttu-id="6192f-120">For more information, see [How to: Use Approval Workflows](across-how-use-approval-workflows.md).</span><span class="sxs-lookup"><span data-stu-id="6192f-120">For more information, see [How to: Use Approval Workflows](across-how-use-approval-workflows.md).</span></span>

## <a name="to-set-up-an-ocr-service"></a><span data-ttu-id="6192f-121">To set up an OCR service</span><span class="sxs-lookup"><span data-stu-id="6192f-121">To set up an OCR service</span></span>
1. <span data-ttu-id="6192f-122">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **OCR Service Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="6192f-122">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **OCR Service Setup**, and then choose the related link.</span></span>
2. <span data-ttu-id="6192f-123">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="6192f-123">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="to-encrypt-your-login-information"></a><span data-ttu-id="6192f-124">To encrypt your login information</span><span class="sxs-lookup"><span data-stu-id="6192f-124">To encrypt your login information</span></span>
<span data-ttu-id="6192f-125">It is recommended that you protect the logon information that you enter in the **OCR Service Setup** window.</span><span class="sxs-lookup"><span data-stu-id="6192f-125">It is recommended that you protect the logon information that you enter in the **OCR Service Setup** window.</span></span> <span data-ttu-id="6192f-126">You can encrypt data on the server by generating new or importing existing encryption keys that you enable on the server instance that connects to the database.</span><span class="sxs-lookup"><span data-stu-id="6192f-126">You can encrypt data on the server by generating new or importing existing encryption keys that you enable on the server instance that connects to the database.</span></span>

1. <span data-ttu-id="6192f-127">In the **OCR Service Setup** window, choose the **Encryption Management** action.</span><span class="sxs-lookup"><span data-stu-id="6192f-127">In the **OCR Service Setup** window, choose the **Encryption Management** action.</span></span>
2. <span data-ttu-id="6192f-128">In the **Data Encryption Management** window, enable encryption of your data.</span><span class="sxs-lookup"><span data-stu-id="6192f-128">In the **Data Encryption Management** window, enable encryption of your data.</span></span>

## <a name="see-also"></a><span data-ttu-id="6192f-129">See Also</span><span class="sxs-lookup"><span data-stu-id="6192f-129">See Also</span></span>
[<span data-ttu-id="6192f-130">Process Incoming Documents</span><span class="sxs-lookup"><span data-stu-id="6192f-130">Process Incoming Documents</span></span>](across-process-income-documents.md)  
[<span data-ttu-id="6192f-131">Incoming Documents</span><span class="sxs-lookup"><span data-stu-id="6192f-131">Incoming Documents</span></span>](across-income-documents.md)  
[<span data-ttu-id="6192f-132">Purchasing</span><span class="sxs-lookup"><span data-stu-id="6192f-132">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="6192f-133">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="6192f-133">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

