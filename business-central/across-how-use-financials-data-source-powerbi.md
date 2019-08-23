---
title: Use Business Central in Power BI reports | Microsoft Docs
description: Make your data available as a data source in Power BI and build powerful reports of the state of your business.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: business intelligence, KPI, Odata, Power App, SOAP, analysis
ms.date: 07/08/2019
ms.author: edupont
ms.openlocfilehash: c86f1c3c40f80ec993d0a3a89154047ddf9e8126
ms.sourcegitcommit: 519623f9a5134c9ffa97eeaed0841ae59835f453
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 07/16/2019
ms.locfileid: "1755257"
---
# <a name="using-include-prodlongincludesprodlongmd-as-power-bi-data-source-for-building-reports"></a><span data-ttu-id="584ea-103">Using [!INCLUDE [prodlong](includes/prodlong.md)] as Power BI Data Source for Building Reports</span><span class="sxs-lookup"><span data-stu-id="584ea-103">Using [!INCLUDE [prodlong](includes/prodlong.md)] as Power BI Data Source for Building Reports</span></span>

<span data-ttu-id="584ea-104">You can make your [!INCLUDE[prodlong](includes/prodlong.md)] data available as a data source in Power BI and build powerful reports of the state of your business.</span><span class="sxs-lookup"><span data-stu-id="584ea-104">You can make your [!INCLUDE[prodlong](includes/prodlong.md)] data available as a data source in Power BI and build powerful reports of the state of your business.</span></span>  

