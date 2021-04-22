---
title: Setting Up Your Browser
description: Describes how to set up browsers to work with Business Central and products that integrate with it.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: Teams, web client, troubleshooting, errors
ms.date: 04/01/2021
ms.author: jswymer
ms.openlocfilehash: 90625ed6d5664efc9605aeacbc66d8174e55799d
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 03/31/2021
ms.locfileid: "5776313"
---
# <a name="setting-up-and-troubleshooting-your-browser-to-work-with-business-central-web-client"></a><span data-ttu-id="11f28-103">Setting Up and Troubleshooting Your Browser to Work With Business Central Web Client</span><span class="sxs-lookup"><span data-stu-id="11f28-103">Setting Up and Troubleshooting Your Browser to Work With Business Central Web Client</span></span>

<span data-ttu-id="11f28-104">This article explains how to set up your browser so that the [!INCLUDE[web_client](includes/web_client.md)] and all its features work properly.</span><span class="sxs-lookup"><span data-stu-id="11f28-104">This article explains how to set up your browser so that the [!INCLUDE[web_client](includes/web_client.md)] and all its features work properly.</span></span> <span data-ttu-id="11f28-105">Read this article if you're having problems opening the [!INCLUDE[web_client](includes/web_client.md)], because some problems may be caused by your browser's settings.</span><span class="sxs-lookup"><span data-stu-id="11f28-105">Read this article if you're having problems opening the [!INCLUDE[web_client](includes/web_client.md)], because some problems may be caused by your browser's settings.</span></span>

<span data-ttu-id="11f28-106">The article provides details for setting up Microsoft Edge, but the requirements for JavaScript, cookies, and pop-ups are the same for all supported browsers.</span><span class="sxs-lookup"><span data-stu-id="11f28-106">The article provides details for setting up Microsoft Edge, but the requirements for JavaScript, cookies, and pop-ups are the same for all supported browsers.</span></span> <span data-ttu-id="11f28-107">For other browsers, refer to the instructions provided by the manufacturer.</span><span class="sxs-lookup"><span data-stu-id="11f28-107">For other browsers, refer to the instructions provided by the manufacturer.</span></span>  

## <a name="use-a-supported-browser"></a><span data-ttu-id="11f28-108">Use a supported browser</span><span class="sxs-lookup"><span data-stu-id="11f28-108">Use a supported browser</span></span>

