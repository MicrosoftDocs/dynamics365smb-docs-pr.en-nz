---
title: Use Your Data to Create an App| Microsoft Docs
description: You can make your Business Central data available as a data source and specify an OData URL of your web services to build a business app using Power Apps.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: OData, Power App, SOAP
ms.date: 06/22/2020
ms.author: edupont
ms.openlocfilehash: 8f0eb7a1562a8300bd7181ef6470c70f60934470
ms.sourcegitcommit: 3e9c89f90db5eaed599630299353300621fe4007
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 07/01/2020
ms.locfileid: "3528654"
---
# <a name="connecting-to-your-business-central-data-to-build-a-business-app-using-power-apps"></a>Connecting to Your Business Central Data to Build a Business App Using Power Apps

You can make your [!INCLUDE[prodshort](includes/prodshort.md)] data available as a data source in Power Apps.  

> [!NOTE]  
> You must have a valid account with [!INCLUDE[prodshort](includes/prodshort.md)] and with Power Apps.  

## <a name="to-add-prodshort-as-a-data-source-in-power-apps"></a>To add [!INCLUDE[prodshort](includes/prodshort.md)] as a data source in Power Apps

1. In your browser, navigate to [powerapps.microsoft.com](https://powerapps.microsoft.com/), and then sign in.
2. On the Home page, in the **Start from data** section, choose the **Other data sources** tile.  

    This opens Power Apps Studio. On first login, you must specify the country/region.  
3. In the list of available connections, choose **Business Central**, and then choose the **Create** button.

    Power Apps will connect to your [!INCLUDE[prodshort](includes/prodshort.md)] using the credentials that you are signed in with. If you are not an administrator of your [!INCLUDE[prodshort](includes/prodshort.md)], you may have to sign in with another account.  

4. Power Apps will display a list of *Environments and companies* that are available from [!INCLUDE[prodshort](includes/prodshort.md)]. Choose the environment and company that contains the data you want to connect to, such as *PRODUCTION - My Company*.  

5. Next, you will be presented with a list of tables that are exposed as part of the API for your environment. Select the table that you want to connect to, and then choose **Connect**.

These so-called tables are exposed as endpoints by the [!INCLUDE[prodshort](includes/prodshort.md)] connector for Power Apps.  

> [!NOTE]
> If you want to include data from other tables in [!INCLUDE[prodshort](includes/prodshort.md)] in your app, then you must work with a developer to define a custom API in [!INCLUDE[prodshort](includes/prodshort.md)] and then consume that custom API through a custom connector in Power Apps. For more information, see [Create a custom connector from scratch](/connectors/custom-connectors/define-blank).  

At this point, you have successfully connected to your [!INCLUDE[prodshort](includes/prodshort.md)] data and are ready to begin building your PowerApp. You can add additional screens and connect to additional data from your [!INCLUDE[prodshort](includes/prodshort.md)]. For more information, see [Create a canvas app from a sample in Power Apps](/powerapps/maker/canvas-apps/open-and-run-a-sample-app).  

When you have designed and built your app, you can share it with your colleagues. For more information, see [Save and publish a canvas app in Power Apps](/powerapps/maker/canvas-apps/save-publish-app).  

> [!NOTE]
> If you want to connect to [!INCLUDE[prodshort](includes/prodshort.md)] on-premises, then you must choose the **Business Central (on-premises)** connector in step 3.  

## <a name="see-also"></a>See Also

[Create a canvas app from a template in Power Apps](/powerapps/maker/canvas-apps/get-started-test-drive)  
[Importing Business Data from Other Finance Systems](across-import-data-configuration-packages.md)  
[Setting Up [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)  
[Getting Started Developing Connect Apps for Dynamics 365 Business Central](/dynamics365/business-central/dev-itpro/developer/devenv-develop-connect-apps)  
