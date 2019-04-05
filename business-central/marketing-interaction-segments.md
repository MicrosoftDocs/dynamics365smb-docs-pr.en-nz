---
title: Keep Track of Segments and Related Interactions| Microsoft Docs
description: Learn about creating segments to define groups of contacts and specifying interactions for segments.
services: project-madeira
documentationcenter: ''
author: jswymer
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: relationship, prospect
ms.date: 10/01/2018
ms.author: jswymer
ms.openlocfilehash: 1fcec3051fdabae818528742fba5d9ca57a721c8
ms.sourcegitcommit: 1bcfaa99ea302e6b84b8361ca02730b135557fc1
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 03/08/2019
ms.locfileid: "823109"
---
# <a name="managing-interactions-for-segments"></a><span data-ttu-id="0bd5a-103">Managing Interactions for Segments</span><span class="sxs-lookup"><span data-stu-id="0bd5a-103">Managing Interactions for Segments</span></span>
<span data-ttu-id="0bd5a-104">The **Segment** page is a type of worksheet where you can:</span><span class="sxs-lookup"><span data-stu-id="0bd5a-104">The **Segment** page is a type of worksheet where you can:</span></span>

* <span data-ttu-id="0bd5a-105">Create segments.</span><span class="sxs-lookup"><span data-stu-id="0bd5a-105">Create segments.</span></span>
* <span data-ttu-id="0bd5a-106">Save the segmentation criteria you have used to select contacts.</span><span class="sxs-lookup"><span data-stu-id="0bd5a-106">Save the segmentation criteria you have used to select contacts.</span></span>
* <span data-ttu-id="0bd5a-107">Log the segment and record interactions involving the contacts within the segment.</span><span class="sxs-lookup"><span data-stu-id="0bd5a-107">Log the segment and record interactions involving the contacts within the segment.</span></span>

## <a name="segmenting"></a><span data-ttu-id="0bd5a-108">Segmenting</span><span class="sxs-lookup"><span data-stu-id="0bd5a-108">Segmenting</span></span>
<span data-ttu-id="0bd5a-109">There are several ways to create segments:</span><span class="sxs-lookup"><span data-stu-id="0bd5a-109">There are several ways to create segments:</span></span>

* <span data-ttu-id="0bd5a-110">You can manually enter the contacts you want to include in the segment in the segment lines.</span><span class="sxs-lookup"><span data-stu-id="0bd5a-110">You can manually enter the contacts you want to include in the segment in the segment lines.</span></span>
* <span data-ttu-id="0bd5a-111">You can select contacts.</span><span class="sxs-lookup"><span data-stu-id="0bd5a-111">You can select contacts.</span></span>
* <span data-ttu-id="0bd5a-112">You can reuse a logged segment as the basis to create a new one.</span><span class="sxs-lookup"><span data-stu-id="0bd5a-112">You can reuse a logged segment as the basis to create a new one.</span></span>
* <span data-ttu-id="0bd5a-113">You can reuse saved segmentation criteria.</span><span class="sxs-lookup"><span data-stu-id="0bd5a-113">You can reuse saved segmentation criteria.</span></span>

## <a name="interactions"></a><span data-ttu-id="0bd5a-114">Interactions</span><span class="sxs-lookup"><span data-stu-id="0bd5a-114">Interactions</span></span>
<span data-ttu-id="0bd5a-115">On the **Segment** page, you can create interactions for several contacts simultaneously.</span><span class="sxs-lookup"><span data-stu-id="0bd5a-115">On the **Segment** page, you can create interactions for several contacts simultaneously.</span></span> <span data-ttu-id="0bd5a-116">For example, you can merge a segment with a Microsoft Word document, so that you can send a letter to all the contacts in the segment.</span><span class="sxs-lookup"><span data-stu-id="0bd5a-116">For example, you can merge a segment with a Microsoft Word document, so that you can send a letter to all the contacts in the segment.</span></span>

