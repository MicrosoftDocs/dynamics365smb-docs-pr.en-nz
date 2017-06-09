---
title: Setting up marketing campaigns in Financials | Microsoft Docs
description: Describes how you can set up and conduct marketing campaigns in Dynamics 365 for Financials
services: project-madeira
documentationcenter: 
author: edupont04
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: marketing, campaign, promo, prospect
ms.date: 03/08/2017
ms.author: edupont
ms.translationtype: Human Translation
ms.sourcegitcommit: a31be0f9d07e2abb591e26f6bae34c6f6e4dcda6
ms.openlocfilehash: 8f616382e28e29aab1ce7d9b45b8efb4ad374b96
ms.contentlocale: en-nz
ms.lasthandoff: 05/04/2017


---
# <a name="managing-marketing-campaigns"></a>Managing Marketing Campaigns
Having a strong marketing plan in place enables you to identify, attract, and retain customers. A marketing plan consists of various campaigns and other interactions in connection with your sales and marketing activities. While planning a campaign, you need to decide which contacts to target, what type of campaign (such as trade show or direct mail), and what salespeople will perform each task.

<!-- Each campaign consists of various activities or to-dos. Activities are large tasks that can be broken down into several smaller tasks or to-dos. To-dos are individual or team tasks that can be created within activities or individually and then be assigned to individual salespeople or groups of salespeople.-->

## <a name="defining-individual-campaigns"></a>Defining individual campaigns
Before you can create a campaign, you must set up *campaign status codes*. Using these codes will help you manage your campaigns by assigning a status to the campaign. As you work through the stages of a campaign, you are able to see what step a campaign is at and what step comes next. You set up campaign status codes in the **Campaign Status** window.

You can create a *campaign card* for each campaign that you want to keep track of. You can also view these campaign cards to view general information about your campaigns.
You can delete campaign entries, such as if the entry records an action that has been cancelled. Only cancelled campaign entries can be deleted.

### <a name="selecting-the-target-audience"></a>Selecting the target audience
After you have created a campaign, you can start creating segments that specify the target audience of the campaign. For more information, see [Managing Segments](marketing-segments.md).

### <a name="registering-discount-percentages"></a>Registering discount percentages
When you have set up your campaign, decided what segments you want the campaign to cover, and set the starting and ending dates, you register the discount percentage that the customer will receive on the individual items on the lines in the **Sales Line Discounts** window. You can also register the sales prices for the individual items on the lines in the **Sales Prices** window. You can access both windows from the campaign card.

 When you have set up the sales prices/line discounts and the segments on the campaign card, you must activate them so that the campaign prices/discounts will be reflected on the lines.

> [!NOTE]  
>  In order to activate the sales prices/line discounts, you must specify if the whole segment or only some contacts are targets of the campaign. If the sales prices/line discounts covers all the contacts in the segment, select the **Campaign Target** field on the **Campaign** FastTab of the **Segment** card.
If the sales prices/line discounts are not to be offered to all the contacts in the segment, you can clear the **Campaign Target** field for the relevant contacts. If you cannot see this field, you can add it to your view. For more information, see [User Personalization](ui-user-personalization.md).

<!-- ## Conducting campaigns
As a campaign runs, all interactions with your contacts, or segment, are recorded so that you can get statistics and other information about the costs and success rates of the campaign.

Campaigns are conducted by salespeople, and you must create activities to represent each task and assign them to the relevant salespeople.  -->

## <a name="see-also"></a>See Also
[Managing Contacts](marketing-contacts.md)  
[Managing Segments](marketing-segments.md)  
[Managing Sales Opportunities](marketing-manage-sales-opportunities.md)  
[Working With Financials](ui-work-product.md)  

