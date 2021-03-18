---
title: Use Invoicing and Business Central | Microsoft Docs
description: Workaround for accessing Microsoft Invoicing when you have signed up for Dynamics 365 Business Central.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: Invoicing, Microsoft 365
ms.date: 10/01/2020
ms.author: bholtorf
ms.openlocfilehash: 0c6b739faf2d531505bde4ad2dc7eb85c39ed223
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "5385040"
---
# <a name="using-the-same-microsoft-365-account-in-prod_short-and-microsoft-invoicing"></a><span data-ttu-id="de431-103">Using the same Microsoft 365 Account in [!INCLUDE[prod_short](includes/prod_long.md)] and Microsoft Invoicing</span><span class="sxs-lookup"><span data-stu-id="de431-103">Using the same Microsoft 365 Account in [!INCLUDE[prod_short](includes/prod_long.md)] and Microsoft Invoicing</span></span>
<span data-ttu-id="de431-104">When you sign up for a trial with [!INCLUDE[prod_short](includes/prod_short.md)], you can move to a 30-day evaluation phase, you can start a subscription, or you can stop using [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="de431-104">When you sign up for a trial with [!INCLUDE[prod_short](includes/prod_short.md)], you can move to a 30-day evaluation phase, you can start a subscription, or you can stop using [!INCLUDE[prod_short](includes/prod_short.md)].</span></span> <span data-ttu-id="de431-105">In all cases, you may at some point have seen something called **Microsoft Invoicing** and clicked it.</span><span class="sxs-lookup"><span data-stu-id="de431-105">In all cases, you may at some point have seen something called **Microsoft Invoicing** and clicked it.</span></span> <span data-ttu-id="de431-106">This was an app that was part of what is now Microsoft 365 Business Standard and was formerly known as Microsoft 365 Business Premium subscription, so not everyone will have seen that tile in their Microsoft 365 experience.</span><span class="sxs-lookup"><span data-stu-id="de431-106">This was an app that was part of what is now Microsoft 365 Business Standard and was formerly known as Microsoft 365 Business Premium subscription, so not everyone will have seen that tile in their Microsoft 365 experience.</span></span>  

<span data-ttu-id="de431-107">Microsoft Invoicing is no longer available, but if you need to sign into Invoicing to retrieve your data, you might see a message that you cannot access Microsoft Invoicing because your account is used in [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="de431-107">Microsoft Invoicing is no longer available, but if you need to sign into Invoicing to retrieve your data, you might see a message that you cannot access Microsoft Invoicing because your account is used in [!INCLUDE[prod_short](includes/prod_short.md)].</span></span>  

<span data-ttu-id="de431-108">You see a similar message if you install the mobile app for Invoicing.</span><span class="sxs-lookup"><span data-stu-id="de431-108">You see a similar message if you install the mobile app for Invoicing.</span></span>  

## <a name="workaround"></a><span data-ttu-id="de431-109">Workaround</span><span class="sxs-lookup"><span data-stu-id="de431-109">Workaround</span></span>
<span data-ttu-id="de431-110">Invoicing and [!INCLUDE[prod_short](includes/prod_short.md)] have a shared platform.</span><span class="sxs-lookup"><span data-stu-id="de431-110">Invoicing and [!INCLUDE[prod_short](includes/prod_short.md)] have a shared platform.</span></span> <span data-ttu-id="de431-111">That means that you are recognised as an existing user of [!INCLUDE[prod_short](includes/prod_short.md)] when you click Invoicing in the Microsoft 365 admin centre.</span><span class="sxs-lookup"><span data-stu-id="de431-111">That means that you are recognized as an existing user of [!INCLUDE[prod_short](includes/prod_short.md)] when you click Invoicing in the Microsoft 365 admin center.</span></span> <span data-ttu-id="de431-112">The reason is that Invoicing cannot use the same company as [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="de431-112">The reason is that Invoicing cannot use the same company as [!INCLUDE[prod_short](includes/prod_short.md)].</span></span>  

<span data-ttu-id="de431-113">So you will have to sign in to [!INCLUDE[prod_short](includes/prod_short.md)] and rename your existing company, and then create a new company that you can then use in Invoicing.</span><span class="sxs-lookup"><span data-stu-id="de431-113">So you will have to sign in to [!INCLUDE[prod_short](includes/prod_short.md)] and rename your existing company, and then create a new company that you can then use in Invoicing.</span></span> <span data-ttu-id="de431-114">No data is moved or overwritten during this workaround.</span><span class="sxs-lookup"><span data-stu-id="de431-114">No data is moved or overwritten during this workaround.</span></span>

### <a name="to-rename-your-company"></a><span data-ttu-id="de431-115">To rename your company</span><span class="sxs-lookup"><span data-stu-id="de431-115">To rename your company</span></span>
1. <span data-ttu-id="de431-116">Sign in to [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="de431-116">Sign in to [!INCLUDE[prod_short](includes/prod_short.md)].</span></span>
2. <span data-ttu-id="de431-117">In the top right corner, choose the **Settings** icon ![Settings](media/ui-experience/settings_icon_small.png "Settings icon for role centre"), and then choose **My Settings**.</span><span class="sxs-lookup"><span data-stu-id="de431-117">In the top right corner, choose the **Settings** icon ![Settings](media/ui-experience/settings_icon_small.png "Settings icon for role center"), and then choose **My Settings**.</span></span>
3. <span data-ttu-id="de431-118">In the **Company** field, choose a different company.</span><span class="sxs-lookup"><span data-stu-id="de431-118">In the **Company** field, choose a different company.</span></span>
4. <span data-ttu-id="de431-119">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Companies**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="de431-119">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Companies**, and then choose the related link.</span></span>  
5. <span data-ttu-id="de431-120">On the **Companies** page, choose **Edit List**.</span><span class="sxs-lookup"><span data-stu-id="de431-120">On the **Companies** page, choose **Edit List**.</span></span>  
6. <span data-ttu-id="de431-121">Change the name of the *My Company* entry to something else.</span><span class="sxs-lookup"><span data-stu-id="de431-121">Change the name of the *My Company* entry to something else.</span></span>  

    <span data-ttu-id="de431-122">Wait a number of minutes.</span><span class="sxs-lookup"><span data-stu-id="de431-122">Wait a number of minutes.</span></span> <span data-ttu-id="de431-123">We’ll be making a number of changes in the underlying database, and that takes a while.</span><span class="sxs-lookup"><span data-stu-id="de431-123">We’ll be making a number of changes in the underlying database, and that takes a while.</span></span>
7.  <span data-ttu-id="de431-124">When the system is ready again, choose the **Create New Company** button.</span><span class="sxs-lookup"><span data-stu-id="de431-124">When the system is ready again, choose the **Create New Company** button.</span></span>  
8.  <span data-ttu-id="de431-125">In the dialogue that appears, specify the name as *My Company*, and choose the **Production – Setup Data Only** option.</span><span class="sxs-lookup"><span data-stu-id="de431-125">In the dialog that appears, specify the name as *My Company*, and choose the **Production – Setup Data Only** option.</span></span>  

<span data-ttu-id="de431-126">This again takes a number of minutes.</span><span class="sxs-lookup"><span data-stu-id="de431-126">This again takes a number of minutes.</span></span> <span data-ttu-id="de431-127">When the process completes, you will be able to access Invoicing as part of your Microsoft 365 Business Standard experience.</span><span class="sxs-lookup"><span data-stu-id="de431-127">When the process completes, you will be able to access Invoicing as part of your Microsoft 365 Business Standard experience.</span></span> <span data-ttu-id="de431-128">but only to export data since the Invoicing app is deprecated.</span><span class="sxs-lookup"><span data-stu-id="de431-128">but only to export data since the Invoicing app is deprecated.</span></span>  

### <a name="what-about-my-data"></a><span data-ttu-id="de431-129">What about my data?</span><span class="sxs-lookup"><span data-stu-id="de431-129">What about my data?</span></span>
<span data-ttu-id="de431-130">When you rename the original My Company, the database tables that store your existing [!INCLUDE[prod_short](includes/prod_short.md)] data are renamed, but the data itself is not touched.</span><span class="sxs-lookup"><span data-stu-id="de431-130">When you rename the original My Company, the database tables that store your existing [!INCLUDE[prod_short](includes/prod_short.md)] data are renamed, but the data itself is not touched.</span></span>  

<span data-ttu-id="de431-131">If you use both Invoicing and [!INCLUDE[prod_short](includes/prod_short.md)], the data is stored in two different containers (the two companies).</span><span class="sxs-lookup"><span data-stu-id="de431-131">If you use both Invoicing and [!INCLUDE[prod_short](includes/prod_short.md)], the data is stored in two different containers (the two companies).</span></span> <span data-ttu-id="de431-132">Nothing is shared, so you'll have to manage customers and items in both companies.</span><span class="sxs-lookup"><span data-stu-id="de431-132">Nothing is shared, so you'll have to manage customers and items in both companies.</span></span>  

## <a name="see-also"></a><span data-ttu-id="de431-133">See Also</span><span class="sxs-lookup"><span data-stu-id="de431-133">See Also</span></span>
[<span data-ttu-id="de431-134">Frequently Asked Questions</span><span class="sxs-lookup"><span data-stu-id="de431-134">Frequently Asked Questions</span></span>](across-faq.md)  
[<span data-ttu-id="de431-135">Administration</span><span class="sxs-lookup"><span data-stu-id="de431-135">Administration</span></span>](admin-setup-and-administration.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]