---
title: How to Create a New Company | Microsoft Docs
description: To use RapidStart Services tables and pages are created, but there is no data in them.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 095d939d247a419d2adba16f9d3f61c8afb70e4d
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 10/01/2020
ms.locfileid: "3911371"
---
# <a name="create-a-new-company"></a><span data-ttu-id="7b185-103">Create a New Company</span><span class="sxs-lookup"><span data-stu-id="7b185-103">Create a New Company</span></span>
<span data-ttu-id="7b185-104">To use RapidStart Services for [!INCLUDE[d365fin](includes/d365fin_md.md)], you first create a new company for which you want to perform a customer implementation.</span><span class="sxs-lookup"><span data-stu-id="7b185-104">To use RapidStart Services for [!INCLUDE[d365fin](includes/d365fin_md.md)], you first create a new company for which you want to perform a customer implementation.</span></span> <span data-ttu-id="7b185-105">When you create a new company, the standard [!INCLUDE[d365fin](includes/d365fin_md.md)] tables and pages are created, but there is no data in them.</span><span class="sxs-lookup"><span data-stu-id="7b185-105">When you create a new company, the standard [!INCLUDE[d365fin](includes/d365fin_md.md)] tables and pages are created, but there is no data in them.</span></span>

<span data-ttu-id="7b185-106">In addition, you can apply specific setup data to your company after you initialise it.</span><span class="sxs-lookup"><span data-stu-id="7b185-106">In addition, you can apply specific setup data to your company after you initialize it.</span></span> <span data-ttu-id="7b185-107">The information is provided in a configuration package, a .rapidstart file, which delivers content in a compressed format.</span><span class="sxs-lookup"><span data-stu-id="7b185-107">The information is provided in a configuration package, a .rapidstart file, which delivers content in a compressed format.</span></span>  

<span data-ttu-id="7b185-108">Example configuration packages, including country/region-specific files, are included with the CRONUS demonstration company.</span><span class="sxs-lookup"><span data-stu-id="7b185-108">Example configuration packages, including country/region-specific files, are included with the CRONUS demonstration company.</span></span> <span data-ttu-id="7b185-109">Use the following procedures to use the example configuration package with a new company.</span><span class="sxs-lookup"><span data-stu-id="7b185-109">Use the following procedures to use the example configuration package with a new company.</span></span>  

## <a name="to-use-the-sample-basicconfig-configuration-package"></a><span data-ttu-id="7b185-110">To use the sample BASICCONFIG configuration package</span><span class="sxs-lookup"><span data-stu-id="7b185-110">To use the sample BASICCONFIG configuration package</span></span>  
1. <span data-ttu-id="7b185-111">Open the CRONUS International Ltd. company.</span><span class="sxs-lookup"><span data-stu-id="7b185-111">Open the CRONUS International Ltd. company.</span></span> <span data-ttu-id="7b185-112">For more information, see [Change Basic Settings](ui-change-basic-settings.md).</span><span class="sxs-lookup"><span data-stu-id="7b185-112">For more information, see [Change Basic Settings](ui-change-basic-settings.md).</span></span>
2. <span data-ttu-id="7b185-113">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Configuration Packages** , and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="7b185-113">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Configuration Packages** , and then choose the related link.</span></span>  
3. <span data-ttu-id="7b185-114">Choose the BASICCONFIG package from the list, and then choose the **Export Package** action.</span><span class="sxs-lookup"><span data-stu-id="7b185-114">Choose the BASICCONFIG package from the list, and then choose the **Export Package** action.</span></span>  

<span data-ttu-id="7b185-115">Use the following procedure to create a new company, and use the BASICCONFIG package as part of the process.</span><span class="sxs-lookup"><span data-stu-id="7b185-115">Use the following procedure to create a new company, and use the BASICCONFIG package as part of the process.</span></span>  

## <a name="to-create-a-new-company"></a><span data-ttu-id="7b185-116">To create a new company</span><span class="sxs-lookup"><span data-stu-id="7b185-116">To create a new company</span></span>  
1. <span data-ttu-id="7b185-117">Create a new company.</span><span class="sxs-lookup"><span data-stu-id="7b185-117">Create a new company.</span></span> <span data-ttu-id="7b185-118">For more information, see [Creating New Companies in [!INCLUDE[d365fin](includes/d365fin_md.md)]](about-new-company.md).</span><span class="sxs-lookup"><span data-stu-id="7b185-118">For more information, see [Creating New Companies in [!INCLUDE[d365fin](includes/d365fin_md.md)]](about-new-company.md).</span></span>
2. <span data-ttu-id="7b185-119">From the RapidStart Services Implementer Role Centre, you can now import the configuration package that you exported from the CRONUS International Ltd. company.</span><span class="sxs-lookup"><span data-stu-id="7b185-119">From the RapidStart Services Implementer Role Center, you can now import the configuration package that you exported from the CRONUS International Ltd. company.</span></span>

