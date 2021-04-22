---
title: Upgrading an Integration with Dynamics 365 Sales
description: Learn how to move your Dynamics 365 Business Central integration with Dynamics 365 Sales to the latest version.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: sales, crm, integration, integrating
ms.date: 04/01/2021
ms.author: bholtorf
ms.openlocfilehash: 4e3b79d6245a0f1b8277c94faa58c24edc66662e
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 03/31/2021
ms.locfileid: "5777032"
---
# <a name="upgrading-an-integration-with-dynamics-365-sales"></a>Upgrading an Integration with Dynamics 365 Sales
[!INCLUDE[prod_short](includes/prod_short.md)] integrates with [!INCLUDE[prod_short](includes/cds_long_md.md)], which makes it easy to connect and synchronise data with other Dynamics 365 applications, such as [!INCLUDE[crm_md](includes/crm_md.md)], or even apps that you build yourself. If you are integrating for the first time, we recommend that you do so through [!INCLUDE[prod_short](includes/cds_long_md.md)]. For more information, see [Integration with Dataverse](admin-common-data-service.md).

If you have already integrated [!INCLUDE[crm_md](includes/crm_md.md)] with [!INCLUDE[prod_short](includes/prod_short.md)], you can continue to synchronise data using your setup. However, if you upgrade [!INCLUDE[prod_short](includes/prod_short.md)], or turn off your [!INCLUDE[crm_md](includes/crm_md.md)] integration, to turn it on again you must connect through [!INCLUDE[prod_short](includes/cds_long_md.md)]. 

> [!NOTE]
> Reconnecting through [!INCLUDE[prod_short](includes/cds_long_md.md)] will apply default synchronisation settings, and will overwrite any configurations you have. For example, the default table mappings will be applied.

## <a name="to-upgrade-your-connection-to-use-dataverse"></a>To upgrade your connection to use Dataverse
1. Open the **Microsoft Dynamics 365 Connection Setup** page, and then turn off the **Enabled** toggle to disconnect from [!INCLUDE[crm_md](includes/crm_md.md)].
2. Open the **Dataverse Connection Setup** page, and choose the **Enabled** toggle to turn on the connection to [!INCLUDE[prod_short](includes/cds_long_md.md)].
  
   > [!NOTE]
   > After you enable the connection, the Business Central Integration Solution is deployed to Dataverse.
3. Choose **Redeploy Integration Solution** to reinstall the Business Central Integration Solution.
4. On the **Microsoft Dynamics 365 Connection Setup** page, turn on the **Enabled** toggle to reconnect to [!INCLUDE[crm_md](includes/crm_md.md)].
  
   > [!NOTE]
   > After you enable the connection, the Business Central Integration Solution is deployed to [!INCLUDE[prod_short](includes/prod_short.md)]. This enables integration with tables that are specific to [!INCLUDE[crm_md](includes/crm_md.md)], such as sales orders, quotes, and invoices.
5. Choose **Redeploy Integration Solution** to reinstall the Business Central Integration Solution.
6. On the **Sales Connection Setup** page, choose **Use Default Synchronisation Setup** to initialise the integration table mappings for [!INCLUDE[crm_md](includes/crm_md.md)].

## <a name="see-also"></a>See Also
[Integrating with Dynamics 365 Sales](admin-prepare-dynamics-365-for-sales-for-integration.md)  
[Integrating with Microsoft Dataverse](admin-common-data-service.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]