---
title: 'How to: Use Resources for Jobs| Microsoft Docs'
description: Describes how to use time sheets to manage projects.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: project management, capacity, staff
ms.date: 03/28/2017
ms.author: sgroespe
ms.translationtype: Human Translation
ms.sourcegitcommit: a31be0f9d07e2abb591e26f6bae34c6f6e4dcda6
ms.openlocfilehash: 34d8b133a11324e1821780e3988158bb0989349b
ms.contentlocale: en-nz
ms.lasthandoff: 05/04/2017


---
# <a name="how-to-use-resources-for-jobs"></a>How to: Use Resources for Jobs
You record the usage of resources in the job journal to keep track of costs, prices, and the work types that are linked to jobs. For more information, see [How to: Record Usage for Jobs](projects-how-record-job-usage.md).

You can also post the usage of a resource in a resource journal. Entries posted in a resource journal have no effect on the general ledger.

**Note**: This functionality requires that your experience is set to **Suite**. For more information, see [Customizing Your [!INCLUDE[d365fin](includes/d365fin_md.md)] Experience](ui-experiences.md).

## <a name="to-assign-resources-to-jobs"></a>To assign resources to jobs
You assign resources to jobs by creating job planning lines for the job. For more information, see [How to: Create Jobs](projects-how-create-jobs.md).

## <a name="to-record-resource-usage-for-a-job"></a>To record resource usage for a job
1. In the top right corner, choose the **Search for Page or Report** icon ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon"), enter **Job Journals**, and then choose the related link.
2. Open a relevant job journal batch, and then fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. When the journal is complete, choose the **Post** action.

## <a name="to-adjust-resource-prices"></a>To adjust resource prices
If you want to change costs or prices for a large number of resources, you can use a batch job.  

1. In the top right corner, choose the **Search for Page or Report** icon ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon"), enter **Adjust Resource Costs/Prices**, and then choose the related link.
2. Fill in the fields on a line as necessary, and then choose the **OK** button.

**Note**: This batch job does not create or adjust alternate costs or prices for resources. It only changes the contents of the field on the resource card for the **Adjust Field** field that you selected in the batch job. The adjustment will take effect immediately for resources, so check your adjustment factors before you run the batch job.

## <a name="to-get-resource-price-change-suggestions-based-on-existing-alternate-prices"></a>To get resource price change suggestions based on existing alternate prices
If you have already set up alternate resource price for some resources, you can use a batch job to set up multiple alternate resource prices.

1. In the top right corner, choose the **Search for Page or Report** icon ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon"), enter **Resource Price Changes**, and then choose the related link.
2. Choose the **Suggest Res. Price Chg. (Price)** action, and then fill in the fields as necessary.
3. Choose the **OK** button.  
4. When the batch job is finished, the **Resource Price Changes** window shows the results of the batch job.

## <a name="to-get-resource-price-change-suggestions-based-on-standard-prices"></a>To get resource price change suggestions based on standard prices
If you want to set up multiple alternate resource prices based on the standard prices on the resource cards, you can use a batch job.  

1. In the top right corner, choose the **Search for Page or Report** icon ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon"), enter **Resource Price Changes**, and then choose the related link.
2. Choose the **Suggest Res. Price Chg. (Res.)** action, and then fill in the fields as necessary.  
3. Choose the **OK** button.  
4. When the batch job is finished, open the **Resource Price Changes** window to see the results of the batch job.

## <a name="to-get-resource-price-change-suggestions-based-on-alternate-prices"></a>To get resource price change suggestions based on alternate prices
If you have already set up alternate resource price for some resources, you can use a batch job to set up multiple alternate resource prices.

1. In the **Search** box, enter **Suggest Res. Price Chg. (Price)**, and then choose the related link.  
2. Fill in the fields as necessary.
3. Choose the **OK** button.  
4. When the batch job is finished, open the **Resource Price Changes** window to see the results of the batch job.

## <a name="see-also"></a>See Also
[Project Management](projects-manage-projects.md)  
[Finance](finance.md)  
[Purchasing](purchasing-manage-purchasing.md)         
[Sales](sales-manage-sales.md)     
[Working With [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

