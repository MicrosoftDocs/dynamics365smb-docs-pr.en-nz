---
title: Mobile Apps FAQ
description: See answers to frequently asked questions about using Business Central on your phone or tablet.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: phone, tablet
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: f92fdec0329286750fd844fc18ed79c7f7c642d5
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 03/31/2021
ms.locfileid: "5771076"
---
# <a name="mobile-apps-faq"></a>Mobile Apps FAQ

This article answers questions that our advanced users often ask about the mobile apps for [!INCLUDE [prod_short](includes/prod_short.md)].  

## <a name="is-there-an-app-for-my-device"></a>Is there an app for my device?

Probably! Install the [!INCLUDE[prod_short](includes/prod_short.md)] app on your mobile device by downloading the app from the Windows Store, App Store, or Google Play.

- [Windows Store](https://go.microsoft.com/fwlink/?LinkId=734848) (PC only)
- [App Store](https://go.microsoft.com/fwlink/?LinkId=734847)
- [Google Play](https://go.microsoft.com/fwlink/?LinkId=734849)

## <a name="is-it-the-same-experience-in-the-apps-as-in-the-browser"></a>Is it the same experience in the apps as in the browser?

No, not exactly. For example, we show only the **Home** activity group due to the limited screen size on mobile devices. Similarly, the keyboard shortcuts are not available because you mainly use touch rather than a keyboard to navigate on mobile devices.

The following table describes some of the most common differences and limitations that you might experience when using [!INCLUDE [prod_short](includes/prod_short.md)] on mobile devices, compared to the browser.

| Concept | On tablets | On phones | Example from the browser |
|--|--|--|--|
| Activity groups | Only the **Home** activity group is shown. | Only the **Home** activity group is shown. | **Home** and **Posted Documents** on the `Sales Order Processor` Role Centre. |  |
| Selecting multiple records in lists | Not available. | Not available. | `Ctrl+A` or `Ctrl+Click` on rows in a list in the browser. |
| Actions in the action bar | Only Promoted actions are shown. | Only Promoted actions are shown. |  |
| FactBoxes | Not shown on List pages or Worksheet pages. | Not shown on List pages or Worksheet pages. | `Customer` list on the `Small Business` Role Centre. |
| Advanced filters | No column-specific filtering is available. | No column-specific filtering is available. | On the `Customer` list page. |
| Tell Me | Not available yet. | Not available yet. | See [Finding Pages and Information with Tell Me](ui-search.md). |  |
| Role Explorer | Not available yet. | Not available yet. | See [Finding Pages with the Role Explorer](ui-role-explorer.md). |
| Fields in FastTabs | Fields in FastTabs on list pages are not shown. Only the repeater control is shown in the content area of the page. | Not available. |  |
| Select from full list | Not available on lookups. Users are not able to run actions on a lookup page, and they cannot access the full set of records. | Not available on lookups. Users are not able to run actions on a lookup page, and they cannot access the full set of records. | On the `Item Card` when selecting the **Base Units of Measure**. |
| Search across list columns | Partly supported. Search will not include FlowFields. | Partly supported. Search will not include FlowFields. | See examples on the `Customers` list page. |
| Lookups | Available. | Available, with the difference that advanced and simple lookups behave similarly on the phone. The lookup will not bring up the card, show FactBoxes, or any field groups. | See examples on the `Customer Card` page. |
| Matrix controls | Not available. | Not available. | See example in `G/L Budget`. |
| File download | Available. Cannot download multiple files at the same time. | Available. Cannot download multiple files at the same time. | `Trial Balance` report in the **Print to Excel** check box. |
| Worksheet pages | Available. | Not available; an error message is displayed. | `Sales Price` Worksheet or `Cash Flow` Worksheet. |
| Lists | Available. | Available, with the difference that these are displayed in a brick layout. | Customers or Sales Orders pages. |
| Indentation in repeater controls | Available. | Not available. The repeater control will be rendered as a regular flat brick layout. | Chart of Accounts and Contacts List pages. |
| Automatic input focus on first editable field of a page | Not available. | Not available. | `Customer Card` page.<BR /><BR />In the browser, focus will automatically be on the first editable field (such as the `Name` field), enabling you to change the value right away.<BR /><BR />In the tablet and phone apps, this field will not be in focus; instead, you will have to manually select the field first in order to make changes.|

## <a name="is-it-the-same-experience-on-tables-and-phones"></a>Is it the same experience on tables and phones?

Almost, but not quite. See the list in the [Is it the same experience in the apps as in the browser?](#is-it-the-same-experience-in-the-apps-as-in-the-browser) section.  

## <a name="can-i-connect-the-app-to-our-on-premises-solution"></a>Can I connect the app to our on-premises solution?

Yes, you can! It's a slightly different way to signing in, that's all. For more information, see [Using Business Central on-premises?](install-mobile-app.md#using-business-central-on-premises).  

## <a name="see-also"></a>See also

[Getting Business Central on Your Mobile Device](install-mobile-app.md)  
[Install the Business Central App for Microsoft Teams](across-install-app-for-teams.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]