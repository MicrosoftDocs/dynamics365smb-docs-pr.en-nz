---
title: Set Up Finance Charge Terms
description: Learn how to set up Business Central so that you can inform customers of added charges by sending finance charge memos.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: payment due, debt, overdue, fee, charge
ms.date: 12/03/2020
ms.author: edupont
ms.openlocfilehash: dad02adfb6cc0a0ebb6d950b67f2e092b3313c59
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "5377103"
---
# <a name="set-up-finance-charge-terms"></a><span data-ttu-id="0e4aa-103">Set Up Finance Charge Terms</span><span class="sxs-lookup"><span data-stu-id="0e4aa-103">Set Up Finance Charge Terms</span></span>

<span data-ttu-id="0e4aa-104">When a customer does not pay by the due date, you can have finance charges calculated automatically and add them to the overdue amounts on the customer's account.</span><span class="sxs-lookup"><span data-stu-id="0e4aa-104">When a customer does not pay by the due date, you can have finance charges calculated automatically and add them to the overdue amounts on the customer's account.</span></span> <span data-ttu-id="0e4aa-105">You can inform customers of the added charges by sending finance charge memos.</span><span class="sxs-lookup"><span data-stu-id="0e4aa-105">You can inform customers of the added charges by sending finance charge memos.</span></span> <span data-ttu-id="0e4aa-106">But first, you must set up a code that represents each finance charge calculation.</span><span class="sxs-lookup"><span data-stu-id="0e4aa-106">But first, you must set up a code that represents each finance charge calculation.</span></span> <span data-ttu-id="0e4aa-107">Then you can enter this code in the Fin. Charge Terms Code field on customer cards.</span><span class="sxs-lookup"><span data-stu-id="0e4aa-107">Then you can enter this code in the Fin. Charge Terms Code field on customer cards.</span></span>  

## <a name="finance-charge-terms"></a><span data-ttu-id="0e4aa-108">Finance charge terms</span><span class="sxs-lookup"><span data-stu-id="0e4aa-108">Finance charge terms</span></span>

<span data-ttu-id="0e4aa-109">You must set up finance charge terms for each finance charge calculation, and then assign the terms to the customer in the **Fin. Charge Terms Code** field on the **Customer** page.</span><span class="sxs-lookup"><span data-stu-id="0e4aa-109">You must set up finance charge terms for each finance charge calculation, and then assign the terms to the customer in the **Fin. Charge Terms Code** field on the **Customer** page.</span></span>

<span data-ttu-id="0e4aa-110">Finance charges can be calculated using either the average daily balance or the balance due methods.</span><span class="sxs-lookup"><span data-stu-id="0e4aa-110">Finance charges can be calculated using either the average daily balance or the balance due methods.</span></span>

* <span data-ttu-id="0e4aa-111">Average daily balance</span><span class="sxs-lookup"><span data-stu-id="0e4aa-111">Average daily balance</span></span>  
  
  <span data-ttu-id="0e4aa-112">The number of days the payment is overdue is taken into account:</span><span class="sxs-lookup"><span data-stu-id="0e4aa-112">The number of days the payment is overdue is taken into account:</span></span>  
  <span data-ttu-id="0e4aa-113">*Average Daily Balance method* - *Finance Charge* = *Overdue Amount* x *(Days Overdue / Interest Period)* x *(Interest Rate/100)*</span><span class="sxs-lookup"><span data-stu-id="0e4aa-113">*Average Daily Balance method* - *Finance Charge* = *Overdue Amount* x *(Days Overdue / Interest Period)* x *(Interest Rate/100)*</span></span>

* <span data-ttu-id="0e4aa-114">Balance due</span><span class="sxs-lookup"><span data-stu-id="0e4aa-114">Balance due</span></span>  
  
  <span data-ttu-id="0e4aa-115">The finance charge is a percentage of the overdue amount:</span><span class="sxs-lookup"><span data-stu-id="0e4aa-115">The finance charge is a percentage of the overdue amount:</span></span>  
  <span data-ttu-id="0e4aa-116">*Balance Due method* - *Finance Charge* = *Overdue Amount* x *(Interest Rate / 100)*</span><span class="sxs-lookup"><span data-stu-id="0e4aa-116">*Balance Due method* - *Finance Charge* = *Overdue Amount* x *(Interest Rate / 100)*</span></span>

