---
title: Create a Purchase Quote to Request an Offer from Your Vendor | Microsoft Docs
description: Describes how to create a sales offer or a request for proposal (RFQ) document to record your offer to a customer to sell products under certain terms.
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: rfq
ms.date: 08/08/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: 3fe5eca9c26380248471facbd945838b1bf47a1d
ms.contentlocale: en-nz
ms.lasthandoff: 01/30/2018

---
# <a name="request-quotes"></a>Request Quotes
A purchase quote can be used as a preliminary draft for a purchase order, and the order can then be converted to a purchase invoice or an order.


## <a name="to-create-a-purchase-quote"></a>To create a purchase quote
1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Purchase Quotes**, and then choose the related link.
2. Create a new document, in the same way as you make a purchase order. For more information, see [Record Purchases](purchasing-how-record-purchases.md).

## <a name="to-convert-a-purchase-quote-to-a-purchase-order"></a>To convert a purchase quote to a purchase order
When you have accepted the vendor's quote, you can convert it to a purchase invoice or order to process the purchase.

1. Open a purchase quote that is ready to convert, and then choose the **Make Order** action.

The purchase quote is removed from the database. A purchase invoice or a purchase order is created based on the information in the purchase quote in which you can process the purchase. In the **Quote No.** field on the purchase invoice or purchase order, you can see the number of the purchase quote that it was made from.

## <a name="see-also"></a>See Also
[Purchasing](purchasing-manage-purchasing.md)  
[Setting Up Purchasing](purchasing-setup-purchasing.md)  
[Send Documents by Email](ui-how-send-documents-email.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

