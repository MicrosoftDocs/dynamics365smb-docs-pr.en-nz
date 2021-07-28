---
title: Importing Many Item Pictures from a ZIP File| Microsoft Docs
description: To import multiple item pictures give picture files names corresponding to item numbers, compress them to a ZIP file, and use the Import Item Pictures page.
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: product, image
ms.date: 06/16/2021
ms.author: edupont
ms.openlocfilehash: ac8d68d067c03039433d78be475d74efb3fec1fd
ms.sourcegitcommit: a7cb0be8eae6ece95f5259d7de7a48b385c9cfeb
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 07/08/2021
ms.locfileid: "6440540"
---
# <a name="import-multiple-item-pictures"></a>Import Multiple Item Pictures
 You can import multiple item pictures in one go. Simply name your picture files with names corresponding to your item numbers, compress them to a zip file, and then use the Import Item Pictures page to manage which item pictures to import.

All common file formats are supported.

## <a name="to-name-picture-files-by-the-item-names-and-prepare-the-zip-file"></a>To name picture files by the item names and prepare the ZIP file
1. At the location where your item pictures are stored, name each files according to the number of the related item. For example:

    |Item No.|File Name|
    |-|-|
    |1000|1000.bmp|
    |1001|1001.bmp|
    |1002|1002.bmp|

2. Collect all the files in a ZIP file. For example, in Windows Explorer, select the files, and then choose **Send to**, **Compressed (zipped) folder**.     

## <a name="to-import-item-pictures"></a>To import item pictures
1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Inventory Setup**, and then choose the related link.
2. Choose the **Import Item Pictures** action.
3. In the **Select a ZIP file** field, select the relevant ZIP folder, and then choose the **Open** button.

    A line for each item and picture is created on the **Import Item Pictures** page.

    > [!NOTE]
    > For item cards that already have a picture, the **Picture Already Exists** check box is selected. If you do not want any existing pictures to be replaced, deselect the **Replace Pictures** check box. If you do not want individual existing pictures to be replaced, delete the lines in question.

3. Choose the **Import Pictures** action.

The **Import Status** field is updated to show if the picture import was skipped or completed.       

## <a name="see-also"></a>See Also
[Register New Items](inventory-how-register-new-items.md)  
[Create Number Series](ui-create-number-series.md)  
[Inventory](inventory-manage-inventory.md)  
[Purchasing](purchasing-manage-purchasing.md)  
[Sales](sales-manage-sales.md)  
[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]