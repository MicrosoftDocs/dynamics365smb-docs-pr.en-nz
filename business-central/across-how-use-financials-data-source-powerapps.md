---
title: Use Your Data to Create an App| Microsoft Docs
description: You can make your Business Central data available as a data source and specify an OData URL of your web services to build a business app using PowerApps.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: Odata, Power App, SOAP
ms.date: 10/01/2019
ms.author: edupont
ms.openlocfilehash: 4b8005154afb988cf25c6a04b7beeaafd199afca
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 10/01/2019
ms.locfileid: "2305055"
---
# <a name="connecting-to-your-business-central-data-to-build-a-business-app-using-powerapps"></a>Connecting to Your Business Central Data to Build a Business App Using PowerApps
You can make your [!INCLUDE[d365fin](includes/d365fin_md.md)] data available as a data source in PowerApps.  

> [!NOTE]  
>   You must have a valid account with [!INCLUDE[d365fin](includes/d365fin_md.md)] and with PowerApps.  

## <a name="to-add-included365finincludesd365fin_mdmd-as-a-data-source-in-powerapps"></a>To add [!INCLUDE[d365fin](includes/d365fin_md.md)] as a data source in PowerApps
1. In your browser, navigate to [powerapps.microsoft.com](https://powerapps.microsoft.com/en-us/), and then sign in.
2. On the Home page, choose the **Apps**, **Create an app** and **Canvas** to create a new canvas app. This app will be designed for use on a mobile device, but you can also choose to use another template.

    The next step to create a PowerApp is to select your data. Choose the Arrow icon then choose the **New connection** option in the upper left side of the page.
3. In the list of available connections, choose **Business Central**, and then choose the **Create** button.

    PowerApps will connect to your [!INCLUDE [prodshort](includes/prodshort.md)] using the credentials that you are signed in with. If you are not an administrator of your [!INCLUDE [prodshort](includes/prodshort.md)], you may have to sign in with another account.  

4.  PowerApps will display a list of *Environments and companies* that are available from [!INCLUDE [prodshort](includes/prodshort.md)]. Choose the environment and company that contains the data you want to connect to. Next, you will be presented with a list of APIs. Select the **API** you want to connect to.

These so-called tables are part of the [!INCLUDE [prodshort](includes/prodshort.md)] API. You do not have to configure the end points yourself - the [!INCLUDE [prodshort](includes/prodshort.md)] connector for PowerApps does it for you.  

    If you want to include data from other tables in [!INCLUDE [prodshort](includes/prodshort.md)] in your app, then you must work with a developer to define a custom API in [!INCLUDE [prodshort](includes/prodshort.md)] and then consume that custom API through a custom connector in PowerApps. For more information, see [Create a custom connector from scratch](/connectors/custom-connectors/define-blank).  

At this point, you have successfully connected to your [!INCLUDE [prodshort](includes/prodshort.md)] data and are ready to begin building your PowerApp. You can add additional screens and connect to additional data from your [!INCLUDE [prodshort](includes/prodshort.md)]. For more information, see [Create a canvas app from a template in PowerApps](/powerapps/maker/canvas-apps/get-started-test-drive).  

When you have designed and built your app, you can share it with your colleagues. For more information, see [Save and publish a canvas app in PowerApps](/powerapps/maker/canvas-apps/save-publish-app).  

> [!NOTE]
> If you want to connect to [!INCLUDE [prodshort](includes/prodshort.md)] on-premises, then you must choose the **Business Central (on-premises)** connector in step 3.  

## <a name="see-also"></a>See Also

[Create a canvas app from a template in PowerApps](/powerapps/maker/canvas-apps/get-started-test-drive)  
[Getting Started](product-get-started.md)  
[Importing Business Data from Other Finance Systems](across-import-data-configuration-packages.md)  
[Setting Up [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)  
[Finance](finance.md)  
[Getting Started Developing Connect Apps for Dynamics 365 Business Central](/dynamics365/business-central/dev-itpro/developer/devenv-develop-connect-apps)  