<span data-ttu-id="11f28-109">Make sure to use a one of the supported browsers.</span><span class="sxs-lookup"><span data-stu-id="11f28-109">Make sure to use a one of the supported browsers.</span></span> <span data-ttu-id="11f28-110">See [Minimum Requirements for Using Business Central](product-requirements.md#browsers).</span><span class="sxs-lookup"><span data-stu-id="11f28-110">See [Minimum Requirements for Using Business Central](product-requirements.md#browsers).</span></span>  

## <a name="allow-javascript-from-business-central"></a><span data-ttu-id="11f28-111">Allow JavaScript from Business Central</span><span class="sxs-lookup"><span data-stu-id="11f28-111">Allow JavaScript from Business Central</span></span>

<span data-ttu-id="11f28-112">*Problem:*</span><span class="sxs-lookup"><span data-stu-id="11f28-112">*Problem:*</span></span>

<span data-ttu-id="11f28-113">If the browser doesn't allow JavaScript, you'll see **NotSupported/DisabledJavaScript** in the address bar and an **HTTP Error 404.0 - Not Found** message when you try to open [!INCLUDE[prod_short](includes/prod_short.md)], and the</span><span class="sxs-lookup"><span data-stu-id="11f28-113">If the browser doesn't allow JavaScript, you'll see **NotSupported/DisabledJavaScript** in the address bar and an **HTTP Error 404.0 - Not Found** message when you try to open [!INCLUDE[prod_short](includes/prod_short.md)], and the</span></span> 

<!-- http://localhost:8080/NotSupported/DisabledJavaScript HTTP Error 404.0 - Not Found
The resource you are looking for has been removed, had its name changed, or is temporarily unavailable. -->

<span data-ttu-id="11f28-114">*Fix:*</span><span class="sxs-lookup"><span data-stu-id="11f28-114">*Fix:*</span></span>

1. <span data-ttu-id="11f28-115">In Microsoft Edge, go to **Settings** > **Cookies and site permissions** > **JavaScript**.</span><span class="sxs-lookup"><span data-stu-id="11f28-115">In Microsoft Edge, go to **Settings** > **Cookies and site permissions** > **JavaScript**.</span></span>
2. <span data-ttu-id="11f28-116">Do one of the following steps.</span><span class="sxs-lookup"><span data-stu-id="11f28-116">Do one of the following steps.</span></span> <span data-ttu-id="11f28-117">Choose the step that is recommended by your organisation:</span><span class="sxs-lookup"><span data-stu-id="11f28-117">Choose the step that is recommended by your organization:</span></span>

    - <span data-ttu-id="11f28-118">Move the **Allowed** toggle to the left (Off).</span><span class="sxs-lookup"><span data-stu-id="11f28-118">Move the **Allowed** toggle to the left (Off).</span></span> <span data-ttu-id="11f28-119">Then, select **Add** and type the address (URL) for [!INCLUDE[prod_short](includes/prod_short.md)] in the **Site** box.</span><span class="sxs-lookup"><span data-stu-id="11f28-119">Then, select **Add** and type the address (URL) for [!INCLUDE[prod_short](includes/prod_short.md)] in the **Site** box.</span></span> <span data-ttu-id="11f28-120">Select **Add** when done.</span><span class="sxs-lookup"><span data-stu-id="11f28-120">Select **Add** when done.</span></span>
    - <span data-ttu-id="11f28-121">Move the **Allowed** toggle to the right (On).</span><span class="sxs-lookup"><span data-stu-id="11f28-121">Move the **Allowed** toggle to the right (On).</span></span>

## <a name="allow-cookies-from-business-central"></a><span data-ttu-id="11f28-122">Allow cookies from Business Central</span><span class="sxs-lookup"><span data-stu-id="11f28-122">Allow cookies from Business Central</span></span>

<span data-ttu-id="11f28-123">*Problem:*</span><span class="sxs-lookup"><span data-stu-id="11f28-123">*Problem:*</span></span>

<span data-ttu-id="11f28-124">If the browser doesn't allow cookies, you'll get the following error:</span><span class="sxs-lookup"><span data-stu-id="11f28-124">If the browser doesn't allow cookies, you'll get the following error:</span></span>

<span data-ttu-id="11f28-125">**Sorry, the page could not be found. Please check the address and try again.**</span><span class="sxs-lookup"><span data-stu-id="11f28-125">**Sorry, the page could not be found. Please check the address and try again.**</span></span> 

<span data-ttu-id="11f28-126">*Fix:*</span><span class="sxs-lookup"><span data-stu-id="11f28-126">*Fix:*</span></span>

1. <span data-ttu-id="11f28-127">In Microsoft Edge, go to **Settings** > **Cookies and site permissions** > **Cookies and site data**.</span><span class="sxs-lookup"><span data-stu-id="11f28-127">In Microsoft Edge, go to **Settings** > **Cookies and site permissions** > **Cookies and site data**.</span></span>
2. <span data-ttu-id="11f28-128">Move the **Allow sites to save and read cookie data** toggle to the right (On).</span><span class="sxs-lookup"><span data-stu-id="11f28-128">Move the **Allow sites to save and read cookie data** toggle to the right (On).</span></span>  

## <a name="allow-pop-ups-from-business-central"></a><a name="popup"></a><span data-ttu-id="11f28-129">Allow pop-ups from Business Central</span><span class="sxs-lookup"><span data-stu-id="11f28-129">Allow pop-ups from Business Central</span></span>

[!INCLUDE[prod_short](includes/prod_short.md)] <span data-ttu-id="11f28-130">integrates with several products.</span><span class="sxs-lookup"><span data-stu-id="11f28-130">integrates with several products.</span></span> <span data-ttu-id="11f28-131">In some cases, like with Microsoft Teams, [!INCLUDE[prod_short](includes/prod_short.md)] opens, or "pop-ups", within the product.</span><span class="sxs-lookup"><span data-stu-id="11f28-131">In some cases, like with Microsoft Teams, [!INCLUDE[prod_short](includes/prod_short.md)] opens, or "pop-ups", within the product.</span></span> <span data-ttu-id="11f28-132">This capability requires that your browser allows pop-ups from [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="11f28-132">This capability requires that your browser allows pop-ups from [!INCLUDE[prod_short](includes/prod_short.md)].</span></span>

<span data-ttu-id="11f28-133">*Problem:*</span><span class="sxs-lookup"><span data-stu-id="11f28-133">*Problem:*</span></span>

<span data-ttu-id="11f28-134">If pop-ups for [!INCLUDE[prod_short](includes/prod_short.md)] are being blocked, you get a message similar to the following message:</span><span class="sxs-lookup"><span data-stu-id="11f28-134">If pop-ups for [!INCLUDE[prod_short](includes/prod_short.md)] are being blocked, you get a message similar to the following message:</span></span>

<span data-ttu-id="11f28-135">**Something went wrong. Your browser may be blocking pop-ups needed by Business Central.**</span><span class="sxs-lookup"><span data-stu-id="11f28-135">**Something went wrong. Your browser may be blocking pop-ups needed by Business Central.**</span></span>

<!--
Something went wrong
Your browser may be blocking pop-ups needed by Business Central.

Change your browser settings to allow pop-ups or allow this for trusted domains, then try again.
If these settings are managed for your organization, you should contact your administrator for assistance.

Try again
-->
<span data-ttu-id="11f28-136">*Fix:*</span><span class="sxs-lookup"><span data-stu-id="11f28-136">*Fix:*</span></span>

1. <span data-ttu-id="11f28-137">In Microsoft Edge, go to **Settings** > **Cookies and site permissions** > **Pop-ups and redirects**.</span><span class="sxs-lookup"><span data-stu-id="11f28-137">In Microsoft Edge, go to **Settings** > **Cookies and site permissions** > **Pop-ups and redirects**.</span></span>
2. <span data-ttu-id="11f28-138">Move the **Blocked** toggle to the right (On).</span><span class="sxs-lookup"><span data-stu-id="11f28-138">Move the **Blocked** toggle to the right (On).</span></span>
3. <span data-ttu-id="11f28-139">Select **Add**.</span><span class="sxs-lookup"><span data-stu-id="11f28-139">Select **Add**.</span></span> <span data-ttu-id="11f28-140">In the **Site** box, type `https://businesscentral.dynamics.com`, then select **Add**.</span><span class="sxs-lookup"><span data-stu-id="11f28-140">In the **Site** box, type `https://businesscentral.dynamics.com`, then select **Add**.</span></span>

## <a name="see-also"></a><span data-ttu-id="11f28-141">See Also</span><span class="sxs-lookup"><span data-stu-id="11f28-141">See Also</span></span>

[<span data-ttu-id="11f28-142">Troubleshooting Teams</span><span class="sxs-lookup"><span data-stu-id="11f28-142">Troubleshooting Teams</span></span>](admin-teams-troubleshooting.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]