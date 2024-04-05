---
title: Run Tasks in the Background and Recurrently
description: Configure synchronisation of data between Business Central and Shopify in background.
ms.date: 03/26/2024
ms.topic: article
ms.service: dynamics-365-business-central
ms.reviewer: solsen
author: brentholtorf
ms.author: bholtorf
---

# Run tasks in the background

It's efficient to run some tasks simultaneously and in an automated manner. You can perform such tasks in the background and can also set a schedule when you want those tasks to run automatically. To run tasks in the background, two modes are supported:

- Manually triggered tasks are scheduled immediately via **Job Queue Entries**.
- Recurring tasks are scheduled in **Job Queue Entries**.

## Run tasks in the background for a specific shop

1. Choose the ![Lightbulb that opens the Tell Me feature.](../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Shopify Shop**, and choose the related link.
2. Select the shop for which you want to run synchronisation in background to open the **Shopify Shop Card** page.
3. Turn on the **Allow Background Syncs** toggle.

Now, when the sync action starts, instead of running a task in the foreground it asks you to wait. When it completes, you can proceed to the next action. The task is created as a **Job Queue Entry** and starts immediately.

## To schedule recurring tasks

You can schedule the following recurring activities to be performed in an automated manner. Learn more about scheduling tasks at [Job Queue](../admin-job-queues-schedule-tasks.md).

|Task|Object|
|------|------------|
|**Sync orders from Shopify**|Report 30104 Sync orders from Shopify|
|**Process Shopify orders**|Report 30103 Shopify create sales orders|
|**Sync shipments to Shopify**|Report 30109 Sync shipment to Shopify|
|**Sync products and/or prices**|Report 30108 Shopify sync products|
|**Sync inventory**|Report 30102 Sync stock to Shopify|
|**Sync images**|Report 30107 Shopify sync images|
|**Sync customers**|Report 30100 Shopify sync customers|
|**Sync companies**|Report 30114 Shopify sync companies (B2B)|
|**Sync payments**|Report 30105 Shopify sync payments|
|**Sync catalogues**|Report 30115 Shopify sync catalogues (B2B)|
|**Sync catalogue prices**|Report 30116 Shopify sync catalogue prices (B2B)|

> [!NOTE]
> Some elements might be updated by several tasks, for example when you import orders, depending on the setting in the **Shopify Shop Card**, the system may also import and update customer and/or product data. Remember to use the same job queue category to avoid conflicts.

Other tasks that can be helpful to automate further processing of sales documents:

- report 297 Batch Post Sales Invoices
- report 296 Batch Post Sales Orders

You can use the **Shopify Order No.** field to identify sales documents that were imported from Shopify.

To learn more about posting sales orders in a batch, go to [To create a job queue entry for batch posting of sales orders](../ui-batch-posting.md#to-create-a-job-queue-entry-for-batch-posting-of-sales-orders).

## To check the status of synchronisation

On the **Business Manager** Role Centre, the **Shopify Activities** part offers several cues that can help you quickly identify whether there are issues with Shopify Connector.

- **Unmapped Customers** - Shopify customer is imported, but isn't linked to a corresponding customer entry in [!INCLUDE [prod_short](../includes/prod_short.md)].
- **Unmapped Products** - Shopify product is imported, but isn't linked to a corresponding item entry in [!INCLUDE [prod_short](../includes/prod_short.md)].
- **Unprocessed Orders** - Shopify orders are imported, but sales documents in [!INCLUDE [prod_short](../includes/prod_short.md)] weren't created, often because of unmapped products or customers.
- **Unprocessed Shipments** - Posted sales shipments originated from Shopify orders aren't synchronised with Shopify.
- **Shipments Errors** - Shopify Connector couldn't synchronise posted sales shipments with Shopify.
- **Synchronisation Errors** - There are failed job queue entries related to synchronisation with Shopify.

## See also

[Get Started with the Connector for Shopify](get-started.md)  
