---
title: Transfer Bank Funds
description: You can transfer amounts from one bank account to another, including different currencies, by posting the transaction in the general journal.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: bank account transfer, multiple currencies
ms.date: 04/29/2021
ms.author: edupont
ms.openlocfilehash: da9c8711751040cecb267a3b2209bad2534b618b
ms.sourcegitcommit: 08ca5798cf3f04fc3ea38fff40c1860196a70adf
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 05/06/2021
ms.locfileid: "5985403"
---
# <a name="transfer-bank-funds"></a><span data-ttu-id="a0856-103">Transfer Bank Funds</span><span class="sxs-lookup"><span data-stu-id="a0856-103">Transfer Bank Funds</span></span>

<span data-ttu-id="a0856-104">You may sometimes need to transfer an amount from one bank account in [!INCLUDE[prod_short](includes/prod_short.md)] to another.</span><span class="sxs-lookup"><span data-stu-id="a0856-104">You may sometimes need to transfer an amount from one bank account in [!INCLUDE[prod_short](includes/prod_short.md)] to another.</span></span> <span data-ttu-id="a0856-105">To do this, you must post the transaction on the **General Journal** page.</span><span class="sxs-lookup"><span data-stu-id="a0856-105">To do this, you must post the transaction on the **General Journal** page.</span></span> <span data-ttu-id="a0856-106">The task varies depending on whether the bank accounts use the same currency or different currencies.</span><span class="sxs-lookup"><span data-stu-id="a0856-106">The task varies depending on whether the bank accounts use the same currency or different currencies.</span></span>

## <a name="to-post-a-transfer-between-bank-accounts-with-the-same-currency-code"></a><span data-ttu-id="a0856-107">To post a transfer between bank accounts with the same currency code</span><span class="sxs-lookup"><span data-stu-id="a0856-107">To post a transfer between bank accounts with the same currency code</span></span>

1. <span data-ttu-id="a0856-108">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **General Journal**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="a0856-108">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **General Journal**, and then choose the related link.</span></span>
2. <span data-ttu-id="a0856-109">On a journal line, fill in the **Posting Date** and **Document No.** fields.</span><span class="sxs-lookup"><span data-stu-id="a0856-109">On a journal line, fill in the **Posting Date** and **Document No.** fields.</span></span>
3. <span data-ttu-id="a0856-110">In the **Account Type** field, select **Bank Account**.</span><span class="sxs-lookup"><span data-stu-id="a0856-110">In the **Account Type** field, select **Bank Account**.</span></span>
4. <span data-ttu-id="a0856-111">In the **Account No.** field, select the bank from which you want to transfer the funds.</span><span class="sxs-lookup"><span data-stu-id="a0856-111">In the **Account No.** field, select the bank from which you want to transfer the funds.</span></span>
5. <span data-ttu-id="a0856-112">In the **Amount** field, enter the amount to be transferred.</span><span class="sxs-lookup"><span data-stu-id="a0856-112">In the **Amount** field, enter the amount to be transferred.</span></span>

    <span data-ttu-id="a0856-113">Next, you must specify the balancing account.</span><span class="sxs-lookup"><span data-stu-id="a0856-113">Next, you must specify the balancing account.</span></span> <span data-ttu-id="a0856-114">If you can't see the relevant fields, then choose the **Show More Columns** action to view all available fields.</span><span class="sxs-lookup"><span data-stu-id="a0856-114">If you can't see the relevant fields, then choose the **Show More Columns** action to view all available fields.</span></span>
6. <span data-ttu-id="a0856-115">In the **Bal. Account Type** field, select **Bank Account**.</span><span class="sxs-lookup"><span data-stu-id="a0856-115">In the **Bal. Account Type** field, select **Bank Account**.</span></span>
7. <span data-ttu-id="a0856-116">In the **Bal. Account No.** field, select the bank account to which you want to transfer the funds.</span><span class="sxs-lookup"><span data-stu-id="a0856-116">In the **Bal. Account No.** field, select the bank account to which you want to transfer the funds.</span></span>
8. <span data-ttu-id="a0856-117">Post the journal.</span><span class="sxs-lookup"><span data-stu-id="a0856-117">Post the journal.</span></span>

