---
title: 'Troubleshooting: Accessing Camera and Location'
description: This article describes how to troubleshoot access to camera and location information in Business Central.
author: blrobl
ms.author: t-blrobl
ms.date: 04/22/2020
ms.custom: na
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.service: dynamics365-business-central
ms.openlocfilehash: 10338040ddcfb64dd91e9e55f607280e99720403
ms.sourcegitcommit: a80afd4e5075018716efad76d82a54e158f1392d
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 09/09/2020
ms.locfileid: "3781151"
---
# <a name="troubleshooting-accessing-camera-and-location"></a><span data-ttu-id="b4c65-103">Troubleshooting: Accessing Camera and Location</span><span class="sxs-lookup"><span data-stu-id="b4c65-103">Troubleshooting: Accessing Camera and Location</span></span>

<span data-ttu-id="b4c65-104">You might come across some issues when trying to access the camera and location information of a device from [!INCLUDE[prodshort](includes/prodshort.md)].</span><span class="sxs-lookup"><span data-stu-id="b4c65-104">You might come across some issues when trying to access the camera and location information of a device from [!INCLUDE[prodshort](includes/prodshort.md)].</span></span> <span data-ttu-id="b4c65-105">You can find the possible causes behind these problems and how to work around them listed below.</span><span class="sxs-lookup"><span data-stu-id="b4c65-105">You can find the possible causes behind these problems and how to work around them listed below.</span></span>

## <a name="device-must-have-camera-and-location-capabilities"></a><span data-ttu-id="b4c65-106">Device must have Camera and Location Capabilities</span><span class="sxs-lookup"><span data-stu-id="b4c65-106">Device must have Camera and Location Capabilities</span></span>

<span data-ttu-id="b4c65-107">In order to access the camera or a user's location from a device, the device must have a physical camera or the capability to retrieve location information, respectively.</span><span class="sxs-lookup"><span data-stu-id="b4c65-107">In order to access the camera or a user's location from a device, the device must have a physical camera or the capability to retrieve location information, respectively.</span></span>

<span data-ttu-id="b4c65-108">If your device has camera and location capabilities but you still encounter problems, it is possible that some drivers need updating or reinstalling.</span><span class="sxs-lookup"><span data-stu-id="b4c65-108">If your device has camera and location capabilities but you still encounter problems, it is possible that some drivers need updating or reinstalling.</span></span> <span data-ttu-id="b4c65-109">Even if you are unsure, we always recommend you update your device operating system, drivers, and browser to the latest version for the best experience.</span><span class="sxs-lookup"><span data-stu-id="b4c65-109">Even if you are unsure, we always recommend you update your device operating system, drivers, and browser to the latest version for the best experience.</span></span>

## <a name="access-permissions-not-enabled"></a><span data-ttu-id="b4c65-110">Access Permissions not Enabled</span><span class="sxs-lookup"><span data-stu-id="b4c65-110">Access Permissions not Enabled</span></span>

<span data-ttu-id="b4c65-111">You must enable general access to camera and location from your device's privacy settings and explicitly give permission to  [!INCLUDE[prodshort](includes/prodshort.md)] to access them.</span><span class="sxs-lookup"><span data-stu-id="b4c65-111">You must enable general access to camera and location from your device's privacy settings and explicitly give permission to  [!INCLUDE[prodshort](includes/prodshort.md)] to access them.</span></span> <span data-ttu-id="b4c65-112">For example, to see or change permissions for a device running on Windows, go to **Settings**, choose **Privacy**, and then **App permissions**.</span><span class="sxs-lookup"><span data-stu-id="b4c65-112">For example, to see or change permissions for a device running on Windows, go to **Settings**, choose **Privacy**, and then **App permissions**.</span></span> 

<span data-ttu-id="b4c65-113">For mobile devices, you must give camera and location access permissions to the [!INCLUDE[prodshort](includes/prodshort.md)] Mobile App.</span><span class="sxs-lookup"><span data-stu-id="b4c65-113">For mobile devices, you must give camera and location access permissions to the [!INCLUDE[prodshort](includes/prodshort.md)] Mobile App.</span></span> <span data-ttu-id="b4c65-114">To do so for an iOS device, go to **Settings**, choose **Privacy**, and then **Camera** or **Location**.</span><span class="sxs-lookup"><span data-stu-id="b4c65-114">To do so for an iOS device, go to **Settings**, choose **Privacy**, and then **Camera** or **Location**.</span></span> <span data-ttu-id="b4c65-115">For Android devices go to **Settings**, choose **Apps & Notifications**, **Advanced**, **Permission Manager**, and then **Camera** or **Location**.</span><span class="sxs-lookup"><span data-stu-id="b4c65-115">For Android devices go to **Settings**, choose **Apps & Notifications**, **Advanced**, **Permission Manager**, and then **Camera** or **Location**.</span></span>

