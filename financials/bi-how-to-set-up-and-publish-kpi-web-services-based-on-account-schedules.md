---
title: How to Set Up and Publish KPI Web Services Based on Account Schedules | Microsoft Docs
description: In the **Account Schedule KPI Web Service Setup** window, you set up how to show the account-schedule KPI data and which specific account schedules to base the KPIs on.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/08/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: 57f36592105faf0801864e034c3b930ae196ee62
ms.contentlocale: en-nz
ms.lasthandoff: 01/30/2018

---
# <a name="set-up-and-publish-kpi-web-services-based-on-account-schedules"></a>Set Up and Publish KPI Web Services Based on Account Schedules
In the **Account Schedule KPI Web Service Setup** window, you set up how to show the account-schedule KPI data and which specific account schedules to base the KPIs on. When you choose the **Publish Web Service** button, the specified account-schedule KPI data is added to the list of published web services in the **Web Services** window.  

## <a name="to-set-up-and-publish-a-kpi-web-service-that-is-based-on-account-schedules"></a>To set up and publish a KPI web service that is based on account schedules  

1.  Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Account Schedule KPI Web Service Setup**, and then choose the related link.  
2.  On the **General** FastTab, fill in the fields as described in the following table.  

    |Field|Description|  
    |---------------------------------|---------------------------------------|  
    |**Forecasted Values Start**|Specify at what point in time forecasted values are shown on the account-schedule KPI graphic.<br /><br /> The forecasted values are retrieved from the general ledger budget that you select in the **G/L Budget Name** field. **Note:**  To obtain KPIs that show forecasted figures after a certain date and actual figures before the date, you can change the **Allow Posting From** field in the **General Ledger Setup** window. For more information, see Allow Posting From.|  
    |**G/L Budget Name**|Specify the name of the general ledger budget that provides forecasted values to the account-schedule KPI web service.|  
    |**Period**|Specify the period that the account-schedule KPI web service is based on.|  
    |**View By**|Specify which time interval the account-schedule KPI is shown in.|  
    |**Web Service Name**|Specify the name of the account-schedule KPI web service.<br /><br /> This name will appear in the **Service Name** field in the **Web Services** window.|  

    Proceed to specify one or more account schedules that you want to publish as a KPI web service according to the setup that you made in the previous table.  

3.  On the **Account Schedules** FastTab, fill in the fields as described in the following table.  

    |Field|Description|  
    |---------------------------------|---------------------------------------|  
    |**Acc. Schedule Name**|Specify the account schedule that the KPI web service is based on.|  
    |**Acc. Schedule Description**|Specify the description of the account schedule that the KPI web service is based on.|  

4.  Repeat step 3 for all the account schedules that you want to base the account-schedule KPI web service on.  
5.  To view or edit the selected account schedule, on the **Account Schedule** FastTab, choose the **Edit Account Schedule** action.  
6.  To view the account-schedule KPI data that you have set up, choose the **Account Schedule KPI Web Service** action.  
7.  To publish the account-schedule KPI web service, choose the **Publish Web Service** action. The web service is added to the list of published web services in the **Web Services** window.  

> [!NOTE]  
>  You can also publish the KPI web service by pointing to the **Account Schedule KPI Web Service Setup** page object from the **Web Services** window. For more information, see [Publish a Web Service](across-how-publish-web-service.md).  

## <a name="see-also"></a>See Also  
[Business Intelligence](bi.md)  
[Finance](finance.md)  
[Setting Up Finance](finance-setup-finance.md)  
[The General Ledger and the Chart of Accounts](finance-general-ledger.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

