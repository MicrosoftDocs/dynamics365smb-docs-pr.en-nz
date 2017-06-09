---
title: 'How to: Export Positive Pay Files| Microsoft Docs'
description: Describes how to make sure that your bank only clears validated checks and amounts by exporting a Positive Pay file that contains vendor and payment information.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: check, clearing
ms.date: 03/24/2017
ms.author: sgroespe
ms.translationtype: Human Translation
ms.sourcegitcommit: a31be0f9d07e2abb591e26f6bae34c6f6e4dcda6
ms.openlocfilehash: ee93f8eb889ae1d635bca22ff133e1523fd1b825
ms.contentlocale: en-nz
ms.lasthandoff: 05/04/2017


---
# <a name="how-to-export-a-positive-pay-file"></a>How to: Export a Positive Pay file
To make sure that your bank only clears validated cheques and amounts, you can export a Positive Pay file that contains vendor information, cheque number, and payment amount, which you send to the bank for reference when you process payments.

[!INCLUDE[d365fin](includes/d365fin_md.md)] is preconfigured to support Positive Pay files for Bank of America and City Bank.

## <a name="to-set-up-a-bank-account-for-positive-pay"></a>To set up a bank account for Positive Pay
1. In the top right corner, choose the **Search for Page or Report** icon ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon"), enter **Bank Accounts**, and then choose the related link.
2. Open the card for the bank that you want to use Positive Pay for.
3. In the **Positive Pay Export Code** field, enter POSPAYBANK.
4. Close the window.

## <a name="to-export-a-positive-pay-file"></a>To export a Positive Pay file
1. In the top right corner, choose the **Search for Page or Report** icon ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon"), enter **Bank Accounts**, and then choose the related link.
2. Select the bank account that you want to export a Positive Pay file for.
3. Choose **Positive Pay Export** action.

    The **Positive Pay Export** window opens displaying payments that have been made for the bank account since the last upload date, as shown in the **Last Upload Date** and **Last Upload Time** fields.
4. In the **Cutoff Upload Date** field, specify a date before which payments are not included in the exported file.
5. Choose the **Export** action.
6. In the **Export File** window, choose the **Save** button, and then save the file to a convenient location.
7. Upload the file to your electronic bank site.
8. Write down or copy the confirmation number that is displayed when the file upload is successful.

To view exported Positive Pay records

1. In the top right corner, choose the **Search for Page or Report** icon ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon"), enter **Bank Accounts**, and then choose the related link.
2. Select the bank account that you want to view Positive Pay export records for.
3. Choose the **Positive Pay Entries** action.

    In the **Positive Pay Entries** window, you can see all the Positive Pay export records for the bank account.
4. In the **Confirmation Number** field, enter, for each export record, the confirmation number that you receive when the file upload to the bank is successful.
5. To view the related payment lines, choose the **Positive Pay Entry Details** action.

To reexport Positive Pay files

1. In the top right corner, choose the **Search for Page or Report** icon ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon"), enter **Bank Accounts**, and then choose the related link.
2. Select the bank account that you want to reexport Positive Pay files for.
3. Choose the **Positive Pay Entries** action.
4. Select the line for the Positive Pay export file that you want to reexport.
5. In the **Positive Pay Entries** window, choose the **Reexport Positive Pay to File** action.

## <a name="see-also"></a>See Also
[Finance](finance.md)  
[Setting Up Finance](finance-setup-finance.md)  
[How to: Work With General Journals](ui-work-general-journals.md)  
[Working With [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

