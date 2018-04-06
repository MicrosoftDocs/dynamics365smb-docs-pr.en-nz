---
title: Use Your Data to Create an App| Microsoft Docs
description: You can make your Financials data available as a data source and specify an OData URL of your web services to build a business app using PowerApps.
services: project-madeira
documentationcenter: 
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: Odata, Power App, SOAP
ms.date: 06/02/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 8db67d30ba18e9f7dba14b93ddf7b4de6e2b6444
ms.contentlocale: en-nz
ms.lasthandoff: 03/22/2018

---
# <a name="connecting-to-your-financials-data-to-build-a-business-app-using-powerapps"></a><span data-ttu-id="da017-103">Connecting to Your Financials Data to Build a Business App Using PowerApps</span><span class="sxs-lookup"><span data-stu-id="da017-103">Connecting to Your Financials Data to Build a Business App Using PowerApps</span></span>
<span data-ttu-id="da017-104">You can make your [!INCLUDE[d365fin](includes/d365fin_md.md)] data available as a data source in PowerApps.</span><span class="sxs-lookup"><span data-stu-id="da017-104">You can make your [!INCLUDE[d365fin](includes/d365fin_md.md)] data available as a data source in PowerApps.</span></span>  

> [!NOTE]  
>   <span data-ttu-id="da017-105">You must have a valid account with [!INCLUDE[d365fin](includes/d365fin_md.md)] and with PowerApps.</span><span class="sxs-lookup"><span data-stu-id="da017-105">You must have a valid account with [!INCLUDE[d365fin](includes/d365fin_md.md)] and with PowerApps.</span></span>  

