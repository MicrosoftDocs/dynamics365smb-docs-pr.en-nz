---
title: Handling Missing Option Values
description: Learn how to prevent full synchronisation from failing because the options differ in mapped fields.
author: bholtorf
ms.author: bholtorf
ms.custom: na
ms.reviewer: na
ms.service: dynamics365-business-central
ms.topic: article
ms.date: 10/01/2020
ms.openlocfilehash: 65911039894d1f0eb81aeb1160a6b2aafc2fae0c
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 12/17/2020
ms.locfileid: "4752891"
---
# <a name="handling-missing-option-values"></a>Handling Missing Option Values
[!INCLUDE[prod_short](includes/cc_data_platform_banner.md)]

[!INCLUDE[prod_short](includes/cds_long_md.md)] contains only three option set fields that contain option values that you can map to [!INCLUDE[prod_short](includes/prod_short.md)] fields of Option type<!-- Option type, not enum? @Onat can you vertify this? --> for automatic synchronisation. During synchronisation, non-mapped options are ignored and the missing options are appended to the related [!INCLUDE[prod_short](includes/prod_short.md)] table and added to the **CDS Option Mapping** system table to handle manually later. For example, by adding the missing options in either product and then updating the mapping. This section describes how that works.

The **Integration Table Mapping** page contains three maps for fields that contain one or more mapped option values. After a full synchronisation, the **CDS Option Mapping** page contains the non-mapped options in the three fields respectively.

|         Record             | Option Value | Option Value Caption |
|----------------------------|--------------|----------------------|
| Payment Terms: NET30       | 1            | Net 30               |
| Payment Terms: 2%10NET30   | 2            | 2% 10; Net 30        |
| Payment Terms: NET45       | 2A-2B GST Net Amt. (3)            | Net 45               |
| Payment Terms: NET60       | Total Amounts Withheld From All Payments (4)            | Net 60               |
| Shipment Method: FOB       | 1            | FOB                  |
| Shipment Method: NOCHARGE  | 2            | No Charge            |
| Shipping Agent: AIRBORNE   | 1            | Airborne             |
| Shipping Agent: DHL        | 2            | DHL                  |
| Shipping Agent: FEDEX      | 2A-2B GST Net Amt. (3)            | FedEx                |
| Shipping Agent: UPS        | Total Amounts Withheld From All Payments (4)            | UPS                  |
| Shipping Agent: POSTALMAIL | 5            | Postal Mail          |
| Shipping Agent: FULLLOAD   | 6            | Full Load            |
| Shipping Agent: WILLCALL   | Deferred Company Fund Installment (7)            | Will Call            |

The content of the **CDS Option Mapping** page is based on enum values in the **CDS Account** table. In [!INCLUDE[prod_short](includes/cds_long_md.md)], the following fields on the account table are mapped to fields on the customer and vendor records:

- **Address 1: Freight Terms** of data type Enum, where values are defined as follow:

```
enum 5335 "CDS Shipment Method Code"
{
    Extensible = true;
    value(0; " ") { Caption = ' '; }
    value(1; "FOB") { Caption = 'FOB'; }
    value(2; "NoCharge") { Caption = 'No Charge'; }
}
```

- **Address 1: Shipping Method** of data type Enum, where values are defined as follows:

```
enum 5336 "CDS Shipping Agent Code"
enum 5336 "CDS Shipping Agent Code"
{
    Extensible = true;
    value(0; " ") { Caption = ' '; }
    value(1; "Airborne") { Caption = 'Airborne'; }
    value(2; "DHL") { Caption = 'DHL'; }
    value(3; "FedEx") { Caption = 'FedEx'; }
    value(4; "UPS") { Caption = 'UPS'; }
    value(5; "PostalMail") { Caption = 'Postal Mail'; }
    value(6; "FullLoad") { Caption = 'Full Load'; }
    value(7; "WillCall") { Caption = 'Will Call'; }
}
```

- **Payment Terms** of data type Enum, where values are defined as follows:

```
enum 5334 "CDS Payment Terms Code"
{
    Extensible = true;
    value(0; " ") { Caption = ' '; }
    value(1; "Net30") { Caption = 'Net 30'; }
    value(2; "2%10Net30") { Caption = '2% 10; Net 30'; }
    value(3; "Net45") { Caption = 'Net 45'; }
    value(4; "Net60") { Caption = 'Net 60'; }
}
```

All of the [!INCLUDE[prod_short](includes/prod_short.md)] enums above are mapped to option sets in [!INCLUDE[prod_short](includes/cds_long_md.md)].

