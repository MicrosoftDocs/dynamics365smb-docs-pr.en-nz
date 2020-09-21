---
title: Expose objects as web services | Microsoft Docs
description: Publish objects as web services to make them immediately available for your Business Central solution.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: ''
ms.date: 05/19/2020
ms.author: edupont
ms.openlocfilehash: 230f3a7fc11e19813d77da2ff15388433642c744
ms.sourcegitcommit: aeaa0dc64e54432a70c4b0e1faf325cd17d01389
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 08/17/2020
ms.locfileid: "3697663"
---
# <a name="publish-a-web-service"></a><span data-ttu-id="1d060-103">Publish a Web Service</span><span class="sxs-lookup"><span data-stu-id="1d060-103">Publish a Web Service</span></span>

<span data-ttu-id="1d060-104">Web services are a lightweight way to make application functionality available to a variety of external systems and users.</span><span class="sxs-lookup"><span data-stu-id="1d060-104">Web services are a lightweight way to make application functionality available to a variety of external systems and users.</span></span> [!INCLUDE[d365fin](includes/d365fin_md.md)] <span data-ttu-id="1d060-105">includes an number of objects that are exposed as web services by default due to integration with other Microsoft services, but you can also add other web services.</span><span class="sxs-lookup"><span data-stu-id="1d060-105">includes an number of objects that are exposed as web services by default due to integration with other Microsoft services, but you can also add other web services.</span></span>  

<span data-ttu-id="1d060-106">You set up a web service in the [!INCLUDE[d365fin](includes/d365fin_md.md)] client.</span><span class="sxs-lookup"><span data-stu-id="1d060-106">You set up a web service in the [!INCLUDE[d365fin](includes/d365fin_md.md)] client.</span></span> <span data-ttu-id="1d060-107">You must then publish the web service so that it is available to service requests over the network.</span><span class="sxs-lookup"><span data-stu-id="1d060-107">You must then publish the web service so that it is available to service requests over the network.</span></span> <span data-ttu-id="1d060-108">Users can discover web services by pointing a browser at the server location and requesting a list of available services.</span><span class="sxs-lookup"><span data-stu-id="1d060-108">Users can discover web services by pointing a browser at the server location and requesting a list of available services.</span></span> <span data-ttu-id="1d060-109">When you publish a web service, it is immediately available over the network for authenticated users.</span><span class="sxs-lookup"><span data-stu-id="1d060-109">When you publish a web service, it is immediately available over the network for authenticated users.</span></span> <span data-ttu-id="1d060-110">All authorised users can access metadata for web services, but only users who have sufficient permissions can access actual data.</span><span class="sxs-lookup"><span data-stu-id="1d060-110">All authorized users can access metadata for web services, but only users who have sufficient permissions can access actual data.</span></span>

## <a name="creating-and-publishing-a-web-service"></a><span data-ttu-id="1d060-111">Creating and Publishing a Web Service</span><span class="sxs-lookup"><span data-stu-id="1d060-111">Creating and Publishing a Web Service</span></span>

<span data-ttu-id="1d060-112">The following steps explain how to create and publish a web service.</span><span class="sxs-lookup"><span data-stu-id="1d060-112">The following steps explain how to create and publish a web service.</span></span>  

<!--
    You can also create a new web service URL in [!INCLUDE [prodshort](includes/prodshort.md)] instead. Choose one of the following methods:

      - Use the **Create Data Set** action on the **Web Services** page
      - Use the **Set Up Reporting** Assisted Setup guide
      - Choose the **Edit in Excel** action in any lists
    -->

### <a name="to-create-and-publish-a-web-service"></a><span data-ttu-id="1d060-113">To create and publish a web service</span><span class="sxs-lookup"><span data-stu-id="1d060-113">To create and publish a web service</span></span>  

