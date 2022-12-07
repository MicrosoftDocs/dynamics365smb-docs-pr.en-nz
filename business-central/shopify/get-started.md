---
title: Getting started with connector for Shopify
description: First steps when configuring connection between Business Central and Shopify
ms.date: 05/27/2022
ms.topic: article
ms.service: dynamics365-business-central
ms.reviewer: solsen
ms.search.form: 30100, 30101, 30102, 30103, 30104, 30135,
author: AndreiPanko
ms.author: andreipa
ms.openlocfilehash: bc3c5769a100909faedbfacce58bb1a2b146f5ad
ms.sourcegitcommit: bb6ecb20cbd82fdb5235e3cb426fc73c29c0a7ae
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 11/23/2022
ms.locfileid: "9803000"
---
# <a name="get-started-with-the-shopify-connector"></a>Get Started with the Shopify Connector

Connect your Shopify store (or stores) with [!INCLUDE [prod_short](../includes/prod_short.md)] and maximise your business productivity. Manage and view insights from your business and your Shopify store as one unit.

To use Shopify with [!INCLUDE [prod_short](../includes/prod_short.md)], you have to do a couple of things first. This article serves as a guide to integrate your Shopify store with [!INCLUDE [prod_short](../includes/prod_short.md)].

## <a name="prerequisites-for-shopify"></a>Prerequisites for Shopify

You must have:

- A Shopify account
- A Shopify online store

For more information on how to create Shopify trials and recommended settings, go to [Creating and Setting Up Shopify Account](shopify-account.md).

## <a name="prerequisites-for-business-central"></a>Prerequisites for Business Central

- Make sure that the **[Shopify Connector](https://go.microsoft.com/fwlink/?linkid=2196238)** app is installed.

  The app is pre-installed for all new sign-ups and trials. Learn more about installing apps from AppSource at [Installing and Uninstalling Extensions](../ui-extensions-install-uninstall.md#install). Follow the steps listed below if you don't have [!INCLUDE[prod_short](../includes/prod_short.md)].

- Ensure that user has enough permissions. Shopify Connector is covered by the *Shopify – Admin (SHPFY – ADMIN)* permission set. Learn more at [Create Users According to Licences](../ui-how-users-permissions.md) and [Assign Permissions to Users and Groups](../ui-define-granular-permissions.md)


## <a name="install-the-dynamics-365-business-central-app-to-your-shopify-online-store"></a>Install the Dynamics 365 Business Central app to your Shopify online store

For existing [!INCLUDE[prod_short](../includes/prod_short.md)], this step is optional and can be skipped.

1. Locate the [Dynamics 365 Business Central](https://apps.shopify.com/dynamics-365-business-central) app on the [Shopify AppStore](https://apps.shopify.com/)
2. Choose the **Add App** button. Sign in to your Shopify account if prompted. Select the required online shop if you've more than one.
3. After reviewing privacy and permissions, choose the **Install App** button.

   You can find and open the installed **Dynamics 365 Business Central** app in the **Apps** section on the sidebar of the **Shopify admin** page.
4. Choose **Sign up now** to start the [!INCLUDE[prod_short](../includes/prod_short.md)] trial or **Sign in** if you already have [!INCLUDE[prod_short](../includes/prod_short.md)]. You'll be redirected to your [Business Central](https://businesscentral.dynamics.com) page.
5. The next steps should be done in [!INCLUDE[prod_short](../includes/prod_short.md)].

## <a name="connect-business-central-to-the-shopify-online-store"></a>Connect Business Central to the Shopify online store

1. Choose the ![Lightbulb that opens the Tell Me feature.](../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Shopify Shop** and choose the related link.
2. Choose the **New** action.  
3. In the **Code** field, enter the code that will make it easy to find in [!INCLUDE[prod_short](../includes/prod_short.md)]. For example, a name might reflect what a shop sells, such as "Furniture" or "Coffee", or the country or region it serves.
4. In the **Shopify URL** field, enter your online shop URL, which needs to be connected. Use the following format: `https://{shop}.myshopify.com/`.
5. Activate the **Enabled** toggle, review, and accept the terms and conditions.
6. If prompted, sign in to your Shopify account, review the privacy terms and permissions, then choose the **Install App** button.

Repeat steps 2-6 for all online shops that you want to connect.

### <a name="known-issues"></a>Known issues

- The browser blocks the pop-up window. When you activate the **Enabled** toggle the system opens the **Waiting for a response - do not close this page** page, that is waiting for an access token from Shopify, if that page is closed or blocked - you can't connect to Shopify. Learn more at [Request the access token](troubleshoot.md#request-the-access-token)
- [Oauth error invalid_request: Could not find Shopify API application with api_key](troubleshoot.md#oauth-error-invalid_request-could-not-find-shopify-api-application-with-api_key)
- [Can't connect from sandbox](troubleshoot.md#verify-and-enable-permissions-to-make-http-requests-when-running-in-a-non-production-environment)


## <a name="next-steps"></a>Next steps

Now your online shop is connected to [!INCLUDE[prod_short](../includes/prod_short.md)]. In the next steps, you'll define how and what to synchronise.

- [Synchronise Items](synchronize-items.md)
- [Synchronise Customers](synchronize-customers.md)
- [Synchronise Orders](synchronize-orders.md)

## <a name="see-also"></a>See also

[Walkthrough: Setting Up and Using Shopify Connector](walkthrough-setting-up-and-using-shopify.md)  

