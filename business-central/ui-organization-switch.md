---
title: Switching to Another Company or Environment
description: If you do work for multiple organisations, you can quickly switch between the environments and companies.
author: brentholtorf
ms.topic: conceptual
ms.search.keywords: environments, companies, tenants, organization
ms.search.form: 9020, 9022, 9026, 9027, 9030, 9000, 9009, 9004, 9005, 9024, 9006, 9007, 9010, 9016, 9017
ms.date: 08/16/2022
ms.author: bholtorf
ms.openlocfilehash: 0cc18a4a84e24ce58d486275442ba686ed559047
ms.sourcegitcommit: 8ad79e0ec6e625796af298f756a142624f514cf3
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 09/30/2022
ms.locfileid: "9605971"
---
# <a name="switching-to-another-company-or-environment"></a>Switching to Another Company or Environment

[!INCLUDE [prod_short](includes/prod_short.md)] is available in many different countries and supports many different types of organisations. Your organisation may choose to organise work in [!INCLUDE [prod_short](includes/prod_short.md)] into multiple *companies* and *environments*. This article helps you understand the key differences and how to work across them.

## <a name="about-companies-and-environments"></a>About companies and environments

[!INCLUDE [company_environment](includes/company_environment.md)]

> [!TIP]
> If you often switch between companies, or work with [!INCLUDE[prod_short](includes/prod_short.md)] from within another app like Microsoft Teams, it can be easy to lose track of where you are. To help you keeping track, you can add a badge that will display the company name, so you can quickly verify that you're in the right place. For more information, see [Display a company badge](admin-company-information.md#badge).
> 
> Depending on your browser, you can also pin the different companies to your favourites bar.  

<!--
[!INCLUDE [about-ui-learn](includes/about-ui-learn.md)]-->

## <a name="features-for-switching-company-or-environment"></a>Features for switching company or environment

There are a few features you can use to switch the company or environment as you work. The following table compares the capabilities of the feature, which are explained in more detail in the sections that follow.

|Feature|Switch company|Switch environment|Switch in new browser tab| Available on-premises|
|-------|--------------|------------------|-------------------------|----------------------|
|[Company switcher](#use-the-company-switcher)|![check mark](media/check.png "cheque")|![check mark](media/check.png "cheque")|![check mark](media/check.png "cheque")|![check mark](media/check.png "cheque")|
|[App launcher](#use-the-app-launcher)||![check mark](media/check.png "cheque")|![check mark](media/check.png "cheque")||
|[My Settings](#use-my-settings)|![check mark](media/check.png "cheque")|||![check mark](media/check.png "cheque")|
|[Company Hub](#use-company-hub)|![check mark](media/check.png "cheque")|![check mark](media/check.png "cheque")|![check mark](media/check.png "cheque")||

## <a name="use-the-company-switcher"></a>Use the company switcher

Using the company switcher is probably the quickest and most versatile way to switch company. The company switcher is a pane that's readily available from any page. The pane gives an overview of all companies in all environments that you have access to, and lets you switch directly to any one of them&mdash;either in the same browser tab or a new one. It's especially useful when you work in many companies across different environments.

1. In upper-right corner, near the search icon, you'll see either the standard company icon, like ![company icon Launcher.](media/ui-experience/company-icon.png "Displays the company switcher icon used when there is a single environment") and ![company-icon-mult-env](media/ui-experience/company-icon-multi-env.png "Displays the company switcher icon used when there are multiple environments"), or a [custom badge](admin-company-information.md#badge) for the company you're currently working with. Select the icon to open the company switcher pane.

   :::image type="content" source="media/ui-experience/company-switch-2.png" alt-text="Shows the company switcher icon in the heading of the Business Central client.":::  

   > [!TIP]
   > You can also use the Crtl+O keyboard shortcut to open the pane.
2. In the **Available Companies** pane, select the company that you want to switch to, select the **Switch** arrow, then choose one of the following options:

   |Option|Description|
   |------|-----------|
   |Switch|Opens the role centre for selected company in the same browser tab that you're working in. The company becomes the default company that opens in Business Central, until you switch again or change the company by using **My Settings**. |
   |Open in new tab|Opens the role centre for selected company in a new browser tab, keeping the original company open in the other tab.|
   |Open in new tab and go to same page|This option is only active on list pages, like customers, sales orders, or items. It opens the same list, but for the selected company, in a new browser tab. |

> [!TIP]
> Press F5 to refresh list of environments and companies.

## <a name="use-the-app-launcher"></a>Use the app launcher

When you're signed in to [!INCLUDE[prod_short](includes/prod_short.md)], the environments that you can access are available on the Office.com.  

1. Select the **App Launcher** icon ![App Launcher.](media/app-launcher-icon.png "The App Launcher provides access to more features").
2. In the pane that opens, look for and choose [!INCLUDE[prod_short](includes/prod_short.md)]. If you don't see [!INCLUDE[prod_short](includes/prod_short.md)], choose **All apps**, then enter **Business Central** in the **Search** box.

   :::image type="content" source="media/app-launcher-bc-tile.png" alt-text="The Microsoft 365 app launcher showing the Business Central tile.":::  

3. If there's more than one environment, you'll be asked to choose the environment to access.

<!--
The following image shows tiles for accessing production and sandbox environments on the Dynamics 365 Home page.

:::image type="content" source="media/app-picker-environments.png" alt-text="The Dynamics 365 Home page showing production and sandbox environments.":::
-->
## <a name="use-my-settings"></a>Use My Settings

When you're signed in to [!INCLUDE[prod_short](includes/prod_short.md)], you can quickly switch to another company in the same environment. After you make the switch, the company you choose becomes your default company and will open the next time you sign in.

1. In the top-right corner, choose the **Settings** icon ![Settings.](media/ui-experience/settings_icon_small.png "Settings icon for role centre"), and then choose the **My Settings** action.

    > [!TIP]
    > You can also use the Alt+T keyboard shortcut to quickly open the My Settings page.

2. On the **My Settings** page, in the **Company** field, select the company.  
3. Choose the **OK** button.

> [!TIP]
> A good way to go directly to your default company when you sign in, and avoid having to specify an environment, is to add the the URL to your list of favourites after you sign in.

## <a name="use-company-hub"></a>Use company hub

*Company hub* is a highly Specialised role centre that gives a financial overview across companies and environments. Available as an [extension](ui-extensions-company-hub.md), company hub provides a dashboard with summary data for each company that you have access to. The home page displays financial KPIs and a direct link to the individual environments and companies. For more information, see [Manage Work across Multiple Companies in the Company Hub](company-hub.md).

[![Shows the company hub page that lists all companies.](media/company-hub.png)](media/company-hub.png#lightbox)  

## <a name="see-also"></a>See also

[Creating New Companies in [!INCLUDE[prod_short](includes/prod_short.md)]](about-new-company.md)  
[Change Basic Settings](ui-change-basic-settings.md)  
[Environments and companies (English only)](/dynamics365/business-central/dev-itpro/administration/tenant-environment-topology)  
[Company Information](admin-company-information.md)  
[The Business Central Administration Centre](/dynamics365/business-central/dev-itpro/administration/tenant-admin-center)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
