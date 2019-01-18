---
title: Configuring API Templates | Microsoft Docs
description: Describing the steps you must go through to configure API templates for Dynamics 365 Business Central.
services: project-madeira
documentationcenter: 
author: SusanneWindfeldPedersen
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: API templates, configuring templates
ms.date: 10/01/2018
ms.author: solsen
ms.translationtype: HT
ms.sourcegitcommit: 33b900f1ac9e295921e7f3d6ea72cc93939d8a1b
ms.openlocfilehash: 7420bd1b8c1c246b608910a35a47ac025eec6b8b
ms.contentlocale: en-nz
ms.lasthandoff: 11/26/2018

---

# <a name="configuring-api-templates"></a><span data-ttu-id="37aa2-103">Configuring API Templates</span><span class="sxs-lookup"><span data-stu-id="37aa2-103">Configuring API Templates</span></span>
<span data-ttu-id="37aa2-104">The API library for [!INCLUDE[d365fin_md](includes/d365fin_md.md)] provides a simplified representation of the underlying entities.</span><span class="sxs-lookup"><span data-stu-id="37aa2-104">The API library for [!INCLUDE[d365fin_md](includes/d365fin_md.md)] provides a simplified representation of the underlying entities.</span></span> <span data-ttu-id="37aa2-105">All the properties in the application are not exposed through the associated API.</span><span class="sxs-lookup"><span data-stu-id="37aa2-105">All the properties in the application are not exposed through the associated API.</span></span> <span data-ttu-id="37aa2-106">The **API Setup** page allows you to define templates that are used to populate empty properties on an entity when you create a POST action through the API.</span><span class="sxs-lookup"><span data-stu-id="37aa2-106">The **API Setup** page allows you to define templates that are used to populate empty properties on an entity when you create a POST action through the API.</span></span> 

<span data-ttu-id="37aa2-107">For example, if a configuration template is defined for the item entity, when a new item record is created through the items API, any properties for the new item that are not defined in the API call will be populated from the selected template.</span><span class="sxs-lookup"><span data-stu-id="37aa2-107">For example, if a configuration template is defined for the item entity, when a new item record is created through the items API, any properties for the new item that are not defined in the API call will be populated from the selected template.</span></span> <span data-ttu-id="37aa2-108">If, for example, no value is defined for the **Gen. Prod. Posting Group** field through the API, but a value is defined in the selected template, then the posting group value defined in the template will be applied to the new item.</span><span class="sxs-lookup"><span data-stu-id="37aa2-108">If, for example, no value is defined for the **Gen. Prod. Posting Group** field through the API, but a value is defined in the selected template, then the posting group value defined in the template will be applied to the new item.</span></span> 

## <a name="setting-up-the-entity-template"></a><span data-ttu-id="37aa2-109">Setting up the Entity Template</span><span class="sxs-lookup"><span data-stu-id="37aa2-109">Setting up the Entity Template</span></span>
<span data-ttu-id="37aa2-110">To use templates with the API library, you must first set up and define properties for the templates.</span><span class="sxs-lookup"><span data-stu-id="37aa2-110">To use templates with the API library, you must first set up and define properties for the templates.</span></span> <span data-ttu-id="37aa2-111">You can set up these templates on the **Configuration Templates** page.</span><span class="sxs-lookup"><span data-stu-id="37aa2-111">You can set up these templates on the **Configuration Templates** page.</span></span> <span data-ttu-id="37aa2-112">For more information, see [Prepare to Migrate Customer Data](admin-use-templates-to-prepare-customer-data-for-migration.md).</span><span class="sxs-lookup"><span data-stu-id="37aa2-112">For more information, see [Prepare to Migrate Customer Data](admin-use-templates-to-prepare-customer-data-for-migration.md).</span></span> 

## <a name="assign-the-template-to-an-api"></a><span data-ttu-id="37aa2-113">Assign the template to an API</span><span class="sxs-lookup"><span data-stu-id="37aa2-113">Assign the template to an API</span></span>

<span data-ttu-id="37aa2-114">To assign a template to an API, you must go through the following steps.</span><span class="sxs-lookup"><span data-stu-id="37aa2-114">To assign a template to an API, you must go through the following steps.</span></span>

