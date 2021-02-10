---
title: Send Electronic Documents
description: learn how to send invoices electronically.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 43f61682a1068a8e1652fd28421f83d5291c8fe8
ms.sourcegitcommit: fe6943d410f5dca4e8b2986f95501009ae982d98
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 01/05/2021
ms.locfileid: "4827084"
---
# <a name="send-electronic-documents"></a><span data-ttu-id="5fd2e-103">Send Electronic Documents</span><span class="sxs-lookup"><span data-stu-id="5fd2e-103">Send Electronic Documents</span></span>

<span data-ttu-id="5fd2e-104">The generic version of [!INCLUDE[prod_short](includes/prod_short.md)] supports sending electronic invoices and credit memos in the PEPPOL format, a format that the largest document exchange service providers support.</span><span class="sxs-lookup"><span data-stu-id="5fd2e-104">The generic version of [!INCLUDE[prod_short](includes/prod_short.md)] supports sending electronic invoices and credit memos in the PEPPOL format, a format that the largest document exchange service providers support.</span></span> <span data-ttu-id="5fd2e-105">A document exchange service provider dispatches electronic documents between trading partners.</span><span class="sxs-lookup"><span data-stu-id="5fd2e-105">A document exchange service provider dispatches electronic documents between trading partners.</span></span> <span data-ttu-id="5fd2e-106">To provide support for other electronic document formats, you use the data exchange framework.</span><span class="sxs-lookup"><span data-stu-id="5fd2e-106">To provide support for other electronic document formats, you use the data exchange framework.</span></span>  

 <span data-ttu-id="5fd2e-107">In the generic version of [!INCLUDE[prod_short](includes/prod_short.md)], a document exchange service is preconfigured and ready to be set up for your company.</span><span class="sxs-lookup"><span data-stu-id="5fd2e-107">In the generic version of [!INCLUDE[prod_short](includes/prod_short.md)], a document exchange service is preconfigured and ready to be set up for your company.</span></span> <span data-ttu-id="5fd2e-108">For more information, see [Set Up a Document Exchange Service](across-how-to-set-up-a-document-exchange-service.md).</span><span class="sxs-lookup"><span data-stu-id="5fd2e-108">For more information, see [Set Up a Document Exchange Service](across-how-to-set-up-a-document-exchange-service.md).</span></span> <span data-ttu-id="5fd2e-109">However, in some cases, you must install an app.</span><span class="sxs-lookup"><span data-stu-id="5fd2e-109">However, in some cases, you must install an app.</span></span> <span data-ttu-id="5fd2e-110">For more information, see [Electronic Invoicing FAQ](faq-electronic-invoicing.yml).</span><span class="sxs-lookup"><span data-stu-id="5fd2e-110">For more information, see [Electronic Invoicing FAQ](faq-electronic-invoicing.yml).</span></span>  

 <span data-ttu-id="5fd2e-111">To send a sales invoice as an electronic PEPPOL document, you select the **Electronic Document** option in the **Post and Send** dialogue box.</span><span class="sxs-lookup"><span data-stu-id="5fd2e-111">To send a sales invoice as an electronic PEPPOL document, you select the **Electronic Document** option in the **Post and Send** dialog box.</span></span> <span data-ttu-id="5fd2e-112">You can also set up the customer's default document sending profile from that dialogue box.</span><span class="sxs-lookup"><span data-stu-id="5fd2e-112">You can also set up the customer's default document sending profile from that dialog box.</span></span> <span data-ttu-id="5fd2e-113">First, you must set up various master data, such as company information, customers, items, and units of measure.</span><span class="sxs-lookup"><span data-stu-id="5fd2e-113">First, you must set up various master data, such as company information, customers, items, and units of measure.</span></span> <span data-ttu-id="5fd2e-114">These are used to identify the business partners and items when converting data in fields in [Set Up Electronic Document Sending and Receiving](across-how-to-set-up-electronic-document-sending-and-receiving.md).</span><span class="sxs-lookup"><span data-stu-id="5fd2e-114">These are used to identify the business partners and items when converting data in fields in [Set Up Electronic Document Sending and Receiving](across-how-to-set-up-electronic-document-sending-and-receiving.md).</span></span>  

### <a name="to-send-an-electronic-sales-invoice"></a><span data-ttu-id="5fd2e-115">To send an electronic sales invoice</span><span class="sxs-lookup"><span data-stu-id="5fd2e-115">To send an electronic sales invoice</span></span>

1. <span data-ttu-id="5fd2e-116">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Invoices**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="5fd2e-116">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Invoices**, and then choose the related link.</span></span>  

2. <span data-ttu-id="5fd2e-117">Create a new sales invoice.</span><span class="sxs-lookup"><span data-stu-id="5fd2e-117">Create a new sales invoice.</span></span>  

3. <span data-ttu-id="5fd2e-118">When the sales invoice is ready to be invoiced, choose the **Post and Send** action.</span><span class="sxs-lookup"><span data-stu-id="5fd2e-118">When the sales invoice is ready to be invoiced, choose the **Post and Send** action.</span></span>  

     <span data-ttu-id="5fd2e-119">If the customer's default sending profile is **Electronic Document**, then it will be shown in the **Post and Send Confirmation** dialogue box.</span><span class="sxs-lookup"><span data-stu-id="5fd2e-119">If the customer's default sending profile is **Electronic Document**, then it will be shown in the **Post and Send Confirmation** dialog box.</span></span> <span data-ttu-id="5fd2e-120">This way, you just have to choose the **Yes** button to post and send the invoice electronically in the selected format.</span><span class="sxs-lookup"><span data-stu-id="5fd2e-120">This way, you just have to choose the **Yes** button to post and send the invoice electronically in the selected format.</span></span>  

