---
title: Inland Revenue Department Numbers and Adjustment Notes
description: Learn about IRD numbers and adjustment notes and how they are supported in the New Zealand version of Business Central.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: bholtorf
ms.openlocfilehash: d98582d0e051e3d90f753086088124ca918cbbd7
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "5383550"
---
# <a name="new-zealand-inland-revenue-department-numbers-and-adjustment-notes"></a>New Zealand Inland Revenue Department Numbers and Adjustment Notes

A New Zealand Inland Revenue Department Number (IRD) is a single identifier for all business dealings with the tax office, and for dealings with other government departments and agencies.  

IRDs and adjustment notes—or credit memos—are used to satisfy tax requirements.  

## <a name="ird-number"></a>IRD number  
All companies must register and apply for an IRD number to report the details of payment summaries issued to their payees during the financial year. The payment summary includes the Tax File Numbers (TFN) or business numbers of the payees.  

## <a name="adjustment-notes"></a>Adjustment Notes  
Adjustment notes are issued by suppliers to a business when the amount of consideration for taxable supplies changes. The recipient needs an adjustment note to claim more or less GST credits than previously claimed.  

An adjustment event may result in an increase or decrease to your net amount for the tax period.  

Adjustment notes—or credit memos—should be connected to an invoice.  

Because credit memos are used for adjustment notes, each credit memo should satisfy all of the legal requirements for an adjustment note. Each credit memo should have an original invoice number, date, and reason code assigned to it. The following fields are included in the adjustment note:  

- **Adjustment Applies to**: The number of the document to which the adjustment note applies. If you use the **Copy Document** function, this field populates automatically. You must enter a reason code before the transaction can be posted. You can use this field to create an adjustment note for a paid or closed transaction.  

- **Adjustment Reference No**: The number of the adjustment note. For **Sales & Receivables**, the number assigned to the posted document populates automatically in this field.  

- **Adjustment Note Date**: Automatically populated from the document date.  
- **Adjustment**: These entries populate automatically. Adjustment notes can only be applied against a single document.  

## <a name="see-also"></a>See Also  
[Enter New Zealand IRD Numbers](how-to-enter-new-zealand-business-numbers.md)   
[New Zealand Local Functionality](new-zealand-local-functionality.md)



[!INCLUDE[footer-include](../../includes/footer-banner.md)]