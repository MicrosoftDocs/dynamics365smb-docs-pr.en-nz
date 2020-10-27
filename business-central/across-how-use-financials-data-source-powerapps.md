---
title: Use Your Data to Create an App| Microsoft Docs
description: You can make your Business Central data available as a data source and specify an OData URL of your web services to build a business app using Power Apps.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: OData, Power App, SOAP
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 718d4378a897b187ba3073449869184fef5cec98
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 10/01/2020
ms.locfileid: "3924844"
---
# <a name="connecting-to-your-business-central-data-to-build-a-business-app-using-power-apps"></a><span data-ttu-id="17d41-103">Connecting to Your Business Central Data to Build a Business App Using Power Apps</span><span class="sxs-lookup"><span data-stu-id="17d41-103">Connecting to Your Business Central Data to Build a Business App Using Power Apps</span></span>

<span data-ttu-id="17d41-104">You can make your [!INCLUDE[prodshort](includes/prodshort.md)] data available as a data source in Power Apps.</span><span class="sxs-lookup"><span data-stu-id="17d41-104">You can make your [!INCLUDE[prodshort](includes/prodshort.md)] data available as a data source in Power Apps.</span></span>  

> [!NOTE]  
> <span data-ttu-id="17d41-105">You must have a valid account with [!INCLUDE[prodshort](includes/prodshort.md)] and with Power Apps.</span><span class="sxs-lookup"><span data-stu-id="17d41-105">You must have a valid account with [!INCLUDE[prodshort](includes/prodshort.md)] and with Power Apps.</span></span>  

## <a name="to-add-prodshort-as-a-data-source-in-power-apps"></a><span data-ttu-id="17d41-106">To add [!INCLUDE[prodshort](includes/prodshort.md)] as a data source in Power Apps</span><span class="sxs-lookup"><span data-stu-id="17d41-106">To add [!INCLUDE[prodshort](includes/prodshort.md)] as a data source in Power Apps</span></span>

