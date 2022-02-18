---
title: Keep Track of Segments and Related Interactions
description: Learn about creating segments to define groups of contacts and specifying interactions for segments.
documentationcenter: ''
author: jswymer
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: relationship, prospect
ms.search.forms: 5139,
ms.date: 04/01/2021
ms.author: jswymer
ms.openlocfilehash: 0da5f065b1a455ae9829c4ac6d10b90c3f326c04
ms.sourcegitcommit: 189bf08d7ddf6c8b7ef2c09058c6847aa6e590d3
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 01/31/2022
ms.locfileid: "8059664"
---
# <a name="manage-interactions-for-segments"></a>Manage Interactions for Segments
The **Segment** page is a type of worksheet where you can:

* Create segments.
* Save the segmentation criteria you have used to select contacts.
* Log the segment and record interactions involving the contacts within the segment.

## <a name="segmenting"></a>Segmenting
There are several ways to create segments:

* You can manually enter the contacts you want to include in the segment in the segment lines.
* You can select contacts.
* You can reuse a logged segment as the basis to create a new one.
* You can reuse saved segmentation criteria.

## <a name="interactions"></a>Interactions
On the **Segment** page, you can create interactions for several contacts simultaneously. For example, you can merge a segment with a Microsoft Word document, so that you can send a letter to all the contacts in the segment.

You can specify information about the interaction for the segment on the **Segment** header. For example, you can decide which interaction template you want to use for all the contacts, specify a description, a correspondence type, and so on. However, you can modify this information in the segment line for each particular contact, for example, by specifying another description for one contact. If you are merging a segment with a Microsoft Word document, you can personalise the document to be sent for one or several of the contacts within the segment, for example, by adding individualised comments to the document.

## <a name="logging"></a>Logging
On the **Segment** page, when you choose **Log**, the application records the interactions on the **Interaction Log Entry** page, and logs the segment. After you have logged the segment, you can only find it on the **Logged Segments** page.

On the **Logged Segments** page, you can decide to create a follow-up segment containing the same contacts as the segment you have logged.

## <a name="see-also"></a>See Also
[Create Segments](marketing-how-create-segment.md)  
[Create Interactions for Segments](marketing-how-create-interactions.md)  
[Managing Segments](marketing-segments.md)  
[Recording Interactions With Contacts](marketing-interactions.md)  
[Managing Sales Opportunities](marketing-manage-sales-opportunities.md)  
[Creating and Managing Contacts](marketing-contacts.md)  
[Working with Business Central](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]