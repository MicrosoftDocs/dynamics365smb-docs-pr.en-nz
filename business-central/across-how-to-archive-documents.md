---
title: How to Archive Sales and Purchase Documents | Microsoft Docs
description: You can archive sales and purchase orders, quotes, return orders, and blanket orders, and you can use the archived document to recreate the document that it was archived from.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 33b900f1ac9e295921e7f3d6ea72cc93939d8a1b
ms.openlocfilehash: 4827e25d97127faf691b96df9868320bb47dee39
ms.contentlocale: en-nz
ms.lasthandoff: 11/26/2018

---
# <a name="archive-documents"></a>Archive Documents
You can archive sales and purchase orders, quotes, return orders, and blanket orders, and you can use the archived document to recreate the document that it was archived from.

## <a name="to-set-up-automatic-document-archiving"></a>To set up automatic document archiving  
You can set up automatic archiving of sales and purchase orders, quotes, blanket orders, and return orders, before you delete documents.

The following procedure describes how to set up automatic archiving of sales documents. The steps are similar for purchase documents.
1.  Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales & Receivables Setup**, and then choose the related link.
2. On the **Sales & Receivables Setup** page, fill in the fields as follows.

|Field|Description|
|-----|-----------|
|**Archiving Sales Quotes**|**Never** to never archive sales quotes when they are deleted. **Question** to prompt the user to choose whether to archive sales quotes when they are deleted. **Always** to archive sales quotes automatically when they are deleted.|
|**Archiving Blanket Sales Orders**|Select to archive blanket sales orders automatically each time they are deleted.|
|**Arch. Orders and Ret. Orders**|Select to automatically archive sales orders each time they are deleted.|

## <a name="to-archive-a-sales-order"></a>To archive a sales order
The following procedure describes how to archive a sales order. The steps are similar for all orders, blanket orders, return orders, and quotes.

1.  Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.  
2.  Open a sales order that you want to archive.  
3.  Choose the **Archive Document** action.

The sales order is archived. You can view it on the **Archived Sales orders** page. From here, you can also use it to recreate the sales order that it was archived from.

## <a name="to-recreate-a-sales-order-from-the-archive"></a>To recreate a sales order from the archive
The following procedure describes how to recreate a sales order. The steps are similar for all orders, blanket orders, return orders, and quotes.

1.  Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Archived Sales Orders**, and then choose the related link.
2.  Select the archived sales order that you want to recreate, and then choose the **Restore** action.  

The sales order is created and added to the **Sales Orders** page.

## <a name="to-delete-archived-sales-orders"></a>To delete archived sales orders
The following procedure describes how to delete archived sales orders. The steps are similar for other archived sales and purchase documents.

1.  Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Delete Archived Sales Order Versions**, and then choose the related link.  
2.  On the **Delete Archived Sales Order Versions** page, select the appropriate filters.  
3.  Choose the **OK** button.

## <a name="see-also"></a>See Also
[Track Document Lines](across-how-to-track-document-lines.md)  
[Sales](sales-manage-sales.md)  
[General Business Functionality](ui-across-business-areas.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

