---
title: Why Can't I Personalise a Page | Microsoft Docs
description: Explains why you cannot personalise a page and what you can do to unlock it so you can personalise it.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: customize, personalize, personalization, hide columns, remove fields, move fields
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 0bd24833f37fe70f8e642685be4d28dbb593a16d
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 10/01/2020
ms.locfileid: "3923411"
---
# <a name="why-a-page-is-locked-from-personalization"></a><span data-ttu-id="b7939-103">Why a Page is Locked from Personalisation</span><span class="sxs-lookup"><span data-stu-id="b7939-103">Why a Page is Locked from Personalization</span></span>

<span data-ttu-id="b7939-104">There are two conditions that prevent you from personalising a page.</span><span class="sxs-lookup"><span data-stu-id="b7939-104">There are two conditions that prevent you from personalizing a page.</span></span> <span data-ttu-id="b7939-105">Either the page is locked (as indicated by the ![Personalise Lock](media/personalization-lock-icon.png "Personalise lock")) icon or it is blocked (as indicated by the ![Personalisation blocked](media/personalization-blocked-icon.png "Personalisation blocked") icon).</span><span class="sxs-lookup"><span data-stu-id="b7939-105">Either the page is locked (as indicated by the ![Personalize Lock](media/personalization-lock-icon.png "Personalize lock")) icon or it is blocked (as indicated by the ![Personalization blocked](media/personalization-blocked-icon.png "Personalization blocked") icon).</span></span>

## <a name="locked-from-personalizing"></a><span data-ttu-id="b7939-106">Locked from Personalising</span><span class="sxs-lookup"><span data-stu-id="b7939-106">Locked from Personalizing</span></span>

<span data-ttu-id="b7939-107">If there is a ![Personalise Lock](media/personalization-lock-icon.png "Personalise lock") icon in the **Personalising** banner when you open a page, this means that you are currently prevented from making any more personalisation changes to the page.</span><span class="sxs-lookup"><span data-stu-id="b7939-107">If there is a ![Personalize Lock](media/personalization-lock-icon.png "Personalize lock") icon in the **Personalizing** banner when you open a page, this means that you are currently prevented from making any more personalization changes to the page.</span></span>

<!-- This is because we changed the way personalization works behind the scenes since the last time that you personalized the page. Unfortunately, the old way and new of doing things do not work together.

The page currently includes the last personalization changes that you made. If you want to continue personalizing the page, then you can choose the lock icon and then **Unlock**. Just be aware that if you choose to unlock the page, the current personalization of the page will be cleared, and you will have to start from scratch.
-->

<span data-ttu-id="b7939-108">There can be two reasons for this:</span><span class="sxs-lookup"><span data-stu-id="b7939-108">There can be two reasons for this:</span></span>

1. <span data-ttu-id="b7939-109">You have personalised the page before, but it was done using an earlier version of the product.</span><span class="sxs-lookup"><span data-stu-id="b7939-109">You have personalized the page before, but it was done using an earlier version of the product.</span></span> <span data-ttu-id="b7939-110">We changed the way personalisation works behind the scenes since the last time that you personalised the page.</span><span class="sxs-lookup"><span data-stu-id="b7939-110">We changed the way personalization works behind the scenes since the last time that you personalized the page.</span></span> <span data-ttu-id="b7939-111">Unfortunately, the old way and new way of doing things do not work together.</span><span class="sxs-lookup"><span data-stu-id="b7939-111">Unfortunately, the old way and new way of doing things do not work together.</span></span>

2. <span data-ttu-id="b7939-112">Until now, you have only used the [!INCLUDE[nav_windows_md](includes/nav_windows_md.md)] to personalise the page.</span><span class="sxs-lookup"><span data-stu-id="b7939-112">Until now, you have only used the [!INCLUDE[nav_windows_md](includes/nav_windows_md.md)] to personalize the page.</span></span>

### <a name="unlocking-the-page"></a><span data-ttu-id="b7939-113">Unlocking the Page</span><span class="sxs-lookup"><span data-stu-id="b7939-113">Unlocking the Page</span></span>

<span data-ttu-id="b7939-114">If you want to unlock a page and continue personalising it, choose the ![Personalise Lock](media/personalization-lock-icon.png "Personalise lock") icon, and then choose the **Unlock** action.</span><span class="sxs-lookup"><span data-stu-id="b7939-114">If you want to unlock a page and continue personalizing it, choose the ![Personalize Lock](media/personalization-lock-icon.png "Personalize lock") icon, and then choose the **Unlock** action.</span></span>  

