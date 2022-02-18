---
author: edupont04
ms.service: dynamics365-business-central
ms.topic: include
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: e66b50cec6d3f9e2606f3f698e12a06eccdd5cf6
ms.sourcegitcommit: 2c972dfc94d27245eaa99efcf638d030dedafb22
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 02/09/2022
ms.locfileid: "8104440"
---
The following table describes some of the key reports in accounts payable reporting.

| Report | Object ID | Description |
|--|--|--|
| **Aged Accounts Payable** | 322|Shows overdue balances for vendors in overdue time intervals. The overdue amounts can be shown by due date, posting date, or by document date as needed. You can choose to show the amounts in local currency (LCY) and print details of the overdue documents. The time intervals can have headings with dates or with number of dates overdue, relative to the specified ageing by type.<br>This report is the main report for reconciling vendor ledger to G/L. Assuming that you have not allowed direct posting to the accounts used in the vendor posting groups' payables account, this report is a specification of the amounts you find in the general ledger.|
| **Vendor - Balance to Date** | 321 | Shows the vendor balance by the ending date of the specified date range. You can choose to display the vendor balance in your local currency (LCY). Select the **Include Unapplied Entries** field to show entries that have been closed by the ending date but have been un-applied (opened) at a later date. Select the **Show Entries with Zero Balance** to show vendors with a balance of zero by the ending date of the date filter. The date filter applies to the detailed vendor ledger entries for the entries in the report. If you have payments later than the ending date that have been applied to invoices in within the date range, the invoices will appear in the report as they have not been closed as by the ending date. |
| **Vendor – Trial Balance** | 329 | Shows the net changes for vendors for the period specified in the date filter as well as the net change year-to-date for the financial year corresponding to the period selected. The report is grouped by vendor posting groups and will give a different view of the vendor ledger than the **Aged Accounts Payable** report. **Note**: If you haven't set up any accounting period, the system will not know what financial year to use and will either show year-to-date from the most recent financial year defined or just select the period, which may or may not be from beginning of a year.|
| **Vendor – Detail Trial Balance** | 304 | Shows all the vendor ledger entries within the specified date filter. The report shows the vendor's beginning balances relative to the date filter. |
| **Purchase Statistics** |312 |[!INCLUDE [reports-purchase-statistics](reports-purchase-statistics.md)]<br>This report can also be used in accounts payable as it's easier to do a quick look-up of posted payments, discounts, and other transactions for a given vendor.|
|**Vendor – Summary Ageing**|305| Legacy report for aged accounts payable. We recommend that you use **Aged Accounts Payables** report instead. You can choose a period length and a date to use as set *overdue per* date.|
|**Payments on Hold**|319|Shows vendor ledger entries where the **On Hold** field is not blank.|
|**Vendor Pre-Receipt Journal**|317|Shows the receipt journal with payment discount and tolerance information. The report can be used to check payments before creating payment files and posting the journal. **Note**: The report will show payment discounts incorrectly when multiple credit memos have been used in an application. In this case, the payment discount for the additional credit memos will be shown as an un-applied amount.|
|**Vendor – List**|301|Shows various kinds of basic information for vendors, such as vendor posting group, discount and payment information, priority level and the vendor's default currency, and the vendor's current balance (in LCY). The report can be used, for example, to maintain the information in the Vendor table.|
