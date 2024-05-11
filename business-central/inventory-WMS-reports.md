---
title: Inventory and warehouse reports and analytics
description: See which inventory and warehouse reports and analytics are available in the standard version of Business Central so that you can keep track of your business.
author: brentholtorf
ms.author: bholtorf
ms.reviewer: andreipa
ms.topic: conceptual
ms.search.keywords: reporting
ms.search.form: 'Report_707, Report_716, Report_813, Report_1001, Report_5807, Report_5808, Report_5809, Report_7313, Report_7319, Report_7320'
ms.date: 03/21/2024
ms.custom: bap-template
ms.service: dynamics-365-business-central
---
# <a name="inventory-and-warehouse-reports-and-analytics"></a>Inventory and warehouse reports and analytics

Inventory and warehouse reporting in [!INCLUDE [prod_short](includes/prod_short.md)] gives inventory and business professionals insights and statistics about current and past inventory and warehouse activities.  

## <a name="reports"></a>Reports

[!INCLUDE [inventory_WMS_reports](includes/inventory-WMS-reports-include.md)]

## <a name="tasks"></a>Tasks

The following articles describe some of the key tasks for analysing the state of your business:

* [Create Analysis Reports](bi-how-create-analysis-views-reports.md)  
* [View the Availability of Items](inventory-how-availability-overview.md)

## <a name="print-and-scan-barcodes"></a>Print and scan barcodes

Using barcodes can help streamline your inbound, outbound, and internal warehouse processes. 

[!INCLUDE [barcode-mobile-app](includes/barcode-mobile-app.md)]

After you install the app, you can use the **Print Label** action to print 1D and 2D barcodes from the pages listed in the following table.

|Page  |Field values barcodes can include  |
|---------|---------|
|Items, Item Card     |Item No., Description, and GTIN         |
|Item Reference List, Item Reference     |Item No., Description, Unit of Measure, and Reference No.         |
|Lot No. Information List, Lot No. Label     |Item No., Description, and Lot Number       |
|SN Label     |No., Description, and Serial Number         |

> [!NOTE]
> Some printers and barcode/QR code formats require a specific implementation. You might need to upload a different Word template or clone the report to create your own customised version.


## <a name="explore-inventory-reports-with-report-explorer"></a>Explore inventory reports with Report Explorer

To get an overview of the reports that are available for inventory, choose **All Reports** on your Home page. This action opens the Role Explorer, which is filtered to the features in the **Report & Analysis** option. Under the **Sales and Marketing** heading, choose **Explore**.

:::image type="content" source="media/report-explorer-sales.png" alt-text="Example of reports on the finance role centre." lightbox="media/report-explorer-sales.png":::

To learn more, go to [Finding Reports with the Role Explorer](ui-role-explorer.md).


## <a name="see-also"></a>See also

[Ad-hoc analysis of inventory data](ad-hoc-analysis-inventory.md)  
[Inventory analytics overview](inventory-analytics-overview.md)   
[Setting Up Inventory](inventory-setup-inventory.md)  
[Inventory](inventory-manage-inventory.md)  
[Setting Up Warehouse Management](warehouse-setup-warehouse.md)  
[Warehouse Management Overview](design-details-warehouse-management.md)

[!INCLUDE[footer-include](includes/footer-banner.md)]
