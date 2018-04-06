---
title: Set Up Company Configuration | Microsoft Docs
description: The implementation process begins with the Business Central solution will require. You bundle all of this information into configuration packages.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 03/05/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: eeca45a36e38ab80a63156995a2f11466262d512
ms.contentlocale: en-nz
ms.lasthandoff: 03/22/2018

---
# <a name="set-up-company-configuration"></a><span data-ttu-id="217f8-104">Set Up Company Configuration</span><span class="sxs-lookup"><span data-stu-id="217f8-104">Set Up Company Configuration</span></span>
<span data-ttu-id="217f8-105">The implementation process begins with the Microsoft partner.</span><span class="sxs-lookup"><span data-stu-id="217f8-105">The implementation process begins with the Microsoft partner.</span></span> <span data-ttu-id="217f8-106">The partner is responsible for thinking through the configuration details and creating a package that a customer can easily apply.</span><span class="sxs-lookup"><span data-stu-id="217f8-106">The partner is responsible for thinking through the configuration details and creating a package that a customer can easily apply.</span></span> <span data-ttu-id="217f8-107">Before you create a new company, you should plan how it will be configured.</span><span class="sxs-lookup"><span data-stu-id="217f8-107">Before you create a new company, you should plan how it will be configured.</span></span> <span data-ttu-id="217f8-108">You must consider basic setup data and the types of data that your [!INCLUDE[d365fin](includes/d365fin_md.md)] solution will require.</span><span class="sxs-lookup"><span data-stu-id="217f8-108">You must consider basic setup data and the types of data that your [!INCLUDE[d365fin](includes/d365fin_md.md)] solution will require.</span></span> <span data-ttu-id="217f8-109">You bundle all of this information in configuration packages.</span><span class="sxs-lookup"><span data-stu-id="217f8-109">You bundle all of this information in configuration packages.</span></span>

<span data-ttu-id="217f8-110">RapidStart Services also provides you with the tools that you will use to migrate your legacy data, such as customers and vendors.</span><span class="sxs-lookup"><span data-stu-id="217f8-110">RapidStart Services also provides you with the tools that you will use to migrate your legacy data, such as customers and vendors.</span></span>  

<span data-ttu-id="217f8-111">We recommend that you create configuration packages with most of the setup tables already filled in, so that customers only have to change a few settings after the package is applied.</span><span class="sxs-lookup"><span data-stu-id="217f8-111">We recommend that you create configuration packages with most of the setup tables already filled in, so that customers only have to change a few settings after the package is applied.</span></span> <span data-ttu-id="217f8-112">For example, when you create a new company, the **No. Series** and the **No. Series Line** tables are filled in with a set of number series and starting numbers.</span><span class="sxs-lookup"><span data-stu-id="217f8-112">For example, when you create a new company, the **No. Series** and the **No. Series Line** tables are filled in with a set of number series and starting numbers.</span></span> <span data-ttu-id="217f8-113">The corresponding **No. Series** fields in the setup tables are also filled in automatically.</span><span class="sxs-lookup"><span data-stu-id="217f8-113">The corresponding **No. Series** fields in the setup tables are also filled in automatically.</span></span> <span data-ttu-id="217f8-114">You do not have to do the work of entering number series and other basic setup data.</span><span class="sxs-lookup"><span data-stu-id="217f8-114">You do not have to do the work of entering number series and other basic setup data.</span></span> <span data-ttu-id="217f8-115">You can also manually change all default data that is used with RapidStart Services by using the configuration worksheet.</span><span class="sxs-lookup"><span data-stu-id="217f8-115">You can also manually change all default data that is used with RapidStart Services by using the configuration worksheet.</span></span>  

<span data-ttu-id="217f8-116">The configuration packages are built on a preconfigured company.</span><span class="sxs-lookup"><span data-stu-id="217f8-116">The configuration packages are built on a preconfigured company.</span></span> <span data-ttu-id="217f8-117">After you have set up a company that meets your needs, you can create a configuration package that contains relevant data from this company.</span><span class="sxs-lookup"><span data-stu-id="217f8-117">After you have set up a company that meets your needs, you can create a configuration package that contains relevant data from this company.</span></span> <span data-ttu-id="217f8-118">You can then use it when you create a new company that is to be configured in the same way.</span><span class="sxs-lookup"><span data-stu-id="217f8-118">You can then use it when you create a new company that is to be configured in the same way.</span></span>  

<span data-ttu-id="217f8-119">To facilitate the import of master data, such as customer and vendor information, you can use configuration templates.</span><span class="sxs-lookup"><span data-stu-id="217f8-119">To facilitate the import of master data, such as customer and vendor information, you can use configuration templates.</span></span> <span data-ttu-id="217f8-120">Configuration templates contain a set of default settings that are automatically assigned to the records imported into [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="217f8-120">Configuration templates contain a set of default settings that are automatically assigned to the records imported into [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>

<span data-ttu-id="217f8-121">The following table describes a sequence of tasks with links to topics that describe them.</span><span class="sxs-lookup"><span data-stu-id="217f8-121">The following table describes a sequence of tasks with links to topics that describe them.</span></span>

|<span data-ttu-id="217f8-122">**To**</span><span class="sxs-lookup"><span data-stu-id="217f8-122">**To**</span></span>|<span data-ttu-id="217f8-123">**See**</span><span class="sxs-lookup"><span data-stu-id="217f8-123">**See**</span></span>|  
|------------|-------------|  
|<span data-ttu-id="217f8-124">Plan a company configuration by filling in the configuration worksheet.</span><span class="sxs-lookup"><span data-stu-id="217f8-124">Plan a company configuration by filling in the configuration worksheet.</span></span>|[<span data-ttu-id="217f8-125">Manage Company Configuration in a Worksheet</span><span class="sxs-lookup"><span data-stu-id="217f8-125">Manage Company Configuration in a Worksheet</span></span>](admin-how-to-manage-company-configuration-in-a-worksheet.md)|  
|<span data-ttu-id="217f8-126">Create a configuration package, customise a package, assign tables to a package, review or edit existing customer data, create the new company and then move test data to the production environment.</span><span class="sxs-lookup"><span data-stu-id="217f8-126">Create a configuration package, customize a package, assign tables to a package, review or edit existing customer data, create the new company and then move test data to the production environment.</span></span>|[<span data-ttu-id="217f8-127">Prepare a Configuration Package</span><span class="sxs-lookup"><span data-stu-id="217f8-127">Prepare a Configuration Package</span></span>](admin-how-to-prepare-a-configuration-package.md)| 

## <a name="see-also"></a><span data-ttu-id="217f8-128">See Also</span><span class="sxs-lookup"><span data-stu-id="217f8-128">See Also</span></span>  
[<span data-ttu-id="217f8-129">Setting Up a Company With RapidStart Services</span><span class="sxs-lookup"><span data-stu-id="217f8-129">Setting Up a Company With RapidStart Services</span></span>](admin-set-up-a-company-with-rapidstart.md)  
[<span data-ttu-id="217f8-130">Administration</span><span class="sxs-lookup"><span data-stu-id="217f8-130">Administration</span></span>](admin-setup-and-administration.md)