1. <span data-ttu-id="1d060-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Web Services**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="1d060-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Web Services**, and then choose the related link.</span></span>  
2. <span data-ttu-id="1d060-115">On the **Web Services** page, choose **New**.</span><span class="sxs-lookup"><span data-stu-id="1d060-115">On the **Web Services** page, choose **New**.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

    > [!NOTE]  
    > <span data-ttu-id="1d060-116">**Codeunit** and **Page** are valid types for SOAP web services.</span><span class="sxs-lookup"><span data-stu-id="1d060-116">**Codeunit** and **Page** are valid types for SOAP web services.</span></span> <span data-ttu-id="1d060-117">**Page** and **Query** are valid types for OData web services.</span><span class="sxs-lookup"><span data-stu-id="1d060-117">**Page** and **Query** are valid types for OData web services.</span></span>  
    > <span data-ttu-id="1d060-118">Also, if the database contains multiple companies, you can choose an object ID that is specific to one of the companies.</span><span class="sxs-lookup"><span data-stu-id="1d060-118">Also, if the database contains multiple companies, you can choose an object ID that is specific to one of the companies.</span></span>  
    > <span data-ttu-id="1d060-119">Finally, the service name is visible to consumers of your web service and is the basis for identifying and distinguishing web services, so you should make the name meaningful.</span><span class="sxs-lookup"><span data-stu-id="1d060-119">Finally, the service name is visible to consumers of your web service and is the basis for identifying and distinguishing web services, so you should make the name meaningful.</span></span>

3. <span data-ttu-id="1d060-120">Select the check box in the **Published** column.</span><span class="sxs-lookup"><span data-stu-id="1d060-120">Select the check box in the **Published** column.</span></span>  

<span data-ttu-id="1d060-121">When you publish the web service, in the **OData URL** and **SOAP URL** fields, you can see the URLs that are generated for the web service.</span><span class="sxs-lookup"><span data-stu-id="1d060-121">When you publish the web service, in the **OData URL** and **SOAP URL** fields, you can see the URLs that are generated for the web service.</span></span> <span data-ttu-id="1d060-122">You can test the web service immediately by choosing the links in the **OData URL** and **SOAP URL** fields.</span><span class="sxs-lookup"><span data-stu-id="1d060-122">You can test the web service immediately by choosing the links in the **OData URL** and **SOAP URL** fields.</span></span> <span data-ttu-id="1d060-123">Optionally, you can copy the value of the field and save it for later use.</span><span class="sxs-lookup"><span data-stu-id="1d060-123">Optionally, you can copy the value of the field and save it for later use.</span></span>  

> [!NOTE]
> <span data-ttu-id="1d060-124">If the objects that you expose as web services must not be accessible from [!INCLUDE[prodshort](includes/prodshort.md)] online, you must mark the methods exposed in the code as `[Scope('OnPrem')]`.</span><span class="sxs-lookup"><span data-stu-id="1d060-124">If the objects that you expose as web services must not be accessible from [!INCLUDE[prodshort](includes/prodshort.md)] online, you must mark the methods exposed in the code as `[Scope('OnPrem')]`.</span></span> <span data-ttu-id="1d060-125">For more information, see [Scope Attribute](/dynamics365/business-central/dev-itpro/developer/methods/devenv-scope-attribute).</span><span class="sxs-lookup"><span data-stu-id="1d060-125">For more information, see [Scope Attribute](/dynamics365/business-central/dev-itpro/developer/methods/devenv-scope-attribute).</span></span>

<span data-ttu-id="1d060-126">After you publish a web service, it is available to external parties.</span><span class="sxs-lookup"><span data-stu-id="1d060-126">After you publish a web service, it is available to external parties.</span></span> <span data-ttu-id="1d060-127">You can verify the availability of that web service by using a browser, or you can choose the link in the **OData URL** and **SOAP URL** fields on the **Web Services** page.</span><span class="sxs-lookup"><span data-stu-id="1d060-127">You can verify the availability of that web service by using a browser, or you can choose the link in the **OData URL** and **SOAP URL** fields on the **Web Services** page.</span></span> <span data-ttu-id="1d060-128">The following procedure illustrates how you can verify the availability of the web service for later use.</span><span class="sxs-lookup"><span data-stu-id="1d060-128">The following procedure illustrates how you can verify the availability of the web service for later use.</span></span>  

### <a name="to-verify-the-availability-of-a-web-service"></a><span data-ttu-id="1d060-129">To verify the availability of a web service</span><span class="sxs-lookup"><span data-stu-id="1d060-129">To verify the availability of a web service</span></span>  

