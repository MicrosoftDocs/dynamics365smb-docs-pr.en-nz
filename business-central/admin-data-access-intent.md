---
title: Manage database access intent in Business Central | Microsoft Docs
description: Change the database access intent for reports, API pages, and queries.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: jswymer
ms.openlocfilehash: 6d79f5b2851df85ea9f19faeeb941eccfd1b397b
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 12/17/2020
ms.locfileid: "4752841"
---
# <a name="managing-database-access-intent"></a>Managing Database Access Intent 

As a super user or administrator, you can change the database access intent on reports, pages of the type API, and queries to improve performance of the service.

## <a name="overview"></a>Overview

[!INCLUDE[prod_short](includes/prod_short.md)] can be set up to use read-only replicas of the primary (read-write) database. Using the database replica reduces the load on the primary database. In some cases, it will also improve the performance when viewing data in the client. Replicas are beneficial for objects, like reports, queries, and API pages, that are used for viewing data only, not modifying data.

When objects run, the database access intent determines whether to use a read-only replica, if one is available, or the primary database. Reports, API pages, and queries are developed with a predefined database access intent (see [DatabaseAccessIntent property](/dynamics365/business-central/dev-itpro/developer/properties/devenv-dataaccessintent-property)).

The **Database Access Intent List** page lets you override the predefined database access intent for objects when they're run.

In database terms, this feature is commonly known as *read scale-out*. For more information about read-scale out and data access intent in [!INCLUDE[prod_short](includes/prod_short.md)], see [Utilising Read Scale-Out for Better Performance](/dynamics365/business-central/dev-itpro/administration/database-read-scale-out-overview) in the [!INCLUDE[prod_short](includes/prod_short.md)] Developer and Administration help.

## <a name="to-change-the-database-access-intent"></a>To change the database access intent

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Database Access Intent List**, and then choose the related link.

    The page lists all reports, pages, and queries. The **Access Intent** column includes one of the following values:

    |**Setting**|**Description**|  
    |------------|-------------|  
    |**Default**|Indicates that the object uses the predefined database access intent.|
    |**Allow Write**|Sets the object to use the primary database, allowing the user to modify data.|
    |**Read Only**|Sets the object to use the database replica, which means that the user can only view data, not change data.|

2. Choose the **Edit List** action.

3. On the **Edit - Database Access Intent List** page, change the **Access Intent** field for the objects.

    > [!NOTE]
    > If an object that is editable, like the Customer Card, is set to **Read Only**, the primary database will still be used, regardless of the access intent, allowing users to make changes as normal.

## <a name="see-related-training-at-microsoft-learn"></a>See Related Training at [Microsoft Learn](/learn/paths/deploy-configure-dynamics-365-business-central/)

## <a name="see-also"></a>See Also
[Business Functionality](across-business-functionality.md)  
[General Business Functionality](ui-across-business-areas.md)  
[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  
[Getting Started](product-get-started.md)    

## [!INCLUDE[prod_short](includes/free_trial_md.md)]  


[!INCLUDE[footer-include](includes/footer-banner.md)]