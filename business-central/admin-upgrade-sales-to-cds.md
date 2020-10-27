---
title: Upgrading an Integration with Dynamics 365 Sales
description: Learn how to move your Dynamics 365 Business Central integration with Dynamics 365 Sales to the latest version.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: sales, crm, integration, integrating
ms.date: 10/01/2020
ms.author: bholtorf
ms.openlocfilehash: 3bb6b26e011afc515fbd4f492f56b3090c56e860
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 10/01/2020
ms.locfileid: "3922383"
---
# <a name="upgrading-an-integration-with-dynamics-365-sales"></a>Upgrading an Integration with Dynamics 365 Sales
[!INCLUDE[d365fin](includes/d365fin_md.md)] integrates with [!INCLUDE[d365fin](includes/cds_long_md.md)], which makes it easy to connect and synchronise data with other Dynamics 365 applications, such as [!INCLUDE[crm_md](includes/crm_md.md)], or even apps that you build yourself. If you are integrating for the first time, we recommend that you do so through [!INCLUDE[d365fin](includes/cds_long_md.md)]. For more information, see [Integration with Common Data Service](admin-common-data-service.md).

If you have already integrated [!INCLUDE[crm_md](includes/crm_md.md)] with [!INCLUDE[d365fin](includes/d365fin_md.md)], you can continue to synchronise data using your setup. However, if you upgrade [!INCLUDE[d365fin](includes/d365fin_md.md)], or turn off your [!INCLUDE[crm_md](includes/crm_md.md)] integration, to turn it on again you must connect through [!INCLUDE[d365fin](includes/cds_long_md.md)]. 

> [!NOTE]
> Reconnecting through [!INCLUDE[d365fin](includes/cds_long_md.md)] will apply default synchronisation settings, and will overwrite any configurations you have. For example, the default table mappings will be applied.

## <a name="to-upgrade-your-connection-to-use-common-data-service"></a>To upgrade your connection to use Common Data Service
1. Open the **Microsoft Dynamics 365 Connection Setup** page, choose the **Enable** toggle to turn off your existing connection to [!INCLUDE[crm_md](includes/crm_md.md)].
2. Open the **Common Data Service Connection Setup** page, and choose the **Enable** toggle to turn on the connection.
  
   After you enable the CDS connection, the Business Central CDS Base Integration Solution is deployed to Common Data Service.
3. Uninstall the Microsoft Dynamics 365 Business Central Integration solution from your Dynamics 365 Sales. For more information, see [Uninstall or delete a solution topic](/powerapps/developer/common-data-service/uninstall-delete-solution). 

4. On the **Microsoft Dynamics 365 Connection Setup** page, turn on the **Enable** toggle to connect to [!INCLUDE[crm_md](includes/crm_md.md)].
  
   After you enable the Sales connection, the Business Central Integration Solution is deployed to Sales. This enables integration with entities that are specific to [!INCLUDE[crm_md](includes/crm_md.md)], such as sales orders, quotes, and invoices.
5. On the **Sales Connection Setup** page, choose **Use Default Synchronisation Setup** to initialise the integration table mappings for [!INCLUDE[crm_md](includes/crm_md.md)].

## <a name="see-also"></a>See Also
[Integrating with Dynamics 365 Sales](admin-prepare-dynamics-365-for-sales-for-integration.md)  
[Integrating with Common Data Service](admin-common-data-service.md)