<span data-ttu-id="b4c65-116">In addition, if you are using [!INCLUDE[prodshort](includes/prodshort.md)] in a browser, you must also grant the [!INCLUDE[prodshort](includes/prodshort.md)] site permission to access the camera or location information.</span><span class="sxs-lookup"><span data-stu-id="b4c65-116">In addition, if you are using [!INCLUDE[prodshort](includes/prodshort.md)] in a browser, you must also grant the [!INCLUDE[prodshort](includes/prodshort.md)] site permission to access the camera or location information.</span></span> <span data-ttu-id="b4c65-117">To see or change a site's permissions in the Microsoft Edge browser, go to **Settings**, choose **Site Permissions**, and then **Camera** or **Location**.</span><span class="sxs-lookup"><span data-stu-id="b4c65-117">To see or change a site's permissions in the Microsoft Edge browser, go to **Settings**, choose **Site Permissions**, and then **Camera** or **Location**.</span></span> <span data-ttu-id="b4c65-118">Note that this might be different for other browsers.</span><span class="sxs-lookup"><span data-stu-id="b4c65-118">Note that this might be different for other browsers.</span></span>

<span data-ttu-id="b4c65-119">By default, the device or browser will pop up a request to access these capabilities when the user activates them for the first time.</span><span class="sxs-lookup"><span data-stu-id="b4c65-119">By default, the device or browser will pop up a request to access these capabilities when the user activates them for the first time.</span></span>

> [!NOTE]  
> <span data-ttu-id="b4c65-120">Some old browsers do not grant access to camera and location.</span><span class="sxs-lookup"><span data-stu-id="b4c65-120">Some old browsers do not grant access to camera and location.</span></span> <span data-ttu-id="b4c65-121">For example, camera is not available in Internet Explorer or the legacy Edge browser.</span><span class="sxs-lookup"><span data-stu-id="b4c65-121">For example, camera is not available in Internet Explorer or the legacy Edge browser.</span></span>

## <a name="web-client-connection-not-secure"></a><span data-ttu-id="b4c65-122">Web Client Connection not Secure</span><span class="sxs-lookup"><span data-stu-id="b4c65-122">Web Client Connection not Secure</span></span>

<span data-ttu-id="b4c65-123">The camera and location capabilities are only available when accessing the Web Client through SSL secured HTTP connections, using the `https://` URI scheme.</span><span class="sxs-lookup"><span data-stu-id="b4c65-123">The camera and location capabilities are only available when accessing the Web Client through SSL secured HTTP connections, using the `https://` URI scheme.</span></span> 

<span data-ttu-id="b4c65-124">The only exception is connecting to `http://localhost`, used for development and test purposes.</span><span class="sxs-lookup"><span data-stu-id="b4c65-124">The only exception is connecting to `http://localhost`, used for development and test purposes.</span></span>


## <a name="working-with-virtualization-technologies"></a><span data-ttu-id="b4c65-125">Working with Virtualization Technologies</span><span class="sxs-lookup"><span data-stu-id="b4c65-125">Working with Virtualization Technologies</span></span>

<span data-ttu-id="b4c65-126">When connecting to [!INCLUDE[prodshort](includes/prodshort.md)] through Remote Desktop or another virtualization, the access to camera or location might not be available.</span><span class="sxs-lookup"><span data-stu-id="b4c65-126">When connecting to [!INCLUDE[prodshort](includes/prodshort.md)] through Remote Desktop or another virtualization, the access to camera or location might not be available.</span></span> <span data-ttu-id="b4c65-127">If this is the case, use the physical system instead.</span><span class="sxs-lookup"><span data-stu-id="b4c65-127">If this is the case, use the physical system instead.</span></span>

## <a name="antivirus-software"></a><span data-ttu-id="b4c65-128">Antivirus Software</span><span class="sxs-lookup"><span data-stu-id="b4c65-128">Antivirus Software</span></span>
<span data-ttu-id="b4c65-129">Some antivirus software block access to camera and location by default.</span><span class="sxs-lookup"><span data-stu-id="b4c65-129">Some antivirus software block access to camera and location by default.</span></span> <span data-ttu-id="b4c65-130">Remember to check your antivirus software settings.</span><span class="sxs-lookup"><span data-stu-id="b4c65-130">Remember to check your antivirus software settings.</span></span>

## <a name="see-also"></a><span data-ttu-id="b4c65-131">See Also</span><span class="sxs-lookup"><span data-stu-id="b4c65-131">See Also</span></span>
[<span data-ttu-id="b4c65-132">Implementing the Camera in AL</span><span class="sxs-lookup"><span data-stu-id="b4c65-132">Implementing the Camera in AL</span></span>](/dynamics365/business-central/dev-itpro/developer/devenv-implement-camera-al)  
[<span data-ttu-id="b4c65-133">Implementing the Location in AL</span><span class="sxs-lookup"><span data-stu-id="b4c65-133">Implementing the Location in AL</span></span>](/dynamics365/business-central/dev-itpro/developer/devenv-implement-location-al)
