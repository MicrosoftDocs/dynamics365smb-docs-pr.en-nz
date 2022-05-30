---
title: Troubleshooting the Shopify and Business Central synchronisation
description: Learn what to do if something when wrong during synchronisation of data between Shopify and Business Central
ms.date: 05/16/2022
ms.topic: article
ms.service: dynamics365-business-central
author: edupont04
ms.author: andreipa
ms.reviewer: solsen
ms.openlocfilehash: 01ff5ab1c5e6f132098f914f6bfe97e097cc88b0
ms.sourcegitcommit: f071aef3660cc3202006e00f2f790faff849a240
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 05/18/2022
ms.locfileid: "8768255"
---
# <a name="troubleshooting-the-shopify-and-business-central-synchronization"></a>Troubleshooting the Shopify and Business Central Synchronisation

It's possible to run into situations where you need to troubleshoot issues. This page defines steps to troubleshoot some common scenarios that may arise.

## <a name="logs"></a>Logs

If a synchronisation task fails, you can activate logging by enabling **Log Enable** toggle in the **Shopify Shop Card**. Manually trigger synchronisation task and review logs.

1. Go to the search ![Lightbulb that opens the Tell Me feature.](../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Shopify Log Entries**, and choose the related link.
2. Select the related log entry and open the **Shopify Log Entry** window.
3. Review request, status code and description, and response.

Remember to switch off logging to avoid negative performance impact and increase in database size.

From the **Shopify Log Entries** window, you can trigger deletion of all log entries or ones that are older than seven days.

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

For optimal performance, the connector imports only customers, products, and orders created or changed since last synchronisation. On the **Shopify Shop card**, there are functions available to change date/time of last synchronisation or completely reset it. This function ensures that when the sync is run, all data is synced and not just the changes since the last sync.

This function only applies to syncs from Shopify to [!INCLUDE[prod_short](../includes/prod_short.md)] and can be useful if you need to restore deleted data such as products, customers, or deleted orders.

## <a name="update-the-access-token"></a>Update the access token

If [!INCLUDE[prod_short](../includes/prod_short.md)] can't connect to your Shopify account, try resetting the access token.

1. Go to the search ![Lightbulb that opens the Tell Me feature.](../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Shopify Shop**, and choose the related link.
2. Select the shop for which you want to get the access token to open the **Shopify Shop Card** page.
3. In the **Code** field, enter the code.  
4. Choose the **Request Access** action.
5. If prompted sign-in to your Shopify account.

## <a name="see-also"></a>See Also

[Get Started with the Connector for Shopify](get-started.md)  
