---
title: How to Configure New Companies using a Cmdlet | Microsoft Docs
description: In a number of scenarios, you may want to load and import a configuration package without involving your users or using the RapidStart Services user interface. You can do so by using a Windows PowerShell cmdlet.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 03/06/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: e7dcdc0935a8793ae226dfc2f9709b5b8f487a62
ms.openlocfilehash: 9d248f2f8676c392451ae4a6f99932145f354f5b
ms.contentlocale: en-nz
ms.lasthandoff: 03/22/2018

---
# <a name="configure-new-companies-using-a-cmdlet"></a><span data-ttu-id="c0467-104">Configure New Companies using a Cmdlet</span><span class="sxs-lookup"><span data-stu-id="c0467-104">Configure New Companies using a Cmdlet</span></span>
<span data-ttu-id="c0467-105">In a number of scenarios, you may want to load and import a configuration package without involving your users or using the RapidStart Services user interface.</span><span class="sxs-lookup"><span data-stu-id="c0467-105">In a number of scenarios, you may want to load and import a configuration package without involving your users or using the RapidStart Services user interface.</span></span> <span data-ttu-id="c0467-106">You can do so by using a Windows PowerShell cmdlet.</span><span class="sxs-lookup"><span data-stu-id="c0467-106">You can do so by using a Windows PowerShell cmdlet.</span></span> <span data-ttu-id="c0467-107">Scenarios where this may be useful include:</span><span class="sxs-lookup"><span data-stu-id="c0467-107">Scenarios where this may be useful include:</span></span>  

- <span data-ttu-id="c0467-108">Performing data import across multiple [!INCLUDE[d365fin](includes/d365fin_md.md)] installations.</span><span class="sxs-lookup"><span data-stu-id="c0467-108">Performing data import across multiple [!INCLUDE[d365fin](includes/d365fin_md.md)] installations.</span></span>
- <span data-ttu-id="c0467-109">Configuring additional application areas for multiple customers.</span><span class="sxs-lookup"><span data-stu-id="c0467-109">Configuring additional application areas for multiple customers.</span></span>  

## <a name="to-deploy-a-configuration-package-using-a-cmdlet"></a><span data-ttu-id="c0467-110">To deploy a configuration package using a cmdlet</span><span class="sxs-lookup"><span data-stu-id="c0467-110">To deploy a configuration package using a cmdlet</span></span>  

1. <span data-ttu-id="c0467-111">Prepare a RapidStart Services package.</span><span class="sxs-lookup"><span data-stu-id="c0467-111">Prepare a RapidStart Services package.</span></span> <span data-ttu-id="c0467-112">For example, you can create a package to import certain values and the names of the table and the fields to insert these values into.</span><span class="sxs-lookup"><span data-stu-id="c0467-112">For example, you can create a package to import certain values and the names of the table and the fields to insert these values into.</span></span>  
2. <span data-ttu-id="c0467-113">Place the package on a computer where you will run the cmdlet.</span><span class="sxs-lookup"><span data-stu-id="c0467-113">Place the package on a computer where you will run the cmdlet.</span></span>  
3. <span data-ttu-id="c0467-114">Open the [!INCLUDE[d365fin](includes/d365fin_md.md)] administration shell.</span><span class="sxs-lookup"><span data-stu-id="c0467-114">Open the [!INCLUDE[d365fin](includes/d365fin_md.md)] administration shell.</span></span>  
4. <span data-ttu-id="c0467-115">Enter **Invoke-NAVCodeUnit**, and specify information similar to the following example.</span><span class="sxs-lookup"><span data-stu-id="c0467-115">Enter **Invoke-NAVCodeUnit**, and specify information similar to the following example.</span></span>  
    ```powershell  
    Invoke-NAVCodeunit -Tenant Default -CompanyName "CRONUS International Ltd." -CodeunitId 8620 -MethodName ImportRapidStartPackage -Argument "C:TEMPRS_CONFIG.rapidstart" -ServerInstance DynamicsNAV71  

    ```
<span data-ttu-id="c0467-116">The cmdlet imports the package into each company.</span><span class="sxs-lookup"><span data-stu-id="c0467-116">The cmdlet imports the package into each company.</span></span> <span data-ttu-id="c0467-117">Users can start to use the new functionality immediately.</span><span class="sxs-lookup"><span data-stu-id="c0467-117">Users can start to use the new functionality immediately.</span></span>  

## <a name="see-also"></a><span data-ttu-id="c0467-118">See Also</span><span class="sxs-lookup"><span data-stu-id="c0467-118">See Also</span></span>  
[<span data-ttu-id="c0467-119">Configure New Companies</span><span class="sxs-lookup"><span data-stu-id="c0467-119">Configure New Companies</span></span>](admin-how-to-configure-new-companies.md)  
[<span data-ttu-id="c0467-120">Apply Configurations to New Companies</span><span class="sxs-lookup"><span data-stu-id="c0467-120">Apply Configurations to New Companies</span></span>](admin-apply-configuration-to-new-companies.md)  
[<span data-ttu-id="c0467-121">Setting Up a Company With RapidStart Services</span><span class="sxs-lookup"><span data-stu-id="c0467-121">Setting Up a Company With RapidStart Services</span></span>](admin-set-up-a-company-with-rapidstart.md)  
[<span data-ttu-id="c0467-122">Administration</span><span class="sxs-lookup"><span data-stu-id="c0467-122">Administration</span></span>](admin-setup-and-administration.md)  
[<span data-ttu-id="c0467-123">Microsoft Dynamics NAV Windows PowerShell Cmdlets</span><span class="sxs-lookup"><span data-stu-id="c0467-123">Microsoft Dynamics NAV Windows PowerShell Cmdlets</span></span>](/dynamics-nav/microsoft-dynamics-nav-windows-powershell-cmdlets)

