---
title: Acquire fixed assets
description: 'You can set up a fixed asset, assign a depreciation book, and record the fixed asset’s acquisition cost.'
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bholtorf
ms.topic: conceptual
ms.search.keywords: purchase fixed asset
ms.search.form: '5605, 5551, 5600, 5628, 5629, 5633'
ms.date: 05/15/2024
ms.service: dynamics-365-business-central
ms.custom: bap-template
---
# <a name="acquire-fixed-assets"></a>Acquire fixed assets

Use the **Fixed Asset Card** page to enter information about an asset. You can set up buildings or production equipment as a main asset with a component list, and you can group them in various ways, such as by class, department, or location. You must set up and assign a depreciation book to each fixed asset before you can acquire it.

After you set up a fixed asset and assign a depreciation book, you must acquire the fixed asset. To acquire a fixed asset, you record its acquisition cost in the relevant G/L account, bank account, or vendor by posting an acquisition transaction from the **Fixed Asset G/L Journal** page. You can use the **Assisted Fixed Asset Acquisition** page to create and post the required general journal lines automatically.

Use indexation to adjust values for general price-level changes. Use the **Index Fixed Assets** batch job to calculate the acquisition costs and replacement costs.

## <a name="add-a-fixed-asset-to-your-list-of-fixed-assets"></a>Add a fixed asset to your list of fixed assets

Before you can acquire a fixed asset, you must add it to your list of assets. There are several ways to add fixed assets to your list:

* Enter information about the assets on the **Fixed Asset Card** page.
* Use the **Edit in Excel** action to download your list of assets to a worksheet, add new assets to the list, and then publish the update to [!INCLUDE [prod_short](includes/prod_short.md)].
* Use a purchase order to add assets.
* Use the **Copy fixed asset** action.

