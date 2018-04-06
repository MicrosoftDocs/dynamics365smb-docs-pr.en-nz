---
title: Troubleshooting Integration with Microsoft Flow| Microsoft Docs
description: Troubleshoot how you can make your Financials data available as a data source and specify an OData URL of your web services to build an automated workflow.
documentationcenter: 
author: SusanneWindfeldPedersen
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: workflow, Odata, Power App, SOAP
ms.date: 01/25/2018
ms.author: solsen
ms.translationtype: HT
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: 4c28b5b6dce6152399cf599877180e806227b5ef
ms.contentlocale: en-nz
ms.lasthandoff: 03/22/2018

---
# <a name="troubleshooting-integration-with-microsoft-flow---request-url-too-long"></a>Troubleshooting Integration with Microsoft Flow - Request URL Too Long
You can use your [!INCLUDE[d365fin](includes/d365fin_md.md)] data as part of a workflow in Microsoft Flow.  

> [!NOTE]  
>   You must have a valid account with [!INCLUDE[d365fin](includes/d365fin_md.md)] and with Flow.  

If you are creating a Microsoft Flow using the [!INCLUDE[d365fin](includes/d365fin_md.md)] connector, you may receive an error message stating that the requsted URL is too long after creating the flow, such as the following: **RequestUriTooLong**.

## <a name="cause"></a>Cause
For a flow to trigger, it looks for changes in your data. When determining if your data has changed, the connectors compare the cached data to the new data requested from the source.  

If the data request creates a URL that is too long, it will fail. Common causes may include:
- Generally, any source table with over 250 rows
- Source tables containing multiple thousands of records

## <a name="workaround"></a>Workaround
Follow these steps as a workaround.
1. Choose to edit the flow that is failing.
2. Expand the **Show advanced options** on the flow trigger.
3. In the **Skip Count** field, enter the number of records to skip.  
For example, if the table that you are using as a data source has 4,000 records, enter 4,000 as the number of records to skip.
4. Update your flow.

> [!NOTE]  
> The connector is currently in Beta. Updates to how data changes are targeted for a future release.


## <a name="see-also"></a>See Also
[Using [!INCLUDE[d365fin](includes/d365fin_md.md)] in an Automated Workflow](across-how-use-financials-data-source-flow.md)  
[Welcome to [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)  
[Importing Business Data from Other Finance Systems](upload-data.md)  
[Manage Users and Permissions](ui-how-users-permissions.md)    
[Setting Up [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)  
[Finance](finance.md)  

