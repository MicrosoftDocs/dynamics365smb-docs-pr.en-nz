---
title: Set up nondeductible GST
description: This article explains how to configure nondeductible GST in Microsoft Dynamics 365 Business Central.
author: altotovi
ms.author: altotovi
ms.reviewer: null
ms.service: dynamics-365-business-central
ms.topic: how-to
ms.search.keywords: 'VAT, non-deductible, setup'
ms.search.form: '187, 472, 473'
ms.date: 04/26/2023
ms.custom: bap-template
---

# Set up nondeductible GST

Nondeductible goods and services tax (GST) is the GST that's payable by a purchaser but that isn't deductible from the purchaser's own GST liability. Companies can usually recover GST on the purchase of goods and services that are related to their business activities. However, in some situations, a business incurs GST that isn't deductible. These situations are typically related to the local regulations and can differ among countries/regions. However, the model of using nondeductible or partially deductible GST is similar. You can use proportional GST to calculate GST when there's deductible and nondeductible GST.

In general, GST can't be deducted for some purchases because of the following factors:

- **The type of goods or services that are purchased** – GST is fully or partially nondeductible according to the law about goods such as cars, mobile phones, and food purchased at restaurants.
- **Partially deductible pro-rated GST** – GST is pro-rated according to the ratio between the sales operations that GST is owed for and all performed operations. GST that exceeds this ratio can't be deducted.

Because it can be difficult to know where and how an item is used, contact the local tax authorities in your country/region. They can help determine whether you can deduct a specified percentage of the GST, based on historical data.

> [!IMPORTANT]
> This global feature is available in all countries with enabled VAT **except for Belgium, Italy, and Norway**. These localisations already have existing local feature and will be upgraded in the future. Don't run this feature in these countries because the upgrade procedure doesn't exist.

## Use nondeductible GST

1. Select the ![Lightbulb that opens the Tell Me feature 3.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **GST Setup**, and then select the related link.
2. Select the **Enable Non-Deductible GST** checkbox.

    > [!IMPORTANT]
    > After you enable non-deductible GST, you can't turn it off, because the feature might include changes to data and might initiate an upgrade of some database tables. Microsoft strongly recommends that you first enable and test this feature in the sandbox environment before you enable it in the production environment.

3. Configure how the [!INCLUDE [prod_short](includes/prod_short.md)] treats nondeductible GST values.

    1. In the **Use For Item Cost** field, specify whether the nondeductible GST must be added to the item cost when you purchase items. Otherwise, the nondeductible GST won't influence the item cost and the full amount is recorded only at the general ledger level.
    2. Select the **Use For Fixed Asset Cost** checkbox to add the nondeductible GST to the fixed asset cost when you purchase new fixed assets. Otherwise, the nondeductible GST won't influence the fixed asset cost and the full amount is recorded only at the general ledger level.
    3. Select the **Use For Job Cost** checkbox to specify that the nondeductible GST must be added to the project cost when you purchase items for the project. Otherwise, the nondeductible GST won't influence the project cost and the full amount is recorded only at the general ledger level.
    4. Select the **Show Non-Ded. GST In Lines** checkbox to specify that the nondeductible GST must be shown on document line pages for easier manipulation of GST amounts.

## Use the nondeductible GST percentage

1. Select the ![Lightbulb that opens the Tell Me feature 3.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **GST Posting Setup**, and then select the related link.
2. On the **GST Posting Setup** page, set the fields as described in the following table.

    | Field | Description |
    |-------|-------------|
    | Allow Non-Deductible GST | Specify whether the nondeductible GST is considered for the current combination of a GST business posting group and a GST product posting group. |
    | Non-Deductible GST % | Specify the percentage of the transaction amount that GST isn't applied to. |
    | Non-Deductible Purchase GST Account | Specify the account associated with the GST amount that isn't deducted because of the type of goods or services that are purchased. |

    > [!NOTE]
    > To have general ledger (G/L) entries that use the dedicated account instead of the sales/purchase account, you can either leave the **Non-Deductible Purchase GST Account** field blank or set the **G/L Account** field.

3. Select **OK**.

> [!NOTE]
> You can't use unrealised GST together with non-deductible GST.
>
> Don't use the same **GST identifier** value for both normal GST where the **Non-Deductible GST %** field is set to **0** (zero) and normal GST where the **Non-Deductible GST %** field is set to a non-zero value. Otherwise, the total non-deductible GST amount will be incorrectly calculated.

## See also

[Financial Management](finance.md)  
[Design details: Nondeductible GST](design-details-nondeductible-vat.md)  
[Use nondeductible GST](finance-how-use-non-deductible-vat.md)  
[Set Up Calculations and Posting Methods for Goods and Services Tax](finance-setup-vat.md)  
[Work with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
