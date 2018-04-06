---
title: Troubleshooting Integration with Microsoft Flow| Microsoft Docs
description: Troubleshoot how you can make your Financials data available as a data source and specify an OData URL of your web services to build an automated workflow.
documentationcenter: 
author: SusanneWindfeldPedersen
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: workflow, Odata, Power App, SOAP
ms.date: 01/25/2018
ms.author: solsen
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 60ce05760251da39280eb8a4884cb80586c2ab62
ms.contentlocale: en-nz
ms.lasthandoff: 03/22/2018

---
# <a name="troubleshooting-integration-with-microsoft-flow---request-url-too-long"></a><span data-ttu-id="df794-103">Troubleshooting Integration with Microsoft Flow - Request URL Too Long</span><span class="sxs-lookup"><span data-stu-id="df794-103">Troubleshooting Integration with Microsoft Flow - Request URL Too Long</span></span>
<span data-ttu-id="df794-104">You can use your [!INCLUDE[d365fin](includes/d365fin_md.md)] data as part of a workflow in Microsoft Flow.</span><span class="sxs-lookup"><span data-stu-id="df794-104">You can use your [!INCLUDE[d365fin](includes/d365fin_md.md)] data as part of a workflow in Microsoft Flow.</span></span>  

> [!NOTE]  
>   <span data-ttu-id="df794-105">You must have a valid account with [!INCLUDE[d365fin](includes/d365fin_md.md)] and with Flow.</span><span class="sxs-lookup"><span data-stu-id="df794-105">You must have a valid account with [!INCLUDE[d365fin](includes/d365fin_md.md)] and with Flow.</span></span>  

<span data-ttu-id="df794-106">If you are creating a Microsoft Flow using the [!INCLUDE[d365fin](includes/d365fin_md.md)] connector, you may receive an error message stating that the requsted URL is too long after creating the flow, such as the following: **RequestUriTooLong**.</span><span class="sxs-lookup"><span data-stu-id="df794-106">If you are creating a Microsoft Flow using the [!INCLUDE[d365fin](includes/d365fin_md.md)] connector, you may receive an error message stating that the requsted URL is too long after creating the flow, such as the following: **RequestUriTooLong**.</span></span>

## <a name="cause"></a><span data-ttu-id="df794-107">Cause</span><span class="sxs-lookup"><span data-stu-id="df794-107">Cause</span></span>
<span data-ttu-id="df794-108">For a flow to trigger, it looks for changes in your data.</span><span class="sxs-lookup"><span data-stu-id="df794-108">For a flow to trigger, it looks for changes in your data.</span></span> <span data-ttu-id="df794-109">When determining if your data has changed, the connectors compare the cached data to the new data requested from the source.</span><span class="sxs-lookup"><span data-stu-id="df794-109">When determining if your data has changed, the connectors compare the cached data to the new data requested from the source.</span></span>  

<span data-ttu-id="df794-110">If the data request creates a URL that is too long, it will fail.</span><span class="sxs-lookup"><span data-stu-id="df794-110">If the data request creates a URL that is too long, it will fail.</span></span> <span data-ttu-id="df794-111">Common causes may include:</span><span class="sxs-lookup"><span data-stu-id="df794-111">Common causes may include:</span></span>
- <span data-ttu-id="df794-112">Generally, any source table with over 250 rows</span><span class="sxs-lookup"><span data-stu-id="df794-112">Generally, any source table with over 250 rows</span></span>
- <span data-ttu-id="df794-113">Source tables containing multiple thousands of records</span><span class="sxs-lookup"><span data-stu-id="df794-113">Source tables containing multiple thousands of records</span></span>

## <a name="workaround"></a><span data-ttu-id="df794-114">Workaround</span><span class="sxs-lookup"><span data-stu-id="df794-114">Workaround</span></span>
<span data-ttu-id="df794-115">Follow these steps as a workaround.</span><span class="sxs-lookup"><span data-stu-id="df794-115">Follow these steps as a workaround.</span></span>
1. <span data-ttu-id="df794-116">Choose to edit the flow that is failing.</span><span class="sxs-lookup"><span data-stu-id="df794-116">Choose to edit the flow that is failing.</span></span>
2. <span data-ttu-id="df794-117">Expand the **Show advanced options** on the flow trigger.</span><span class="sxs-lookup"><span data-stu-id="df794-117">Expand the **Show advanced options** on the flow trigger.</span></span>
3. <span data-ttu-id="df794-118">In the **Skip Count** field, enter the number of records to skip.</span><span class="sxs-lookup"><span data-stu-id="df794-118">In the **Skip Count** field, enter the number of records to skip.</span></span>  
<span data-ttu-id="df794-119">For example, if the table that you are using as a data source has 4,000 records, enter 4,000 as the number of records to skip.</span><span class="sxs-lookup"><span data-stu-id="df794-119">For example, if the table that you are using as a data source has 4,000 records, enter 4,000 as the number of records to skip.</span></span>
4. <span data-ttu-id="df794-120">Update your flow.</span><span class="sxs-lookup"><span data-stu-id="df794-120">Update your flow.</span></span>

> [!NOTE]  
> <span data-ttu-id="df794-121">The connector is currently in Beta.</span><span class="sxs-lookup"><span data-stu-id="df794-121">The connector is currently in Beta.</span></span> <span data-ttu-id="df794-122">Updates to how data changes are targeted for a future release.</span><span class="sxs-lookup"><span data-stu-id="df794-122">Updates to how data changes are targeted for a future release.</span></span>


## <a name="see-also"></a><span data-ttu-id="df794-123">See Also</span><span class="sxs-lookup"><span data-stu-id="df794-123">See Also</span></span>
<span data-ttu-id="df794-124">[Using [!INCLUDE[d365fin](includes/d365fin_md.md)] in an Automated Workflow](across-how-use-financials-data-source-flow.md)</span><span class="sxs-lookup"><span data-stu-id="df794-124">[Using [!INCLUDE[d365fin](includes/d365fin_md.md)] in an Automated Workflow](across-how-use-financials-data-source-flow.md)</span></span>  
<span data-ttu-id="df794-125">[Welcome to [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)</span><span class="sxs-lookup"><span data-stu-id="df794-125">[Welcome to [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)</span></span>  
[<span data-ttu-id="df794-126">Importing Business Data from Other Finance Systems</span><span class="sxs-lookup"><span data-stu-id="df794-126">Importing Business Data from Other Finance Systems</span></span>](upload-data.md)  
<span data-ttu-id="df794-127">[Manage Users and Permissions](ui-how-users-permissions.md)  </span><span class="sxs-lookup"><span data-stu-id="df794-127">[Manage Users and Permissions](ui-how-users-permissions.md)  </span></span>  
<span data-ttu-id="df794-128">[Setting Up [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)</span><span class="sxs-lookup"><span data-stu-id="df794-128">[Setting Up [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)</span></span>  
[<span data-ttu-id="df794-129">Finance</span><span class="sxs-lookup"><span data-stu-id="df794-129">Finance</span></span>](finance.md)  

