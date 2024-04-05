---
title: Suggest sales lines with Copilot
description: Learn how to suggest lines on sales orders with Copilot.
author: brentholtorf
ms.author: bholtorf
ms.reviewer: andreipa
ms.topic: how-to
ms.search.keywords: 'Copilot, AI, sell'
ms.search.form: null
ms.date: 02/02/2024
ms.service: dynamics-365-business-central
ms.custom: bap-template
ms.collection: bap-ai-copilot
---

# Suggest lines on sales documents with Copilot (preview)

[!INCLUDE[preview-banner](includes/preview-banner.md)]

This article explains how to create sales documents faster by letting Copilot suggest the items to add to lines on sales documents for your customers.

[!INCLUDE[production-ready-preview-dynamics365](includes/production-ready-preview-dynamics365.md)]

## About sales line suggestions with Copilot

Sales line suggestion with Copilot can assist with creating lines on sales documents such as sales quotes, orders, and invoices based on structured input or natural language. The feature isn't a general-purpose chat, but a highly specific and integrated experience that you can use on sales documents. The feature offers two distinct skills that help you find data about individual products or the entire documents.

* Find products

  Information that describes products is stored in multiple places in [!INCLUDE [prod_short](includes/prod_short.md)]. For example, item numbers and descriptions are stored in the **Item** table, multiple barcodes are stored in the **Item Reference** table, and product properties are stored in the **Item Attributes** table. While you might prompt for *Red bicycle*, the actual product might be *Crimson tourer*, where *Bicycle* is a product category and *red* is an attribute.

* Find documents by reference

  People often repeat a previous order, or at least use it as a starting point. But it might be tricky to find the right order in a stack of orders. You might remember some of the order's ID, which can be a company assigned number or a reference number received from a customer. Being able to use prompts such as *Need last invoice from April* should help you find an order faster.

## Prerequisites

* Sales line suggestion with Copilot is enabled and activated by an administrator. To learn more about how to enable AI capabilities, go to [Configure Copilot and AI capabilities](enable-ai.md).
* You're familiar with creating sales orders.

## Geographic availability

The following table shows the Microsoft Azure geographic areas in which his feature is available.

|Environment Azure region  |Azure OpenAI Service geography   |Admin action required to unlock Copilot  |
|---------|---------|---------|
|Germany (North, West Central)     | Sweden or Switzerland        |  Yes       |
|Norway (East, West)     | Sweden or Switzerland        | Yes     |
|Singapore     |         |         |
|South Africa (North, West)     |   United States      |   Yes      |
|Switzerland (North, West)     |  Sweden or Switzerland       |    Yes     |
|United Arab Emirates (North, West)     |    United States     |   Yes     |
|United States (Central, East, North Central, South Central, West)     |   United States      |   No      |
|Europe (West, North)     |   Sweden or Switzerland      |   Yes      |
|Asia Pacific     |         |         |
|Australia (South East)     |   United States      |    Yes     |
|South America     |         |         |
|India (Central, South)     |    United States     |   Yes      |
|Japan (East, West)     |    United States     |    Yes     |
|France (Central, South)     |    Sweden or Switzerland     |    Yes     |
|Korea (Central, South)     |    United States     |    Yes     |

## Examples of prompts

Suggest sales lines with Copilot can handle a wide variety of prompt input. This section offers some examples of prompts for various scenarios we've tested.

### Sample inquiry to repeat the past document

Prompt: *Need all the products from invoice 103031*

### During phone call user quickly types list of required products and quantities, not always accurate enough or using internal product names

Prompt: *2 Red Kids Biicycle*

Note that the prompt works, even with multiple typos.

### A user copies an inquiry from an inbound communication and pastes it to the Sales Lines Suggestions page

Prompt: *Hello, I am interested in buying some accessories for my XXXX Laptop, such as a wireless mouse, a keyboard cover, and a laptop bag. I wonder if you have any recommendations or suggestions for these items. Do you have any special offers or discounts for loyal customers like me? Kind regards, M*

Note that XXXX Laptop is not included in search.

## Suggest lines on a sales document

This process describes how to suggest lines on a sales order. The steps are the same for sales quotes and invoices.

1. Select the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Order**, and then choose the related link.
1. Open the sales order.
1. On the **Lines** FastTab, choose **Get line suggestions**.
1. In the **Suggest lines with Copilot** window, enter your prompt or select one from prompt guides.

## Review, save, discard, or regenerate suggestions

After Copilot suggests the items to add to lines, review its suggestions and decide whether they're what you want:

* To discard a single proposed line, select it in the list, and then choose the **Delete Line** action.
* To discard all proposed lines and close the Copilot window, choose the Discard button (trash can) next to the **Keep it** button.
* To transfer the lines shown in the Copilot window, choose **Keep it**. 

There is a **Reliability** field that displays **High (80+)**, **Medium (60-80)**, and **Low (60-)** scores and points you to lines that need attention.

This step confirms that you want to transfer the lines to a sales document. You can delete or edit the transferred lines there as well, or delete the whole document.

## See also

[FAQ for Sales Line Suggestions with Copilot](faq-sales-suggest-sales-lines-with-copilot.md)
[Configure Copilot and AI capabilities](enable-ai.md)
