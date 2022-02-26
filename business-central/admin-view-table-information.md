---
title: View Table Information
description: Learn how you can view information about the database tables directly from the client interface in Business Central.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.form: 8700
ms.date: 06/14/2021
ms.author: jswymer
ms.openlocfilehash: 70aff9cf0aa2af7096c8c4c047e249585e34c777
ms.sourcegitcommit: 8464b37c4f1e5819aed81d9cfdc382fc3d0762fc
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 01/19/2022
ms.locfileid: "8010980"
---
# <a name="viewing-table-information"></a>Viewing Table Information

The page **8700 Table Information** provides information about all system and business tables in a Business Central solution. In particular, the page displays information about the amount of data the tables contain.

This information is useful for troubleshooting performance problems, because let's you see the distribution of data size across tables.

## <a name="viewing-table-information"></a>Viewing table information

To open this page, select the ![Search for Page or Report.](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Table Information**, and then choose the related link.

The following table describes the information provided for each table:

|Column|Description|
|------|-----------|
|Company Name|The name of the company, if any, that the table belongs to.|
|Table Name|The name of the table.|
|Table No.|The ID of the table|
|No. of Records|The total number of records stored in the table.|
|Record Size|The average record size in KB/record. The value is calculated using the following formula: 1024(Size)/(No. of Records)`. |

## <a name="see-also"></a>See Also

[Inspecting Pages](across-inspect-page.md)  
[Performance Articles For Developers](/dynamics365/business-central/dev-itpro/performance/performance-developer)  


[!INCLUDE[footer-include](includes/footer-banner.md)]