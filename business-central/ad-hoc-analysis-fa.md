---
title: Ad-hoc analysis of fixed assets data
description: Learn how to use the data analysis mode to analyse fixed assets data.
author: kennienp
ms.author: kepontop
ms.reviewer: bholtorf
ms.topic: conceptual
ms.search.keywords: 'bi, power BI, analysis, KPI'
ms.search.form: '5604, 20'
ms.date: 05/02/2024
ms.service: dynamics-365-business-central
ms.custom: bap-template
---

# <a name="ad-hoc-analysis-of-fixed-assets-data"></a>Ad-hoc analysis of fixed assets data

This article explains how to use the **Data Analysis** feature to analyse fixed assets data directly from list pages and queries. You don't have to run a report or switch to another application, such as Excel. The feature provides an interactive and versatile way to calculate, summarise, and examine data. Instead of running reports using options and filters, you can add multiple tabs that represent different tasks or views on the data. Some examples are "Total assets," "Depreciations over time," or any other view you can imagine. To learn more about how to use the **Data Analysis** feature, go to [Analyse list and query data with analysis mode](analysis-mode.md).

Use the following list pages to start doing ad-hoc analysis of fixed assets processes:

- [FA Ledger Entries](https://businesscentral.dynamics.com/?page=5604)
- [General Ledger Entries](https://businesscentral.dynamics.com/?page=20)

## <a name="fixed-assets-ad-hoc-analysis-scenarios"></a>Fixed assets ad-hoc analysis scenarios

Use the **Data Analysis** feature for quick fact checking and ad-hoc analysis:

- If you don't want to run a report.
- If a report for your specific need doesn't exist.
- If you want to quickly iterate to get a good overview on a part of your business.

The following sections provide examples of fixed assets scenarios in [!INCLUDE [prod_short](includes/prod_short.md)].

| Area | To... | Open this page in analysis mode | Using these fields |
| ---- | ----- | ------------------------------- |------------------- |
| [Fixed Assets (Current value)](#example-fixed-assets-current-value) | Track asset value, both across all assets and on a single asset. | [FA Ledger Entries](https://businesscentral.dynamics.com/?page=5604) | **Depreciation Book**, **FA No.**, **FA Posting Date**, **FA Posting Type**, and **Amount** |
| [Asset value changes over time](#example-asset-value-changes-over-time) | Track asset value changes over time. | [FA Ledger Entries](https://businesscentral.dynamics.com/?page=5604) | **FA Posting Type**, **FA Posting Date**, and **Amount** |
|[Fixed asset depreciations over time](#example-fixed-asset-depreciations-over-time) | Track depreciations over time, both across all assets and on a single asset. | [FA Ledger Entries](https://businesscentral.dynamics.com/?page=5604) | **Depreciation Book**, **FA No.**, **FA Posting Year**, **FA Posting Month**, **Amount**, and **FA Posting Type** |

### <a name="example-fixed-assets-current-value"></a>Example: fixed assets current value

To track the value of one or more fixed assets, follow these steps:

1. Open the [FA Ledger Entries](https://businesscentral.dynamics.com/?page=5604) list, and choose :::image type="content" source="media/analysis-mode-icon.png" alt-text="Enter analysis mode."::: to turn on analysis mode.
1. Go to the **Columns** menu and remove all columns (select the box next to the **Search** field on the right).
1. Drag the **Depreciation Book** and **FA No.** fields to the **Row Groups** area.
1. Choose the **FA Posting Date** and **FA Posting Type** fields.
1. Drag the **Amount** field to the **Values** area.
1. Rename your analysis tab to **Asset overview - value**, or something that describes this analysis.

The following image shows the result of these steps.

:::image type="content" source="media/data-analysis-fa-ledger-entries-asset-overview-current-value.png" alt-text="Example of how to do data analysis on the FA Ledger Entries page to see the value of an asset." lightbox="media/data-analysis-fa-ledger-entries-asset-overview-current-value.png":::

### <a name="example-asset-value-changes-over-time"></a>Example: asset value changes over time

To track asset value changes over time, follow these steps:

1. Open the [FA Ledger Entries](https://businesscentral.dynamics.com/?page=5604) list, and choose :::image type="content" source="media/analysis-mode-icon.png" alt-text="Enter analysis mode."::: to turn on analysis mode.
1. Go to the **Columns** menu and remove all columns (select the box next to the **Search** field on the right).
1. Turn on the **Pivot Mode** toggle (located above the **Search** field on the right).
1. Drag the **FA Posting Type** field to the **Row Groups** area.
1. Drag the **FA Posting Year** and **FA Posting Month** fields to the **Column Labels** area.
1. Drag the **Amount** field to the **Values** area.
1. Rename your analysis tab to **Asset value changes over time**, or something that describes this analysis.

The following image shows the result of these steps.

:::image type="content" source="media/data-analysis-fa-ledger-entries-asset-changes-over-time.png" alt-text="Example of how to do data analysis on the FA Ledger Entries page to see asset value changes over time." lightbox="media/data-analysis-fa-ledger-entries-asset-changes-over-time.png":::

### <a name="example-fixed-asset-depreciations-over-time"></a>Example: fixed asset depreciations over time

To track depreciation for one or more fixed assets, follow these steps:

1. Open the [FA Ledger Entries](https://businesscentral.dynamics.com/?page=5604) list, and choose :::image type="content" source="media/analysis-mode-icon.png" alt-text="Enter analysis mode."::: to turn on analysis mode.
1. Go to the **Columns** menu and remove all columns (select the box next to the **Search** field on the right).
1. Turn on the **Pivot Mode** toggle (located above the **Search** field on the right).
1. Drag the **Depreciation Book** and **FA No.** fields to the **Row Groups** area.
1. Drag the **FA Posting Year** and **FA Posting Month** fields to the **Column Labels** area.
1. Drag the **Amount** field to the **Values** area.
1. In the **FA Posting Type** filter field, choose **Depreciation**.
1. Rename your analysis tab to **Depreciations over time**, or something that describes this analysis.

The following image shows the result of these steps.

:::image type="content" source="media/data-analysis-fa-ledger-entries-depreciation-by-asset.png" alt-text="Example of how to do data analysis on the FA Ledger Entries page to see depreciation over time." lightbox="media/data-analysis-fa-ledger-entries-depreciation-by-asset.png":::

## <a name="data-foundation-for-ad-hoc-analysis-on-fixed-assets"></a>Data foundation for ad-hoc analysis on fixed assets

When you post fixed asset journals, [!INCLUDE [prod_short](includes/prod_short.md)] creates entries in the **FA Entry** table. Therefore, ad-hoc analysis on fixed assets is typically done on the [FA Ledger Entries](https://businesscentral.dynamics.com/?page=5604) page.

## <a name="contributors"></a>Contributors

*Microsoft maintains this article. Parts of the examples were originally written by the following contributor.*

* [Aldona Stec](https://www.linkedin.com/in/aldona-stec-25283bb1) | [!INCLUDE[prod_short](includes/prod_short.md)] Consultant

## <a name="see-also"></a>See also

[Analyse list and query data with analysis mode](analysis-mode.md)  
[Fixed assets analytics overview](fa-analytics-overview.md)  
[Analytics, business intelligence, and reporting overview](reports-bi-reporting.md)  
[Fixed assets overview](fa-manage.md)  
[Work with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  

## [!INCLUDE[prod_short](includes/free_trial_md.md)]  

[!INCLUDE[footer-include](includes/footer-banner.md)]
