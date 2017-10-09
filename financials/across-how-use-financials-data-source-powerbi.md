---
title: Make a Power BI data source with your Financials | Microsoft Docs
description: You can make your Financials data available as a data source in Power BI and build powerful reports of the state of your business.
author: edupont04
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: business intelligence, KPI, Odata, Power App, SOAP, analysis
ms.date: 06/06/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 3f98a08415a896c37868bf0ed5efd9314d5ab07a
ms.contentlocale: en-nz
ms.lasthandoff: 09/22/2017

---
# <a name="using-included365finincludesd365finmdmd-as-a-power-bi-data-source"></a>Using [!INCLUDE[d365fin](includes/d365fin_md.md)] as a Power BI Data Source
You can make your [!INCLUDE[d365fin](includes/d365fin_md.md)] data available as a data source in Power BI and build powerful reports of the state of your business.  

> [!NOTE]  
>   You must have a valid account with [!INCLUDE[d365fin](includes/d365fin_md.md)] and with Power BI. Also, you must download [Power BI Desktop](https://powerbi.microsoft.com/en-us/desktop/).  

## <a name="to-add-included365finincludesd365finmdmd-as-a-data-source-in-power-bi-desktop"></a>To add [!INCLUDE[d365fin](includes/d365fin_md.md)] as a data source in Power BI Desktop
1. In Power BI Desktop, in the left navigation pane, choose **Get Data**.
2. In the **Get Data** window, choose **Online Services**, choose **Dynamics 365 for Financials**, and then choose the **Connect** button.

   Power BI displays a wizard that will guide you though the connection process. The first step will be to enter an OData URL and the company name that is associated with your [!INCLUDE[d365fin](includes/d365fin_md.md)] account.  

   For the *OData URL*, you can copy the OData V4 URL of any of the web services that are listed in the **Web Services** page in [!INCLUDE[d365fin](includes/d365fin_md.md)], such as `https://mycompany.financials.dynamics.com:7048/MS/ODataV4/`.  

   For the *Company Name*, use the name that is shown in the **Name** field in the **Company Information** window in [!INCLUDE[d365fin](includes/d365fin_md.md)]. If your [!INCLUDE[d365fin](includes/d365fin_md.md)] contains multiple companies, choose the relevant company name from the list in the **Companies** window. In both cases, make sure that the name that you specify in the Power BI wizard matches exactly the text shown in [!INCLUDE[d365fin](includes/d365fin_md.md)], such as `My Company`.
3. Once you have entered the information, choose the OK button. The next step in the wizard will be to enter your username and password.

   > [!NOTE]  
>    If there are other authentication options available in the left hand navigation, choose *Basic*.
4. Enter your username and password. You can find this information in the **Users** window in [!INCLUDE[d365fin](includes/d365fin_md.md)]. Use the **Web Access Key** as your password.

   For example, your username is *ADMIN*, and the web service access key that serves as your password is *EgzeUFQ9Uv0o5O0lUMyqCzo1ueUW9yRF3SsLU=*.
5. Choose the **Connection** button to continue. The Power BI wizard shows a list of [!INCLUDE[d365fin](includes/d365fin_md.md)] data sources. These data source represent all the web services that you have published from your [!INCLUDE[d365fin](includes/d365fin_md.md)].

   Alternatively, create a new web service URL in [!INCLUDE[d365fin](includes/d365fin_md.md)] by using the **Create Data Set** action in the **Web Services** page, using the **Set Up Reporting** Assisted Setup guide, or by choosing the **Edit in Excel** action in any lists.

6. Specify the data you want to add to your data model, and then choose the **Load** button.
7. Repeat the previous steps to add additional [!INCLUDE[d365fin](includes/d365fin_md.md)] data to your Power BI data model.

   > [!NOTE]  
>    Once you have successfully connected to [!INCLUDE[d365fin](includes/d365fin_md.md)], you will not be prompted again for the OData URL, username, or password.

Once the data is loaded it will appear in the right navigation on the page. At this point, you have successfully connected to your Dynamics 365 data and are ready to begin building your Power BI report. For more information, see the [Power BI documentation](https://powerbi.microsoft.com/documentation/powerbi-landing-page/).

## <a name="see-also"></a>See Also
[Business Intelligence](bi.md)  
[Welcome to [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)  
[Importing Business Data from Other Finance Systems](upload-data.md)  
[Setting Up [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)  
[Finance](finance.md)  

