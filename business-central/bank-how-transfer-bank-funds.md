---
title: Transfer Bank Funds| Microsoft Docs
description: You can transfer amounts from one bank account to another, including different currencies, by posting the transaction in the general journal.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: bank account transfer, multiple currencies
ms.date: 04/01/2020
ms.author: edupont
ms.openlocfilehash: 0183f9a8184b67cb10155b3aecfd7ab4a121eb6c
ms.sourcegitcommit: a80afd4e5075018716efad76d82a54e158f1392d
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 09/09/2020
ms.locfileid: "3786562"
---
# <a name="transfer-bank-funds"></a><span data-ttu-id="8ae23-103">Transfer Bank Funds</span><span class="sxs-lookup"><span data-stu-id="8ae23-103">Transfer Bank Funds</span></span>
<span data-ttu-id="8ae23-104">You may sometimes need to transfer an amount from one bank account in [!INCLUDE[d365fin](includes/d365fin_md.md)] to another.</span><span class="sxs-lookup"><span data-stu-id="8ae23-104">You may sometimes need to transfer an amount from one bank account in [!INCLUDE[d365fin](includes/d365fin_md.md)] to another.</span></span> <span data-ttu-id="8ae23-105">To do this, you must post the a transaction on the **General Journal** page.</span><span class="sxs-lookup"><span data-stu-id="8ae23-105">To do this, you must post the a transaction on the **General Journal** page.</span></span> <span data-ttu-id="8ae23-106">The task varies depending on whether the bank accounts use the same currency or different currencies.</span><span class="sxs-lookup"><span data-stu-id="8ae23-106">The task varies depending on whether the bank accounts use the same currency or different currencies.</span></span>

## <a name="to-post-a-transfer-between-bank-accounts-with-the-same-currency-code"></a><span data-ttu-id="8ae23-107">To post a transfer between bank accounts with the same currency code</span><span class="sxs-lookup"><span data-stu-id="8ae23-107">To post a transfer between bank accounts with the same currency code</span></span>
1. <span data-ttu-id="8ae23-108">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **General Journal**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="8ae23-108">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **General Journal**, and then choose the related link.</span></span>
2. <span data-ttu-id="8ae23-109">On a journal line, fill in the **Posting Date** and **Document No.** fields.</span><span class="sxs-lookup"><span data-stu-id="8ae23-109">On a journal line, fill in the **Posting Date** and **Document No.** fields.</span></span>
3. <span data-ttu-id="8ae23-110">In the **Account Type** field, select **Bank Account**.</span><span class="sxs-lookup"><span data-stu-id="8ae23-110">In the **Account Type** field, select **Bank Account**.</span></span>
4. <span data-ttu-id="8ae23-111">In the **Account No.** field, select the bank from which you want to transfer the funds.</span><span class="sxs-lookup"><span data-stu-id="8ae23-111">In the **Account No.** field, select the bank from which you want to transfer the funds.</span></span>
5. <span data-ttu-id="8ae23-112">In the **Amount** field, enter the amount to be transferred.</span><span class="sxs-lookup"><span data-stu-id="8ae23-112">In the **Amount** field, enter the amount to be transferred.</span></span>
6. <span data-ttu-id="8ae23-113">Choose the **Show More Columns** action to view all available fields.</span><span class="sxs-lookup"><span data-stu-id="8ae23-113">Choose the **Show More Columns** action to view all available fields.</span></span>
7. <span data-ttu-id="8ae23-114">In the **Bal. Account Type** field, select **Bank Account**.</span><span class="sxs-lookup"><span data-stu-id="8ae23-114">In the **Bal. Account Type** field, select **Bank Account**.</span></span>
8. <span data-ttu-id="8ae23-115">In the **Bal. Account No.** field, select the bank account to which you want to transfer the funds.</span><span class="sxs-lookup"><span data-stu-id="8ae23-115">In the **Bal. Account No.** field, select the bank account to which you want to transfer the funds.</span></span>
9. <span data-ttu-id="8ae23-116">Post the journal.</span><span class="sxs-lookup"><span data-stu-id="8ae23-116">Post the journal.</span></span>

## <a name="to-post-a-transfer-between-bank-accounts-with-different-currency-codes"></a><span data-ttu-id="8ae23-117">To post a transfer between bank accounts with different currency codes</span><span class="sxs-lookup"><span data-stu-id="8ae23-117">To post a transfer between bank accounts with different currency codes</span></span>
<span data-ttu-id="8ae23-118">To transfer funds between bank accounts that use different currencies, you must post two general journal lines.</span><span class="sxs-lookup"><span data-stu-id="8ae23-118">To transfer funds between bank accounts that use different currencies, you must post two general journal lines.</span></span>

