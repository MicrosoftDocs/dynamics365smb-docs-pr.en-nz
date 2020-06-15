---
title: Upgrading an Integration with Dynamics 365 Sales| Microsoft Docs
description: Learn how to get Dynamics 365 Business Central ready to integrate with Dynamics 365 Sales.
services: project-madeira
documentationcenter: ''
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: sales, crm, integration, integrating
ms.date: 10/01/2019
ms.author: bholtorf
ms.openlocfilehash: 2a5f58ac904ea05f4410ac9e1b804df1cb01c609
ms.sourcegitcommit: 4545bb597dd9dc4c563b30af762977ee1d815497
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 05/29/2020
ms.locfileid: "3410684"
---
# <a name="upgrading-an-integration-with-dynamics-365-sales"></a><span data-ttu-id="67dee-103">Upgrading an Integration with Dynamics 365 Sales</span><span class="sxs-lookup"><span data-stu-id="67dee-103">Upgrading an Integration with Dynamics 365 Sales</span></span>
[!INCLUDE[d365fin](includes/d365fin_md.md)] <span data-ttu-id="67dee-104">integrates with [!INCLUDE[d365fin](includes/cds_long_md.md)], which makes it easy to connect and synchronise data with other Dynamics 365 applications, such as [!INCLUDE[crm_md](includes/crm_md.md)], or even apps that you build yourself.</span><span class="sxs-lookup"><span data-stu-id="67dee-104">integrates with [!INCLUDE[d365fin](includes/cds_long_md.md)], which makes it easy to connect and synchronize data with other Dynamics 365 applications, such as [!INCLUDE[crm_md](includes/crm_md.md)], or even apps that you build yourself.</span></span> <span data-ttu-id="67dee-105">If you are integrating for the first time, we recommend that you do so through [!INCLUDE[d365fin](includes/cds_long_md.md)].</span><span class="sxs-lookup"><span data-stu-id="67dee-105">If you are integrating for the first time, we recommend that you do so through [!INCLUDE[d365fin](includes/cds_long_md.md)].</span></span> <span data-ttu-id="67dee-106">For more information, see [Integration with Common Data Service](admin-common-data-service.md).</span><span class="sxs-lookup"><span data-stu-id="67dee-106">For more information, see [Integration with Common Data Service](admin-common-data-service.md).</span></span>

<span data-ttu-id="67dee-107">If you have already integrated [!INCLUDE[crm_md](includes/crm_md.md)] with [!INCLUDE[d365fin](includes/d365fin_md.md)], you can continue to synchronise data using your setup.</span><span class="sxs-lookup"><span data-stu-id="67dee-107">If you have already integrated [!INCLUDE[crm_md](includes/crm_md.md)] with [!INCLUDE[d365fin](includes/d365fin_md.md)], you can continue to synchronize data using your setup.</span></span> <span data-ttu-id="67dee-108">However, if you upgrade [!INCLUDE[d365fin](includes/d365fin_md.md)], or turn off your [!INCLUDE[crm_md](includes/crm_md.md)] integration, to turn it on again you must connect through [!INCLUDE[d365fin](includes/cds_long_md.md)].</span><span class="sxs-lookup"><span data-stu-id="67dee-108">However, if you upgrade [!INCLUDE[d365fin](includes/d365fin_md.md)], or turn off your [!INCLUDE[crm_md](includes/crm_md.md)] integration, to turn it on again you must connect through [!INCLUDE[d365fin](includes/cds_long_md.md)].</span></span> 

> [!NOTE]
> <span data-ttu-id="67dee-109">Reconnecting through [!INCLUDE[d365fin](includes/cds_long_md.md)] will apply default synchronisation settings, and will overwrite any configurations you have.</span><span class="sxs-lookup"><span data-stu-id="67dee-109">Reconnecting through [!INCLUDE[d365fin](includes/cds_long_md.md)] will apply default synchronization settings, and will overwrite any configurations you have.</span></span> <span data-ttu-id="67dee-110">For example, the default table mappings will be applied.</span><span class="sxs-lookup"><span data-stu-id="67dee-110">For example, the default table mappings will be applied.</span></span>