<span data-ttu-id="0bd5a-117">You can specify information about the interaction for the segment on the **Segment** header.</span><span class="sxs-lookup"><span data-stu-id="0bd5a-117">You can specify information about the interaction for the segment on the **Segment** header.</span></span> <span data-ttu-id="0bd5a-118">For example, you can decide which interaction template you want to use for all the contacts, specify a description, a correspondence type, and so on.</span><span class="sxs-lookup"><span data-stu-id="0bd5a-118">For example, you can decide which interaction template you want to use for all the contacts, specify a description, a correspondence type, and so on.</span></span> <span data-ttu-id="0bd5a-119">However, you can modify this information in the segment line for each particular contact, for example, by specifying another description for one contact.</span><span class="sxs-lookup"><span data-stu-id="0bd5a-119">However, you can modify this information in the segment line for each particular contact, for example, by specifying another description for one contact.</span></span> <span data-ttu-id="0bd5a-120">If you are merging a segment with a Microsoft Word document, you can personalise the document to be sent for one or several of the contacts within the segment, for example, by adding individualised comments to the document.</span><span class="sxs-lookup"><span data-stu-id="0bd5a-120">If you are merging a segment with a Microsoft Word document, you can personalize the document to be sent for one or several of the contacts within the segment, for example, by adding individualized comments to the document.</span></span>

## <a name="logging"></a><span data-ttu-id="0bd5a-121">Logging</span><span class="sxs-lookup"><span data-stu-id="0bd5a-121">Logging</span></span>
<span data-ttu-id="0bd5a-122">On the **Segment** page, when you choose **Log**, the application records the interactions on the **Interaction Log Entry** page, and logs the segment.</span><span class="sxs-lookup"><span data-stu-id="0bd5a-122">On the **Segment** page, when you choose **Log**, the application records the interactions on the **Interaction Log Entry** page, and logs the segment.</span></span> <span data-ttu-id="0bd5a-123">After you have logged the segment, you can only find it on the **Logged Segments** page.</span><span class="sxs-lookup"><span data-stu-id="0bd5a-123">After you have logged the segment, you can only find it on the **Logged Segments** page.</span></span>

<span data-ttu-id="0bd5a-124">On the **Logged Segments** page, you can decide to create a follow-up segment containing the same contacts as the segment you have logged.</span><span class="sxs-lookup"><span data-stu-id="0bd5a-124">On the **Logged Segments** page, you can decide to create a follow-up segment containing the same contacts as the segment you have logged.</span></span>

## <a name="see-also"></a><span data-ttu-id="0bd5a-125">See Also</span><span class="sxs-lookup"><span data-stu-id="0bd5a-125">See Also</span></span>
[<span data-ttu-id="0bd5a-126">Create Segments</span><span class="sxs-lookup"><span data-stu-id="0bd5a-126">Create Segments</span></span>](marketing-how-create-segment.md)  
[<span data-ttu-id="0bd5a-127">Create Interactions for Segments</span><span class="sxs-lookup"><span data-stu-id="0bd5a-127">Create Interactions for Segments</span></span>](marketing-how-create-interactions.md)  
[<span data-ttu-id="0bd5a-128">Managing Segments</span><span class="sxs-lookup"><span data-stu-id="0bd5a-128">Managing Segments</span></span>](marketing-segments.md)  
[<span data-ttu-id="0bd5a-129">Recording Interactions With Contacts</span><span class="sxs-lookup"><span data-stu-id="0bd5a-129">Recording Interactions With Contacts</span></span>](marketing-interactions.md)  
[<span data-ttu-id="0bd5a-130">Managing Sales Opportunities</span><span class="sxs-lookup"><span data-stu-id="0bd5a-130">Managing Sales Opportunities</span></span>](marketing-manage-sales-opportunities.md)  
[<span data-ttu-id="0bd5a-131">Creating and Managing Contacts</span><span class="sxs-lookup"><span data-stu-id="0bd5a-131">Creating and Managing Contacts</span></span>](marketing-contacts.md)  
[<span data-ttu-id="0bd5a-132">Working with Business Central</span><span class="sxs-lookup"><span data-stu-id="0bd5a-132">Working with Business Central</span></span>](ui-work-product.md)
