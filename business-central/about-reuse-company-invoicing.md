---
title: Use Invoicing and Business Central | Microsoft Docs
description: Workaround for accessing Microsoft Invoicing when you have signed up for Dynamics 365 Business Central.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: Invoicing, Office 365
ms.date: 04/01/2019
ms.author: bholtorf
ms.openlocfilehash: 0173d64e140cfea91bf7f08d821c2d30cf0eb7b3
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 04/29/2019
ms.locfileid: "1241500"
---
# <a name="using-the-same-office-365-account-in-included365finincludesd365finlongmdmd-and-microsoft-invoicing"></a><span data-ttu-id="094b0-103">Using the same Office 365 Account in [!INCLUDE[d365fin](includes/d365fin_long_md.md)] and Microsoft Invoicing</span><span class="sxs-lookup"><span data-stu-id="094b0-103">Using the same Office 365 Account in [!INCLUDE[d365fin](includes/d365fin_long_md.md)] and Microsoft Invoicing</span></span>
<span data-ttu-id="094b0-104">When you sign up for a trial with [!INCLUDE[d365fin](includes/d365fin_md.md)], you can move to a 30-day evaluation phase, you can start a subscription, or you can stop using [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="094b0-104">When you sign up for a trial with [!INCLUDE[d365fin](includes/d365fin_md.md)], you can move to a 30-day evaluation phase, you can start a subscription, or you can stop using [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="094b0-105">In all cases, if you sign in to the Office Portal, you might see a tile called **Microsoft Invoicing** and click it.</span><span class="sxs-lookup"><span data-stu-id="094b0-105">In all cases, if you sign in to the Office Portal, you might see a tile called **Microsoft Invoicing** and click it.</span></span> <span data-ttu-id="094b0-106">This is part of the Office 365 Business Premium subscription, so not everyone will see that tile in the Office Portal.</span><span class="sxs-lookup"><span data-stu-id="094b0-106">This is part of the Office 365 Business Premium subscription, so not everyone will see that tile in the Office Portal.</span></span>  

<span data-ttu-id="094b0-107">If you access Microsoft Invoicing, you will see a message that you cannot access Microsoft Invoicing because your account is used in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="094b0-107">If you access Microsoft Invoicing, you will see a message that you cannot access Microsoft Invoicing because your account is used in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  

<span data-ttu-id="094b0-108">You see a similar message if you install the mobile app for Invoicing.</span><span class="sxs-lookup"><span data-stu-id="094b0-108">You see a similar message if you install the mobile app for Invoicing.</span></span>  

## <a name="workaround"></a><span data-ttu-id="094b0-109">Workaround</span><span class="sxs-lookup"><span data-stu-id="094b0-109">Workaround</span></span>
<span data-ttu-id="094b0-110">Invoicing and [!INCLUDE[d365fin](includes/d365fin_md.md)] have a shared platform.</span><span class="sxs-lookup"><span data-stu-id="094b0-110">Invoicing and [!INCLUDE[d365fin](includes/d365fin_md.md)] have a shared platform.</span></span> <span data-ttu-id="094b0-111">That means that you are recognised as an existing user of [!INCLUDE[d365fin](includes/d365fin_md.md)] when you click Invoicing in the Office Portal.</span><span class="sxs-lookup"><span data-stu-id="094b0-111">That means that you are recognized as an existing user of [!INCLUDE[d365fin](includes/d365fin_md.md)] when you click Invoicing in the Office Portal.</span></span> <span data-ttu-id="094b0-112">The reason is that Invoicing cannot use the same company as [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="094b0-112">The reason is that Invoicing cannot use the same company as [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  

<span data-ttu-id="094b0-113">So you will have to sign in to [!INCLUDE[d365fin](includes/d365fin_md.md)] and rename your existing company, and then create a new company that you can then use in Invoicing.</span><span class="sxs-lookup"><span data-stu-id="094b0-113">So you will have to sign in to [!INCLUDE[d365fin](includes/d365fin_md.md)] and rename your existing company, and then create a new company that you can then use in Invoicing.</span></span> <span data-ttu-id="094b0-114">No data is moved or overwritten during this workaround.</span><span class="sxs-lookup"><span data-stu-id="094b0-114">No data is moved or overwritten during this workaround.</span></span>

### <a name="to-rename-your-company"></a><span data-ttu-id="094b0-115">To rename your company</span><span class="sxs-lookup"><span data-stu-id="094b0-115">To rename your company</span></span>
1. <span data-ttu-id="094b0-116">Sign in to [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="094b0-116">Sign in to [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>
2. <span data-ttu-id="094b0-117">In the top right corner, choose the **Settings** icon ![Settings](media/ui-experience/settings_icon_small.png "Settings icon for role centre"), and then choose **My Settings**.</span><span class="sxs-lookup"><span data-stu-id="094b0-117">In the top right corner, choose the **Settings** icon ![Settings](media/ui-experience/settings_icon_small.png "Settings icon for role center"), and then choose **My Settings**.</span></span>
3. <span data-ttu-id="094b0-118">In the **Company** field, choose a different company.</span><span class="sxs-lookup"><span data-stu-id="094b0-118">In the **Company** field, choose a different company.</span></span>
4. <span data-ttu-id="094b0-119">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Companies**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="094b0-119">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Companies**, and then choose the related link.</span></span>  
5. <span data-ttu-id="094b0-120">On the **Companies** page, choose **Edit List**.</span><span class="sxs-lookup"><span data-stu-id="094b0-120">On the **Companies** page, choose **Edit List**.</span></span>  
6. <span data-ttu-id="094b0-121">Change the name of the *My Company* entry to something else.</span><span class="sxs-lookup"><span data-stu-id="094b0-121">Change the name of the *My Company* entry to something else.</span></span>  

    <span data-ttu-id="094b0-122">Wait a number of minutes.</span><span class="sxs-lookup"><span data-stu-id="094b0-122">Wait a number of minutes.</span></span> <span data-ttu-id="094b0-123">We’ll be making a number of changes in the underlying database, and that takes a while.</span><span class="sxs-lookup"><span data-stu-id="094b0-123">We’ll be making a number of changes in the underlying database, and that takes a while.</span></span>
7.  <span data-ttu-id="094b0-124">When the system is ready again, choose the **Create New Company** button.</span><span class="sxs-lookup"><span data-stu-id="094b0-124">When the system is ready again, choose the **Create New Company** button.</span></span>  
8.  <span data-ttu-id="094b0-125">In the dialogue that appears, specify the name as *My Company*, and choose the **Production – Setup Data Only** option.</span><span class="sxs-lookup"><span data-stu-id="094b0-125">In the dialog that appears, specify the name as *My Company*, and choose the **Production – Setup Data Only** option.</span></span>  

<span data-ttu-id="094b0-126">This again takes a number of minutes.</span><span class="sxs-lookup"><span data-stu-id="094b0-126">This again takes a number of minutes.</span></span> <span data-ttu-id="094b0-127">When the process completes, you will be able to access Invoicing as part of your Office 365 Business Premium experience.</span><span class="sxs-lookup"><span data-stu-id="094b0-127">When the process completes, you will be able to access Invoicing as part of your Office 365 Business Premium experience.</span></span>  

### <a name="what-about-my-data"></a><span data-ttu-id="094b0-128">What about my data?</span><span class="sxs-lookup"><span data-stu-id="094b0-128">What about my data?</span></span>
<span data-ttu-id="094b0-129">When you rename the original My Company, the database tables that store your existing [!INCLUDE[d365fin](includes/d365fin_md.md)] data are renamed, but the data itself is not touched.</span><span class="sxs-lookup"><span data-stu-id="094b0-129">When you rename the original My Company, the database tables that store your existing [!INCLUDE[d365fin](includes/d365fin_md.md)] data are renamed, but the data itself is not touched.</span></span>  

<span data-ttu-id="094b0-130">If you use both Invoicing and [!INCLUDE[d365fin](includes/d365fin_md.md)], the data is stored in two different containers (the two companies).</span><span class="sxs-lookup"><span data-stu-id="094b0-130">If you use both Invoicing and [!INCLUDE[d365fin](includes/d365fin_md.md)], the data is stored in two different containers (the two companies).</span></span> <span data-ttu-id="094b0-131">Nothing is shared, so you'll have to manage customers and items in both companies.</span><span class="sxs-lookup"><span data-stu-id="094b0-131">Nothing is shared, so you'll have to manage customers and items in both companies.</span></span>  

## <a name="see-also"></a><span data-ttu-id="094b0-132">See Also</span><span class="sxs-lookup"><span data-stu-id="094b0-132">See Also</span></span>
[<span data-ttu-id="094b0-133">Frequently Asked Questions</span><span class="sxs-lookup"><span data-stu-id="094b0-133">Frequently Asked Questions</span></span>](across-faq.md)  
[<span data-ttu-id="094b0-134">Administration</span><span class="sxs-lookup"><span data-stu-id="094b0-134">Administration</span></span>](admin-setup-and-administration.md)  