1. <span data-ttu-id="17d41-107">In your browser, navigate to [powerapps.microsoft.com](https://powerapps.microsoft.com/), and then sign in.</span><span class="sxs-lookup"><span data-stu-id="17d41-107">In your browser, navigate to [powerapps.microsoft.com](https://powerapps.microsoft.com/), and then sign in.</span></span>
2. <span data-ttu-id="17d41-108">On the Home page, in the **Start from data** section, choose the **Other data sources** tile.</span><span class="sxs-lookup"><span data-stu-id="17d41-108">On the Home page, in the **Start from data** section, choose the **Other data sources** tile.</span></span>  

    <span data-ttu-id="17d41-109">This opens Power Apps Studio.</span><span class="sxs-lookup"><span data-stu-id="17d41-109">This opens Power Apps Studio.</span></span> <span data-ttu-id="17d41-110">On first login, you must specify the country/region.</span><span class="sxs-lookup"><span data-stu-id="17d41-110">On first login, you must specify the country/region.</span></span>  
3. <span data-ttu-id="17d41-111">In the list of available connections, choose **Business Central** , and then choose the **Create** button.</span><span class="sxs-lookup"><span data-stu-id="17d41-111">In the list of available connections, choose **Business Central** , and then choose the **Create** button.</span></span>

    <span data-ttu-id="17d41-112">Power Apps will connect to your [!INCLUDE[prodshort](includes/prodshort.md)] using the credentials that you are signed in with.</span><span class="sxs-lookup"><span data-stu-id="17d41-112">Power Apps will connect to your [!INCLUDE[prodshort](includes/prodshort.md)] using the credentials that you are signed in with.</span></span> <span data-ttu-id="17d41-113">If you are not an administrator of your [!INCLUDE[prodshort](includes/prodshort.md)], you may have to sign in with another account.</span><span class="sxs-lookup"><span data-stu-id="17d41-113">If you are not an administrator of your [!INCLUDE[prodshort](includes/prodshort.md)], you may have to sign in with another account.</span></span>  

4. <span data-ttu-id="17d41-114">Power Apps will display a list of *Environments and companies* that are available from [!INCLUDE[prodshort](includes/prodshort.md)].</span><span class="sxs-lookup"><span data-stu-id="17d41-114">Power Apps will display a list of *Environments and companies* that are available from [!INCLUDE[prodshort](includes/prodshort.md)].</span></span> <span data-ttu-id="17d41-115">Choose the environment and company that contains the data you want to connect to, such as *PRODUCTION - My Company* .</span><span class="sxs-lookup"><span data-stu-id="17d41-115">Choose the environment and company that contains the data you want to connect to, such as *PRODUCTION - My Company* .</span></span>  

5. <span data-ttu-id="17d41-116">Next, you will be presented with a list of tables that are exposed as part of the API for your environment.</span><span class="sxs-lookup"><span data-stu-id="17d41-116">Next, you will be presented with a list of tables that are exposed as part of the API for your environment.</span></span> <span data-ttu-id="17d41-117">Select the table that you want to connect to, and then choose **Connect** .</span><span class="sxs-lookup"><span data-stu-id="17d41-117">Select the table that you want to connect to, and then choose **Connect** .</span></span>

<span data-ttu-id="17d41-118">These so-called tables are exposed as endpoints by the [!INCLUDE[prodshort](includes/prodshort.md)] connector for Power Apps.</span><span class="sxs-lookup"><span data-stu-id="17d41-118">These so-called tables are exposed as endpoints by the [!INCLUDE[prodshort](includes/prodshort.md)] connector for Power Apps.</span></span>  

> [!NOTE]
> <span data-ttu-id="17d41-119">If you want to include data from other tables in [!INCLUDE[prodshort](includes/prodshort.md)] in your app, then you must work with a developer to define a custom API in [!INCLUDE[prodshort](includes/prodshort.md)] and then consume that custom API through a custom connector in Power Apps.</span><span class="sxs-lookup"><span data-stu-id="17d41-119">If you want to include data from other tables in [!INCLUDE[prodshort](includes/prodshort.md)] in your app, then you must work with a developer to define a custom API in [!INCLUDE[prodshort](includes/prodshort.md)] and then consume that custom API through a custom connector in Power Apps.</span></span> <span data-ttu-id="17d41-120">For more information, see [Create a custom connector from scratch](/connectors/custom-connectors/define-blank).</span><span class="sxs-lookup"><span data-stu-id="17d41-120">For more information, see [Create a custom connector from scratch](/connectors/custom-connectors/define-blank).</span></span>  

<span data-ttu-id="17d41-121">At this point, you have successfully connected to your [!INCLUDE[prodshort](includes/prodshort.md)] data and are ready to begin building your PowerApp.</span><span class="sxs-lookup"><span data-stu-id="17d41-121">At this point, you have successfully connected to your [!INCLUDE[prodshort](includes/prodshort.md)] data and are ready to begin building your PowerApp.</span></span> <span data-ttu-id="17d41-122">You can add additional screens and connect to additional data from your [!INCLUDE[prodshort](includes/prodshort.md)].</span><span class="sxs-lookup"><span data-stu-id="17d41-122">You can add additional screens and connect to additional data from your [!INCLUDE[prodshort](includes/prodshort.md)].</span></span> <span data-ttu-id="17d41-123">For more information, see [Create a canvas app from a sample in Power Apps](/powerapps/maker/canvas-apps/open-and-run-a-sample-app).</span><span class="sxs-lookup"><span data-stu-id="17d41-123">For more information, see [Create a canvas app from a sample in Power Apps](/powerapps/maker/canvas-apps/open-and-run-a-sample-app).</span></span>  

<span data-ttu-id="17d41-124">When you have designed and built your app, you can share it with your colleagues.</span><span class="sxs-lookup"><span data-stu-id="17d41-124">When you have designed and built your app, you can share it with your colleagues.</span></span> <span data-ttu-id="17d41-125">For more information, see [Save and publish a canvas app in Power Apps](/powerapps/maker/canvas-apps/save-publish-app).</span><span class="sxs-lookup"><span data-stu-id="17d41-125">For more information, see [Save and publish a canvas app in Power Apps](/powerapps/maker/canvas-apps/save-publish-app).</span></span>  

> [!NOTE]
> <span data-ttu-id="17d41-126">If you want to connect to [!INCLUDE[prodshort](includes/prodshort.md)] on-premises, then you must choose the **Business Central (on-premises)** connector in step 3.</span><span class="sxs-lookup"><span data-stu-id="17d41-126">If you want to connect to [!INCLUDE[prodshort](includes/prodshort.md)] on-premises, then you must choose the **Business Central (on-premises)** connector in step 3.</span></span>  

## <a name="see-also"></a><span data-ttu-id="17d41-127">See Also</span><span class="sxs-lookup"><span data-stu-id="17d41-127">See Also</span></span>

[<span data-ttu-id="17d41-128">Create a canvas app from a template in Power Apps</span><span class="sxs-lookup"><span data-stu-id="17d41-128">Create a canvas app from a template in Power Apps</span></span>](/powerapps/maker/canvas-apps/get-started-test-drive)  
[<span data-ttu-id="17d41-129">Importing Business Data from Other Finance Systems</span><span class="sxs-lookup"><span data-stu-id="17d41-129">Importing Business Data from Other Finance Systems</span></span>](across-import-data-configuration-packages.md)  
<span data-ttu-id="17d41-130">[Setting Up [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)</span><span class="sxs-lookup"><span data-stu-id="17d41-130">[Setting Up [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)</span></span>  
[<span data-ttu-id="17d41-131">Getting Started Developing Connect Apps for Dynamics 365 Business Central</span><span class="sxs-lookup"><span data-stu-id="17d41-131">Getting Started Developing Connect Apps for Dynamics 365 Business Central</span></span>](/dynamics365/business-central/dev-itpro/developer/devenv-develop-connect-apps)  
