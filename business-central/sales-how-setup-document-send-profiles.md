---
title: Set Up Preferred Methods of Sending Sales Documents | Microsoft Docs
description: Describes how to set up each customer’s preferred method of sending sales documents, for example, email, PDF, electronic document, and so on.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: email, PDF, electronic document
ms.date: 04/01/2019
ms.author: sgroespe
ms.openlocfilehash: a6521a6f67fa39ded3b3baa863fc0d4341aa0524
ms.sourcegitcommit: bd78a5d990c9e83174da1409076c22df8b35eafd
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 03/31/2019
ms.locfileid: "916963"
---
# <a name="set-up-document-sending-profiles"></a>Set Up Document Sending Profiles
You can set each customer up with a preferred method of sending sales documents, so that you do not have to select a sending option every time you choose the **Post and Send** action.

On the **Document Sending Profiles** page, you set up different sending profiles that you can select from in the **Document Sending Profile** field on a customer card. You can select the **Default** check box to specify that the document sending profile is the default profile for all customers, except for customers where the **Document Sending Profile** field is filled with another sending profile.

When you choose the **Post and Send** action on a sales document, the **Post and Send Confirmation** dialogue box shows the sending profile used, either the one set up for the customer or the default for all customers. In the dialogue box, you can change the sending profile for the sales document. For more information, see [Invoice Sales](sales-how-invoice-sales.md).

## <a name="to-set-up-a-document-sending-profile"></a>To set up a document sending profile
1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Document Sending Profiles**, and then choose the related link.
2. On the **Document Sending Profiles** page, choose the **New** action.
3. Fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="to-specify-a-sending-profile-on-a-customer-card"></a>To specify a sending profile on a customer card
1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Customers**, and then choose the related link.
2. Open the card of the customer who you want to set up a sending profile for.
3. In the **Document Sending Profile** field, select a profile that you have set up as described in the previous procedure.

## <a name="see-also"></a>See Also
[Setting Up Sales](sales-setup-sales.md)  
[Sales](sales-manage-sales.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
