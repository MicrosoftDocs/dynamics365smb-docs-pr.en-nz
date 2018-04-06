---
title: Set Up Marketing Campaigns in Finance and Operations, Business edition| Microsoft Docs
description: Describes how you can set up and conduct marketing campaigns in Finance and Operations, Business edition to help you identify and attract prospects and retain customers.
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: marketing, campaign, promo, prospect
ms.date: 06/06/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: 4ca4fc6eee45c69be3de746ce1d799a481d7ea48
ms.contentlocale: en-nz
ms.lasthandoff: 03/22/2018

---
# <a name="managing-marketing-campaigns"></a>Managing Marketing Campaigns
Having a strong marketing plan in place enables you to identify, attract, and retain customers. A marketing plan consists of various campaigns and other interactions in connection with your sales and marketing activities. While planning a campaign, you need to decide which contacts to target, what type of campaign (such as trade show or direct mail), and what salespeople will perform each task.

Each campaign consists of various activities or tasks. You can combine multiple task, for example tasks that each represent a step, in activities. Activity tasks are related to each other by a date formula. Individual tasks can only be assigned to salespeople. Activities can be assigned to opportunities, salespeople, groups of sales people, and contacts. For more information, see [Set Up Opportunity Sales Cycles and Cycle Stages](marketing-how-setup-opportunity-sales-cycles-stages.md).

## <a name="defining-individual-campaigns"></a>Defining individual campaigns
Before you can create a campaign, you must set up *campaign status codes*. Using these codes will help you manage your campaigns by assigning a status to the campaign. As you work through the stages of a campaign, you are able to see what step a campaign is at and what step comes next. You set up campaign status codes in the **Campaign Status** window.

You can create a campaign card for each campaign that you want to keep track of. You can also view these campaign cards to view general information about your campaigns.
You can delete campaign entries, such as if the entry records an action that has been cancelled. Only cancelled campaign entries can be deleted.

### <a name="selecting-the-target-audience"></a>Selecting the target audience
After you have created a campaign, you can start creating segments that specify the target audience of the campaign. For more information, see [Managing Segments](marketing-segments.md).

### <a name="registering-discount-percentages"></a>Registering discount percentages
When you have set up your campaign, decided what segments you want the campaign to cover, and set the starting and ending dates, you register the discount percentage that the customer will receive on the individual items on the lines in the **Sales Line Discounts** window. You can also register the sales prices for the individual items on the lines in the **Sales Prices** window. You can access both windows from the campaign card.

 When you have set up the sales prices/line discounts and the segments on the campaign card, you must activate them so that the campaign prices/discounts will be reflected on the lines.

> [!NOTE]  
>   In order to activate the sales prices/line discounts, you must specify if the whole segment or only some contacts are targets of the campaign. If the sales prices/line discounts covers all the contacts in the segment, select the **Campaign Target** field on the **Campaign** FastTab of the **Segment** card.

If the sales prices/line discounts are not to be offered to all the contacts in the segment, you can clear the **Campaign Target** field for the relevant contacts. If you cannot see this field, you can add it to your view. For more information, see [Personalising Your Workspace](ui-personalization-user.md).

## <a name="conducting-campaigns"></a>Conducting campaigns
As a campaign runs, all interactions with your contacts, or segment, are recorded so that you can get statistics and other information about the costs and success rates of the campaign.

Campaigns are conducted by salespeople, and you must create activities to represent each task and assign them to the relevant salespeople. For more information, see [Set Up Opportunity Sales Cycles and Cycle Stages](marketing-how-setup-opportunity-sales-cycles-stages.md).

## <a name="see-also"></a>See Also
[Managing Contacts](marketing-contacts.md)  
[Managing Segments](marketing-segments.md)  
[Managing Sales Opportunities](marketing-manage-sales-opportunities.md)  
[Working with Finance and Operations, Business edition](ui-work-product.md)  

