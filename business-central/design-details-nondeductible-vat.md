---
title: Design details - Non-deductible GST
description: 'This article provides information about non-deductible goods and services tax (GST) that''s payable by a purchaser, but that isn''t deductible from the purchaser''s own GST liability.'
author: altotovi
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: null
ms.date: 07/04/2023
ms.author: altotovi
---

# Design details: Non-deductible GST

Non-deductible goods and services tax (GST) is the GST that's payable by a purchaser, but that isn't deductible from the purchaser's own GST liability. Because it can be difficult to know where and how an item is used, you must contact the local tax authorities in your country or region to determine whether a specified percentage of the GST is deductible. Even when you know that a specific percentage of the GST isn't deductible, there are different models for handling non-deductible amounts as they are related to **items** and **fixed assets**.

## Prerequisites for using non-deductible GST

To use and post non-deductible GST, follow these steps.

1. On the **GST Setup** page, select **Enable Non-Deductible GST** to enable the feature.
2. On the **GST Posting Setup** page, select which GST posting groups can use non-deductible GST.

## Examples

For the following examples, non-deductible GST is enabled, and the following setup is completed:

- The **GST Product Posting Group** field is set to **NDGST**.
- On the **GST Posting Setup** page:

    - **NDGST** is set as the GST product posting group, and **DOMESTIC** is set as the GST business posting group.
    - The **GST Identifier** value must be unique.
    - The **GST %** field is set to **25**.
    - The **Allow Non-deductible GST** field is set to **Allow**.
    - The **Non-deductible GST %** field is set to **100**.
    - The **GST Calculation Type** field is set to **Normal GST**.
    - Only the sales GST account and purchase GST account are configured.

All the examples use items and fixed assets where the GST product posting group is **NDGST**.

### Items

A new item has **NDGST** set as the GST product posting group. In the purchase document, **Quantity** = **1** and **Direct Unit Cost Excl. GST** = **1,000.00**.

Regardless of the option that's used, the results in the GST entry are the same.

| Document Type | Type | Base | Amount | Non-Deductible GST Base | Non-deductible GST Amount |
|---|---|---|---|---|---|
| Invoice | Purchase | 0.00 | 0.00 | 1,000.00 | 250.00 |

The details are shown in the value entries.

> [!NOTE]
> You can enable the **Use for Item Cost** field on the **GST Setup** page.

#### Use for Item Cost isn't enabled

| Item Ledger Entry Type | Entry Type | Cost Amount (Actual) | Item Ledger Entry Quantity |
|---|---|---|---|
| Purchase | Direct Cost | 1,000.00 | 1 |

#### Use for Item Cost is enabled

| Item Ledger Entry Type | Entry Type | Cost Amount (Actual) | Item Ledger Entry Quantity |
|---|---|---|---|
| Purchase | Direct Cost | 1,250.00 | 1 |

### Fixed assets

A new fixed asset has the acquisition cost account set to use **NDGST** as the GST product posting group. In the purchase document, **Quantity** = **1** and **Direct Unit Cost Excl. GST** = **1,000.00**.

Regardless of the option that's used, the results in the GST entry are the same.

| Document Type | Type | Base | Amount | Non-Deductible GST Base | Non-deductible GST Amount |
|---|---|---|---|---|---|
| Invoice | Purchase | 0.00 | 0.00 | 1,000.00 | 250.00 |

The details are shown in the fixed asset ledger entries.

> [!NOTE]
> You can enable the **Use for Fixed Asset Cost** field on the **GST Setup** page.

#### Use for Fixed Asset Cost isn't enabled

| Document Type | FA Posting Type | Amount | GST Amount |
|---|---|---|---|
| Invoice | Acquisition Cost | 1,000.00 | 250.00 |

#### Use for Fixed Asset Cost is enabled

| Document Type | FA Posting Type | Amount | GST Amount |
|---|---|---|---|
| Invoice | Acquisition Cost | 1,000.00 | 250.00 |
| Invoice | Acquisition Cost | 250.00 | 0.00 |

## See also

[Set up non-deductible GST](finance-setup-nondeductible-vat.md)  
[Finance](finance.md)  
[Work with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)

[!INCLUDE[footer-include](includes/footer-banner.md)]