## <a name="to-post-a-transfer-between-bank-accounts-with-different-currency-codes"></a><span data-ttu-id="a0856-118">To post a transfer between bank accounts with different currency codes</span><span class="sxs-lookup"><span data-stu-id="a0856-118">To post a transfer between bank accounts with different currency codes</span></span>

<span data-ttu-id="a0856-119">To transfer funds between bank accounts that use different currencies, you must post two general journal lines.</span><span class="sxs-lookup"><span data-stu-id="a0856-119">To transfer funds between bank accounts that use different currencies, you must post two general journal lines.</span></span>

1. <span data-ttu-id="a0856-120">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **General Journal**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="a0856-120">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **General Journal**, and then choose the related link.</span></span>
2. <span data-ttu-id="a0856-121">Create two journal lines, and fill in the **Posting Date** and **Document No.** fields.</span><span class="sxs-lookup"><span data-stu-id="a0856-121">Create two journal lines, and fill in the **Posting Date** and **Document No.** fields.</span></span>
3. <span data-ttu-id="a0856-122">On the first journal line, in the **Type** field, select **Bank Account**.</span><span class="sxs-lookup"><span data-stu-id="a0856-122">On the first journal line, in the **Type** field, select **Bank Account**.</span></span>
4. <span data-ttu-id="a0856-123">In the **Account No.** field, select the bank account from which you want to transfer the funds.</span><span class="sxs-lookup"><span data-stu-id="a0856-123">In the **Account No.** field, select the bank account from which you want to transfer the funds.</span></span>
5. <span data-ttu-id="a0856-124">In the **Amount** field, enter the amount in the currency of the bank account with or without a minus sign.</span><span class="sxs-lookup"><span data-stu-id="a0856-124">In the **Amount** field, enter the amount in the currency of the bank account with or without a minus sign.</span></span>

    > [!TIP]
    > <span data-ttu-id="a0856-125">An amount without a sign is a debit, and an amount with a minus sign is a credit.</span><span class="sxs-lookup"><span data-stu-id="a0856-125">An amount without a sign is a debit, and an amount with a minus sign is a credit.</span></span>

    > [!NOTE]
    > <span data-ttu-id="a0856-126">Some companies prefer to transfer between accounts on separate journal lines.</span><span class="sxs-lookup"><span data-stu-id="a0856-126">Some companies prefer to transfer between accounts on separate journal lines.</span></span> <span data-ttu-id="a0856-127">Other companies prefer to post everything on one journal line by using a balancing account.</span><span class="sxs-lookup"><span data-stu-id="a0856-127">Other companies prefer to post everything on one journal line by using a balancing account.</span></span> <span data-ttu-id="a0856-128">Check with your local expert if you're not sure what to do.</span><span class="sxs-lookup"><span data-stu-id="a0856-128">Check with your local expert if you're not sure what to do.</span></span>
    >
    > <span data-ttu-id="a0856-129">If your company prefers to use a balancing account, then set the **Bal. Account Type** field to **Bank Account**, and set the **Bal. Account No.** field to the bank account to which you want to transfer the funds.</span><span class="sxs-lookup"><span data-stu-id="a0856-129">If your company prefers to use a balancing account, then set the **Bal. Account Type** field to **Bank Account**, and set the **Bal. Account No.** field to the bank account to which you want to transfer the funds.</span></span> <span data-ttu-id="a0856-130">Then proceed to step 9 or 10.</span><span class="sxs-lookup"><span data-stu-id="a0856-130">Then proceed to step 9 or 10.</span></span>
    >
    > <span data-ttu-id="a0856-131">If your company prefers to use a separate journal line, then move on to the next step.</span><span class="sxs-lookup"><span data-stu-id="a0856-131">If your company prefers to use a separate journal line, then move on to the next step.</span></span>
