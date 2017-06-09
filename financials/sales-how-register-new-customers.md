---
title: 'How to: Register New Customers| Microsoft Docs'
description: 'How to: Register New Customers'
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: client
ms.date: 03/29/2017
ms.author: sgroespe
ms.translationtype: Human Translation
ms.sourcegitcommit: a31be0f9d07e2abb591e26f6bae34c6f6e4dcda6
ms.openlocfilehash: 6789e6a4129789e950c7f71ff86e62263ae9c087
ms.contentlocale: en-nz
ms.lasthandoff: 05/04/2017


---
# <a name="how-to-register-new-customers"></a>How to: Register New Customers
Customers are the source of your income. You must register each customer you sell to as a customer card. Customer cards hold the information that is required to sell products to the customer. For more information, see [How to: Invoice Sales](sales-how-invoice-sales.md) and [How to: Register New Items](inventory-how-register-new-items.md).  

Before you can register new customers, you must set up various sales codes that you can select from when you fill in customer cards. For more information, see [Set Up Sales](sales-setup-sales.md).

**Note**: If customer templates exist for different customer types, then a window appears when you create a new customer card from where you can select an appropriate template. If only one customer template exists, then new customer cards always use that template.

## <a name="to-create-a-new-customer-card"></a>To create a new customer card
1. On the Home page, choose the **Customers** action to open the list of existing customers.  
2. In the **Customers** window, choose the **New** action.

    If only one customer template exists, then a new customer card opens with some fields filled with information from the template.

    If more than one customer template exists, then a window opens from which you can select a customer template. In that case, follow the next two steps.
3. In the **Select a template for a new customer** window, choose the template that you want to use for the new customer card.
4. Choose the **OK** button. A new customer card opens with some fields filled with information from the template.  
5. Proceed to fill or change fields on the customer card as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

On the **Sales Prices** FastTab, you can view special prices or discounts that you grant for the customer if certain criteria are met, such as item, minimum order quantity, or ending date. Each row represents a special price or line discount. Each column represents a criterion that must apply to warrant the special price that you enter in the **Unit Price** field, or the line discount that you enter in the **Line Discount %** field. For more information, see [Record Sales Price, Discount, and Payment Agreements](sales-how-record-sales-price-discount-payment-agreements.md).

The customer is now registered, and the customer card is ready to be used on sales documents.

If you want to use this customer card as a template when you create new customer cards, you can save it as a template. For more information, see the following section.

## <a name="to-save-the-customer-card-as-a-template"></a>To save the customer card as a template
1. In the **Customer Card** window, choose the **Save as Template** action. The **Customer Template** window opens showing the customer card as a template.
2. Fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. To reuse dimensions in templates, choose the **Dimensions** action. The **Dimension Templates** window opens showing any dimension codes that are set up for the customer.
4. Edit or enter dimension codes that will apply to new customer cards created by using the template.  
5. When you have completed the new customer template, choose the **OK** button.

The customer template is added to the list of customer templates, so that you can use it to create new customer cards.

## <a name="see-also"></a>See Also
[Sales](sales-manage-sales.md)    
[Setting Up Sales](sales-setup-sales.md)    
[Working With [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

