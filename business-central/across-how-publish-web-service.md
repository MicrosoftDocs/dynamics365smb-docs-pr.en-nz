---
title: Expose objects as web services | Microsoft Docs
description: Publish objects as web services to make them immediately available for your Business Central solution.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2019
ms.author: edupont
ms.openlocfilehash: 05a414d6f12243f55105863b66d9b6e759a29189
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 10/01/2019
ms.locfileid: "2305721"
---
# <a name="publish-a-web-service"></a><span data-ttu-id="726a6-103">Publish a Web Service</span><span class="sxs-lookup"><span data-stu-id="726a6-103">Publish a Web Service</span></span>

<span data-ttu-id="726a6-104">Web services are a lightweight way to make application functionality available to a variety of external systems and users.</span><span class="sxs-lookup"><span data-stu-id="726a6-104">Web services are a lightweight way to make application functionality available to a variety of external systems and users.</span></span> [!INCLUDE[d365fin](includes/d365fin_md.md)] <span data-ttu-id="726a6-105">includes an number of objects that are exposed as web services by default due to integration with other Microsoft services, but you can also add other web services.</span><span class="sxs-lookup"><span data-stu-id="726a6-105">includes an number of objects that are exposed as web services by default due to integration with other Microsoft services, but you can also add other web services.</span></span>  

<span data-ttu-id="726a6-106">You set up a web service in the [!INCLUDE[d365fin](includes/d365fin_md.md)] client.</span><span class="sxs-lookup"><span data-stu-id="726a6-106">You set up a web service in the [!INCLUDE[d365fin](includes/d365fin_md.md)] client.</span></span> <span data-ttu-id="726a6-107">You must then publish the web service so that it is available to service requests over the network.</span><span class="sxs-lookup"><span data-stu-id="726a6-107">You must then publish the web service so that it is available to service requests over the network.</span></span> <span data-ttu-id="726a6-108">Users can discover web services by pointing a browser at the server location and requesting a list of available services.</span><span class="sxs-lookup"><span data-stu-id="726a6-108">Users can discover web services by pointing a browser at the server location and requesting a list of available services.</span></span> <span data-ttu-id="726a6-109">When you publish a web service, it is immediately available over the network for authenticated users.</span><span class="sxs-lookup"><span data-stu-id="726a6-109">When you publish a web service, it is immediately available over the network for authenticated users.</span></span> <span data-ttu-id="726a6-110">All authorised users can access metadata for web services, but only users who have sufficient permissions can access actual data.</span><span class="sxs-lookup"><span data-stu-id="726a6-110">All authorized users can access metadata for web services, but only users who have sufficient permissions can access actual data.</span></span>

## <a name="creating-and-publishing-a-web-service"></a><span data-ttu-id="726a6-111">Creating and Publishing a Web Service</span><span class="sxs-lookup"><span data-stu-id="726a6-111">Creating and Publishing a Web Service</span></span>  
<span data-ttu-id="726a6-112">The following steps explain how to create and publish a web service.</span><span class="sxs-lookup"><span data-stu-id="726a6-112">The following steps explain how to create and publish a web service.</span></span>  

### <a name="to-create-and-publish-a-web-service"></a><span data-ttu-id="726a6-113">To create and publish a web service</span><span class="sxs-lookup"><span data-stu-id="726a6-113">To create and publish a web service</span></span>  

1. <span data-ttu-id="726a6-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Web Services**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="726a6-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Web Services**, and then choose the related link.</span></span>  
2. <span data-ttu-id="726a6-115">On the **Web Services** page, choose **New**.</span><span class="sxs-lookup"><span data-stu-id="726a6-115">On the **Web Services** page, choose **New**.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

    > [!NOTE]  
    > <span data-ttu-id="726a6-116">**Codeunit** and **Page** are valid types for SOAP web services.</span><span class="sxs-lookup"><span data-stu-id="726a6-116">**Codeunit** and **Page** are valid types for SOAP web services.</span></span> <span data-ttu-id="726a6-117">**Page** and **Query** are valid types for OData web services.</span><span class="sxs-lookup"><span data-stu-id="726a6-117">**Page** and **Query** are valid types for OData web services.</span></span>  
    > <span data-ttu-id="726a6-118">Also, if the database contains multiple companies, you can choose an object ID that is specific to one of the companies.</span><span class="sxs-lookup"><span data-stu-id="726a6-118">Also, if the database contains multiple companies, you can choose an object ID that is specific to one of the companies.</span></span>  
    > <span data-ttu-id="726a6-119">Finally, the service name is visible to consumers of your web service and is the basis for identifying and distinguishing web services, so you should make the name meaningful.</span><span class="sxs-lookup"><span data-stu-id="726a6-119">Finally, the service name is visible to consumers of your web service and is the basis for identifying and distinguishing web services, so you should make the name meaningful.</span></span>