## <a name="to-add-included365finincludesd365finmdmd-as-a-data-source-in-powerapps"></a><span data-ttu-id="da017-106">To add [!INCLUDE[d365fin](includes/d365fin_md.md)] as a data source in PowerApps</span><span class="sxs-lookup"><span data-stu-id="da017-106">To add [!INCLUDE[d365fin](includes/d365fin_md.md)] as a data source in PowerApps</span></span>
1. <span data-ttu-id="da017-107">In your browser, navigate to [powerapps.microsoft.com](https://powerapps.microsoft.com/en-us/), and then sign in.</span><span class="sxs-lookup"><span data-stu-id="da017-107">In your browser, navigate to [powerapps.microsoft.com](https://powerapps.microsoft.com/en-us/), and then sign in.</span></span>
2. <span data-ttu-id="da017-108">In the left navigation pane, choose **New App**.</span><span class="sxs-lookup"><span data-stu-id="da017-108">In the left navigation pane, choose **New App**.</span></span>
3. <span data-ttu-id="da017-109">Choose your editor, PowerApps Studio for Windows or PowerApps Studio for Web.</span><span class="sxs-lookup"><span data-stu-id="da017-109">Choose your editor, PowerApps Studio for Windows or PowerApps Studio for Web.</span></span>

   <span data-ttu-id="da017-110">PowerApps Studio for Windows is a desktop application used to create and publish PowerApps.</span><span class="sxs-lookup"><span data-stu-id="da017-110">PowerApps Studio for Windows is a desktop application used to create and publish PowerApps.</span></span> <span data-ttu-id="da017-111">The PowerApps Studio for Web is the online solution used to create and publish PowerApps.</span><span class="sxs-lookup"><span data-stu-id="da017-111">The PowerApps Studio for Web is the online solution used to create and publish PowerApps.</span></span>
4. <span data-ttu-id="da017-112">The next step to create a PowerApp is to select your data.</span><span class="sxs-lookup"><span data-stu-id="da017-112">The next step to create a PowerApp is to select your data.</span></span> <span data-ttu-id="da017-113">Choose the Arrow icon then choose the **New connection** option in the upper left side of the page.</span><span class="sxs-lookup"><span data-stu-id="da017-113">Choose the Arrow icon then choose the **New connection** option in the upper left side of the page.</span></span>
5. <span data-ttu-id="da017-114">In the list of available connections, choose **Dynamics 365 Business Central**.</span><span class="sxs-lookup"><span data-stu-id="da017-114">In the list of available connections, choose **Dynamics 365 Business Central**.</span></span>
6. <span data-ttu-id="da017-115">PowerApps will display a connection page that prompts you for the information that is required to connect to your [!INCLUDE[d365fin](includes/d365fin_md.md)] data.</span><span class="sxs-lookup"><span data-stu-id="da017-115">PowerApps will display a connection page that prompts you for the information that is required to connect to your [!INCLUDE[d365fin](includes/d365fin_md.md)] data.</span></span> <span data-ttu-id="da017-116">To connect, you must specify an OData URL, username, password, and company name.</span><span class="sxs-lookup"><span data-stu-id="da017-116">To connect, you must specify an OData URL, username, password, and company name.</span></span>

   <span data-ttu-id="da017-117">For the *OData URL*, you can copy the OData V4 URL of any of the web services that are listed in the **Web Services** page in [!INCLUDE[d365fin](includes/d365fin_md.md)], such as `https://mycompany.financials.dynamics.com:7048/MS/ODataV4/`.</span><span class="sxs-lookup"><span data-stu-id="da017-117">For the *OData URL*, you can copy the OData V4 URL of any of the web services that are listed in the **Web Services** page in [!INCLUDE[d365fin](includes/d365fin_md.md)], such as `https://mycompany.financials.dynamics.com:7048/MS/ODataV4/`.</span></span>  

   <span data-ttu-id="da017-118">For the *Company Name*, use the name that is shown in the **Name** field in the **Company Information** window in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="da017-118">For the *Company Name*, use the name that is shown in the **Name** field in the **Company Information** window in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="da017-119">If your [!INCLUDE[d365fin](includes/d365fin_md.md)] contains multiple companies, choose the relevant company name from the list in the **Companies** window.</span><span class="sxs-lookup"><span data-stu-id="da017-119">If your [!INCLUDE[d365fin](includes/d365fin_md.md)] contains multiple companies, choose the relevant company name from the list in the **Companies** window.</span></span> <span data-ttu-id="da017-120">In both cases, make sure that the name that you specify in the PowerApps wizard matches exactly the text shown in [!INCLUDE[d365fin](includes/d365fin_md.md)], such as `My Company`.</span><span class="sxs-lookup"><span data-stu-id="da017-120">In both cases, make sure that the name that you specify in the PowerApps wizard matches exactly the text shown in [!INCLUDE[d365fin](includes/d365fin_md.md)], such as `My Company`.</span></span>

   <span data-ttu-id="da017-121">For the username and password, use the name and web service access key that are specified for your account in the **Users** window in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="da017-121">For the username and password, use the name and web service access key that are specified for your account in the **Users** window in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="da017-122">For example, your username is *ADMIN*, and the web service access key that serves as your password is *EgzeUFQ9Uv0o5O0lUMyqCzo1ueUW9yRF3SsLU=*.</span><span class="sxs-lookup"><span data-stu-id="da017-122">For example, your username is *ADMIN*, and the web service access key that serves as your password is *EgzeUFQ9Uv0o5O0lUMyqCzo1ueUW9yRF3SsLU=*.</span></span>
7. <span data-ttu-id="da017-123">Choose the **Connection** button to continue.</span><span class="sxs-lookup"><span data-stu-id="da017-123">Choose the **Connection** button to continue.</span></span> <span data-ttu-id="da017-124">PowerApps will display a default dataset for [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="da017-124">PowerApps will display a default dataset for [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="da017-125">Choose the **Default** dataset.</span><span class="sxs-lookup"><span data-stu-id="da017-125">Choose the **Default** dataset.</span></span>

   <span data-ttu-id="da017-126">PowerApps will display a list of tables that are available from [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="da017-126">PowerApps will display a list of tables that are available from [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="da017-127">These tables, or end points,  represent all the web services you have published from [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="da017-127">These tables, or end points,  represent all the web services you have published from [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>

   <span data-ttu-id="da017-128">Alternatively, create a new web service URL in [!INCLUDE[d365fin](includes/d365fin_md.md)] by using the **Create Data Set** action in the **Web Services** page, using the **Set Up Reporting** Assisted Setup guide, or by choosing the **Edit in Excel** action in any lists.</span><span class="sxs-lookup"><span data-stu-id="da017-128">Alternatively, create a new web service URL in [!INCLUDE[d365fin](includes/d365fin_md.md)] by using the **Create Data Set** action in the **Web Services** page, using the **Set Up Reporting** Assisted Setup guide, or by choosing the **Edit in Excel** action in any lists.</span></span>
8. <span data-ttu-id="da017-129">Choose the table that you want to use for your PowerApp, and then choose the **Connect** button.</span><span class="sxs-lookup"><span data-stu-id="da017-129">Choose the table that you want to use for your PowerApp, and then choose the **Connect** button.</span></span>
9. <span data-ttu-id="da017-130">Repeat the previous steps to add additional [!INCLUDE[d365fin](includes/d365fin_md.md)] data to your Power BI data model.</span><span class="sxs-lookup"><span data-stu-id="da017-130">Repeat the previous steps to add additional [!INCLUDE[d365fin](includes/d365fin_md.md)] data to your Power BI data model.</span></span>

   > [!NOTE]  
>    <span data-ttu-id="da017-131">Once you have successfully connected to [!INCLUDE[d365fin](includes/d365fin_md.md)], you will not be prompted again for the OData URL, username, or password.</span><span class="sxs-lookup"><span data-stu-id="da017-131">Once you have successfully connected to [!INCLUDE[d365fin](includes/d365fin_md.md)], you will not be prompted again for the OData URL, username, or password.</span></span>

<span data-ttu-id="da017-132">At this point, you have successfully connected to your Business Central data and are ready to begin building your PowerApp.</span><span class="sxs-lookup"><span data-stu-id="da017-132">At this point, you have successfully connected to your Business Central data and are ready to begin building your PowerApp.</span></span> <span data-ttu-id="da017-133">For more information, see the [PowerApps documentation](https://powerapps.microsoft.com/tutorials/getting-started/).</span><span class="sxs-lookup"><span data-stu-id="da017-133">For more information, see the [PowerApps documentation](https://powerapps.microsoft.com/tutorials/getting-started/).</span></span>

## <a name="see-also"></a><span data-ttu-id="da017-134">See Also</span><span class="sxs-lookup"><span data-stu-id="da017-134">See Also</span></span>
<span data-ttu-id="da017-135">[Welcome to [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)</span><span class="sxs-lookup"><span data-stu-id="da017-135">[Welcome to [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)</span></span>  
[<span data-ttu-id="da017-136">Importing Business Data from Other Finance Systems</span><span class="sxs-lookup"><span data-stu-id="da017-136">Importing Business Data from Other Finance Systems</span></span>](upload-data.md)  
<span data-ttu-id="da017-137">[Setting Up [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)</span><span class="sxs-lookup"><span data-stu-id="da017-137">[Setting Up [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)</span></span>  
[<span data-ttu-id="da017-138">Finance</span><span class="sxs-lookup"><span data-stu-id="da017-138">Finance</span></span>](finance.md)  
