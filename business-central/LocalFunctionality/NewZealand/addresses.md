---
title: Addresses in New Zealand
description: A single postcode can include multiple cities in the same region.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 4b4dabccff6ec188ce677db4cdfe5a64664a4ed1
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 10/01/2020
ms.locfileid: "3919859"
---
# <a name="addresses-in-the-new-zealand-version"></a>Addresses in the New Zealand Version

A single postcode can include multiple cities in the same region.  

At the same time, cities with the same name are sometimes located in different regions.  

To avoid confusion and improve address accuracy, available options display when you enter data in address fields. For example, when you enter a postcode on a customer card, you can select from a list of all available cities for that postcode in the **City** field drop-down list. Likewise, when you enter a city name, you can select from a list of all available regions in the **Region** field drop-down list.  

To enable this functionality, you must enter the data into the **Postcode** table. You can do this manually, or you can download a copy of the New Zealand postcodes for New Zealand.  
  
To increase postal efficiency in New Zealand, the postal department has introduced an address bar coding system in which every address is assigned a unique identifier called a Delivery Point Identifier (DPID). From the DPID, a bar code is generated and printed for each address. Companies can receive discounts on bulk mailings if they use these bar codes. To retrieve a DPID, you must connect to the local postal database that uses authorised Address Matching Approval System (AMAS) software. You can reduce your number of postal returns by validating customer addresses using the AMAS database.  

When you print an address that has a DPID, a bar code will be printed together with the address. If you cannot print bar codes, the DPID will be printed together with the address.  

Contact your Microsoft partner for information on how to obtain AMAS software.  

## <a name="see-also"></a>See Also  
 [New Zealand Local Functionality](new-zealand-local-functionality.md)