3. <span data-ttu-id="726a6-120">Select the check box in the **Published** column.</span><span class="sxs-lookup"><span data-stu-id="726a6-120">Select the check box in the **Published** column.</span></span>  

<span data-ttu-id="726a6-121">When you publish the web service, in the **OData URL** and **SOAP URL** fields, you can see the URLs that are generated for the web service.</span><span class="sxs-lookup"><span data-stu-id="726a6-121">When you publish the web service, in the **OData URL** and **SOAP URL** fields, you can see the URLs that are generated for the web service.</span></span> <span data-ttu-id="726a6-122">You can test the web service immediately by choosing the links in the **OData URL** and **SOAP URL** fields.</span><span class="sxs-lookup"><span data-stu-id="726a6-122">You can test the web service immediately by choosing the links in the **OData URL** and **SOAP URL** fields.</span></span> <span data-ttu-id="726a6-123">Optionally, you can copy the value of the field and save it for later use.</span><span class="sxs-lookup"><span data-stu-id="726a6-123">Optionally, you can copy the value of the field and save it for later use.</span></span>  

> [!IMPORTANT]
> <span data-ttu-id="726a6-124">For codeunits that are published as a SOAP web service, the methods exposed in the codeunit must be marked as `[External]` in the code.</span><span class="sxs-lookup"><span data-stu-id="726a6-124">For codeunits that are published as a SOAP web service, the methods exposed in the codeunit must be marked as `[External]` in the code.</span></span>

<span data-ttu-id="726a6-125">After you publish a web service, it is available to external parties.</span><span class="sxs-lookup"><span data-stu-id="726a6-125">After you publish a web service, it is available to external parties.</span></span> <span data-ttu-id="726a6-126">You can verify the availability of that web service by using a browser, or you can choose the link in the **OData URL** and **SOAP URL** fields on the **Web Services** page.</span><span class="sxs-lookup"><span data-stu-id="726a6-126">You can verify the availability of that web service by using a browser, or you can choose the link in the **OData URL** and **SOAP URL** fields on the **Web Services** page.</span></span> <span data-ttu-id="726a6-127">The following procedure illustrates how you can verify the availability of the web service for later use.</span><span class="sxs-lookup"><span data-stu-id="726a6-127">The following procedure illustrates how you can verify the availability of the web service for later use.</span></span>  

### <a name="to-verify-the-availability-of-a-web-service"></a><span data-ttu-id="726a6-128">To verify the availability of a web service</span><span class="sxs-lookup"><span data-stu-id="726a6-128">To verify the availability of a web service</span></span>  