<span data-ttu-id="584ea-105">You must have a valid account with [!INCLUDE[prodshort](includes/prodshort.md)] and with Power BI.</span><span class="sxs-lookup"><span data-stu-id="584ea-105">You must have a valid account with [!INCLUDE[prodshort](includes/prodshort.md)] and with Power BI.</span></span> <span data-ttu-id="584ea-106">Also, you must download [Power BI Desktop](https://powerbi.microsoft.com/en-us/desktop/).</span><span class="sxs-lookup"><span data-stu-id="584ea-106">Also, you must download [Power BI Desktop](https://powerbi.microsoft.com/en-us/desktop/).</span></span> <span data-ttu-id="584ea-107">For more information, see [Quickstart: Connect to data in Power BI Desktop](/power-bi/desktop-quickstart-connect-to-data).</span><span class="sxs-lookup"><span data-stu-id="584ea-107">For more information, see [Quickstart: Connect to data in Power BI Desktop](/power-bi/desktop-quickstart-connect-to-data).</span></span>  

## <a name="to-add-includeprodshortincludesprodshortmd-as-a-data-source-in-power-bi-desktop"></a><span data-ttu-id="584ea-108">To add [!INCLUDE[prodshort](includes/prodshort.md)] as a data source in Power BI Desktop</span><span class="sxs-lookup"><span data-stu-id="584ea-108">To add [!INCLUDE[prodshort](includes/prodshort.md)] as a data source in Power BI Desktop</span></span>

1. <span data-ttu-id="584ea-109">In Power BI Desktop, in the left navigation pane, choose **Get Data**.</span><span class="sxs-lookup"><span data-stu-id="584ea-109">In Power BI Desktop, in the left navigation pane, choose **Get Data**.</span></span>
2. <span data-ttu-id="584ea-110">On the **Get Data** page, choose **Online Services**, choose **Microsoft Dynamics 365 Business Central**, and then choose the **Connect** button.</span><span class="sxs-lookup"><span data-stu-id="584ea-110">On the **Get Data** page, choose **Online Services**, choose **Microsoft Dynamics 365 Business Central**, and then choose the **Connect** button.</span></span>
3. <span data-ttu-id="584ea-111">Power BI displays a wizard that will guide you through the connection process.</span><span class="sxs-lookup"><span data-stu-id="584ea-111">Power BI displays a wizard that will guide you through the connection process.</span></span> <span data-ttu-id="584ea-112">You will be prompted to sign into [!INCLUDE [prodshort](includes/prodshort.md)].</span><span class="sxs-lookup"><span data-stu-id="584ea-112">You will be prompted to sign into [!INCLUDE [prodshort](includes/prodshort.md)].</span></span> <span data-ttu-id="584ea-113">Select **Sign in** and choose the account you would like to sign in as.</span><span class="sxs-lookup"><span data-stu-id="584ea-113">Select **Sign in** and choose the account you would like to sign in as.</span></span> <span data-ttu-id="584ea-114">This should be the same account you sign into [!INCLUDE [prodshort](includes/prodshort.md)] with.</span><span class="sxs-lookup"><span data-stu-id="584ea-114">This should be the same account you sign into [!INCLUDE [prodshort](includes/prodshort.md)] with.</span></span>
4. <span data-ttu-id="584ea-115">Choose the **Connect** button to continue.</span><span class="sxs-lookup"><span data-stu-id="584ea-115">Choose the **Connect** button to continue.</span></span> <span data-ttu-id="584ea-116">The Power BI wizard shows a list of Microsoft [!INCLUDE[d365fin](includes/d365fin_md.md)] companies and data sources.</span><span class="sxs-lookup"><span data-stu-id="584ea-116">The Power BI wizard shows a list of Microsoft [!INCLUDE[d365fin](includes/d365fin_md.md)] companies and data sources.</span></span> <span data-ttu-id="584ea-117">These data source represent all the web services that you have published from each company in [!INCLUDE [prodshort](includes/prodshort.md)].</span><span class="sxs-lookup"><span data-stu-id="584ea-117">These data source represent all the web services that you have published from each company in [!INCLUDE [prodshort](includes/prodshort.md)].</span></span>

  ![powerbi_webservices.png](media/across-how-use-financials-data-source-powerbi/powerbi_webservices.png)

5. <span data-ttu-id="584ea-119">Alternatively, create a new web service URL in [!INCLUDE [prodshort](includes/prodshort.md)] by using the **Create Data Set** action on the **Web Services** page, using the **Set Up Reporting** Assisted Setup guide, or by choosing the **Edit in Excel** action in any lists.</span><span class="sxs-lookup"><span data-stu-id="584ea-119">Alternatively, create a new web service URL in [!INCLUDE [prodshort](includes/prodshort.md)] by using the **Create Data Set** action on the **Web Services** page, using the **Set Up Reporting** Assisted Setup guide, or by choosing the **Edit in Excel** action in any lists.</span></span>
6. <span data-ttu-id="584ea-120">Specify the data you want to add to your data model, and then choose the **Load** button.</span><span class="sxs-lookup"><span data-stu-id="584ea-120">Specify the data you want to add to your data model, and then choose the **Load** button.</span></span>
7. <span data-ttu-id="584ea-121">Repeat the previous steps to add additional [!INCLUDE [prodshort](includes/prodshort.md)], or other data, to your Power BI data model.</span><span class="sxs-lookup"><span data-stu-id="584ea-121">Repeat the previous steps to add additional [!INCLUDE [prodshort](includes/prodshort.md)], or other data, to your Power BI data model.</span></span>

> [!NOTE]  
> <span data-ttu-id="584ea-122">Once you have successfully connected to [!INCLUDE [prodshort](includes/prodshort.md)], you will not be prompted again to sign in.</span><span class="sxs-lookup"><span data-stu-id="584ea-122">Once you have successfully connected to [!INCLUDE [prodshort](includes/prodshort.md)], you will not be prompted again to sign in.</span></span>

<span data-ttu-id="584ea-123">Once the data is loaded it will appear in the right navigation on the page.</span><span class="sxs-lookup"><span data-stu-id="584ea-123">Once the data is loaded it will appear in the right navigation on the page.</span></span> <span data-ttu-id="584ea-124">At this point, you have successfully connected to your [!INCLUDE [prodshort](includes/prodshort.md)] data and are ready to begin building your Power BI report.</span><span class="sxs-lookup"><span data-stu-id="584ea-124">At this point, you have successfully connected to your [!INCLUDE [prodshort](includes/prodshort.md)] data and are ready to begin building your Power BI report.</span></span>  

<span data-ttu-id="584ea-125">Before building your report, we recommend that you import the [!INCLUDE [prodshort](includes/prodshort.md)] theme file.</span><span class="sxs-lookup"><span data-stu-id="584ea-125">Before building your report, we recommend that you import the [!INCLUDE [prodshort](includes/prodshort.md)] theme file.</span></span>  <span data-ttu-id="584ea-126">The theme file will create a colour palette so that you can build reports with the same colour styling as the [!INCLUDE [prodshort](includes/prodshort.md)] apps without requiring you to define custom colours for each visual.</span><span class="sxs-lookup"><span data-stu-id="584ea-126">The theme file will create a color palette so that you can build reports with the same color styling as the [!INCLUDE [prodshort](includes/prodshort.md)] apps without requiring you to define custom colors for each visual.</span></span>

<span data-ttu-id="584ea-127">For more information, see the [Power BI documentation](/power-bi/consumer/power-bi-consumer-landing/).</span><span class="sxs-lookup"><span data-stu-id="584ea-127">For more information, see the [Power BI documentation](/power-bi/consumer/power-bi-consumer-landing/).</span></span>

## <a name="see-also"></a><span data-ttu-id="584ea-128">See Also</span><span class="sxs-lookup"><span data-stu-id="584ea-128">See Also</span></span>

[<span data-ttu-id="584ea-129">Enabling Your Business Data for Power BI</span><span class="sxs-lookup"><span data-stu-id="584ea-129">Enabling Your Business Data for Power BI</span></span>](admin-powerbi.md)  
[<span data-ttu-id="584ea-130">Business Intelligence</span><span class="sxs-lookup"><span data-stu-id="584ea-130">Business Intelligence</span></span>](bi.md)  
[<span data-ttu-id="584ea-131">Getting Started</span><span class="sxs-lookup"><span data-stu-id="584ea-131">Getting Started</span></span>](product-get-started.md)  
[<span data-ttu-id="584ea-132">Importing Business Data from Other Finance Systems</span><span class="sxs-lookup"><span data-stu-id="584ea-132">Importing Business Data from Other Finance Systems</span></span>](across-import-data-configuration-packages.md)  
<span data-ttu-id="584ea-133">[Setting Up [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)</span><span class="sxs-lookup"><span data-stu-id="584ea-133">[Setting Up [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)</span></span>  
[<span data-ttu-id="584ea-134">Finance</span><span class="sxs-lookup"><span data-stu-id="584ea-134">Finance</span></span>](finance.md)  
[<span data-ttu-id="584ea-135">Quickstart: Connect to data in Power BI Desktop</span><span class="sxs-lookup"><span data-stu-id="584ea-135">Quickstart: Connect to data in Power BI Desktop</span></span>](/power-bi/desktop-quickstart-connect-to-data)  
