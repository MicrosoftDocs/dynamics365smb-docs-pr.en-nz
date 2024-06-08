---
title: Insure fixed assets
description: You can assign one or multiple fixed assets to one insurance policy by posting to the insurance coverage ledger from the **Insurance Journal** page.
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bholtorf
ms.topic: conceptual
ms.search.keywords: 'policy, coverage'
ms.search.form: '5647, 5644, 5653, 5651, 5655, 5652, 5645, 5656, 5646, 5648, 9275'
ms.date: 05/15/2024
ms.service: dynamics-365-business-central
ms.custom: bap-template
---
# <a name="insure-fixed-assets"></a>Insure fixed assets

Use the **Insurance Card** page to set up an insurance policy to cover one or more fixed assets. You can assign one fixed asset to one insurance policy, or multiple fixed assets to one insurance policy.

You assign a fixed asset to an insurance policy by posting to the insurance coverage ledger from the **Insurance Journal** page.

In addition, you can assign a fixed asset to an insurance policy and create coverage ledger entries when you post its acquisition cost. You post an acquisition cost from the fixed asset journal with the **Insurance No.** field filled in. You must turn on the **Automatic Insurance Posting** toggle on the **Fixed Asset Setup** page. For more information, see [Acquire a fixed asset by using a fixed asset G/L journal](fa-how-acquire.md#acquire-a-fixed-asset-by-using-a-fixed-asset-gl-journal).

If the **Automatic Insurance Posting** toggle on the **Fixed Asset Setup** page isn't turned on, posting acquisitions from the fixed asset journal creates lines on the **Insurance Journal** page. You must post those lines manually.

> [!WARNING]  
> If you don't turn on the **Automatic Insurance Posting** toggle on the **Fixed Asset Setup** page, your insurance journal should be based on a journal template without a number series. This is because the inserted document numbers from the fixed asset journal line will otherwise conflict with the number series of the insurance journal. For more information about journal templates and batches, see [Set Up General Fixed Assets Information](fa-how-setup-general.md).

After you assign a fixed asset to an insurance policy, the **Insured** field on the fixed asset card contains **Yes**. When you sell the fixed asset, the toggle is automatically turned off.

## <a name="to-create-or-modify-an-insurance-card"></a>To create or modify an insurance card

When you receive information about changes in the coverage amount, you must enter the new information on the **Insurance Card** page to ensure that you analyse insurance policy coverage correctly.  

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Insurance**, and then choose the related link.
2. Choose the **New** action to create a new card for an insurance policy. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. Alternatively, select the insurance policy that you want to change, and then choose the **Edit** action.

## <a name="to-assign-a-fixed-asset-to-an-insurance-policy-by-posting-from-the-insurance-journal"></a>To assign a fixed asset to an insurance policy by posting from the insurance journal

You assign a fixed asset to an insurance policy by posting to the insurance coverage ledger.  

The following procedure explains how to create an insurance journal line manually. If the **Automatic Insurance Posting** toggle is turned on the **Fixed Asset Setup** page, insurance journal lines are automatically created when you post acquisition costs. In that case, all you have to do is to post the journal.  

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Insurance Journals**, and then choose the related link.  
2. Open the relevant journal, and fill in the journal lines as necessary.  
3. To assign multiple fixed assets to one insurance policy, create journal lines with the same value in the **Insurance No.** field and different values in the **FA No.** field.  
4. Choose the **Post** action.  

    > [!NOTE]  
    > The entries from an insurance journal are only posted to the insurance coverage ledger.  

## <a name="to-update-the-insurance-value-of-a-fixed-asset"></a>To update the insurance value of a fixed asset

You can use the **Index Insurance** batch job to update the value of the fixed assets that are covered.  

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Index Insurance**, and then choose the related link.
2. Fill in the fields as necessary.

    > [!NOTE]  
    >   In the **Index Figure** field, you enter a decrease of 5%, for example, as 95, whereas you enter an increase of 2% as 102.  
3. Choose the **OK** button.  

   The batch job calculates the new amount as a percentage of the total value insured, as stated on the **Insurance Statistics** page, and then creates a line in the insurance journal.  
4. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Insurance Journals**, and then choose the related link.  
5. Open the relevant insurance journal, review the created values, and then post them to the insurance coverage ledger.  

## <a name="to-monitor-insurance-coverage"></a>To monitor insurance coverage

[!INCLUDE[prod_short](includes/prod_short.md)] provides dedicated reports and statistics pages for use in analysing insurance policies and whether your fixed assets are over- or under-insured.  

### <a name="overview-of-insurance-policies"></a>Overview of insurance policies

To get an overview of your insurance policies, preview or print the **Insurance - List** report. The report shows all the policies and the most important fields from the insurance cards.  

### <a name="insurance-coverage"></a>Insurance coverage

To see which insurance policies cover each asset and by which amount, you can preview or print the **Insurance - Tot. Value Insured** report.  

#### <a name="overunder-coverage"></a>Over/under coverage

You can check whether fixed assets are over- or under-insured in the following ways:  

* The **Insurance Statistics** page. A positive amount in the **Over/Under Insured** field means that the fixed asset is over-insured. A negative amount means that the asset is under-insured.  
* The **Fixed Asset Statistics** page. Choose the **Total Value Insured** field to view the **Ins. Coverage Ledger Entries** page.  
* The **Over/Under Coverage** report.  
* The **Insurance Analysis** report.  

### <a name="uninsured-fixed-assets"></a>Uninsured fixed assets

To check whether you forgot to assign a fixed asset to an insurance policy, you can print or preview the **Insurance - Uninsured FAs** report. This report displays fixed assets for which amounts aren't posted to the insurance coverage ledger.  

## <a name="to-view-insurance-coverage-ledger-entries"></a>To view insurance coverage ledger entries

You can view the entries that you made in the insurance coverage ledger.  

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Insurance**, and then choose the related link.  
2. Select the relevant insurance policy, and then choose the **Coverage Ledger Entries** action.  

## <a name="to-view-the-total-insurance-value-of-fixed-assets"></a>To view the total insurance value of fixed assets

A matrix page shows the insurance values that are registered for each insurance policy for each fixed asset that result from posted insurance-related amounts.  

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Insurance**, and then choose the related link.  
2. Select the relevant insurance policy, and then choose the **Total Value Insures per FA** action.  
3. Fill in the fields as necessary.  
4. Choose the **Show Matrix** action.  
5. To see the underlying insurance coverage ledger entries, choose a value in the matrix.  

## <a name="to-correct-insurance-coverage-entries"></a>To correct insurance coverage entries

If a fixed asset was assigned to the wrong insurance policy, you can correct it by creating two reclassification entries from the insurance journal.  

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Insurance Journals**, and then choose the related link.  
2. Create one journal line for the fixed asset and the correct insurance policy where the value in the **Amount** field is positive.  
3. Create another journal line for the fixed asset and the incorrect insurance policy where the value in the **Amount** field is negative.  
4. Choose the **Post** action.  

The fixed asset is removed from the incorrect insurance policy on the second line. The asset is assigned to the correct insurance policy on the first line of the journal.  

## <a name="see-also"></a>See also

[Fixed Assets](fa-manage.md)  
[Setting Up Fixed Assets](fa-setup.md)  
[Finance](finance.md)  
[Work with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