<span data-ttu-id="0e4aa-117">Additionally, each term in the Finance Charge Terms table is linked to a subtable, the Finance Charge Text table.</span><span class="sxs-lookup"><span data-stu-id="0e4aa-117">Additionally, each term in the Finance Charge Terms table is linked to a subtable, the Finance Charge Text table.</span></span> <span data-ttu-id="0e4aa-118">For each set of finance charge terms, you can define a beginning and/or an ending text to include on the finance charge memo.</span><span class="sxs-lookup"><span data-stu-id="0e4aa-118">For each set of finance charge terms, you can define a beginning and/or an ending text to include on the finance charge memo.</span></span>

### <a name="to-set-up-finance-charge-terms"></a><span data-ttu-id="0e4aa-119">To set up finance charge terms</span><span class="sxs-lookup"><span data-stu-id="0e4aa-119">To set up finance charge terms</span></span>

1. <span data-ttu-id="0e4aa-120">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Finance Charge Terms**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="0e4aa-120">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Finance Charge Terms**, and then choose the related link.</span></span>  
2. <span data-ttu-id="0e4aa-121">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="0e4aa-121">Fill in the fields as necessary.</span></span>
3. <span data-ttu-id="0e4aa-122">To use more than one combination of finance charge terms, set up a code for each one.</span><span class="sxs-lookup"><span data-stu-id="0e4aa-122">To use more than one combination of finance charge terms, set up a code for each one.</span></span>

    <span data-ttu-id="0e4aa-123">For each finance charge term, you can specify individual conditions that can include additional fees in both LCY and in foreign currency.</span><span class="sxs-lookup"><span data-stu-id="0e4aa-123">For each finance charge term, you can specify individual conditions that can include additional fees in both LCY and in foreign currency.</span></span> <span data-ttu-id="0e4aa-124">You can define additional fees in foreign currencies for each term on the **Finance Charge Terms** page.</span><span class="sxs-lookup"><span data-stu-id="0e4aa-124">You can define additional fees in foreign currencies for each term on the **Finance Charge Terms** page.</span></span>
4. <span data-ttu-id="0e4aa-125">Choose the **Currencies** action.</span><span class="sxs-lookup"><span data-stu-id="0e4aa-125">Choose the **Currencies** action.</span></span>
5. <span data-ttu-id="0e4aa-126">On the **Currencies for Fin. Chrg. Terms** page, define for each term a currency code and an additional fee.</span><span class="sxs-lookup"><span data-stu-id="0e4aa-126">On the **Currencies for Fin. Chrg. Terms** page, define for each term a currency code and an additional fee.</span></span>

    > [!NOTE]  
    > <span data-ttu-id="0e4aa-127">When you create finance charges in a foreign currency, the foreign currency conditions that you set up here will be used to create finance charge memos.</span><span class="sxs-lookup"><span data-stu-id="0e4aa-127">When you create finance charges in a foreign currency, the foreign currency conditions that you set up here will be used to create finance charge memos.</span></span> <span data-ttu-id="0e4aa-128">If there are no foreign currency finance charge conditions set up, the LCY finance charge conditions specified on the **Finance Charge Terms** page will be used and then converted to the relevant currency.</span><span class="sxs-lookup"><span data-stu-id="0e4aa-128">If there are no foreign currency finance charge conditions set up, the LCY finance charge conditions specified on the **Finance Charge Terms** page will be used and then converted to the relevant currency.</span></span>

    <span data-ttu-id="0e4aa-129">For each finance charge term, you can specify text that will be printed before (**Beginning Text**) or after (**Ending Text**) on the entries on the finance charge memo.</span><span class="sxs-lookup"><span data-stu-id="0e4aa-129">For each finance charge term, you can specify text that will be printed before (**Beginning Text**) or after (**Ending Text**) on the entries on the finance charge memo.</span></span>  
6. <span data-ttu-id="0e4aa-130">Choose the **Beginning Text** or **Ending Text** actions respectively, and fill on the **Finance Charge Text** page.</span><span class="sxs-lookup"><span data-stu-id="0e4aa-130">Choose the **Beginning Text** or **Ending Text** actions respectively, and fill on the **Finance Charge Text** page.</span></span>
7. <span data-ttu-id="0e4aa-131">To automatically insert related values in the resulting finance charge text, enter the following placeholders in the **Text** field.</span><span class="sxs-lookup"><span data-stu-id="0e4aa-131">To automatically insert related values in the resulting finance charge text, enter the following placeholders in the **Text** field.</span></span>