1. <span data-ttu-id="8ae23-119">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **General Journal**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="8ae23-119">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **General Journal**, and then choose the related link.</span></span>
2. <span data-ttu-id="8ae23-120">Create two journal lines, and fill in the **Posting Date** and **Document No.** fields.</span><span class="sxs-lookup"><span data-stu-id="8ae23-120">Create two journal lines, and fill in the **Posting Date** and **Document No.** fields.</span></span>
3. <span data-ttu-id="8ae23-121">On the first journal line, in the **Type** field, select **Bank Account**.</span><span class="sxs-lookup"><span data-stu-id="8ae23-121">On the first journal line, in the **Type** field, select **Bank Account**.</span></span>
4. <span data-ttu-id="8ae23-122">In the **Account No.** field, select the bank account from which you want to transfer the funds.</span><span class="sxs-lookup"><span data-stu-id="8ae23-122">In the **Account No.** field, select the bank account from which you want to transfer the funds.</span></span>
5. <span data-ttu-id="8ae23-123">In the **Amount** field, enter the amount in the currency of the bank account.</span><span class="sxs-lookup"><span data-stu-id="8ae23-123">In the **Amount** field, enter the amount in the currency of the bank account.</span></span> <span data-ttu-id="8ae23-124">Enter credit amounts with a minus sign.</span><span class="sxs-lookup"><span data-stu-id="8ae23-124">Enter credit amounts with a minus sign.</span></span> <span data-ttu-id="8ae23-125">Enter debit amounts without a minus sign.</span><span class="sxs-lookup"><span data-stu-id="8ae23-125">Enter debit amounts without a minus sign.</span></span>
6. <span data-ttu-id="8ae23-126">In the **Bal. Account Type** field, select **Bank Account**.</span><span class="sxs-lookup"><span data-stu-id="8ae23-126">In the **Bal. Account Type** field, select **Bank Account**.</span></span>
7. <span data-ttu-id="8ae23-127">In the **Bal. Account No.** field, select the bank account to which you want to transfer the funds.</span><span class="sxs-lookup"><span data-stu-id="8ae23-127">In the **Bal. Account No.** field, select the bank account to which you want to transfer the funds.</span></span>
8. <span data-ttu-id="8ae23-128">On the second journal line, in the **Type** field, select **Bank Account**.</span><span class="sxs-lookup"><span data-stu-id="8ae23-128">On the second journal line, in the **Type** field, select **Bank Account**.</span></span>
9. <span data-ttu-id="8ae23-129">In the **Account No.** field, select the bank account to which you want to transfer the funds.</span><span class="sxs-lookup"><span data-stu-id="8ae23-129">In the **Account No.** field, select the bank account to which you want to transfer the funds.</span></span>
10. <span data-ttu-id="8ae23-130">In the **Amount** field, enter the amount in the currency of the bank account.</span><span class="sxs-lookup"><span data-stu-id="8ae23-130">In the **Amount** field, enter the amount in the currency of the bank account.</span></span> <span data-ttu-id="8ae23-131">Enter credit amounts with a minus sign.</span><span class="sxs-lookup"><span data-stu-id="8ae23-131">Enter credit amounts with a minus sign.</span></span> <span data-ttu-id="8ae23-132">Enter debit amounts without a minus sign.</span><span class="sxs-lookup"><span data-stu-id="8ae23-132">Enter debit amounts without a minus sign.</span></span>
11. <span data-ttu-id="8ae23-133">In the **Bal. Account Type** field, select **Bank Account**.</span><span class="sxs-lookup"><span data-stu-id="8ae23-133">In the **Bal. Account Type** field, select **Bank Account**.</span></span>  
12. <span data-ttu-id="8ae23-134">In the **Bal. Account No.** field, select the bank account from which you want to transfer the funds.</span><span class="sxs-lookup"><span data-stu-id="8ae23-134">In the **Bal. Account No.** field, select the bank account from which you want to transfer the funds.</span></span>

    > [!NOTE]  
    > <span data-ttu-id="8ae23-135">If the exchange rates used in the journal are different than the exchange rates on the **Currency Exchange Rates** page, enter a third line for the exchange rate gain or loss.</span><span class="sxs-lookup"><span data-stu-id="8ae23-135">If the exchange rates used in the journal are different than the exchange rates on the **Currency Exchange Rates** page, enter a third line for the exchange rate gain or loss.</span></span> <span data-ttu-id="8ae23-136">Enter **G/L Account** in the **Account Type** field.</span><span class="sxs-lookup"><span data-stu-id="8ae23-136">Enter **G/L Account** in the **Account Type** field.</span></span> <span data-ttu-id="8ae23-137">Enter the G/L account number for exchange rate gain or loss in the **Account No.** field.</span><span class="sxs-lookup"><span data-stu-id="8ae23-137">Enter the G/L account number for exchange rate gain or loss in the **Account No.** field.</span></span> <span data-ttu-id="8ae23-138">Enter the exchange rate gain or loss in the **Amount** field with or without a minus sign for credits and debits respectively.</span><span class="sxs-lookup"><span data-stu-id="8ae23-138">Enter the exchange rate gain or loss in the **Amount** field with or without a minus sign for credits and debits respectively.</span></span>
13. <span data-ttu-id="8ae23-139">Post the journal.</span><span class="sxs-lookup"><span data-stu-id="8ae23-139">Post the journal.</span></span>

## <a name="see-also"></a><span data-ttu-id="8ae23-140">See Also</span><span class="sxs-lookup"><span data-stu-id="8ae23-140">See Also</span></span>
[<span data-ttu-id="8ae23-141">Reconciling Bank Accounts</span><span class="sxs-lookup"><span data-stu-id="8ae23-141">Reconciling Bank Accounts</span></span>](bank-manage-bank-accounts.md)  
[<span data-ttu-id="8ae23-142">Setting Up Banking</span><span class="sxs-lookup"><span data-stu-id="8ae23-142">Setting Up Banking</span></span>](bank-setup-banking.md)  
[<span data-ttu-id="8ae23-143">Working with General Journals</span><span class="sxs-lookup"><span data-stu-id="8ae23-143">Working with General Journals</span></span>](ui-work-general-journals.md)  
<span data-ttu-id="8ae23-144">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="8ae23-144">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
