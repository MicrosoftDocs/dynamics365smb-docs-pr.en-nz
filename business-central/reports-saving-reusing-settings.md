---
title: Apply and Modify Saved Settings on Reports | Microsoft Docs
description: Describes using predefined options and filters to customise a report, and to generate the correct data.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: customization, personalization
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: d9ae0f8e45c940d2a78d4d383a733ad378e90650
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 10/01/2020
ms.locfileid: "3926363"
---
# <a name="manage-saved-settings-for-reports-and-batch-jobs"></a><span data-ttu-id="e1e8d-103">Manage Saved Settings for Reports and Batch jobs</span><span class="sxs-lookup"><span data-stu-id="e1e8d-103">Manage Saved Settings for Reports and Batch jobs</span></span>
<span data-ttu-id="e1e8d-104">When running reports, users are typically presented with a page that lets them select options and set filters to change the data that is included in the generated report.</span><span class="sxs-lookup"><span data-stu-id="e1e8d-104">When running reports, users are typically presented with a page that lets them select options and set filters to change the data that is included in the generated report.</span></span> <span data-ttu-id="e1e8d-105">This page is called the request page.</span><span class="sxs-lookup"><span data-stu-id="e1e8d-105">This page is called the request page.</span></span> <span data-ttu-id="e1e8d-106">A report can include one or more *saved settings* that users can apply to the report from the request page.</span><span class="sxs-lookup"><span data-stu-id="e1e8d-106">A report can include one or more *saved settings* that users can apply to the report from the request page.</span></span> <span data-ttu-id="e1e8d-107">*Saved settings* are basically predefined options and filters.</span><span class="sxs-lookup"><span data-stu-id="e1e8d-107">*Saved settings* are basically predefined options and filters.</span></span> <span data-ttu-id="e1e8d-108">Using saved settings is a fast and reliable way to consistently generate reports that contain the correct data.</span><span class="sxs-lookup"><span data-stu-id="e1e8d-108">Using saved settings is a fast and reliable way to consistently generate reports that contain the correct data.</span></span> <span data-ttu-id="e1e8d-109">For more information, see [Using Saved Settings](ui-work-report.md#SavedSettings).</span><span class="sxs-lookup"><span data-stu-id="e1e8d-109">For more information, see [Using Saved Settings](ui-work-report.md#SavedSettings).</span></span>

> [!NOTE]
> <span data-ttu-id="e1e8d-110">This topic refers mainly to "report", but similar information applies to batch jobs.</span><span class="sxs-lookup"><span data-stu-id="e1e8d-110">This topic refers mainly to "report", but similar information applies to batch jobs.</span></span>

<span data-ttu-id="e1e8d-111">If you have the proper permissions, you can view, create, and modify the saved settings for all reports for all users in a company.</span><span class="sxs-lookup"><span data-stu-id="e1e8d-111">If you have the proper permissions, you can view, create, and modify the saved settings for all reports for all users in a company.</span></span> <span data-ttu-id="e1e8d-112">You can assign saved settings for a report to individual users or to all users in the company.</span><span class="sxs-lookup"><span data-stu-id="e1e8d-112">You can assign saved settings for a report to individual users or to all users in the company.</span></span>

<!--
## Apply saved settings to a report
1. Open the report.

   The request page appears.    
2. In the **Saved Settings** section of the page, set the **Name** field  to the saved settings that you want to use.

   The **Saved Settings** section only appears if the report has been run before or if there are existing saved settings entries. The saved settings entry called **Last used options and filters** is always available. These settings are the option and filter values that were used the last time you ran the report.

-->

## <a name="to-create-and-modify-saved-settings-for-all-users"></a><span data-ttu-id="e1e8d-113">To create and modify saved settings for all users</span><span class="sxs-lookup"><span data-stu-id="e1e8d-113">To create and modify saved settings for all users</span></span>
<span data-ttu-id="e1e8d-114">You manage saved settings on the **Reports Settings** page.</span><span class="sxs-lookup"><span data-stu-id="e1e8d-114">You manage saved settings on the **Reports Settings** page.</span></span> <span data-ttu-id="e1e8d-115">There are two ways to open this page:</span><span class="sxs-lookup"><span data-stu-id="e1e8d-115">There are two ways to open this page:</span></span>
-   <span data-ttu-id="e1e8d-116">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Report Settings** , and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="e1e8d-116">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Report Settings** , and then choose the related link.</span></span>
-   <span data-ttu-id="e1e8d-117">Open a report, choose the lookup in the **Use default values from** field, and then choose the **Select from full list** action.</span><span class="sxs-lookup"><span data-stu-id="e1e8d-117">Open a report, choose the lookup in the **Use default values from** field, and then choose the **Select from full list** action.</span></span>

<span data-ttu-id="e1e8d-118">The page displays all the existing saved settings entries for all users.</span><span class="sxs-lookup"><span data-stu-id="e1e8d-118">The page displays all the existing saved settings entries for all users.</span></span> <span data-ttu-id="e1e8d-119">If there is a user name in the **Assigned to** field, only that user can use the saved settings for the associated report.</span><span class="sxs-lookup"><span data-stu-id="e1e8d-119">If there is a user name in the **Assigned to** field, only that user can use the saved settings for the associated report.</span></span> <span data-ttu-id="e1e8d-120">If there is a check mark in the **Share with all users** field, all users can use the saved settings for the report.</span><span class="sxs-lookup"><span data-stu-id="e1e8d-120">If there is a check mark in the **Share with all users** field, all users can use the saved settings for the report.</span></span>

<span data-ttu-id="e1e8d-121">From the **Report Settings** page, you can:</span><span class="sxs-lookup"><span data-stu-id="e1e8d-121">From the **Report Settings** page, you can:</span></span>
-   <span data-ttu-id="e1e8d-122">Choose the **New** action to create a new saved settings entry from scratch.</span><span class="sxs-lookup"><span data-stu-id="e1e8d-122">Choose the **New** action to create a new saved settings entry from scratch.</span></span>
-   <span data-ttu-id="e1e8d-123">Select a saved settings entry from the list, and choose the **Copy** action to create a copy.</span><span class="sxs-lookup"><span data-stu-id="e1e8d-123">Select a saved settings entry from the list, and choose the **Copy** action to create a copy.</span></span>
-   <span data-ttu-id="e1e8d-124">Select a saved settings entry from the list, and choose the **Edit** action to modify a saved settings entry.</span><span class="sxs-lookup"><span data-stu-id="e1e8d-124">Select a saved settings entry from the list, and choose the **Edit** action to modify a saved settings entry.</span></span>

> [!Important]
> <span data-ttu-id="e1e8d-125">Consider the name that you give a saved settings entry.</span><span class="sxs-lookup"><span data-stu-id="e1e8d-125">Consider the name that you give a saved settings entry.</span></span> <span data-ttu-id="e1e8d-126">If you create a saved settings entry for all users, and you give it the same name as an existing saved settings entry that is assigned to a specific user only, then that user will not be able to use the saved settings entry that is assigned to everyone.</span><span class="sxs-lookup"><span data-stu-id="e1e8d-126">If you create a saved settings entry for all users, and you give it the same name as an existing saved settings entry that is assigned to a specific user only, then that user will not be able to use the saved settings entry that is assigned to everyone.</span></span>  <span data-ttu-id="e1e8d-127">In the **Saved Settings** section on the request page, the user will see two saved settings entries with the same name.</span><span class="sxs-lookup"><span data-stu-id="e1e8d-127">In the **Saved Settings** section on the request page, the user will see two saved settings entries with the same name.</span></span> <span data-ttu-id="e1e8d-128">However, no matter which option they choose, the user-specific saved settings entry will be used.</span><span class="sxs-lookup"><span data-stu-id="e1e8d-128">However, no matter which option they choose, the user-specific saved settings entry will be used.</span></span>

> [!NOTE]
> <span data-ttu-id="e1e8d-129">The Saved Settings feature is available only on reports where the [SaveValues property](/dynamics365/business-central/dev-itpro/developer/properties/devenv-savevalues-property) of the report's request page is set to **Yes** .</span><span class="sxs-lookup"><span data-stu-id="e1e8d-129">The Saved Settings feature is available only on reports where the [SaveValues property](/dynamics365/business-central/dev-itpro/developer/properties/devenv-savevalues-property) of the report's request page is set to **Yes** .</span></span> <span data-ttu-id="e1e8d-130">The **SaveValues** property is set in the development environment.</span><span class="sxs-lookup"><span data-stu-id="e1e8d-130">The **SaveValues** property is set in the development environment.</span></span>  

## <a name="see-also"></a><span data-ttu-id="e1e8d-131">See Also</span><span class="sxs-lookup"><span data-stu-id="e1e8d-131">See Also</span></span>
[<span data-ttu-id="e1e8d-132">Working with Reports, Batch Jobs, and XMLports</span><span class="sxs-lookup"><span data-stu-id="e1e8d-132">Working with Reports, Batch Jobs, and XMLports</span></span>](ui-work-report.md)  
