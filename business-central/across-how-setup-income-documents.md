---
title: Set Up Incoming Documents| Microsoft Docs
description: Use the Incoming Documents feature to create electronic documents, manage OCR tasks, import invoices, and convert image files.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: electronic document, e-invoice, incoming document, OCR, ecommerce, document exchange, import invoice
ms.date: 04/01/2019
ms.author: sgroespe
ms.openlocfilehash: 7e99f4b33767a1bdea7b942d1b183edbacc829ac
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 04/29/2019
ms.locfileid: "1241524"
---
# <a name="set-up-incoming-documents"></a>Set Up Incoming Documents
If you create general journal lines from incoming document records, you must specify on the **Incoming Documents Setup** page which journal template and batch to use.

If you do not want users to create invoices or general journal lines from incoming document records unless the documents are first approved, you must set up approvers on the **Incoming Document Approvers** page.

To turn PDF and image files into electronic documents that you can convert to, for example, purchase invoices inside [!INCLUDE[d365fin](includes/d365fin_md.md)], you must first set up the OCR feature and enable the service.

When the Incoming Documents feature is set up, you can use different functions to review expense receipts, manage OCR tasks, and convert incoming document files, manually or automatically, to the relevant documents or journal lines. The external files can be attached at any process stage, including to posted documents and to the resulting vendor, customer, and general ledger entries. For more information, see [Processing Incoming Documents](across-process-income-documents.md).

## <a name="to-set-up-the-incoming-documents-feature"></a>To set up the Incoming Documents feature
1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Incoming Document Setup**, and then choose the related link.
2. Fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="to-set-up-approvers-of-incoming-document-records"></a>To set up approvers of incoming document records
1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Incoming Document Setup**, and then choose the related link.  
2. On the **Incoming Documents Setup** page, choose the **Approvers** action.

    The **Incoming Document Approvers** page shows all users that are set up in [!INCLUDE[d365fin](includes/d365fin_md.md)].  
3. Select one or more users that can approve an incoming document before a related document or journal line can be created.

When approvers have been set up on the **Incoming Document Approvers** page, only those users can approve an incoming document if the **Require Approval To Create** check box on the **Incoming Documents Setup** page is selected.

> [!NOTE]  
>   This approval setup is not related to approval workflows. For more information, see [Use Approval Workflows](across-how-use-approval-workflows.md).

## <a name="to-set-up-an-ocr-service"></a>To set up an OCR service
1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **OCR Service Setup**, and then choose the related link.
2. Fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

> [!NOTE]  
> You login data is automatically encrypted.

## <a name="see-also"></a>See Also
[Process Incoming Documents](across-process-income-documents.md)  
[Incoming Documents](across-income-documents.md)  
[Purchasing](purchasing-manage-purchasing.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
