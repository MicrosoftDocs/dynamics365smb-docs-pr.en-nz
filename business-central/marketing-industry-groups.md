---
title: Set Up Industry Groups for Contact Companies| Microsoft Docs
description: Describes how to define an industry group and assign it to a contact company, for example, the retail industry or the automobile industry.
services: project-madeira
documentationcenter: ''
author: jswymer
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: relationship, prospect
ms.date: 10/01/2019
ms.author: jswymer
redirect_url: marketing-setup-contacts
ms.openlocfilehash: 9d1f685dce54db493e830096ef5d4749f0fc221a
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 10/01/2019
ms.locfileid: "2309044"
---
# <a name="set-up-industry-groups-for-contact-companies"></a><span data-ttu-id="6d910-103">Set Up Industry Groups for Contact Companies</span><span class="sxs-lookup"><span data-stu-id="6d910-103">Set Up Industry Groups for Contact Companies</span></span>
<span data-ttu-id="6d910-104">You use industry groups to indicate the type of industry to which your contacts belong, for example, the retail industry or the automobile industry.</span><span class="sxs-lookup"><span data-stu-id="6d910-104">You use industry groups to indicate the type of industry to which your contacts belong, for example, the retail industry or the automobile industry.</span></span>

<span data-ttu-id="6d910-105">Using industry groups on contacts is a two-step process.</span><span class="sxs-lookup"><span data-stu-id="6d910-105">Using industry groups on contacts is a two-step process.</span></span> <span data-ttu-id="6d910-106">First, you define the industry group code.</span><span class="sxs-lookup"><span data-stu-id="6d910-106">First, you define the industry group code.</span></span> <span data-ttu-id="6d910-107">You only have to perform this step one time for each industry group.</span><span class="sxs-lookup"><span data-stu-id="6d910-107">You only have to perform this step one time for each industry group.</span></span> <span data-ttu-id="6d910-108">Once you have an industry group code, you can start to assign the code to contact companies.</span><span class="sxs-lookup"><span data-stu-id="6d910-108">Once you have an industry group code, you can start to assign the code to contact companies.</span></span>

> [!NOTE]  
>   <span data-ttu-id="6d910-109">If you plan to synchronise your contacts with vendors, customers, or bank accounts in other parts of the application, you may want to set up a business relation for them.</span><span class="sxs-lookup"><span data-stu-id="6d910-109">If you plan to synchronize your contacts with vendors, customers, or bank accounts in other parts of the application, you may want to set up a business relation for them.</span></span>

## <a name="to-define-an-industry-group-code"></a><span data-ttu-id="6d910-110">To define an industry group code</span><span class="sxs-lookup"><span data-stu-id="6d910-110">To define an industry group code</span></span>
<span data-ttu-id="6d910-111">The industry group code defines the type or category of the group, such as ADVERT for advertising, or PRESS, for TV and radio.</span><span class="sxs-lookup"><span data-stu-id="6d910-111">The industry group code defines the type or category of the group, such as ADVERT for advertising, or PRESS, for TV and radio.</span></span> <span data-ttu-id="6d910-112">You can have several industry group codes.</span><span class="sxs-lookup"><span data-stu-id="6d910-112">You can have several industry group codes.</span></span> <span data-ttu-id="6d910-113">To define the industry groups, you use the **Industry Groups** page.</span><span class="sxs-lookup"><span data-stu-id="6d910-113">To define the industry groups, you use the **Industry Groups** page.</span></span>

1. <span data-ttu-id="6d910-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Industry Groups**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="6d910-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Industry Groups**, and then choose the related link.</span></span>
2. <span data-ttu-id="6d910-115">Choose the **New** action, and fill in a code and description.</span><span class="sxs-lookup"><span data-stu-id="6d910-115">Choose the **New** action, and fill in a code and description.</span></span> <span data-ttu-id="6d910-116">The code can be a maximum of 11 characters, and can be any combination of numbers and letters.</span><span class="sxs-lookup"><span data-stu-id="6d910-116">The code can be a maximum of 11 characters, and can be any combination of numbers and letters.</span></span>

## <a name="AssignIndustryGroupContact"></a> <span data-ttu-id="6d910-117">To assign industry groups to a contact</span><span class="sxs-lookup"><span data-stu-id="6d910-117">To assign industry groups to a contact</span></span>
<span data-ttu-id="6d910-118">You cannot assign industry groups to a contact person - only companies.</span><span class="sxs-lookup"><span data-stu-id="6d910-118">You cannot assign industry groups to a contact person - only companies.</span></span>

1. <span data-ttu-id="6d910-119">Open the contact.</span><span class="sxs-lookup"><span data-stu-id="6d910-119">Open the contact.</span></span>
2. <span data-ttu-id="6d910-120">Choose the **Company** action, and then the **Industry Groups** action.</span><span class="sxs-lookup"><span data-stu-id="6d910-120">Choose the **Company** action, and then the **Industry Groups** action.</span></span> <span data-ttu-id="6d910-121">The **Contact Industry Groups** page opens.</span><span class="sxs-lookup"><span data-stu-id="6d910-121">The **Contact Industry Groups** page opens.</span></span>
3. <span data-ttu-id="6d910-122">In the **Industry Groups Code** field, select the industry groups you want to assign.</span><span class="sxs-lookup"><span data-stu-id="6d910-122">In the **Industry Groups Code** field, select the industry groups you want to assign.</span></span>

<span data-ttu-id="6d910-123">Repeat these steps to assign as many industry groups as you want.</span><span class="sxs-lookup"><span data-stu-id="6d910-123">Repeat these steps to assign as many industry groups as you want.</span></span> <span data-ttu-id="6d910-124">You can also assign industry groups from the contact list by following the same procedure.</span><span class="sxs-lookup"><span data-stu-id="6d910-124">You can also assign industry groups from the contact list by following the same procedure.</span></span>

<span data-ttu-id="6d910-125">The number of industry groups that you have assigned to the contact is displayed in the **No. of Industry Groups** field in the **Segmentation** section on the **Contact** page.</span><span class="sxs-lookup"><span data-stu-id="6d910-125">The number of industry groups that you have assigned to the contact is displayed in the **No. of Industry Groups** field in the **Segmentation** section on the **Contact** page.</span></span>

<span data-ttu-id="6d910-126">After you have assigned industry groups to your contacts, you can use this information to select contacts for your segments.</span><span class="sxs-lookup"><span data-stu-id="6d910-126">After you have assigned industry groups to your contacts, you can use this information to select contacts for your segments.</span></span> <span data-ttu-id="6d910-127">For more information, see [Add Contacts to Segments](marketing-add-contact-segment.md).</span><span class="sxs-lookup"><span data-stu-id="6d910-127">For more information, see [Add Contacts to Segments](marketing-add-contact-segment.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="6d910-128">See Also</span><span class="sxs-lookup"><span data-stu-id="6d910-128">See Also</span></span>
[<span data-ttu-id="6d910-129">Creating Contacts</span><span class="sxs-lookup"><span data-stu-id="6d910-129">Creating Contacts</span></span>](marketing-create-contact-companies.md)  
<span data-ttu-id="6d910-130">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="6d910-130">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
