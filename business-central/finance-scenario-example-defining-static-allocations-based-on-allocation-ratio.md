---
title: Defining Static Allocations Based on Allocation Ratio | Microsoft Docs
description: Static allocation method is based on a definite value, such as square meters used, or an established allocation ratio such as 5:2:4.
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
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: 036aa1f317c1b1de7fc1548e03d40eca8c25be89
ms.contentlocale: en-nz
ms.lasthandoff: 09/28/2018

---
# <a name="scenario-example-defining-static-allocations-based-on-allocation-ratio"></a>Scenario Example: Defining Static Allocations Based on Allocation Ratio
Static allocation method is based on a definite value, such as square meters used, or an established allocation ratio such as 5:2:4.  

This topic describes how to define three new allocation target cost objects for the allocation source PROD cost centre using the established allocation ratio 5:2:4. The three target cost objects are ACCESSO, PAINT, and FITTINGS.  

> [!NOTE]  
>  The example uses the demo data in the [!INCLUDE[d365fin](includes/d365fin_md.md)].  

## <a name="to-define-the-allocation-source-prod-cost-center-on-the-general-fasttab"></a>To define the allocation source PROD cost centre on the General FastTab  

1.  Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Cost Allocation**, and then choose the related link.  
2.  In the **Cost Allocation** window, choose the **New** action.  
3.  In the **ID** field, press Enter or enter an ID.  
4.  In the **Level** field, enter **1**.  
5.  In the **Valid From** and **Valid To** fields, enter appropriate dates.  
6.  In the **Cost Centre Code** field, enter **PROD**.  
7.  In the **Credit to Cost Type** field, enter the cost type **9903**.  

## <a name="to-define-the-allocation-target-cost-objects-on-the-lines-fasttab"></a>To define the allocation target cost objects on the Lines FastTab  

1.  On the first line, in the **Target Cost Type** field, enter **9903**.  
2.  On the first line, in the **Target Cost Object** field, select **ACCESSO**.  
3.  On the first line, in the **Allocation Target Type** field, select **All Costs** to define how all accrued costs are allocated.  
4.  On the first line, in the **Base** field, select **Static** to use the static allocation method.  
5.  On the first line, in the **Share** field, enter the allocation ratio **5**.  
6.  On the second line, in the **Target Cost Type** field, enter **9903**.  
7.  On the second line, in the **Target Cost Object** field, select **PAINT**.  
8.  On the second line, in the **Allocation Target Type** field, select **All Costs** to define how all accrued costs are allocated.  
9. On the second line, in the **Base** field, select **Static** to use the static allocation method.  
10. On the second line, in the **Share** field, enter the allocation ratio **2**.  
11. On the third line, in the **Target Cost Type** field, enter **9903**.  
12. On the third line, in the **Target Cost Object** field, select **FITTINGS**.  
13. On the third line, in the **Allocation Target Type** field, select **All Costs** to define how all accrued costs are allocated.  
14. On the third line, in the **Base** field, select **Static** to use the static allocation method.  
15. On the third line, in the **Share** field, enter the allocation ratio **4**.  

> [!IMPORTANT]  
>  [!INCLUDE[d365fin](includes/d365fin_md.md)] automatically calculates the **Percent** field using a percentage rate that is dependent on all three allocation ratios that are entered in the **Share** field for all three lines.  

## <a name="see-also"></a>See Also  
[Set Up Allocation Source and Targets](finance-how-to-set-up-allocation-source-and-targets.md)   
[Defining and Allocating Costs](finance-define-and-allocate-costs.md)   
[Scenario Example: Defining Dynamic Allocations Based on Items Sold](finance-scenario-example-defining-dynamic-allocations-based-on-items-sold.md)   
[Defining and Allocating Costs](finance-define-and-allocate-costs.md)

