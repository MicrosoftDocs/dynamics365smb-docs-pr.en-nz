---
title: 'How to: Transfer Bank Funds| Microsoft Docs'
description: 'How to: Transfer Bank Funds'
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: bank account transfer, multiple currencies
ms.date: 03/32/2017
ms.author: sgroespe
ms.translationtype: Human Translation
ms.sourcegitcommit: a31be0f9d07e2abb591e26f6bae34c6f6e4dcda6
ms.openlocfilehash: e2e3642d08428367fac1dd5845013e14627fe6ed
ms.contentlocale: en-nz
ms.lasthandoff: 05/04/2017


---
# <a name="how-to-transfer-bank-funds"></a>How to: Transfer Bank Funds
You may sometimes need to transfer an amount from one bank account to another. To do this, you must post the a transaction in the general journal. The task varies depending on whether the bank accounts use the same currency or different currencies.

## <a name="to-post-a-transfer-between-bank-accounts-with-the-same-currency-code"></a>To post a transfer between bank accounts with the same currency code
1. In the top right corner, choose the **Search for Page or Report** icon ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon"), enter **General Journal**, and then choose the related link.
2. On a journal line, fill in the **Posting Date** and **Document No.** fields.
3. In the **Account Type** field, select **Bank Account**.
4. In the **Account No.** field, select the bank from which you want to transfer the funds.
5. In the **Amount** field, enter the amount to be transferred.
6. In the **Bal. Account Type** field, select **Bank Account**.
7. In the **Bal. Account No.** field, select the bank account to which you want to transfer the funds.
8. Post the journal.

## <a name="to-post-a-transfer-between-bank-accounts-with-different-currency-codes"></a>To post a transfer between bank accounts with different currency codes
To transfer funds between bank accounts that use different currencies, you must post two general journal lines.

1. In the top right corner, choose the **Search for Page or Report** icon ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon"), enter **General Journal**, and then choose the related link.
2. Create two journal lines, and fill in the **Posting Date** and **Document No.** fields.
3. On the first journal line, in the **Type** field, select **Bank Account**.
4. In the **Account No.** field, select the bank account from which you want to transfer the funds.
5. In the **Amount** field, enter the amount in the currency of the bank account. Enter credit amounts with a minus sign. Enter debit amounts without a minus sign.
6. In the **Bal. Account Type** field, select **Bank Account**.
7. In the **Bal. Account No.** field, select the bank account to which you want to transfer the funds.
8. On the second journal line, in the **Type** field, select **Bank Account**.
9. In the **Account No.** field, select the bank account to which you want to transfer the funds.
10. In the **Amount** field, enter the amount in the currency of the bank account. Enter credit amounts with a minus sign. Enter debit amounts without a minus sign.
11. In the **Bal. Account Type** field, select **Bank Account**.  
12. In the **Bal. Account No.** field, select the bank account from which you want to transfer the funds.

    **Note**: If the exchange rates used in the journal are different than the exchange rates in the **Currency Exchange Rates** window, enter a third line for the exchange rate gain or loss. Enter **G/L Account** in the **Account Type** field. Enter the G/L account number for exchange rate gain or loss in the **Account No.** field. Enter the exchange rate gain or loss in the **Amount** field with or without a minus sign for credits and debits respectively.
13. Post the journal.

## <a name="see-also"></a>See Also
[Managing Bank Accounts](bank-manage-bank-accounts.md)  
[Setting Up Banking](bank-setup-banking.md)  
[Working With General Journals](ui-work-general-journals.md)  
[Working With [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

