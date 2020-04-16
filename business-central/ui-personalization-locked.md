---
title: Why Can't I Personalise a Page | Microsoft Docs
description: Explains why you cannot personalise a page and what you can do to unlock it so you can personalise it.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: customize, personalize, personalization, hide columns, remove fields, move fields
ms.date: 04/01/2020
ms.author: sgroespe
ms.openlocfilehash: 9774c3472a70967f6b0250e2f02e817f26e9b710
ms.sourcegitcommit: 88e4b30eaf6fa32af0c1452ce2f85ff1111c75e2
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 04/01/2020
ms.locfileid: "3195739"
---
# <a name="why-a-page-is-locked-from-personalization"></a>Why a Page is Locked from Personalisation

There are two conditions that prevent you from personalising a page. Either the page is locked (as indicated by the ![Personalise Lock](media/personalization-lock-icon.png "Personalise lock")) icon or it is blocked (as indicated by the ![Personalisation blocked](media/personalization-blocked-icon.png "Personalisation blocked") icon).

## <a name="locked-from-personalizing"></a>Locked from Personalising

If there is a ![Personalise Lock](media/personalization-lock-icon.png "Personalise lock") icon in the **Personalising** banner when you open a page, this means that you are currently prevented from making any more personalisation changes to the page.

<!-- This is because we changed the way personalization works behind the scenes since the last time that you personalized the page. Unfortunately, the old way and new of doing things do not work together.

The page currently includes the last personalization changes that you made. If you want to continue personalizing the page, then you can choose the lock icon and then **Unlock**. Just be aware that if you choose to unlock the page, the current personalization of the page will be cleared, and you will have to start from scratch.
-->

There can be two reasons for this:

1. You have personalised the page before, but it was done using an earlier version of the product. We changed the way personalisation works behind the scenes since the last time that you personalised the page. Unfortunately, the old way and new way of doing things do not work together.

2. Until now, you have only used the [!INCLUDE[nav_windows_md](includes/nav_windows_md.md)] to personalise the page.

### <a name="unlocking-the-page"></a>Unlocking the Page

If you want to unlock a page and continue personalising it, choose the ![Personalise Lock](media/personalization-lock-icon.png "Personalise lock") icon, and then choose the **Unlock** action.  

Before you unlock the page, be aware of the following:

- The current personalisation of the page will be cleared. The page will go back to its original layout, and you will have to start from scratch.

- In the [!INCLUDE[nav_windows_md](includes/nav_windows_md.md)], the page will remain as-is and will not be affected by the new personalisation changes made in the Business Central client. Going forward, the personalisation in the [!INCLUDE[nav_windows_md](includes/nav_windows_md.md)] and Business Central client will be completely separate from each other.

## <a name="blocked-from-personalizing"></a>Blocked from Personalising

If there is a ![Personalisation blocked](media/personalization-blocked-icon.png "Personalisation blocked") icon in the **Personalising** banner, this means that you are blocked from doing any personalisation to the page.

<!-- Only text is translated, so removing this image for non-English UX reasons.  ![Personalize blocked](media/personalization-blocked.png "Personalize lock") -->

The reason for this is that the Role Centre or role that is currently associated with your user account modifies this page specifically for your role. Contact your administrator for assistance. Alternatively, try switching to a Role Centre that does include role-tailoring for this page. For more information, see [Change Basic Settings](ui-change-basic-settings.md).

## <a name="see-also"></a>See Also
[Personalise Your Workspace](ui-personalization-user.md)  
[Customise Pages for Profiles](ui-personalization-manage.md)  
[Change Basic Settings](ui-change-basic-settings.md)  
[Change Which Features are Displayed](ui-experiences.md)  