1. <span data-ttu-id="1d060-130">In your browser, enter the relevant URL.</span><span class="sxs-lookup"><span data-stu-id="1d060-130">In your browser, enter the relevant URL.</span></span> <span data-ttu-id="1d060-131">The following table illustrates the types of URLs that you can enter for different web service types.</span><span class="sxs-lookup"><span data-stu-id="1d060-131">The following table illustrates the types of URLs that you can enter for different web service types.</span></span>  

    > [!div class="mx-tdBreakAll"]
    > |<span data-ttu-id="1d060-132">Type</span><span class="sxs-lookup"><span data-stu-id="1d060-132">Type</span></span>|<span data-ttu-id="1d060-133">Syntax</span><span class="sxs-lookup"><span data-stu-id="1d060-133">Syntax</span></span>|<span data-ttu-id="1d060-134">Example</span><span class="sxs-lookup"><span data-stu-id="1d060-134">Example</span></span>|
    > |----------------|------|-------|
    > |<span data-ttu-id="1d060-135">SOAP</span><span class="sxs-lookup"><span data-stu-id="1d060-135">SOAP</span></span>|`https://api.businesscentral.dynamics.com/*version*/*tenant*/Production/WS/*CompanyName*/*entity*/` |`https://api.businesscentral.dynamics.com/v2.0/7acc9d3d-d354-4616-8bbd-c4fc9f2b15b3/Production/WS/CRONUS%20USA%2C%20Inc./Page/InvoiceDocument`|
    > |<span data-ttu-id="1d060-136">OData V4</span><span class="sxs-lookup"><span data-stu-id="1d060-136">OData V4</span></span>|`https://api.businesscentral.dynamics.com/*version*/*tenant*/Production/ODataV4/Company('*CompanyName*')/*entity*`|`https://api.businesscentral.dynamics.com/v2.0/7acc9d3d-d354-4616-8bbd-c4fc9f2b15b3/Production/ODataV4/Company('CRONUS%20USA%2C%20Inc.')/InvoiceDocument`<br/>    <span data-ttu-id="1d060-137">The company name is case-sensitive.</span><span class="sxs-lookup"><span data-stu-id="1d060-137">The company name is case-sensitive.</span></span>|

2. <span data-ttu-id="1d060-138">Review the information that is displayed in the browser.</span><span class="sxs-lookup"><span data-stu-id="1d060-138">Review the information that is displayed in the browser.</span></span> <span data-ttu-id="1d060-139">Verify that you can see the name of the web service that you have created.</span><span class="sxs-lookup"><span data-stu-id="1d060-139">Verify that you can see the name of the web service that you have created.</span></span>  

<span data-ttu-id="1d060-140">When you access a web service, and you want to write data back to [!INCLUDE[d365fin](includes/d365fin_md.md)], you must specify the company name.</span><span class="sxs-lookup"><span data-stu-id="1d060-140">When you access a web service, and you want to write data back to [!INCLUDE[d365fin](includes/d365fin_md.md)], you must specify the company name.</span></span> <span data-ttu-id="1d060-141">You can specify the company as part of the URI as shown in the examples, or you can specify the company as part of the query parameters.</span><span class="sxs-lookup"><span data-stu-id="1d060-141">You can specify the company as part of the URI as shown in the examples, or you can specify the company as part of the query parameters.</span></span> <span data-ttu-id="1d060-142">For example, the following URIs point to the same OData web service and are both valid URIs.</span><span class="sxs-lookup"><span data-stu-id="1d060-142">For example, the following URIs point to the same OData web service and are both valid URIs.</span></span>  

```
https://api.businesscentral.dynamics.com/v1.0/OData/Company('CRONUS International Ltd.')/Customer  
```

```
https://api.businesscentral.dynamics.com/v1.0/OData/Customer?company='CRONUS International Ltd.'  
```

## <a name="see-also"></a><span data-ttu-id="1d060-143">See Also</span><span class="sxs-lookup"><span data-stu-id="1d060-143">See Also</span></span>

[<span data-ttu-id="1d060-144">Administration</span><span class="sxs-lookup"><span data-stu-id="1d060-144">Administration</span></span>](admin-setup-and-administration.md)  
[<span data-ttu-id="1d060-145">Business Central Web Services for developers</span><span class="sxs-lookup"><span data-stu-id="1d060-145">Business Central Web Services for developers</span></span>](/dynamics365/business-central/dev-itpro/webservices/web-services)  
[<span data-ttu-id="1d060-146">OData request limits</span><span class="sxs-lookup"><span data-stu-id="1d060-146">OData request limits</span></span>](/dynamics365/business-central/dev-itpro/administration/operational-limits-online#ODataServices)  
