---
title: Track User Activity in a Change Log| Microsoft Docs
Description: You can activate a user log so that you have a history of any changes made to data in tracked tables.
documentationcenter: 
author: edupont04
ms.service: dynamics365-financials
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: user log, user activity, tracking
ms.date: 06/02/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: c27c63ae26f2f97dd15d31978b967f6a08dd55b7
ms.contentlocale: en-nz
ms.lasthandoff: 09/22/2017

---
# <a name="logging-changes-in-dynamics-365-for-financials"></a>Logging Changes in Dynamics 365 for Financials
You can enable the change log in [!INCLUDE[d365fin](includes/d365fin_md.md)] so you have a history of activities. The log is based on changes that are made to data in the tables that you track. In the change log, entries are chronologically ordered and show changes that are made to the fields on the specified tables. The change log collects all changes that are made to the table.  

## <a name="working-with-the-change-log"></a>Working with the change log
A common problem in many financial systems is to locate the origin of errors and changes in data. It could be anything from an incorrect customer telephone number to an incorrect posting to the general ledger. The change log lets you track all direct modifications a user makes to data in the database. You must specify each table and field that you want the system to log, and then you must activate the change log.  

You activate and deactivate the change log in the **Change Log Setup** window. When you activate or deactivate the change log, this activity is logged, so you can always see which user deactivated or reactivated the change log. This cannot be turned off.  

In the **Change Log Setup** window, if you choose the **Tables** action, you can specify which tables you want to track changes for, and which changes to track. [!INCLUDE[d365fin](includes/d365fin_md.md)] also tracks a number of system tables.

After you have set up the change log, activated it, and made a change to data, you can view and filter the changes in the **Change Log Entries** window. If you want to delete entries, you can do that in the **Delete Change Log Entries** window, where you can set filters based on dates and time.  

## <a name="see-also"></a>See Also
[Changing Basic Settings](ui-change-basic-settings.md)  
[Sorting](ui-sorting.md)  
[Using Search for Page or Report](ui-search.md)  
[How to: Manage Users and Permissions](ui-how-users-permissions.md)    
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