<span data-ttu-id="b7939-115">Before you unlock the page, be aware of the following:</span><span class="sxs-lookup"><span data-stu-id="b7939-115">Before you unlock the page, be aware of the following:</span></span>

- <span data-ttu-id="b7939-116">The current personalisation of the page will be cleared.</span><span class="sxs-lookup"><span data-stu-id="b7939-116">The current personalization of the page will be cleared.</span></span> <span data-ttu-id="b7939-117">The page will go back to its original layout, and you will have to start from scratch.</span><span class="sxs-lookup"><span data-stu-id="b7939-117">The page will go back to its original layout, and you will have to start from scratch.</span></span>

- <span data-ttu-id="b7939-118">In the [!INCLUDE[nav_windows_md](includes/nav_windows_md.md)], the page will remain as-is and will not be affected by the new personalisation changes made in the Business Central client.</span><span class="sxs-lookup"><span data-stu-id="b7939-118">In the [!INCLUDE[nav_windows_md](includes/nav_windows_md.md)], the page will remain as-is and will not be affected by the new personalization changes made in the Business Central client.</span></span> <span data-ttu-id="b7939-119">Going forward, the personalisation in the [!INCLUDE[nav_windows_md](includes/nav_windows_md.md)] and Business Central client will be completely separate from each other.</span><span class="sxs-lookup"><span data-stu-id="b7939-119">Going forward, the personalization in the [!INCLUDE[nav_windows_md](includes/nav_windows_md.md)] and Business Central client will be completely separate from each other.</span></span>

## <a name="blocked-from-personalizing"></a><span data-ttu-id="b7939-120">Blocked from Personalising</span><span class="sxs-lookup"><span data-stu-id="b7939-120">Blocked from Personalizing</span></span>

<span data-ttu-id="b7939-121">If there is a ![Personalisation blocked](media/personalization-blocked-icon.png "Personalisation blocked") icon in the **Personalising** banner, this means that you are blocked from doing any personalisation to the page.</span><span class="sxs-lookup"><span data-stu-id="b7939-121">If there is a ![Personalization blocked](media/personalization-blocked-icon.png "Personalization blocked") icon in the **Personalizing** banner, this means that you are blocked from doing any personalization to the page.</span></span>

<!-- Only text is translated, so removing this image for non-English UX reasons.  ![Personalize blocked](media/personalization-blocked.png "Personalize lock") -->

<span data-ttu-id="b7939-122">The reason for this is that the Role Centre or role that is currently associated with your user account modifies this page specifically for your role.</span><span class="sxs-lookup"><span data-stu-id="b7939-122">The reason for this is that the Role Center or role that is currently associated with your user account modifies this page specifically for your role.</span></span> <span data-ttu-id="b7939-123">Contact your administrator for assistance.</span><span class="sxs-lookup"><span data-stu-id="b7939-123">Contact your administrator for assistance.</span></span> <span data-ttu-id="b7939-124">Alternatively, try switching to a Role Centre that does include role-tailoring for this page.</span><span class="sxs-lookup"><span data-stu-id="b7939-124">Alternatively, try switching to a Role Center that does include role-tailoring for this page.</span></span> <span data-ttu-id="b7939-125">For more information, see [Change Basic Settings](ui-change-basic-settings.md).</span><span class="sxs-lookup"><span data-stu-id="b7939-125">For more information, see [Change Basic Settings](ui-change-basic-settings.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="b7939-126">See Also</span><span class="sxs-lookup"><span data-stu-id="b7939-126">See Also</span></span>
[<span data-ttu-id="b7939-127">Personalise Your Workspace</span><span class="sxs-lookup"><span data-stu-id="b7939-127">Personalize Your Workspace</span></span>](ui-personalization-user.md)  
[<span data-ttu-id="b7939-128">Customise Pages for Profiles</span><span class="sxs-lookup"><span data-stu-id="b7939-128">Customize Pages for Profiles</span></span>](ui-personalization-manage.md)  
[<span data-ttu-id="b7939-129">Change Basic Settings</span><span class="sxs-lookup"><span data-stu-id="b7939-129">Change Basic Settings</span></span>](ui-change-basic-settings.md)  
[<span data-ttu-id="b7939-130">Change Which Features are Displayed</span><span class="sxs-lookup"><span data-stu-id="b7939-130">Change Which Features are Displayed</span></span>](ui-experiences.md)  