6. <span data-ttu-id="a0856-132">On the second journal line, in the **Type** field, select **Bank Account**.</span><span class="sxs-lookup"><span data-stu-id="a0856-132">On the second journal line, in the **Type** field, select **Bank Account**.</span></span>
7. <span data-ttu-id="a0856-133">In the **Account No.** field, select the bank account to which you want to transfer the funds.</span><span class="sxs-lookup"><span data-stu-id="a0856-133">In the **Account No.** field, select the bank account to which you want to transfer the funds.</span></span>
8. <span data-ttu-id="a0856-134">In the **Amount** field, enter the amount in the currency of the bank account with or without a minus sign.</span><span class="sxs-lookup"><span data-stu-id="a0856-134">In the **Amount** field, enter the amount in the currency of the bank account with or without a minus sign.</span></span>

    > [!TIP]
    > <span data-ttu-id="a0856-135">An amount without a sign is a debit, and an amount with a minus sign is a credit.</span><span class="sxs-lookup"><span data-stu-id="a0856-135">An amount without a sign is a debit, and an amount with a minus sign is a credit.</span></span>
9. <span data-ttu-id="a0856-136">If the exchange rates used in the journal are different than the exchange rates on the **Currency Exchange Rates** page, enter a new journal line for the exchange rate gain or loss.</span><span class="sxs-lookup"><span data-stu-id="a0856-136">If the exchange rates used in the journal are different than the exchange rates on the **Currency Exchange Rates** page, enter a new journal line for the exchange rate gain or loss.</span></span>  

    1. <span data-ttu-id="a0856-137">Enter **G/L Account** in the **Account Type** field.</span><span class="sxs-lookup"><span data-stu-id="a0856-137">Enter **G/L Account** in the **Account Type** field.</span></span>  

    2. <span data-ttu-id="a0856-138">Enter the G/L account number for exchange rate gain or loss in the **Account No.** field.</span><span class="sxs-lookup"><span data-stu-id="a0856-138">Enter the G/L account number for exchange rate gain or loss in the **Account No.** field.</span></span>  

    3. <span data-ttu-id="a0856-139">Enter the exchange rate gain or loss in the **Amount** field with or without a minus sign.</span><span class="sxs-lookup"><span data-stu-id="a0856-139">Enter the exchange rate gain or loss in the **Amount** field with or without a minus sign.</span></span>

    > [!TIP]
    > <span data-ttu-id="a0856-140">An amount without a sign is a debit, and an amount with a minus sign is a credit.</span><span class="sxs-lookup"><span data-stu-id="a0856-140">An amount without a sign is a debit, and an amount with a minus sign is a credit.</span></span>
10. <span data-ttu-id="a0856-141">Post the journal.</span><span class="sxs-lookup"><span data-stu-id="a0856-141">Post the journal.</span></span>

## <a name="see-also"></a><span data-ttu-id="a0856-142">See Also</span><span class="sxs-lookup"><span data-stu-id="a0856-142">See Also</span></span>

[<span data-ttu-id="a0856-143">Reconciling Bank Accounts</span><span class="sxs-lookup"><span data-stu-id="a0856-143">Reconciling Bank Accounts</span></span>](bank-manage-bank-accounts.md)  
[<span data-ttu-id="a0856-144">Setting Up Banking</span><span class="sxs-lookup"><span data-stu-id="a0856-144">Setting Up Banking</span></span>](bank-setup-banking.md)  
[<span data-ttu-id="a0856-145">Working with General Journals</span><span class="sxs-lookup"><span data-stu-id="a0856-145">Working with General Journals</span></span>](ui-work-general-journals.md)  
<span data-ttu-id="a0856-146">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="a0856-146">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>


[!INCLUDE[footer-include](includes/footer-banner.md)]