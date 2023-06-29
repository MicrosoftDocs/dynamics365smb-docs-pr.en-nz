---
title: Work with Intrastat Reporting
description: Learn how to report trade with companies in other EU countries using the Intrastat system.
author: altotovi
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 'electronic document, Intrastat, trade, EU, European Union'
ms.search.form: '308, 309, 310, 311, 325, 326, 327, 328, 405, 406, 4810, 4811, 8451, 12202, 31077'
ms.date: 09/02/2022
ms.author: altotovi
---
# <a name="work-with-intrastat-reporting"></a><a name="work-with-intrastat-reporting"></a>Work with Intrastat Reporting

All companies in the European Union (EU) must report their trade with other EU countries/regions. You must report the movement of goods to the statistics authorities in your country/region every month, and the report must be delivered to the tax authorities. Intrastat is the system for collecting trade statistics of goods within these countries/regions. You use **Intrastat Report** to complete periodic Intrastat reporting (typically monthly), collecting, recording, and reporting trade of goods as per local government legislation.

Intrastat reporting is based on basic EU regulations that apply to all countries; however, in practice, there are some differences within the individual countries. Each country has its rules of what exactly and how to report.

> [!IMPORTANT]
> This article describes the new Intrastat experience available in [!INCLUDE[prod_short](includes/prod_short.md)] starting in the 2022 release wave 2, which includes extended features and [must be switched on for existing companies](finance-how-setup-report-intrastat.md#enable-the-new-intrastat-experience). Contact your administrator to switch on and set up the new capability.
>
> Read the previous version's Intrastat setup and usage article at [Set Up and Report Intrastat](finance-how-setup-report-intrastat-v20.md).

> [!NOTE]
> Intrastat information doesn't apply to the movement of services between countries, but only goods (Items and Fixed Assets). If the local government requires registering  the movement of services between countries, it can be done using the **Service Declaration** feature.
>
> We currently expect this feature to be available from November 2022 as an app at [AppSource](https://go.microsoft.com/fwlink/?linkid=2081646). At that time, to use it, you must first install it on the **Extension Management** page.

## <a name="fill-in-the-intrastat-report"></a><a name="fill-in-the-intrastat-report"></a>Fill in the Intrastat report

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Intrastat List**, and choose the related link.
2. Choose **New** action to create a new **Intrastat Report**.
3. If you need to enter some internal information about the **Intrastat Report**, fill in this information in the **Description** field.
4. In the **Statistic Period** field, specify the month to report data for. Enter the period as a four-digit number with no spaces or symbols. Depending on your country, enter either the month first and then the year, or vice versa. For example, enter either *2206* or *0622* for June 2022.
5. Choose the **Suggest Lines** action. The **Starting Date** and **Ending Date** fields will already contain the dates specified for the statistics period on the Intrastat report header.
6. In the **Cost Regulation %** field, you can enter a percentage to cover transport and insurance. If you enter a percentage, the content of the **Statistical Value** field in the journal is proportionally higher. But if you want to use this feature, you must switch the **Amount incl. Item Charges** field to **Yes**.
7. You can eventually set up extra configurations on the **Additional** FastTab:
   1. **Skip Recalculation for Zero Amounts** to specify that lines without amounts will not be recalculated during the batch job.
   2. **Skip Zero Amounts** to specify that item ledger entries without amounts will not be included in the batch job.
   3. **Show Item Charge Entries** to specify if you want to show direct costs that your company has assigned and posted as item charges.
   4. **Skip Non-Invoiced Entries** to specify if item ledger entries that are shipped or received but not yet invoiced must be excluded from the process.
8. Choose **OK** to start the batch job.

The batch job retrieves all the item entries in the statistics period and inserts them as lines in the **Intrastat Report** lines. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="modify-the-intrastat-report"></a><a name="modify-the-intrastat-report"></a>Modify the Intrastat report

If needed, you can modify the lines, but whenever you change a value in the Intrastat report line, the **Correction** field will be automatically marked as **Yes**. Eventually, you can add a new line manually if there is a reason for that. To add a new line manually:

1. On the **Intrastat Report** page, choose the **New Line** action in the **Lines** FastTab.
2. Choose the **Receipt** or **Shipment** option in the **Type** field.
3. In the **Source Type** field, choose one of the sources: **Item Entry**, **FA Entry**, or **Job Entry**.
4. Based on the **Source Type** in the **Item No.** field, you can choose an **Item** (in both cases, **Item Entry** or **Job Entry**) or **Fixed Assets**.
5. Fill in other fields as you need for the Intrastat reporting.

> [!NOTE]
> When you manually add a new line to the Intrastat report, the **Date** field in the line must be inside the **Statistic Period** range you added on the header.

## <a name="validate-intrastat-lines"></a><a name="validate-intrastat-lines"></a>Validate Intrastat lines

After you fill in the **Intrastat Report**, you can run the **Checklist Report** action to ensure that all information in the **Intrastat Report** is correct. Mandatory fields you have set on **Intrastat Report Checklist** page that are missing values will be shown in **Errors and warning** FactBox on the **Intrastat Report** page.

Run the **Intrastat Report Checklist** report to check Intrastat lines before they are exported to the required format. The check is run inside the **Intrastat Report**.

## <a name="recalculating-weight-or-supplementary-unit-of-measure"></a><a name="recalculating-weight-or-supplementary-unit-of-measure"></a>Recalculating weight or supplementary unit of measure

If you got the error message *'Total Weight' in Intrastat Report Line must not be blank*, it is probably because you didn't have set the **Net Weight** field on the used source, item, or fixed asset. In this case, search for the item or fixed asset card and add the required value. After that, you just need to reopen the **Intrastat Report** and follow these steps:

1. Choose the **Recalc. Weight/Suppl. UOM** action to recalculate the **Total Weight** and/or **Supplementary Quantity**.
2. Choose one of the options:

    1. **Weight** – to recalculate only the **Total Weight**, based on the current information about **Net Weight** on the item and fixed asset cards.
    2. **Supplemental UOM Qty** – to recalculate only the **Supplementary Quantity** on the **Intrastat Report** line if it exists, based on the current information about **Supplementary UOM** on the item and fixed asset cards.
    3. **Both** – to recalculate both **Total Weight** and **Supplementary Quantity**, based on the current information on the item and fixed asset cards.
3. Choose **OK** to start the batch job.

## <a name="report-intrastat-in-a-file"></a><a name="report-intrastat-in-a-file"></a>Report Intrastat in a file

You can submit the Intrastat report as a file based on different local authorities' requirements. Before creating the file, you should run the **Checklist Report** to check if all lines contain all necessary and valid information. To create a file:

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Intrastat List**, then choose the related link.
2. Choose **Intrastat Report** you want to report as a file.
3. If you have not already done this, fill in the **Intrastat Report** manually or choose the **Suggest Lines** action.
4. Choose the **Create File** action.
5. The Intrastat file will be saved in the required format.

Once you create the file, [!INCLUDE[prod_short](includes/prod_short.md)] will automatically fill in the following details about reporting:

* The **Export Date** to specify the date when the report has been exported.
* The **Export Time** to specify the time when the report has been exported.

> [!NOTE]
> Next time you create a file, the **Export Date** and **Export Time** fields will only keep information about the last file you created.

## <a name="intrastat-rules"></a><a name="intrastat-rules"></a>Intrastat rules

### <a name="grouping-lines"></a><a name="grouping-lines"></a>Grouping lines

In **Intrastat Report** lines, there is no grouping by any fields. All entries are copied from the original source, so you can quickly locate them based on the combination of **Source Type** and **Source Entry No**.

Grouping required by authorities will be provided in the exported file. You need to configure this in the **Data Exchange Definition**, which is fully configurable. Learn more at [Set Up Data Exchange Definitions](across-how-to-set-up-data-exchange-definitions.md).

### <a name="fixed-assets-reporting"></a><a name="fixed-assets-reporting"></a>Fixed assets reporting

Fixed assets will be shown in the Intrastat lines only if:

* The **FA Posting Type** in the **GST Ledger Entry** field is **Acquisition Cost** and if the **Document Type** is **Invoice** in the case of purchases, and
* The **FA Posting Type** in the **GST Ledger Entry** field is **Proceeds on Disposal** and if the **Document Type** is **Invoice** in the case of sales.

### <a name="intrastat-report-statuses"></a><a name="intrastat-report-statuses"></a>Intrastat report statuses

When you work with the **Intrastat Report** you will see a **Status** field on the document header. You can find the following statuses together with related rules:

* *Open*: This status is created automatically when you create a new Intrastat report and you can make all operations in this status.
* *Released*: [!INCLUDE[prod_short](includes/prod_short.md)] automatically changes the status to *Released* when you create a file. From that moment, you cannot modify your **Intrastat Report**. If you need to change something and report again, you can use the **Reopen** action to reopen the Intrastat report. Once the document is reopened, you can use the **Release** action to release the document again.
* **Reported**: Specifies whether the entry has already been reported to the tax authorities. This is not a regular status but an independent field, and even if you reopened the Intrastat report, it would still show that the file is already created for this report.

## <a name="see-related-training-at-microsoft-learn"></a><a name="see-related-training-at-microsoft-learn"></a>See related training at [Microsoft Learn](/learn/modules/process-intrastat-dynamics-365-business-central/index).

## <a name="see-also"></a><a name="see-also"></a>See also

[Set Up Intrastat Reporting](finance-how-setup-report-intrastat.md)  
[Financial Management](finance.md)  
[Work with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
