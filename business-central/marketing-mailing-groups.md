---
title: Set Up Mailing Groups for Contacts| Microsoft Docs
description: You can use mailing groups to identify groups of contacts that you want to receive the same information, for example, for a marketing campaign or promo.
services: project-madeira
documentationcenter: 
author: jswymer
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: marketing, campaign, promo, prospect
ms.date: 10/01/2018
ms.author: jswymer
redirect_url: marketing-setup-contacts
ms.translationtype: HT
ms.sourcegitcommit: 8a73de1aa2f4a0f633c401ea341bb7bde6579723
ms.openlocfilehash: 8fb97913d4a864988e8ef3c62eb27a8a86e361dd
ms.contentlocale: en-nz
ms.lasthandoff: 12/11/2018

---
# <a name="set-up-mailing-groups-for-contacts"></a><span data-ttu-id="c927f-103">Set Up Mailing Groups for Contacts</span><span class="sxs-lookup"><span data-stu-id="c927f-103">Set Up Mailing Groups for Contacts</span></span>
<span data-ttu-id="c927f-104">You can use mailing groups to identify groups of contacts that you want to receive the same information.</span><span class="sxs-lookup"><span data-stu-id="c927f-104">You can use mailing groups to identify groups of contacts that you want to receive the same information.</span></span> <span data-ttu-id="c927f-105">For example, you can set up a mailing group for the contacts that you want to send a notification of an office move, or another group for sending holiday gifts.</span><span class="sxs-lookup"><span data-stu-id="c927f-105">For example, you can set up a mailing group for the contacts that you want to send a notification of an office move, or another group for sending holiday gifts.</span></span>

<span data-ttu-id="c927f-106">Using mailing groups on contacts is a two-step process.</span><span class="sxs-lookup"><span data-stu-id="c927f-106">Using mailing groups on contacts is a two-step process.</span></span> <span data-ttu-id="c927f-107">First, you define the mailing group code.</span><span class="sxs-lookup"><span data-stu-id="c927f-107">First, you define the mailing group code.</span></span> <span data-ttu-id="c927f-108">You only have to perform this step one time for each mailing group.</span><span class="sxs-lookup"><span data-stu-id="c927f-108">You only have to perform this step one time for each mailing group.</span></span> <span data-ttu-id="c927f-109">Once you have a mailing group code, you can start to assign the code to contact companies.</span><span class="sxs-lookup"><span data-stu-id="c927f-109">Once you have a mailing group code, you can start to assign the code to contact companies.</span></span>

## <a name="to-define-mailing-group-codes"></a><span data-ttu-id="c927f-110">To define mailing group codes</span><span class="sxs-lookup"><span data-stu-id="c927f-110">To define mailing group codes</span></span>
<span data-ttu-id="c927f-111">The mailing group code defines the type or category of the group, such as MOVE for office move, or GIFT for holiday gift.</span><span class="sxs-lookup"><span data-stu-id="c927f-111">The mailing group code defines the type or category of the group, such as MOVE for office move, or GIFT for holiday gift.</span></span> <span data-ttu-id="c927f-112">You can have several industry group codes.</span><span class="sxs-lookup"><span data-stu-id="c927f-112">You can have several industry group codes.</span></span> <span data-ttu-id="c927f-113">To define the industry groups, you use the **Mailing Groups** page.</span><span class="sxs-lookup"><span data-stu-id="c927f-113">To define the industry groups, you use the **Mailing Groups** page.</span></span>

1. <span data-ttu-id="c927f-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Mailing Groups**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="c927f-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Mailing Groups**, and then choose the related link.</span></span>
2. <span data-ttu-id="c927f-115">Choose the **New** action, and fill in a code and description.</span><span class="sxs-lookup"><span data-stu-id="c927f-115">Choose the **New** action, and fill in a code and description.</span></span> <span data-ttu-id="c927f-116">The code can be a maximum of 11 characters, and can be any combination of numbers and letters.</span><span class="sxs-lookup"><span data-stu-id="c927f-116">The code can be a maximum of 11 characters, and can be any combination of numbers and letters.</span></span>

## <a name="AssignMailGroupContact"></a> <span data-ttu-id="c927f-117">To assign mailing groups to a contact</span><span class="sxs-lookup"><span data-stu-id="c927f-117">To assign mailing groups to a contact</span></span>
1. <span data-ttu-id="c927f-118">Open the contact.</span><span class="sxs-lookup"><span data-stu-id="c927f-118">Open the contact.</span></span>
2. <span data-ttu-id="c927f-119">Choose the **Mailing Groups** action.</span><span class="sxs-lookup"><span data-stu-id="c927f-119">Choose the **Mailing Groups** action.</span></span> <span data-ttu-id="c927f-120">The **Contact Mailing Groups** page opens.</span><span class="sxs-lookup"><span data-stu-id="c927f-120">The **Contact Mailing Groups** page opens.</span></span>
3. <span data-ttu-id="c927f-121">In the **Mailing Groups Code** field, select the mailing group that you want to assign.</span><span class="sxs-lookup"><span data-stu-id="c927f-121">In the **Mailing Groups Code** field, select the mailing group that you want to assign.</span></span>

<span data-ttu-id="c927f-122">Repeat these steps to assign as many mailing groups as you want.</span><span class="sxs-lookup"><span data-stu-id="c927f-122">Repeat these steps to assign as many mailing groups as you want.</span></span> <span data-ttu-id="c927f-123">You can also assign mailing groups from the contact list by following the same procedure.</span><span class="sxs-lookup"><span data-stu-id="c927f-123">You can also assign mailing groups from the contact list by following the same procedure.</span></span>

<span data-ttu-id="c927f-124">The number of mailing groups you have assigned to the contact is displayed in the **No. of Mailing Groups** field in the **Segmentation** section on the **Contact** page.</span><span class="sxs-lookup"><span data-stu-id="c927f-124">The number of mailing groups you have assigned to the contact is displayed in the **No. of Mailing Groups** field in the **Segmentation** section on the **Contact** page.</span></span>

<span data-ttu-id="c927f-125">After you have assigned mailing groups to your contacts, you can use this information to select contacts for your segments.</span><span class="sxs-lookup"><span data-stu-id="c927f-125">After you have assigned mailing groups to your contacts, you can use this information to select contacts for your segments.</span></span> <span data-ttu-id="c927f-126">For more information, see [Add Contacts to Segments](marketing-add-contact-segment.md).</span><span class="sxs-lookup"><span data-stu-id="c927f-126">For more information, see [Add Contacts to Segments](marketing-add-contact-segment.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="c927f-127">See Also</span><span class="sxs-lookup"><span data-stu-id="c927f-127">See Also</span></span>
[<span data-ttu-id="c927f-128">Creating Contact Companies</span><span class="sxs-lookup"><span data-stu-id="c927f-128">Creating Contact Companies</span></span>](marketing-create-contact-companies.md)  
[<span data-ttu-id="c927f-129">Creating Contact Persons</span><span class="sxs-lookup"><span data-stu-id="c927f-129">Creating Contact Persons</span></span>](marketing-create-contact-persons.md)  
[<span data-ttu-id="c927f-130">Working with Business Central</span><span class="sxs-lookup"><span data-stu-id="c927f-130">Working with Business Central</span></span>](ui-work-product.md)

