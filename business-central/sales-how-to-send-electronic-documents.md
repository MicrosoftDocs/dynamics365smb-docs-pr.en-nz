---
title: Send Electronic Documents
description: learn how to send invoices electronically.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 43f61682a1068a8e1652fd28421f83d5291c8fe8
ms.sourcegitcommit: fe6943d410f5dca4e8b2986f95501009ae982d98
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 01/05/2021
ms.locfileid: "4827084"
---
# <a name="send-electronic-documents"></a>Send Electronic Documents

The generic version of [!INCLUDE[prod_short](includes/prod_short.md)] supports sending electronic invoices and credit memos in the PEPPOL format, a format that the largest document exchange service providers support. A document exchange service provider dispatches electronic documents between trading partners. To provide support for other electronic document formats, you use the data exchange framework.  

 In the generic version of [!INCLUDE[prod_short](includes/prod_short.md)], a document exchange service is preconfigured and ready to be set up for your company. For more information, see [Set Up a Document Exchange Service](across-how-to-set-up-a-document-exchange-service.md). However, in some cases, you must install an app. For more information, see [Electronic Invoicing FAQ](faq-electronic-invoicing.yml).  

 To send a sales invoice as an electronic PEPPOL document, you select the **Electronic Document** option in the **Post and Send** dialogue box. You can also set up the customer's default document sending profile from that dialogue box. First, you must set up various master data, such as company information, customers, items, and units of measure. These are used to identify the business partners and items when converting data in fields in [Set Up Electronic Document Sending and Receiving](across-how-to-set-up-electronic-document-sending-and-receiving.md).  

### <a name="to-send-an-electronic-sales-invoice"></a>To send an electronic sales invoice

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Invoices**, and then choose the related link.  

2. Create a new sales invoice.  

3. When the sales invoice is ready to be invoiced, choose the **Post and Send** action.  

     If the customer's default sending profile is **Electronic Document**, then it will be shown in the **Post and Send Confirmation** dialogue box. This way, you just have to choose the **Yes** button to post and send the invoice electronically in the selected format.  

4. In the **Post and Send Confirmation** dialogue box, choose the AssistEdit button to the right of the **Send Document to** field.  

5. In the **Send Document to** dialogue box, in the **Electronic Document** field, choose **Through Document Exchange Service**.  

6. In the **Format** field, choose **PEPPOL**.  

7. Choose the **OK** button. The **Post and Send Confirmation** dialogue box appears. **Electronic Document (PEPPOL)** is added to the **Send Document to** field.  

8. Choose the **Yes** button.  

     The sales invoice is posted and sent to the customer in the PEPPOL format.  

    > [!NOTE]  
    >  You can also send a posted sales invoice as an electronic document. The procedure is the same as described in this topic for non-posted sales documents. On the **Posted Sales Invoice** page, choose the **Activity Log** action to view the status of the electronic document.  

## <a name="see-related-training-at-microsoft-learn"></a>See Related Training at [Microsoft Learn](/learn/modules/electronic-documents-dynamics-365-business-central/index)

## <a name="see-also"></a>See Also

[Invoice Sales](sales-how-invoice-sales.md)  
[Set Up Document Sending Profiles](sales-how-setup-document-send-profiles.md)  
[Set Up Electronic Document Sending and Receiving](across-how-to-set-up-electronic-document-sending-and-receiving.md)  
[Set Up a Document Exchange Service](across-how-to-set-up-a-document-exchange-service.md)  
[Set Up Data Exchange Definitions](across-how-to-set-up-data-exchange-definitions.md)  
[Exchanging Data Electronically](across-data-exchange.md)  
[Electronic Invoicing FAQ](faq-electronic-invoicing.yml)  
[General Business Functionality](ui-across-business-areas.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]