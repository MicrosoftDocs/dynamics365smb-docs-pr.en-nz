---
title: Revalue Fixed Assets
description: 'Learn how to adjust the value of fixed assets, recording new amounts as a write-down or appreciation, and post other acquisition costs.'
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bholtorf
ms.topic: conceptual
ms.search.form: '5628, 5629, 5633'
ms.date: 02/22/2024
ms.service: dynamics-365-business-central
ms.custom: bap-template
---
# <a name="revalue-fixed-assets"></a>Revalue Fixed Assets

Revaluation of fixed assets can consist of appreciations, write-downs, or general value adjustments.

When the value of a fixed asset increases, you post a journal line with appreciation to the depreciation book. The new amount is recorded as appreciation according to the fixed asset posting setup.

When the value of a fixed asset decreases, you post a journal line with a lower amount, a write-down, to the depreciation book. The new amount is recorded as a write-down according to the fixed asset posting setup.

Indexation is used to adjust multiple fixed asset values, for example per general price changes. The **Index Fixed Assets** batch job can be used to change various amounts, such as write-down and appreciation amounts.

## <a name="to-post-appreciation-from-the-fixed-asset-gl-journal"></a>To post appreciation from the fixed asset G/L journal

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **FA G/L Journals**, and then choose the related link.  
2. Create an initial journal line and fill in the fields as necessary.
3. In the **FA Posting Type** field, select **Revaluation**.
4. Choose the **Insert FA Bal. Account** action. A second journal line is created for the balancing account that is set up for appreciation posting.

    > [!NOTE]  
    >   Step 4 only works if you have set up the following: On the **FA Posting Group Card** page for the posting group of the fixed asset, the **Appreciation Account** field contains the general ledger debit account and the **Appreciation Bal. Account** field contains the general ledger account to which you want to post balancing entries for appreciation. For more information, see [To set up fixed asset posting groups](fa-how-setup-general.md#to-set-up-fixed-asset-posting-groups).  
5. Choose the **Post** action.

## <a name="to-post-a-write-down-from-the-fixed-asset-gl-journal"></a>To post a write-down from the fixed asset G/L journal

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **FA G/L Journals**, and then choose the related link.  
2. Create an initial journal line, and fill in the fields as necessary.
3. In the **FA Posting Type** field, select **Write-Down**.
4. Choose the **Insert FA Bal. Account** action. A second journal line is created for the balancing account that is set up for write-down posting.

    > [!NOTE]  
    >   Step 4 only works if you have set up the following: On the **FA Posting Group Card** page for the posting group of the fixed asset, the **Write-Down Account** field contains the general ledger credit account and the **Write-Down Expense Account** field contains the general ledger debit account to which you want to post balancing entries for write-downs. For more information, see [To set up fixed asset posting groups](fa-how-setup-general.md#to-set-up-fixed-asset-posting-groups).
5. Choose the **Post** action.

## <a name="to-perform-general-revaluation-of-fixed-assets"></a>To perform general revaluation of fixed assets

Indexation is used to adjust multiple fixed asset values, for example per general price changes. The **Index Fixed Assets** batch job can be used to change various amounts, such as write-down and appreciation amounts. The **Allow Indexation** checkbox on the **Depreciation Book** page must be selected.

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Index Fixed Assets**, and then choose the related link.  
2. Fill in the fields as necessary.
3. Choose the **OK** button.

    Revaluation lines are created per your settings in step 2. The lines are created in either the fixed asset journal or the fixed asset G/L journal, depending on your template and batch setup on the **FA Journal Setup** page. For more information, see [Set Up General Fixed Asset Information](fa-how-setup-general.md).
4. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **FA G/L Journals**, and then choose the related link.  
5. Select the journal with the fixed assets that you want to revalue, and then choose the **Ledger Entries** action.  
6. Check the created entries, and then choose the **Post** action to post the journal.

    > [!TIP]  
    >   If the index figures are for simulation purposes only, you can create a special depreciation book to store them in. Then these entries will not affect any of the other depreciation books.

## <a name="to-post-other-acquisition-costs"></a>To post other acquisition costs

You post other acquisition cost for a fixed asset from a purchase invoice or from a fixed asset journal in the same way as you post the original acquisition cost. For more information, see [Acquire Fixed Assets](fa-how-acquire.md).  

If depreciation is already calculated for the fixed asset, select the **Depr. Acquisition Cost** checkbox to have the other acquisition cost less the salvage value depreciated in proportion to the amount by which the previously acquired fixed asset is depreciated. This method ensures that the depreciation period isn't changed.  

The depreciation percentage is calculated as:  

*P = (total depreciation x 100) / depreciable basis*

*Depreciation amount = (P/100) x (extra acquisition cost - salvage value)*  

Remember to select the **Depr. until FA Posting Date** checkbox on the invoice, the fixed asset G/L journal, or the fixed asset journal lines to ensure that depreciation is calculated from the last fixed asset posting date to the posting date of the other acquisition cost.

### <a name="example---posting-other-acquisition-costs"></a>Example - Posting Other Acquisition Costs

A machine is purchased on August 1, 2000. The acquisition cost is 4,800. The depreciation method is straight-line over four years.

On August 31, 2000, the **Calculate Depreciation** batch job is run. Depreciation is calculated as:

*book value x number of depreciation days / total number of depreciation days = 4800 x 30 / 1440 = 100*  

On September 15, 2000, an invoice is posted for painting the machine. The invoice amount is 480.

If you selected the **Depr. until FA Posting Date** checkbox on the invoice before posting, the following calculation is made:  

15 days of depreciation (from 09/01/00 to 09/15/00) is calculated as:

*book value x number of depreciation days / remaining number of depreciation days = (4800 - 100) x 15 / 1410 = 50*

If you selected the **Depr. Acquisition Cost** checkbox on the invoice before posting, the following calculation is made:  

*The other acquisition cost is depreciated as ((150 x 100) / 4800) / 100 x 480 = 15*

The depreciable basis is now *5280 = (4800 + 480)*, and the accumulated depreciation is *165 = (100 + 50 + 15)*, corresponding to 45 days of depreciation of the total acquisition cost. This calculation means that the asset is totally depreciated within the estimated lifetime of four years.  

When the **Calculate Depreciation** batch job is run on 09/30/00, the following calculation is made:  

*Remaining depreciable life is 3 years, 10 months, and 15 days = 1395 days*  

*Book value is (5280 - 165) = 5115*  

*Depreciation amount for September 2000: 5115 x 15 / 1395 = 55.00*  

*Total of depreciation = 165 + 55 = 220*  

If you didn't select the **Depr. until FA Posting Date** checkbox, the asset would lose 15 days of depreciation because the **Calculate Depreciation** batch job run on 09/30/00 would calculate depreciation from 09/15/00 to 09/30/00. This means that when the **Calculate Depreciation** batch job is run on 09/30/00, the calculation is as follows:  

*Remaining life time is 3 years, 10 months, and 15 days = 1395 days*  

*Book value is (4800 + 480 - 100 - 15) = 5165*

*Depreciation amount for September 2000: 5165 x 15 / 1395 = 55.54*  

*Total of depreciation = 100 + 15 + 55.54 = 170.54*

## <a name="see-also"></a>See also

[Fixed Assets](fa-manage.md)  
[Setting Up Fixed Assets](fa-setup.md)  
[Finance](finance.md)  
[Getting Ready for Doing Business](ui-get-ready-business.md)  
[Work with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]
