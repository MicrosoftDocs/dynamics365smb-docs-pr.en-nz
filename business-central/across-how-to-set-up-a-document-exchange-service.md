---
title: How to Set Up a Document Exchange Service | Microsoft Docs
description: You use an external service provider to exchange electronic documents with your trading partners.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 06/08/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: e73c2dd0533aade4aa6225c9d2f385baaea3cfd1
ms.openlocfilehash: 0e57f02f1689de12e75595a26c489eeda68a4b89
ms.contentlocale: en-nz
ms.lasthandoff: 06/11/2018

---
# <a name="set-up-a-document-exchange-service"></a>Set Up a Document Exchange Service
You use an external service provider to exchange electronic documents with your trading partners. For more information, see [Exchanging Data Electronically](across-data-exchange.md).  

## <a name="to-set-up-a-document-exchange-service"></a>To set up a document exchange service  
1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Doc. Exch. Service Setup**, and then choose the related link.  
2. Fill the fields as described in the following table.  

    |Field|Description|  
    |---------------------------------|---------------------------------------|  
    |**User Agent**|Enter any text that can be used to identify your company in document exchange processes.|  
    |**Doc. Exch. Tenant ID**|Enter the tenant in the document exchange service that represents your company. This is provided by the document exchange service provider.|  
    |**Enabled**|Specify if the service is enabled. **Note:**  As soon as you enable the service, at least two job queue entries are created to process the traffic of electronic documents in and out of [!INCLUDE[d365fin](includes/d365fin_md.md)]. When you disable the service, the job queue entries are deleted.|  
    |**Signup URL**|Specify the web page where you sign up for the document exchange service.|  
    |**Service URL**|Specify the address of the document exchange service, which will be called when you send and receive electronic documents.|  
    |**Login URL**|Specify the logon page for the document exchange service, which is where you enter your company’s user name and password to log on to the service.|  
    |**Consumer Key**|Enter the 3-legged OAuth key for the consumer key. This is provided by the document exchange service provider.|  
    |**Consumer Secret**|Enter the secret that protects the consumer key. This is provided by the document exchange service provider.|  
    |**Token**|Enter the 3-legged OAuth key for the token. This is provided by the document exchange service provider.|  
    |**Token Secret**|Enter the secret that protects the token. This is provided by the document exchange service provider.|  

    > [!NOTE]  
    > You login data is automatically encrypted.

## <a name="see-also"></a>See Also  
[Setting Up Data Exchange](across-set-up-data-exchange.md)  
[Exchanging Data Electronically](across-data-exchange.md)