<span data-ttu-id="7b185-120">After you create a new company, some tables are automatically filled in, even if no company template is applied.</span><span class="sxs-lookup"><span data-stu-id="7b185-120">After you create a new company, some tables are automatically filled in, even if no company template is applied.</span></span> <span data-ttu-id="7b185-121">For example, you can review the standard codes for posting and batch transactions on the **Source Code** page.</span><span class="sxs-lookup"><span data-stu-id="7b185-121">For example, you can review the standard codes for posting and batch transactions on the **Source Code** page.</span></span> <span data-ttu-id="7b185-122">If you provide a local version of [!INCLUDE[d365fin](includes/d365fin_md.md)], you should review this table and consider any local language issues.</span><span class="sxs-lookup"><span data-stu-id="7b185-122">If you provide a local version of [!INCLUDE[d365fin](includes/d365fin_md.md)], you should review this table and consider any local language issues.</span></span>

## <a name="about-data-tables"></a><span data-ttu-id="7b185-123">About Data Tables</span><span class="sxs-lookup"><span data-stu-id="7b185-123">About Data Tables</span></span>
[!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="7b185-124">, data tables come in two basic types: Master and Setup.</span><span class="sxs-lookup"><span data-stu-id="7b185-124">, data tables come in two basic types: Master and Setup.</span></span> <span data-ttu-id="7b185-125">When you are setting up a company configuration, you can use these types to focus your configuration strategy.</span><span class="sxs-lookup"><span data-stu-id="7b185-125">When you are setting up a company configuration, you can use these types to focus your configuration strategy.</span></span>  

### <a name="master-data-tables"></a><span data-ttu-id="7b185-126">Master Data Tables</span><span class="sxs-lookup"><span data-stu-id="7b185-126">Master Data Tables</span></span>  
<span data-ttu-id="7b185-127">The following table lists some of the master data tables.</span><span class="sxs-lookup"><span data-stu-id="7b185-127">The following table lists some of the master data tables.</span></span> <span data-ttu-id="7b185-128">When you initialise a new company, these tables are empty.</span><span class="sxs-lookup"><span data-stu-id="7b185-128">When you initialize a new company, these tables are empty.</span></span>  

|<span data-ttu-id="7b185-129">Table No.</span><span class="sxs-lookup"><span data-stu-id="7b185-129">Table No.</span></span>|<span data-ttu-id="7b185-130">Table Name</span><span class="sxs-lookup"><span data-stu-id="7b185-130">Table Name</span></span>|  
|-------------------|--------------------|  
|<span data-ttu-id="7b185-131">15</span><span class="sxs-lookup"><span data-stu-id="7b185-131">15</span></span>|<span data-ttu-id="7b185-132">G/L Account</span><span class="sxs-lookup"><span data-stu-id="7b185-132">G/L Account</span></span>|  
|<span data-ttu-id="7b185-133">18</span><span class="sxs-lookup"><span data-stu-id="7b185-133">18</span></span>|<span data-ttu-id="7b185-134">Customer</span><span class="sxs-lookup"><span data-stu-id="7b185-134">Customer</span></span>|  
|<span data-ttu-id="7b185-135">23</span><span class="sxs-lookup"><span data-stu-id="7b185-135">23</span></span>|<span data-ttu-id="7b185-136">Vendor</span><span class="sxs-lookup"><span data-stu-id="7b185-136">Vendor</span></span>|  
|<span data-ttu-id="7b185-137">27</span><span class="sxs-lookup"><span data-stu-id="7b185-137">27</span></span>|<span data-ttu-id="7b185-138">Item</span><span class="sxs-lookup"><span data-stu-id="7b185-138">Item</span></span>|  
|<span data-ttu-id="7b185-139">5050</span><span class="sxs-lookup"><span data-stu-id="7b185-139">5050</span></span>|<span data-ttu-id="7b185-140">Contact</span><span class="sxs-lookup"><span data-stu-id="7b185-140">Contact</span></span>|  

### <a name="setup-data-tables"></a><span data-ttu-id="7b185-141">Setup Data Tables</span><span class="sxs-lookup"><span data-stu-id="7b185-141">Setup Data Tables</span></span>  
<span data-ttu-id="7b185-142">The following table lists some of the setup data tables, in which you capture setup information in the configuration questionnaire.</span><span class="sxs-lookup"><span data-stu-id="7b185-142">The following table lists some of the setup data tables, in which you capture setup information in the configuration questionnaire.</span></span> <span data-ttu-id="7b185-143">These tables contain baseline information when the company is created.</span><span class="sxs-lookup"><span data-stu-id="7b185-143">These tables contain baseline information when the company is created.</span></span>  

|<span data-ttu-id="7b185-144">Table No.</span><span class="sxs-lookup"><span data-stu-id="7b185-144">Table No.</span></span>|<span data-ttu-id="7b185-145">Table Name</span><span class="sxs-lookup"><span data-stu-id="7b185-145">Table Name</span></span>|  
|-------------------|--------------------|  
|<span data-ttu-id="7b185-146">98</span><span class="sxs-lookup"><span data-stu-id="7b185-146">98</span></span>|<span data-ttu-id="7b185-147">General Ledger Setup</span><span class="sxs-lookup"><span data-stu-id="7b185-147">General Ledger Setup</span></span>|  
|<span data-ttu-id="7b185-148">311</span><span class="sxs-lookup"><span data-stu-id="7b185-148">311</span></span>|<span data-ttu-id="7b185-149">Sales & Receivables Setup</span><span class="sxs-lookup"><span data-stu-id="7b185-149">Sales & Receivables Setup</span></span>|  
|<span data-ttu-id="7b185-150">312</span><span class="sxs-lookup"><span data-stu-id="7b185-150">312</span></span>|<span data-ttu-id="7b185-151">Purchases & Payables Setup</span><span class="sxs-lookup"><span data-stu-id="7b185-151">Purchases & Payables Setup</span></span>|  
|<span data-ttu-id="7b185-152">313</span><span class="sxs-lookup"><span data-stu-id="7b185-152">313</span></span>|<span data-ttu-id="7b185-153">Inventory Setup</span><span class="sxs-lookup"><span data-stu-id="7b185-153">Inventory Setup</span></span>|  

<span data-ttu-id="7b185-154">In addition to setup data tables, [!INCLUDE[d365fin](includes/d365fin_md.md)] also has setup-type data tables that specify core information about the company and its business processes.</span><span class="sxs-lookup"><span data-stu-id="7b185-154">In addition to setup data tables, [!INCLUDE[d365fin](includes/d365fin_md.md)] also has setup-type data tables that specify core information about the company and its business processes.</span></span> <span data-ttu-id="7b185-155">The following table lists some of them.</span><span class="sxs-lookup"><span data-stu-id="7b185-155">The following table lists some of them.</span></span>  

|<span data-ttu-id="7b185-156">Table No.</span><span class="sxs-lookup"><span data-stu-id="7b185-156">Table No.</span></span>|<span data-ttu-id="7b185-157">Table Name</span><span class="sxs-lookup"><span data-stu-id="7b185-157">Table Name</span></span>|  
|-------------------|--------------------|  
|<span data-ttu-id="7b185-158">3</span><span class="sxs-lookup"><span data-stu-id="7b185-158">3</span></span>|<span data-ttu-id="7b185-159">Payment Terms</span><span class="sxs-lookup"><span data-stu-id="7b185-159">Payment Terms</span></span>|  
|<span data-ttu-id="7b185-160">4</span><span class="sxs-lookup"><span data-stu-id="7b185-160">4</span></span>|<span data-ttu-id="7b185-161">Currency</span><span class="sxs-lookup"><span data-stu-id="7b185-161">Currency</span></span>|  
|<span data-ttu-id="7b185-162">6</span><span class="sxs-lookup"><span data-stu-id="7b185-162">6</span></span>|<span data-ttu-id="7b185-163">Customer Price Groups</span><span class="sxs-lookup"><span data-stu-id="7b185-163">Customer Price Groups</span></span>|  
|<span data-ttu-id="7b185-164">5700</span><span class="sxs-lookup"><span data-stu-id="7b185-164">5700</span></span>|<span data-ttu-id="7b185-165">Stockkeeping Unit</span><span class="sxs-lookup"><span data-stu-id="7b185-165">Stockkeeping Unit</span></span>|

  

## <a name="see-also"></a><span data-ttu-id="7b185-166">See Also</span><span class="sxs-lookup"><span data-stu-id="7b185-166">See Also</span></span>  
[<span data-ttu-id="7b185-167">Apply Configurations to New Companies</span><span class="sxs-lookup"><span data-stu-id="7b185-167">Apply Configurations to New Companies</span></span>](admin-apply-configuration-to-new-companies.md)  
[<span data-ttu-id="7b185-168">Setting Up a Company With RapidStart Services</span><span class="sxs-lookup"><span data-stu-id="7b185-168">Setting Up a Company With RapidStart Services</span></span>](admin-set-up-a-company-with-rapidstart.md)  
[<span data-ttu-id="7b185-169">Administration</span><span class="sxs-lookup"><span data-stu-id="7b185-169">Administration</span></span>](admin-setup-and-administration.md)
