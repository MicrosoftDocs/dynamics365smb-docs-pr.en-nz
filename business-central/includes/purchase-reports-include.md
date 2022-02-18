---
author: edupont04
ms.service: dynamics365-business-central
ms.topic: include
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: ae96e5a3fc1cc7f4b17e5ef208650248cbe0b3c2
ms.sourcegitcommit: 2c972dfc94d27245eaa99efcf638d030dedafb22
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 02/09/2022
ms.locfileid: "8104417"
---
The following table describes some of the key reports in purchase reporting.

|Report |Object ID|Description  |
|---------|---------|---------|
|**Purchase statistics**|312|[!INCLUDE [reports-purchase-statistics](reports-purchase-statistics.md)]|
|**Vendor – Top 10 list**|311|Shows information on purchases from vendors for a selected period. You can choose the number of vendors that are included in the report.<br>The vendors are sorted in order of amount, and you can choose whether they are sorted by purchase amount or balance. The report gives a quick overview of the vendors from which you purchase the most or to which you owe the most.|
|**Vendor Item catalogue** or **Item/vendor catalogue**|320 or 720|Displays a list of the vendors for the selected items or items for selected vendors. For each combination of item and vendor, it shows direct unit cost, lead time calculation and the vendor's item number.<br>In the US, Canada, and Mexico, this report is not available. Instead, use the **Item/Vendor Catalogue** (10164) report.|
|**Vendor/Item Purchases**|313|Shows a list of item entries for each vendor in a selected period. The report contains information on invoiced quantity, amount and possible discounts. It can be used, for example, to analyse a company's item purchases and to show whether there is a relationship between discounts and item purchases.|
|**Inventory Cost and price list**|716|Displays a list of price information for the selected items or stockkeeping units: direct unit cost, last direct cost, unit price, profit percentage, and profit.|
|**Inventory Availability Plan**|707|If you would like to have an overview about specific items/stockkeeping units and their availability. This report will show you cumulated values such as gross requirements, scheduled and planned receipts, the inventory, and so on. |
|**Inventory Vendor Purchases**|714|Displays a list of the vendors that your company has purchased items from within a selected period. It shows invoiced quantity, amount and discount. The report can be used to analyse a company's item purchases.|
|**Inventory Purchase Orders**|709|Displays a list of items on order from vendors. It also shows the expected receipt date and the quantity and amount on back orders. For example, use the report to see when items should be received, and whether a reminder of a back order should be issued|
|**Purchase Reservation Availability**|409|Shows the availability of items for shipment on purchase documents, for example return orders. You determine whether the report indicates the status of each document or of each purchase line. <br>When you print the report, you can also update the quantity that is available for shipment in the **Qty. to Receive** field on the purchase lines. On purchase credit memos and negative purchase order lines, the **Qty. to Receive** field contains the quantity to ship.. Then you can use the report to determine which documents to ship. **Note**: This report is not available for advanced warehouse functionality.|
<!--|**Vendor detailed ageing**|11006| DACH specific: A report which could be used by the team leader of your purchased department as will the accounting. Here you will have an overview about the unpaid vendor invoices including the due dates, currencies and amounts. Basis is the open vendor ledger entries.| -->