1. <span data-ttu-id="726a6-129">In your browser, enter the relevant URL.</span><span class="sxs-lookup"><span data-stu-id="726a6-129">In your browser, enter the relevant URL.</span></span> <span data-ttu-id="726a6-130">The following table illustrates the types of URLs that you can enter for different web service types.</span><span class="sxs-lookup"><span data-stu-id="726a6-130">The following table illustrates the types of URLs that you can enter for different web service types.</span></span>  

    > [!div class="mx-tdBreakAll"]
    > |<span data-ttu-id="726a6-131">Type</span><span class="sxs-lookup"><span data-stu-id="726a6-131">Type</span></span>|<span data-ttu-id="726a6-132">Syntax</span><span class="sxs-lookup"><span data-stu-id="726a6-132">Syntax</span></span>|<span data-ttu-id="726a6-133">Example</span><span class="sxs-lookup"><span data-stu-id="726a6-133">Example</span></span>|
    > |----------------|------|-------|
    > |<span data-ttu-id="726a6-134">SOAP</span><span class="sxs-lookup"><span data-stu-id="726a6-134">SOAP</span></span> |<span data-ttu-id="726a6-135">https://api.businesscentral.dynamics.com/*version*/*tenant*/WS/*CompanyName*/*entity*/</span><span class="sxs-lookup"><span data-stu-id="726a6-135">https://api.businesscentral.dynamics.com/*version*/*tenant*/WS/*CompanyName*/*entity*/</span></span> |`https://api.businesscentral.dynamics.com/v1.0/a10b3ee6-d9a2-42fe-926f-946e23bb8ddd/WS/CRONUS%20USA%2C%20Inc./Page/InvoiceDocument`|
    > |<span data-ttu-id="726a6-136">OData V4</span><span class="sxs-lookup"><span data-stu-id="726a6-136">OData V4</span></span>|<span data-ttu-id="726a6-137">https://api.businesscentral.dynamics.com/*version*/*tenant*/ODataV4/Company('*CompanyName*')/*entity*</span><span class="sxs-lookup"><span data-stu-id="726a6-137">https://api.businesscentral.dynamics.com/*version*/*tenant*/ODataV4/Company('*CompanyName*')/*entity*</span></span>|`https://api.businesscentral.dynamics.com/v1.0/a10b3ee6-d9a2-42fe-926f-946e23bb8ddd/ODataV4/Company('CRONUS%20USA%2C%20Inc.')/InvoiceDocument`<br/>    <span data-ttu-id="726a6-138">The company name is case-sensitive.</span><span class="sxs-lookup"><span data-stu-id="726a6-138">The company name is case-sensitive.</span></span>|

2. <span data-ttu-id="726a6-139">Review the information that is displayed in the browser.</span><span class="sxs-lookup"><span data-stu-id="726a6-139">Review the information that is displayed in the browser.</span></span> <span data-ttu-id="726a6-140">Verify that you can see the name of the web service that you have created.</span><span class="sxs-lookup"><span data-stu-id="726a6-140">Verify that you can see the name of the web service that you have created.</span></span>  

<span data-ttu-id="726a6-141">When you access a web service, and you want to write data back to [!INCLUDE[d365fin](includes/d365fin_md.md)], you must specify the company name.</span><span class="sxs-lookup"><span data-stu-id="726a6-141">When you access a web service, and you want to write data back to [!INCLUDE[d365fin](includes/d365fin_md.md)], you must specify the company name.</span></span> <span data-ttu-id="726a6-142">You can specify the company as part of the URI as shown in the examples, or you can specify the company as part of the query parameters.</span><span class="sxs-lookup"><span data-stu-id="726a6-142">You can specify the company as part of the URI as shown in the examples, or you can specify the company as part of the query parameters.</span></span> <span data-ttu-id="726a6-143">For example, the following URIs point to the same OData web service and are both valid URIs.</span><span class="sxs-lookup"><span data-stu-id="726a6-143">For example, the following URIs point to the same OData web service and are both valid URIs.</span></span>  

```
https://api.businesscentral.dynamics.com/v1.0/OData/Company('CRONUS International Ltd.')/Customer  
```

```
https://api.businesscentral.dynamics.com/v1.0/OData/Customer?company='CRONUS International Ltd.'  
```

## <a name="see-also"></a><span data-ttu-id="726a6-144">See Also</span><span class="sxs-lookup"><span data-stu-id="726a6-144">See Also</span></span>

[<span data-ttu-id="726a6-145">Administration</span><span class="sxs-lookup"><span data-stu-id="726a6-145">Administration</span></span>](admin-setup-and-administration.md)  
[<span data-ttu-id="726a6-146">Business Central Web Services for developers</span><span class="sxs-lookup"><span data-stu-id="726a6-146">Business Central Web Services for developers</span></span>](/dynamics365/business-central/dev-itpro/webservices/web-services)  
