---
title: Troubleshooting the Shopify and Business Central synchronisation
description: Learn what to do if something went wrong during the synchronisation of data between Shopify and Business Central
ms.date: 05/16/2022
ms.topic: article
ms.service: dynamics365-business-central
author: edupont04
ms.author: andreipa
ms.reviewer: solsen
ms.openlocfilehash: bebdf73fd1b01a3c750a3d91496a8f5bb87f8db4
ms.sourcegitcommit: f1e272485a0e675d337a694aba3e35a5daf43920
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 07/09/2022
ms.locfileid: "9129657"
---
# <a name="troubleshooting-the-shopify-and-business-central-synchronization"></a>Troubleshooting the Shopify and Business Central Synchronisation

It's possible to run into situations where you need to troubleshoot issues when synchronising data between Shopify and [!INCLUDE[prod_short](../includes/prod_short.md)]. This page defines steps to troubleshoot some common scenarios that may arise.

## <a name="logs"></a>Logs

If a synchronisation task fails, you can activate logging by enabling the **Log Enable** toggle in the **Shopify Shop Card**. Manually trigger the synchronisation task and review logs.

1. Choose the ![Lightbulb that opens the Tell Me feature 1.](../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Shopify Log Entries**, and then choose the related link.
2. Select the related log entry and open the **Shopify Log Entry** window.
3. Review the request, status code and description, and response.

Remember to switch off logging later to avoid negative performance impacts and increases in database size.

From the **Shopify Log Entries** window, you can trigger the deletion of all log entries or ones that are older than seven days.

## <a name="data-capture"></a>Data capture

Regardless of the **Log Activated** settings, some responses from Shopify always get logged that you can inspect or download using the **Data Capture List** window.

Choose the **Retrieved Shopify Data** action in one of following pages:

- **Shopify order**
- **Shopify order fulfillments**
- **Shopify order shipping costs**
- **Shopify order transactions**
- **Shopify payouts**
- **Shopify payment transactions**
- **Shopify transactions**

## <a name="reset-sync"></a>Reset sync

For optimal performance, the connector imports only customers, products, and orders created or changed since last synchronisation. On the **Shopify Shop card**, there are functions available to change the date/time of the last synchronisation or completely reset it. This function ensures that when the sync is run, all data is synced and not just the changes since the last sync.

This function only applies to syncs from Shopify to [!INCLUDE[prod_short](../includes/prod_short.md)] and can be useful if you need to restore deleted data such as products, customers, or deleted orders.

## <a name="request-the-access-token"></a>Request the access token

If [!INCLUDE[prod_short](../includes/prod_short.md)] can't connect to your Shopify account, try to request the access token from Shopify. This request might be needed if there is a rotation of security keys or changes in required permissions (scopes).

1. Choose the ![Lightbulb that opens the Tell Me feature 1.](../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Shopify Shops**, and then choose the related link.
2. Select the shop for which you want to get the access token to open the **Shopify Shop Card** page.
3. Choose the **Request Access** action.
4. If prompted, sign in to your Shopify account.

The **Has AccessKey** toggle will be activated.

### <a name="verify-and-enable-permissions-to-make-http-requests-when-running-in-a-non-production-environment"></a>Verify and enable permissions to make Http requests when running in a non-production environment

In order to work correctly, the Shopify Connector extension requires permission to make Http requests. When testing in Sandboxes, the Http requests are prohibited for all extensions.

1. Choose the ![Lightbulb that opens the Tell Me feature 1.](../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Extension Management**, and then choose the related link.
2. Select the *Shopify Connector* extension.
3. Choose the **Configure** action to open the **Extension Setting** page.
4. Make sure that the **Allow HTTPClient Requests** toggle is enabled.

## <a name="rotate-the-shopify-access-key"></a>Rotate the Shopify Access key

The following procedures describe how to to rotate the access token used by the Shopify Connector to access your Shopify online shop.

### <a name="in-shopify"></a>In Shopify

1. From your **Shopify admin**, go to [Apps](https://www.shopify.com/admin/apps).
2. In the row with the **Dynamics 365 Business Central** app, select **Delete**.
3. In the message that appears, select **Delete**.

### <a name="in-prod_short"></a>In [!INCLUDE[prod_short](../includes/prod_short.md)]

1. Choose the ![Lightbulb that opens the Tell Me feature 1.](../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Shopify Shops**, and then choose the related link.
2. Select the shop for which you want to rotate the access token to open the **Shopify Shop Card** page.
3. Choose the **Request Access** action.
4. If prompted, sign-in into your Shopify account, review privacy and permissions, and then choose the **Install App** button.

## <a name="see-also"></a>See also

[Get Started with the Connector for Shopify](get-started.md)  