1. <span data-ttu-id="37aa2-115">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **API Setup**, and choose the related link.</span><span class="sxs-lookup"><span data-stu-id="37aa2-115">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **API Setup**, and choose the related link.</span></span>
2. <span data-ttu-id="37aa2-116">Choose **New**, and then choose the **Order** value for the record.</span><span class="sxs-lookup"><span data-stu-id="37aa2-116">Choose **New**, and then choose the **Order** value for the record.</span></span>  
<span data-ttu-id="37aa2-117">If there is more than one template selected for an API (Page ID), the templates are applied in the order defined in the **Order** column.</span><span class="sxs-lookup"><span data-stu-id="37aa2-117">If there is more than one template selected for an API (Page ID), the templates are applied in the order defined in the **Order** column.</span></span>   
<span data-ttu-id="37aa2-118">When each template is applied, field values defined in the template are only applied to fields that have not already had a value defined, either explicitly in the API, or in a previously applied template in the order.</span><span class="sxs-lookup"><span data-stu-id="37aa2-118">When each template is applied, field values defined in the template are only applied to fields that have not already had a value defined, either explicitly in the API, or in a previously applied template in the order.</span></span> 
3. <span data-ttu-id="37aa2-119">Select a **Page ID** value.</span><span class="sxs-lookup"><span data-stu-id="37aa2-119">Select a **Page ID** value.</span></span>  
<span data-ttu-id="37aa2-120">This is the page for the API to which the template will be applied.</span><span class="sxs-lookup"><span data-stu-id="37aa2-120">This is the page for the API to which the template will be applied.</span></span> <span data-ttu-id="37aa2-121">The **Page ID** lookup provides a list of all APIs available in the library.</span><span class="sxs-lookup"><span data-stu-id="37aa2-121">The **Page ID** lookup provides a list of all APIs available in the library.</span></span>
4. <span data-ttu-id="37aa2-122">Select a value in the **Template Code** field.</span><span class="sxs-lookup"><span data-stu-id="37aa2-122">Select a value in the **Template Code** field.</span></span>  
<span data-ttu-id="37aa2-123">The template code is the code for the template that was defined on the **Configuration Templates** page.</span><span class="sxs-lookup"><span data-stu-id="37aa2-123">The template code is the code for the template that was defined on the **Configuration Templates** page.</span></span> <span data-ttu-id="37aa2-124">The template values defined are applied to the API.</span><span class="sxs-lookup"><span data-stu-id="37aa2-124">The template values defined are applied to the API.</span></span> 
5. <span data-ttu-id="37aa2-125">In the **Conditions** field, specify which template should be applied.</span><span class="sxs-lookup"><span data-stu-id="37aa2-125">In the **Conditions** field, specify which template should be applied.</span></span>  
<span data-ttu-id="37aa2-126">The defined template is applied to a new record created through the API if, and only if, the conditions defined in the **Conditions** field are met by the values already defined for the new instance of the entity.</span><span class="sxs-lookup"><span data-stu-id="37aa2-126">The defined template is applied to a new record created through the API if, and only if, the conditions defined in the **Conditions** field are met by the values already defined for the new instance of the entity.</span></span>

## <a name="see-also"></a><span data-ttu-id="37aa2-127">See Also</span><span class="sxs-lookup"><span data-stu-id="37aa2-127">See Also</span></span>
[<span data-ttu-id="37aa2-128">API Documentation</span><span class="sxs-lookup"><span data-stu-id="37aa2-128">API Documentation</span></span>](/dynamics-nav/fin-graph)  
<span data-ttu-id="37aa2-129">[Developing Connect Apps for [!INCLUDE[d365fin_md](includes/d365fin_md.md)]](/dynamics365/business-central/dev-itpro/developer/devenv-develop-connect-apps)</span><span class="sxs-lookup"><span data-stu-id="37aa2-129">[Developing Connect Apps for [!INCLUDE[d365fin_md](includes/d365fin_md.md)]](/dynamics365/business-central/dev-itpro/developer/devenv-develop-connect-apps)</span></span>  
[<span data-ttu-id="37aa2-130">Enabling the APIs</span><span class="sxs-lookup"><span data-stu-id="37aa2-130">Enabling the APIs</span></span>](/dynamics-nav/enabling-apis-for-dynamics-nav)  
[<span data-ttu-id="37aa2-131">Endpoints for the APIs</span><span class="sxs-lookup"><span data-stu-id="37aa2-131">Endpoints for the APIs</span></span>](/dynamics-nav/endpoints-apis-for-dynamics)  
[<span data-ttu-id="37aa2-132">Setting Up a Company with RapidStart Services</span><span class="sxs-lookup"><span data-stu-id="37aa2-132">Setting Up a Company with RapidStart Services</span></span>](admin-set-up-a-company-with-rapidstart.md)  
[<span data-ttu-id="37aa2-133">Administration</span><span class="sxs-lookup"><span data-stu-id="37aa2-133">Administration</span></span>](admin-setup-and-administration.md)