After you add fixed assets to your list, the next step is to acquire them so you can use them in transactions. Learn more at [Acquire a fixed asset](#acquire-fixed-assets).

### <a name="add-a-fixed-asset-on-the-fixed-asset-card-page"></a>Add a fixed asset on the Fixed Asset Card page

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Fixed Assets**, and then choose the related link.  
2. Choose the **New** action, and then fill in the fields on the **General** FastTab as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. On the **Depreciation Book** FastTab, fill in the fields as necessary. This step assigns a depreciation book to the fixed asset.  
4. If you need to assign more than one depreciation book to the fixed asset, choose the **Add More Depreciation Books** action. To learn more, go to [To assign a depreciation book to a fixed asset](fa-how-setup-depreciation.md#to-assign-a-depreciation-book-to-a-fixed-asset).

    After you fill in the required fields, the **You are ready to acquire the fixed asset.** notification appears at the top of the page. If you're ready to acquire the asset now, choose the **Acquire** action. Follow the steps on the **Assisted Fixed Asset Acquisition** page to complete the acquisition. If you aren't ready, you can always acquire the asset later.

### <a name="use-edit-in-excel-to-add-assets"></a>Use Edit in Excel to add assets

If you want to add numerous fixed assets, Edit in Excel is a great tool to use. The tool downloads your current list of assets in a worksheet that includes most of the fields available on the Fixed Asset Card page. You can fill in some or all of fields on a row for each asset, and publish your changes to add them to your list in [!INCLUDE [prod_short](includes/prod_short.md)]. If you can't fill in all required field, that's ok. You can update them in [!INCLUDE [prod_short](includes/prod_short.md)] when you're ready.

> [!NOTE]
> To use the Edit in Excel action, you must have the Microsoft Dynamics Office Add-in installed. The add-in creates the connection between Excel and [!INCLUDE [prod_short](includes/prod_short.md)]. To learn more, go to [Get the Business Central Add-in for Excel](admin-deploy-excel-addin.md).

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Fixed Assets**, and then choose the related link.
2. Choose the :::image type="content" source="media/share-icon.png" alt-text="Share this page with other users or apps icon."::: icon, and then choose **Edit in Excel**.
3. Open the downloaded file, and enter information about the new fixed assets.

   > [!TIP]
   > You don't need to enter an identifier in the **No.** column. When you publish your update, [!INCLUDE [prod_short](includes/prod_short.md)] assigns an identifier based on the number series you use for fixed assets.

4. To update [!INCLUDE [prod_short](includes/prod_short.md)], on the **Microsoft Dynamics** pane, choose **Publish**.

### <a name="add-a-fixed-asset-from-a-purchase-order-or-invoice"></a>Add a fixed asset from a purchase order or invoice

The following steps describe how to add a fixed asset from a purchase order. The steps are similar for a purchase invoice.

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchase Orders**, and then choose the related link.
2. Choose **New** to create a new purchase order.
3. On the **General** FastTab, fill in the fields as necessary. [!INCLUDE [tooltip-inline-tip_md](../archive/SetupAndAdministration/includes/tooltip-inline-tip_md.md)]
4. On the **Lines** FastTab, in the **Type** field, choose **Fixed Asset**.
5. In the **No.** field, either choose an existing fixed asset to add an expense, or choose **New** to add a new asset.
6. After you enter the information for the new asset and the purchase order, choose **Post**.

## <a name="acquire-a-fixed-asset-by-using-a-fixed-asset-gl-journal"></a>Acquire a fixed asset by using a fixed asset G/L journal

The following procedure describes how to acquire by creating and posting the required fixed asset G/L journal lines. You can also create and post the journal lines manually. To learn more, go to [Acquire a fixed asset by using a fixed asset G/L journal](#acquire-a-fixed-asset-by-using-a-fixed-asset-gl-journal).

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Fixed Assets**, and then choose the related link.
1. Choose the asset you want to acquire, and then choose the **Acquire** action.
1. Follow the steps on the **Assisted Fixed Asset Acquisition** page to complete the acquisition.

> [!NOTE]  
> You can also post acquisition cost as credits. In that case, remember that the value in the **Acquisition Cost Incl. GST** field must be with a minus sign to indicate a credit.

When you choose **Finish**, the **Book Value** field on the **Fixed Asset Card** page is filled in, which indicates that the fixed asset was acquired at the specified acquisition cost.  

## <a name="to-post-a-fixed-asset-acquisition-manually-with-a-fixed-asset-gl-journal"></a>To post a fixed asset acquisition manually with a fixed asset G/L journal

The following procedure describes how to acquire a fixed asset manually by creating and posting lines on the **Fixed Asset G/L Journal** page. You can also acquire a fixed asset automatically on the **Fixed Asset Card** page by choosing the **Acquire fixed asset** action. To learn more, go to [Acquire a fixed asset](#acquire-fixed-assets).

> [!NOTE]  
> You can also post acquisition cost as credits. In that case, remember that the value in the **Amount** field must be with a minus sign to indicate a credit.

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Fixed Asset G/L Journals**, and then choose the related link.
2. On the **Fixed Asset G/L Journal** page, in the **FA Posting Type** field, select **Acquisition Cost**.
3. Fill in the remaining fields as necessary.
4. Choose the **Post** action.  

> [!TIP]  
> If you fill in the **Insurance No.** field, [!INCLUDE[prod_short](includes/prod_short.md)] also posts the acquisition cost of the fixed asset to the insurance coverage ledger. To learn more, go to [Insure Fixed Assets](fa-how-insure.md).

## <a name="to-set-up-a-component-list-for-a-main-asset"></a>To set up a component list for a main asset

You can group your fixed assets into main assets and their components. For example, you might have a production machine that consists of several parts that you want to group in this manner.  

You must set up the main asset and all its components as individual fixed asset. After you set up a component list, [!INCLUDE[prod_short](includes/prod_short.md)] automatically fills in the **Main Assets/Component** and **Components of Main Asset** fields on the fixed assets.

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Fixed Assets**, and then choose the related link.
2. Select the fixed asset that is the main asset, and then choose the **Main Asset Components** action.
3. On the **Main Asset Components** page, choose the **FA No**. field, and then select the fixed asset that you want to add as a component of the main asset.
4. Close the page.
5. Repeat steps 3 and 4 for each component asset that you want to add.
6. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Fixed Asset Setup**, and then choose the related link.
7. Turn on the **Allow Posting to Main Assets** toggle.

## <a name="to-cancel-an-acquisition-cost-posting-for-one-fixed-asset"></a>To cancel an acquisition cost posting for one fixed asset

If you make an error when posting an acquisition cost, you can remove the entry with the **Cancel FA Entries** batch job and then post the correct acquisition entry. The erroneous entries are transferred to the **FA Error Ledger Entries** page.

For example, if you post an acquisition with the wrong date, you must correct it as soon as possible because the fixed asset posting date is used for many calculations.

> [!IMPORTANT]  
> You can't use the **Reverse Transactions** action for fixed asset entries.

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **FA Ledger Entries**, and then choose the related link.  
2. In the **FA Ledger Entries** page, select the entry or entries that you want to cancel.  
3. Choose the **Actions** menu, and then choose the **Cancel Entries** action.
4. Fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
5. Choose the **OK** button to run the batch job.
6. When the incorrect entry or entries are cancelled, proceed to post the correct acquisition cost.

## <a name="to-post-the-salvage-value-together-with-the-acquisition-cost"></a>To post the salvage value together with the acquisition cost

The salvage value is the residual value of a fixed asset when it can no longer be used. You can post the salvage value at the same time as you post the acquisition cost. To learn more, go to [Depreciate or Amortize Fixed Assets](fa-how-depreciate-amortize.md).

You can post the salvage value together with the acquisition cost from a fixed asset journal.

> [!NOTE]
> This process might require that you personalise the Fixed Asset Journals page by adding the Salvage Value field. By default, the field is not displayed on the page. To learn more, go to [Personalize Your Workspace](ui-personalization-user.md).

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Fixed Asset Journals**, and then choose the related link.
2. On the **Fixed Asset Journals** page, create the acquisition line. To learn more, go to [To post a fixed asset acquisition manually with a fixed asset G/L journal](#to-post-a-fixed-asset-acquisition-manually-with-a-fixed-asset-gl-journal).
3. In the **Salvage Value** field on the journal line, enter the salvage value amount as a credit (prefix the amount with a minus sign, for example, **-** 100).
4. Choose the **Post** action.

> [!NOTE]
> If a salvage value exists for a fixed asset, that value is used in depreciation posting instead of the value in the **Ending Book Value** field on the **FA Depreciation Books** page. To learn more, go to [To manage the ending book value](fa-how-depreciate-amortize.md#to-manage-the-ending-book-value).

## <a name="see-also"></a>See also

[Fixed Assets](fa-manage.md)  
[Setting Up Fixed Assets](fa-setup.md)  
[Design details about nondeductible VAT impact on Fixed Assets](design-details-nondeductible-vat.md)  
[Finance](finance.md)  
[Getting Ready for Doing Business](ui-get-ready-business.md)  
[Work with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