## <a name="to-upgrade-your-connection-to-use-common-data-service"></a><span data-ttu-id="67dee-111">To upgrade your connection to use Common Data Service</span><span class="sxs-lookup"><span data-stu-id="67dee-111">To upgrade your connection to use Common Data Service</span></span>
1. <span data-ttu-id="67dee-112">Open the **Microsoft Dynamics 365 Connection Setup** page, choose the **Enable** toggle to turn off your existing connection to [!INCLUDE[crm_md](includes/crm_md.md)].</span><span class="sxs-lookup"><span data-stu-id="67dee-112">Open the **Microsoft Dynamics 365 Connection Setup** page, choose the **Enable** toggle to turn off your existing connection to [!INCLUDE[crm_md](includes/crm_md.md)].</span></span>
2. <span data-ttu-id="67dee-113">Open the **Common Data Service Connection Setup** page, and choose the **Enable** toggle to turn on the connection.</span><span class="sxs-lookup"><span data-stu-id="67dee-113">Open the **Common Data Service Connection Setup** page, and choose the **Enable** toggle to turn on the connection.</span></span>
  
   <span data-ttu-id="67dee-114">After you enable the CDS connection, the Business Central CDS Base Integration Solution is deployed to Common Data Service.</span><span class="sxs-lookup"><span data-stu-id="67dee-114">After you enable the CDS connection, the Business Central CDS Base Integration Solution is deployed to Common Data Service.</span></span>
3. <span data-ttu-id="67dee-115">Uninstall the Microsoft Dynamics 365 Business Central Integration solution from your Dynamics 365 Sales following [Uninstall or delete a solution topic](/powerapps/developer/common-data-service/uninstall-delete-solution)</span><span class="sxs-lookup"><span data-stu-id="67dee-115">Uninstall the Microsoft Dynamics 365 Business Central Integration solution from your Dynamics 365 Sales following [Uninstall or delete a solution topic](/powerapps/developer/common-data-service/uninstall-delete-solution)</span></span> 

4. <span data-ttu-id="67dee-116">On the Microsoft Dynamics 365 Connection Setup page, choose the Enable toggle to turn on the connection to [!INCLUDE[crm_md](includes/crm_md.md)].</span><span class="sxs-lookup"><span data-stu-id="67dee-116">On the Microsoft Dynamics 365 Connection Setup page, choose the Enable toggle to turn on the connection to [!INCLUDE[crm_md](includes/crm_md.md)].</span></span>
  
   <span data-ttu-id="67dee-117">After you enable the Sales connection, the Business Central Integration Solution is deployed to Sales.</span><span class="sxs-lookup"><span data-stu-id="67dee-117">After you enable the Sales connection, the Business Central Integration Solution is deployed to Sales.</span></span> <span data-ttu-id="67dee-118">This enables integration with entities that are specific to [!INCLUDE[crm_md](includes/crm_md.md)], such as sales orders, quotes, and invoices.</span><span class="sxs-lookup"><span data-stu-id="67dee-118">This enables integration with entities that are specific to [!INCLUDE[crm_md](includes/crm_md.md)], such as sales orders, quotes, and invoices.</span></span>
5. <span data-ttu-id="67dee-119">Choose **Redeploy Integration Solution** to install and configure the upgraded Business Central Integration Solution.</span><span class="sxs-lookup"><span data-stu-id="67dee-119">Choose **Redeploy Integration Solution** to install and configure the upgraded Business Central Integration Solution.</span></span>
6. <span data-ttu-id="67dee-120">On the **Sales Connection Setup** page, choose **Use Default Synchronisation Setup** to initialise the integration table mappings for [!INCLUDE[crm_md](includes/crm_md.md)].</span><span class="sxs-lookup"><span data-stu-id="67dee-120">On the **Sales Connection Setup** page, choose **Use Default Synchronization Setup** to initialize the integration table mappings for [!INCLUDE[crm_md](includes/crm_md.md)].</span></span>

## <a name="see-also"></a><span data-ttu-id="67dee-121">See Also</span><span class="sxs-lookup"><span data-stu-id="67dee-121">See Also</span></span>
[<span data-ttu-id="67dee-122">Integrating with Dynamics 365 Sales</span><span class="sxs-lookup"><span data-stu-id="67dee-122">Integrating with Dynamics 365 Sales</span></span>](admin-prepare-dynamics-365-for-sales-for-integration.md)  
[<span data-ttu-id="67dee-123">Integrating with Common Data Service</span><span class="sxs-lookup"><span data-stu-id="67dee-123">Integrating with Common Data Service</span></span>](admin-common-data-service.md)