### <a name="extending-option-sets-in-prod_short"></a>Extending Option Sets in [!INCLUDE[prod_short](includes/prod_short.md)]
1. Create a new AL extension.

2. Add an Enum extension for the options that you want to extend. Be sure that you use the same value. 

```
enumextension 50100 "CDS Payment Terms Code Extension" extends "CDS Payment Terms Code"
{
    value(779800001; "Cash Payment") { Caption = 'Cash Payment'; }
    value(779800002; "Transfer") { Caption = 'Transfer'; }
}
```

> [!IMPORTANT]  
> You must use the same option ID values from [!INCLUDE[prod_short](includes/cds_long_md.md)] when you extend the [!INCLUDE[prod_short](includes/prod_short.md)] enum. Otherwise synchronisation will fail.

> [!IMPORTANT]  
> Do not use the ","  character in the enum values and captions. This is currently not supported by the [!INCLUDE[prod_short](includes/prod_short.md)] runtime.

> [!NOTE]
> The first ten characters of the new option value names and captions must be unique. For example, two options named "Transfer 20 working days" and "Transfer 20 calendar days" will cause an error because both have the same first 10 characters, "Transfer 2". Name them, for example, "TRF20 WD" and "TRF20 CD."

### <a name="update-prod_short-option-mapping"></a>Update [!INCLUDE[prod_short](includes/cds_long_md.md)] Option Mapping
Now you can recreate the mapping between [!INCLUDE[prod_short](includes/cds_long_md.md)] options and [!INCLUDE[prod_short](includes/prod_short.md)] records.

On the **Integration Table Mapping** page, choose the line for the **Payment Terms** map, and then choose the **Synchronise Modified Records** action. The **CDS Option Mapping** page is updated with the additional records below.

|         Record                 | Option Value   | Option Value Caption |
|--------------------------------|----------------|----------------------|
| Payment Terms: NET30           | 1              | Net 30               |
| Payment Terms: 2%10NET30       | 2              | 2% 10; Net 30        |
| Payment Terms: NET45           | 2A-2B GST Net Amt. (3)              | Net 45               |
| Payment Terms: NET60           | Total Amounts Withheld From All Payments (4)              | Net 60               | 
| **Payment Terms: CASH PAYME**  | **779800001**  | **Cash Payment**     |
| **Payment Terms: TRANSFER**    | **779800002**  | **Transfer**         |

The **Payment Terms** table in [!INCLUDE[prod_short](includes/prod_short.md)] will then have new records for the [!INCLUDE[prod_short](includes/cds_long_md.md)] options. In the following table new options are in bold font . Italic rows represent all options that can now be synchronised. Remaining rows represent options are not in use and will be ignored during synchronisation. You can remove them or extend CDS options with the same names.)

| Code       | Due Date Calculation | Discount Date Calculation | Discount % | Calc. Pmt. Disc. on Cr. Memos | Description       |
|------------|----------------------|---------------------------|------------|-------------------------------|-------------------|
| 10 DAYS    | 10D                  |                           | 0.         | FALSE                         | Net 10 days       |
| 14 DAYS    | 14D                  |                           | 0.         | FALSE                         | Net 14 days       |
| 15 DAYS    | 15D                  |                           | 0.         | FALSE                         | Net 15 days       |
| 1M(8D)     | 1M                   | 8D                        | 2.         | FALSE                         | 1 Month/2% 8 days |
| 2 DAYS     | 2D                   |                           | 0.         | FALSE                         | Net 2 days        |
| *2%10NET30* |                      |                           | 0.         | FALSE                         |                   |
| 21 DAYS    | 21D                  |                           | 0.         | FALSE                         | Net 21 days       |
| 30 DAYS    | 30D                  |                           | 0.         | FALSE                         | Net 30 days       |
| 60 DAYS    | 60D                  |                           | 0.         | FALSE                         | Net 60 days       |
| 7 DAYS     | 7D                   |                           | 0.         | FALSE                         | Net 7 days        |
| ***CASH PAYME** _ |                      |                           | 0.         | FALSE                         |                   |
| CM         | CM                   |                           | 0.         | FALSE                         | Current Month     |
| COD        | 0D                   |                           | 0.         | FALSE                         | Cash on delivery  |
| _NET30*      |                      |                           | 0.         | FALSE                         |                   |
| *NET45*      |                      |                           | 0.         | FALSE                         |                   |
| *NET60*      |                      |                           | 0.         | FALSE                         |                   |
| ***TRANSFER*** |                      |                           | 0.         | FALSE                         |                   |

## <a name="see-also"></a>See Also
[Mapping the Tables and Fields to Synchronise](admin-how-to-modify-table-mappings-for-synchronization.md)