|<span data-ttu-id="0e4aa-132">Placeholder</span><span class="sxs-lookup"><span data-stu-id="0e4aa-132">Placeholder</span></span>|<span data-ttu-id="0e4aa-133">Value</span><span class="sxs-lookup"><span data-stu-id="0e4aa-133">Value</span></span>|  
|-----------------|-----------|  
|<span data-ttu-id="0e4aa-134">%1</span><span class="sxs-lookup"><span data-stu-id="0e4aa-134">%1</span></span>|<span data-ttu-id="0e4aa-135">Content of the **Document Date** field on the finance charge memo header</span><span class="sxs-lookup"><span data-stu-id="0e4aa-135">Content of the **Document Date** field on the finance charge memo header</span></span>|  
|<span data-ttu-id="0e4aa-136">%2</span><span class="sxs-lookup"><span data-stu-id="0e4aa-136">%2</span></span>|<span data-ttu-id="0e4aa-137">Content of the **Due Date** field on the finance charge memo header</span><span class="sxs-lookup"><span data-stu-id="0e4aa-137">Content of the **Due Date** field on the finance charge memo header</span></span>|  
|<span data-ttu-id="0e4aa-138">%3</span><span class="sxs-lookup"><span data-stu-id="0e4aa-138">%3</span></span>|<span data-ttu-id="0e4aa-139">Content of the **Interest Rate** field on the related finance charge terms</span><span class="sxs-lookup"><span data-stu-id="0e4aa-139">Content of the **Interest Rate** field on the related finance charge terms</span></span>|  
|<span data-ttu-id="0e4aa-140">%4</span><span class="sxs-lookup"><span data-stu-id="0e4aa-140">%4</span></span>|<span data-ttu-id="0e4aa-141">Content of the **Remaining Amount** field on the finance charge memo header</span><span class="sxs-lookup"><span data-stu-id="0e4aa-141">Content of the **Remaining Amount** field on the finance charge memo header</span></span>|  
|<span data-ttu-id="0e4aa-142">%5</span><span class="sxs-lookup"><span data-stu-id="0e4aa-142">%5</span></span>|<span data-ttu-id="0e4aa-143">Content of the **Interest Amount** field on the finance charge memo header</span><span class="sxs-lookup"><span data-stu-id="0e4aa-143">Content of the **Interest Amount** field on the finance charge memo header</span></span>|  
|<span data-ttu-id="0e4aa-144">%6</span><span class="sxs-lookup"><span data-stu-id="0e4aa-144">%6</span></span>|<span data-ttu-id="0e4aa-145">Content of the **Additional Fee** field on the finance charge memo header</span><span class="sxs-lookup"><span data-stu-id="0e4aa-145">Content of the **Additional Fee** field on the finance charge memo header</span></span>|  
|<span data-ttu-id="0e4aa-146">%7</span><span class="sxs-lookup"><span data-stu-id="0e4aa-146">%7</span></span>|<span data-ttu-id="0e4aa-147">The total amount of the reminder</span><span class="sxs-lookup"><span data-stu-id="0e4aa-147">The total amount of the reminder</span></span>|  
|<span data-ttu-id="0e4aa-148">%8</span><span class="sxs-lookup"><span data-stu-id="0e4aa-148">%8</span></span>|<span data-ttu-id="0e4aa-149">Content of the **Currency Code** field on the finance charge memo header</span><span class="sxs-lookup"><span data-stu-id="0e4aa-149">Content of the **Currency Code** field on the finance charge memo header</span></span>|  
|<span data-ttu-id="0e4aa-150">%9</span><span class="sxs-lookup"><span data-stu-id="0e4aa-150">%9</span></span>|<span data-ttu-id="0e4aa-151">Content of the **Posting Date** field on the finance charge memo header</span><span class="sxs-lookup"><span data-stu-id="0e4aa-151">Content of the **Posting Date** field on the finance charge memo header</span></span>|  

## <a name="see-also"></a><span data-ttu-id="0e4aa-152">See also</span><span class="sxs-lookup"><span data-stu-id="0e4aa-152">See also</span></span>

[<span data-ttu-id="0e4aa-153">Collect Outstanding Balances</span><span class="sxs-lookup"><span data-stu-id="0e4aa-153">Collect Outstanding Balances</span></span>](receivables-collect-outstanding-balances.md)  
[<span data-ttu-id="0e4aa-154">Set Up Reminder Terms and Levels</span><span class="sxs-lookup"><span data-stu-id="0e4aa-154">Set Up Reminder Terms and Levels</span></span>](finance-setup-reminders.md)  
[<span data-ttu-id="0e4aa-155">Setting Up Finance</span><span class="sxs-lookup"><span data-stu-id="0e4aa-155">Setting Up Finance</span></span>](finance-setup-finance.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]