---
title: 'How to: Create Interactions on Contacts and Segments | Microsoft Docs'
description: Describes how to create interactions on contacts and segments in Financials
services: project-madeira
documentationcenter: 
author: jswymer
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: relationship, prospect
ms.date: 03/28/2017
ms.author: jswymer
ms.translationtype: Human Translation
ms.sourcegitcommit: a31be0f9d07e2abb591e26f6bae34c6f6e4dcda6
ms.openlocfilehash: b50d332441bee01158559616fff5d5f5ca381a90
ms.contentlocale: en-nz
ms.lasthandoff: 05/04/2017


---
# <a name="how-to-create-interactions-on-contacts-and-segments"></a>How to: Create Interactions on Contacts and Segments
You can create interactions to record all the interactions and communications you have with your contacts and segments, for example, direct mail.

Before you create interactions, you must set up interaction templates. For more information, see  [Set Up Interaction Templates](marketing-interactions.md#set-up-interaction-templates).

## <a name="to-create-an-interaction"></a>To create an interaction
1. Open the contact, salesperson, or interaction log entry.
2. Choose the **Create Interaction** action.
3. Fill in the fields, and choose the **OK** button.

**Note**: If you need to perform another task before finishing the interaction, you can choose **Cancel**, and choose to finish the interaction at a later time. This postpones the interaction.

## <a name="to-finish-and-delete-postponed-interactions"></a>To finish and delete postponed interactions
1. Open the contact, salesperson, or interaction log entry.
2. Choose **Postponed Interactions**.
3. Select the interaction you want to finish, and then choose the **Resume** action.

## <a name="to-create-an-interaction-on-a-segment"></a>To create an interaction on a segment
1. On the Home page, choose **Active Segments**, or in the top right corner, choose the **Search for Page or Report** icon ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon"), enter **Segments**, and then choose the related link.
2. In the **Segment window**, in the **Interaction** section, fill in the fields to specify which interaction you want to assign to the segment.

    After you have assigned an interaction to the segment, you can personalise the interaction for each particular contact within the segment, for example, by selecting another interaction template on the lines in the **Segment** window.  
3. To log the segment and interactions, choose the **Log** action. The **Log Segment** window opens.
4. If you want to create a new segment containing the same contacts, select the **Create Follow-up Segment** check box. To create a follow-up segment, you must have specified number series for segments in the **Marketing Setup** window.

An interaction is recorded for each contact within the segment in the **Interaction Log Entry** table, and the segment is logged. Logged segments can be found in the **Logged Segment** window.

If you have selected the **Create Follow-up Segment** check box, a new segment is created that contains the same contacts as the segment you have just logged.

## <a name="see-also"></a>See Also
[Recording Interactions](marketing-interactions.md)  
[Managing Contacts](marketing-contacts.md)  
[Managing Sales Opportunities](marketing-manage-sales-opportunities.md)  
[Setting Up Relationship Management](marketing-setup-marketing.md)  
[Working With Financials](ui-work-product.md)