4. <span data-ttu-id="5fd2e-121">In the **Post and Send Confirmation** dialogue box, choose the AssistEdit button to the right of the **Send Document to** field.</span><span class="sxs-lookup"><span data-stu-id="5fd2e-121">In the **Post and Send Confirmation** dialog box, choose the AssistEdit button to the right of the **Send Document to** field.</span></span>  

5. <span data-ttu-id="5fd2e-122">In the **Send Document to** dialogue box, in the **Electronic Document** field, choose **Through Document Exchange Service**.</span><span class="sxs-lookup"><span data-stu-id="5fd2e-122">In the **Send Document to** dialog box, in the **Electronic Document** field, choose **Through Document Exchange Service**.</span></span>  

6. <span data-ttu-id="5fd2e-123">In the **Format** field, choose **PEPPOL**.</span><span class="sxs-lookup"><span data-stu-id="5fd2e-123">In the **Format** field, choose **PEPPOL**.</span></span>  

7. <span data-ttu-id="5fd2e-124">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="5fd2e-124">Choose the **OK** button.</span></span> <span data-ttu-id="5fd2e-125">The **Post and Send Confirmation** dialogue box appears.</span><span class="sxs-lookup"><span data-stu-id="5fd2e-125">The **Post and Send Confirmation** dialog box appears.</span></span> <span data-ttu-id="5fd2e-126">**Electronic Document (PEPPOL)** is added to the **Send Document to** field.</span><span class="sxs-lookup"><span data-stu-id="5fd2e-126">**Electronic Document (PEPPOL)** is added to the **Send Document to** field.</span></span>  

8. <span data-ttu-id="5fd2e-127">Choose the **Yes** button.</span><span class="sxs-lookup"><span data-stu-id="5fd2e-127">Choose the **Yes** button.</span></span>  

     <span data-ttu-id="5fd2e-128">The sales invoice is posted and sent to the customer in the PEPPOL format.</span><span class="sxs-lookup"><span data-stu-id="5fd2e-128">The sales invoice is posted and sent to the customer in the PEPPOL format.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="5fd2e-129">You can also send a posted sales invoice as an electronic document.</span><span class="sxs-lookup"><span data-stu-id="5fd2e-129">You can also send a posted sales invoice as an electronic document.</span></span> <span data-ttu-id="5fd2e-130">The procedure is the same as described in this topic for non-posted sales documents.</span><span class="sxs-lookup"><span data-stu-id="5fd2e-130">The procedure is the same as described in this topic for non-posted sales documents.</span></span> <span data-ttu-id="5fd2e-131">On the **Posted Sales Invoice** page, choose the **Activity Log** action to view the status of the electronic document.</span><span class="sxs-lookup"><span data-stu-id="5fd2e-131">On the **Posted Sales Invoice** page, choose the **Activity Log** action to view the status of the electronic document.</span></span>  

## <a name="see-related-training-at-microsoft-learn"></a><span data-ttu-id="5fd2e-132">See Related Training at [Microsoft Learn](/learn/modules/electronic-documents-dynamics-365-business-central/index)</span><span class="sxs-lookup"><span data-stu-id="5fd2e-132">See Related Training at [Microsoft Learn](/learn/modules/electronic-documents-dynamics-365-business-central/index)</span></span>

## <a name="see-also"></a><span data-ttu-id="5fd2e-133">See Also</span><span class="sxs-lookup"><span data-stu-id="5fd2e-133">See Also</span></span>

[<span data-ttu-id="5fd2e-134">Invoice Sales</span><span class="sxs-lookup"><span data-stu-id="5fd2e-134">Invoice Sales</span></span>](sales-how-invoice-sales.md)  
[<span data-ttu-id="5fd2e-135">Set Up Document Sending Profiles</span><span class="sxs-lookup"><span data-stu-id="5fd2e-135">Set Up Document Sending Profiles</span></span>](sales-how-setup-document-send-profiles.md)  
[<span data-ttu-id="5fd2e-136">Set Up Electronic Document Sending and Receiving</span><span class="sxs-lookup"><span data-stu-id="5fd2e-136">Set Up Electronic Document Sending and Receiving</span></span>](across-how-to-set-up-electronic-document-sending-and-receiving.md)  
[<span data-ttu-id="5fd2e-137">Set Up a Document Exchange Service</span><span class="sxs-lookup"><span data-stu-id="5fd2e-137">Set Up a Document Exchange Service</span></span>](across-how-to-set-up-a-document-exchange-service.md)  
[<span data-ttu-id="5fd2e-138">Set Up Data Exchange Definitions</span><span class="sxs-lookup"><span data-stu-id="5fd2e-138">Set Up Data Exchange Definitions</span></span>](across-how-to-set-up-data-exchange-definitions.md)  
[<span data-ttu-id="5fd2e-139">Exchanging Data Electronically</span><span class="sxs-lookup"><span data-stu-id="5fd2e-139">Exchanging Data Electronically</span></span>](across-data-exchange.md)  
[<span data-ttu-id="5fd2e-140">Electronic Invoicing FAQ</span><span class="sxs-lookup"><span data-stu-id="5fd2e-140">Electronic Invoicing FAQ</span></span>](faq-electronic-invoicing.yml)  
[<span data-ttu-id="5fd2e-141">General Business Functionality</span><span class="sxs-lookup"><span data-stu-id="5fd2e-141">General Business Functionality</span></span>](ui-across-business-areas.md)  
