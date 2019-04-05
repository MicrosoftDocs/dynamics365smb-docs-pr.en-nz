---
title: Set Up FA Depreciation| Microsoft Docs
description: You specify in a depreciation book how you want fixed assets to be depreciated or written-down.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: write down
ms.date: 10/01/2018
ms.author: sgroespe
ms.openlocfilehash: d417db84cf45356925cf52a36ba08e478b8ee6b9
ms.sourcegitcommit: 1bcfaa99ea302e6b84b8361ca02730b135557fc1
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 03/08/2019
ms.locfileid: "822513"
---
# <a name="set-up-fixed-asset-depreciation"></a>Set Up Fixed Asset Depreciation
 You can use various methods of depreciation for preparing financial statements and income tax returns. Many large corporations use straight-line depreciation in their financial statements because this generally permits reporting higher earnings. For income tax purposes, however, many businesses use an accelerated depreciation method. For more information, see [Depreciation Methods](fa-depreciation-methods.md).

 When you have created the relevant depreciation books, you must assign one or more depreciation books to each fixed asset. A depreciation book that is assigned to a fixed asset is referred to as a fixed asset depreciation book. Accordingly, the page for assigned depreciation books is called **FA Depreciation Books**.

## <a name="to-create-a-depreciation-book"></a>To create a depreciation book
In a fixed asset depreciation book, you specify how fixed assets are depreciated. To accommodate various methods of depreciation, you can set up multiple depreciation books.  

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Depreciation Books**, and then choose the related link.
2. On the **Depreciation Books List** page, choose the **New** action.
3. On the **Depreciation Book Card** page, fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

    > [!NOTE]  
    >   You can record fixed asset transactions on the **Fixed Asset G/L Journal** page or on the **Fixed Asset Journal** page, depending on whether the transactions are for financial reporting or for internal management. Follow the next step to define which type of journal is used for the different fixed asset activities by default.
4. On the **Integration** FastTab, select the check box for each fixed asset activity whose transactions you want to post using the **Fixed Asset G/L Journal** page.
5. Repeat steps 2 through 4 for each depreciation method or posting method that you want to assign to fixed assets as a depreciation book.

## <a name="to-assign-a-depreciation-book-to-a-fixed-asset"></a>To assign a depreciation book to a fixed asset
1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Fixed Assets**, and then choose the related link.
2. Select the fixed asset that you want to set up a fixed asset depreciation book for.
3. On the **Depreciation Book** FastTab, fill in the fields as necessary.
4. If you need to assign more than one depreciation book to the fixed asset, choose the **Add More Depreciation Books** action.
5. Alternatively, choose the **Depreciation Books** action to specify one or more fixed asset depreciation books.

    > [!NOTE]  
    >   When you use the manual depreciation method, you must enter depreciation manually in the fixed asset G/L journal. The **Calculate Depreciation** function omits fixed assets that use the manual depreciation method. You can use this method for assets that are not subject to depreciation, such as land.

## <a name="to-assign-a-depreciation-book-to-multiple-fixed-assets-with-a-batch-job"></a>To assign a depreciation book to multiple fixed assets with a batch job
If you want to assign a depreciation book to several fixed assets, you can use the **Create FA Depreciation Books** batch job to create fixed asset depreciation books.  

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Fixed Assets**, and then choose the related link.
2. Select the fixed asset that you want to set up a assign a depreciation book to, and then choose the **Edit** action.
3. On the **Depreciation Book Card** page, choose the **Create FA Depreciation Books** action.
4. On the **Create FA Depreciation Books** page, fill in the **Depreciation Book** field.
5. Choose the **Copy from FA No.** field, and then select the fixed asset number that you want to use as the basis for creating new fixed asset depreciation books.

    If you fill in this field, the depreciation fields in the new fixed asset depreciation books will contain the same information as the corresponding fields in the fixed asset depreciation book that you copy from. Leave the field blank if you want to create new fixed asset depreciation books with empty depreciation fields.  
6. On the **Fixed Asset** FastTab, you can set a filter to select the assets that you want to create the fixed asset depreciation books for.
7. Choose the **OK** button.

## <a name="to-set-up-depreciation-posting-types"></a>To set up depreciation posting types
For each depreciation book, you must set up how you want [!INCLUDE[d365fin](includes/d365fin_md.md)] to handle various posting types. For example, whether posting should be debit or credit and whether the posting type should be included in the depreciable basis.  

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Depreciation Books**, and then choose the related link.  
2. Select the depreciation book that you want to set up, and them choose the **FA Posting Type Setup** action.
3. On the **FA Posting Type Setup** page, fill in the fields as necessary.

    > [!NOTE]  
    >   You cannot insert or delete lines on the **FA Posting Type Setup** page. You can only modify the existing lines.

We recommend that you do not change the setup for depreciation books for entries that have already been posted. Changes will not affect the entries that are already posted, which would make depreciation book statistics misleading.

## <a name="to-set-up-default-templates-and-batches-for-fixed-asset-depreciation"></a>To set up default templates and batches for fixed asset depreciation
For each depreciation book, you define a default setup of templates and batches. You use these defaults to duplicate lines from one journal to another, create journal lines using the **Calculate Depreciation** or **Index Fixed Assets** batch jobs, duplicate acquisition costs in the insurance journal.  

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Depreciation Books**, and then choose the related link.  
2. Select the depreciation book that you want to define default journals for, and then choose the **FA Journal Setup** action.  
3. If you want to have a default setup for each user, choose the **User ID** field to select from the **Users** page.  
4. In the other fields, select the journal template or journal batch that must be used by default.  

## <a name="see-also"></a>See Also
[Setting Up Fixed Assets](fa-setup.md)  
[Fixed Assets](fa-manage.md)  
[Finance](finance.md)  
[Getting Started](product-get-started.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
