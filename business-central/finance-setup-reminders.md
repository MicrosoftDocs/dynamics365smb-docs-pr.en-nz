---
title: Set Up Reminder Terms and Levels
description: Learn how to set up Business Central so that you can send a reminder to a customer about a payment that is due and add charges, or fees to the payment because of the delay.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: payment due, debt, overdue, fee, charge, reminder
ms.date: 01/21/2021
ms.author: edupont
ms.openlocfilehash: 2d8e233fb1796515314c954d883bda7302fdcd9b
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "5377054"
---
# <a name="set-up-reminder-terms-and-levels"></a><span data-ttu-id="a5781-103">Set Up Reminder Terms and Levels</span><span class="sxs-lookup"><span data-stu-id="a5781-103">Set Up Reminder Terms and Levels</span></span>

<span data-ttu-id="a5781-104">You can use reminders to remind customers about overdue amounts.</span><span class="sxs-lookup"><span data-stu-id="a5781-104">You can use reminders to remind customers about overdue amounts.</span></span> [!INCLUDE [reminder-terms](includes/reminder-terms.md)]

## <a name="reminder-terms"></a><span data-ttu-id="a5781-105">Reminder terms</span><span class="sxs-lookup"><span data-stu-id="a5781-105">Reminder terms</span></span>

<span data-ttu-id="a5781-106">If customers have overdue payments, you must decide when and how to send them a reminder.</span><span class="sxs-lookup"><span data-stu-id="a5781-106">If customers have overdue payments, you must decide when and how to send them a reminder.</span></span> <span data-ttu-id="a5781-107">In addition, you may want to debit their accounts for interest or fees.</span><span class="sxs-lookup"><span data-stu-id="a5781-107">In addition, you may want to debit their accounts for interest or fees.</span></span> <span data-ttu-id="a5781-108">You can set up any number of reminder terms.</span><span class="sxs-lookup"><span data-stu-id="a5781-108">You can set up any number of reminder terms.</span></span>  

> [!NOTE]
> <span data-ttu-id="a5781-109">If you want to calculate interest on overdue payments, you can do so when you create reminders.</span><span class="sxs-lookup"><span data-stu-id="a5781-109">If you want to calculate interest on overdue payments, you can do so when you create reminders.</span></span> <span data-ttu-id="a5781-110">If, however, you just want to calculate interest and inform your customers about this without sending reminders, you should use [finance charge memos](finance-setup-finance-charges.md).</span><span class="sxs-lookup"><span data-stu-id="a5781-110">If, however, you just want to calculate interest and inform your customers about this without sending reminders, you should use [finance charge memos](finance-setup-finance-charges.md).</span></span> <span data-ttu-id="a5781-111">For more information, see [Reminders](receivables-collect-outstanding-balances.md#reminders) or [Finance Charges](receivables-collect-outstanding-balances.md#finance-charges), respectively.</span><span class="sxs-lookup"><span data-stu-id="a5781-111">For more information, see [Reminders](receivables-collect-outstanding-balances.md#reminders) or [Finance Charges](receivables-collect-outstanding-balances.md#finance-charges), respectively.</span></span>

### <a name="to-set-up-reminder-terms"></a><span data-ttu-id="a5781-112">To set up reminder terms</span><span class="sxs-lookup"><span data-stu-id="a5781-112">To set up reminder terms</span></span>

1. <span data-ttu-id="a5781-113">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Reminder Terms**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="a5781-113">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Reminder Terms**, and then choose the related link.</span></span>  
2. <span data-ttu-id="a5781-114">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="a5781-114">Fill in the fields as necessary.</span></span> [!INCLUDE [tooltip-inline-tip_md](includes/tooltip-inline-tip_md.md)]  
3. <span data-ttu-id="a5781-115">To use more than one combination of reminder terms, set up a code for each one.</span><span class="sxs-lookup"><span data-stu-id="a5781-115">To use more than one combination of reminder terms, set up a code for each one.</span></span>

## <a name="reminder-levels"></a><span data-ttu-id="a5781-116">Reminder levels</span><span class="sxs-lookup"><span data-stu-id="a5781-116">Reminder levels</span></span>

<span data-ttu-id="a5781-117">For each reminder terms code, you can define an unlimited number of reminder levels.</span><span class="sxs-lookup"><span data-stu-id="a5781-117">For each reminder terms code, you can define an unlimited number of reminder levels.</span></span> <span data-ttu-id="a5781-118">The first time a reminder is created for a customer, the setting from level 1 is used.</span><span class="sxs-lookup"><span data-stu-id="a5781-118">The first time a reminder is created for a customer, the setting from level 1 is used.</span></span> <span data-ttu-id="a5781-119">When the reminder is issued, the level number is registered on the reminder entries that are created and linked to the individual customer ledger entries.</span><span class="sxs-lookup"><span data-stu-id="a5781-119">When the reminder is issued, the level number is registered on the reminder entries that are created and linked to the individual customer ledger entries.</span></span> <span data-ttu-id="a5781-120">If it is necessary to remind the customer again, all reminder entries linked to open customer ledger entries are checked to locate the highest level number.</span><span class="sxs-lookup"><span data-stu-id="a5781-120">If it is necessary to remind the customer again, all reminder entries linked to open customer ledger entries are checked to locate the highest level number.</span></span> <span data-ttu-id="a5781-121">The conditions from the next level number will then be used for the new reminder.</span><span class="sxs-lookup"><span data-stu-id="a5781-121">The conditions from the next level number will then be used for the new reminder.</span></span>

<span data-ttu-id="a5781-122">If you create more reminders than you have defined levels for, the conditions for the highest level will be used.</span><span class="sxs-lookup"><span data-stu-id="a5781-122">If you create more reminders than you have defined levels for, the conditions for the highest level will be used.</span></span> <span data-ttu-id="a5781-123">You can create as many reminders as are allowed by the **Max. No of Reminders** field in the reminder terms.</span><span class="sxs-lookup"><span data-stu-id="a5781-123">You can create as many reminders as are allowed by the **Max. No of Reminders** field in the reminder terms.</span></span>

### <a name="to-set-up-reminder-levels"></a><span data-ttu-id="a5781-124">To set up reminder levels</span><span class="sxs-lookup"><span data-stu-id="a5781-124">To set up reminder levels</span></span>

1. <span data-ttu-id="a5781-125">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Reminder Terms**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="a5781-125">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Reminder Terms**, and then choose the related link.</span></span>  
2. <span data-ttu-id="a5781-126">On the **Reminder Terms** page, select the line with the terms you want to set up levels for, and then choose **Levels** action.</span><span class="sxs-lookup"><span data-stu-id="a5781-126">On the **Reminder Terms** page, select the line with the terms you want to set up levels for, and then choose **Levels** action.</span></span>  
3. <span data-ttu-id="a5781-127">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="a5781-127">Fill in the fields as necessary.</span></span> [!INCLUDE [tooltip-inline-tip_md](includes/tooltip-inline-tip_md.md)]  

    > [!TIP]
    > <span data-ttu-id="a5781-128">The setting of the **Calculate Interest** field determines if interest will appear on the reminder when the reminder is issued.</span><span class="sxs-lookup"><span data-stu-id="a5781-128">The setting of the **Calculate Interest** field determines if interest will appear on the reminder when the reminder is issued.</span></span> <span data-ttu-id="a5781-129">However, the **Post Interest** field in the **Reminder Terms** page determines if the calculated interest must be posted to G/L and customer accounts.</span><span class="sxs-lookup"><span data-stu-id="a5781-129">However, the **Post Interest** field in the **Reminder Terms** page determines if the calculated interest must be posted to G/L and customer accounts.</span></span>
    >
    > <span data-ttu-id="a5781-130">To indicate that interest should be calculated, choose the **Calculate Interest** field.</span><span class="sxs-lookup"><span data-stu-id="a5781-130">To indicate that interest should be calculated, choose the **Calculate Interest** field.</span></span>

    <span data-ttu-id="a5781-131">Optionally, for each reminder level, specify additional fees in both LCY and in foreign currency.</span><span class="sxs-lookup"><span data-stu-id="a5781-131">Optionally, for each reminder level, specify additional fees in both LCY and in foreign currency.</span></span> <span data-ttu-id="a5781-132">You can define many additional fees in foreign currencies for each code on the **Reminder Levels** page.</span><span class="sxs-lookup"><span data-stu-id="a5781-132">You can define many additional fees in foreign currencies for each code on the **Reminder Levels** page.</span></span>  

    <span data-ttu-id="a5781-133">The additional fees can be calculated in three different ways that are defined by the value of the **Add. Fee Calculation Type** field.</span><span class="sxs-lookup"><span data-stu-id="a5781-133">The additional fees can be calculated in three different ways that are defined by the value of the **Add. Fee Calculation Type** field.</span></span>  

    - <span data-ttu-id="a5781-134">**Fixed**</span><span class="sxs-lookup"><span data-stu-id="a5781-134">**Fixed**</span></span>

        <span data-ttu-id="a5781-135">Fees are calculated based on the values of the **Additional Fee** fields on the line for the reminder level itself.</span><span class="sxs-lookup"><span data-stu-id="a5781-135">Fees are calculated based on the values of the **Additional Fee** fields on the line for the reminder level itself.</span></span>  
    - <span data-ttu-id="a5781-136">**Single Dynamic**</span><span class="sxs-lookup"><span data-stu-id="a5781-136">**Single Dynamic**</span></span>

        <span data-ttu-id="a5781-137">Fees are calculated based on the values of the fields on the relevant line in the **Additional Fee Setup** page for that reminder level.</span><span class="sxs-lookup"><span data-stu-id="a5781-137">Fees are calculated based on the values of the fields on the relevant line in the **Additional Fee Setup** page for that reminder level.</span></span>
    - <span data-ttu-id="a5781-138">**Accumulated Dynamic**</span><span class="sxs-lookup"><span data-stu-id="a5781-138">**Accumulated Dynamic**</span></span>

        <span data-ttu-id="a5781-139">Fees are calculated based on the values of the fields on the combined lines in the **Additional Fee Setup** page for that reminder level.</span><span class="sxs-lookup"><span data-stu-id="a5781-139">Fees are calculated based on the values of the fields on the combined lines in the **Additional Fee Setup** page for that reminder level.</span></span>

4. <span data-ttu-id="a5781-140">Choose the **Currencies** action.</span><span class="sxs-lookup"><span data-stu-id="a5781-140">Choose the **Currencies** action.</span></span>
5. <span data-ttu-id="a5781-141">On the **Currencies for Reminder Levels** page, define for each reminder level code and corresponding reminder level number a currency code and an additional fee.</span><span class="sxs-lookup"><span data-stu-id="a5781-141">On the **Currencies for Reminder Levels** page, define for each reminder level code and corresponding reminder level number a currency code and an additional fee.</span></span>

    > [!NOTE]  
    > <span data-ttu-id="a5781-142">When you create reminders in a foreign currency, the foreign currency conditions that you set up here will be used to create reminders.</span><span class="sxs-lookup"><span data-stu-id="a5781-142">When you create reminders in a foreign currency, the foreign currency conditions that you set up here will be used to create reminders.</span></span> <span data-ttu-id="a5781-143">If there are no foreign currency reminder conditions set up, the LCY reminder conditions that are set up on the **Reminder Levels** page will be used and then converted to the relevant currency.</span><span class="sxs-lookup"><span data-stu-id="a5781-143">If there are no foreign currency reminder conditions set up, the LCY reminder conditions that are set up on the **Reminder Levels** page will be used and then converted to the relevant currency.</span></span>

    <span data-ttu-id="a5781-144">For each reminder level, you can specify text that will be printed before (**Beginning Text**) or after (**Ending Text**) on the entries on the reminder.</span><span class="sxs-lookup"><span data-stu-id="a5781-144">For each reminder level, you can specify text that will be printed before (**Beginning Text**) or after (**Ending Text**) on the entries on the reminder.</span></span>

6. <span data-ttu-id="a5781-145">Choose the **Beginning Text** or **Ending Text** actions respectively, and fill in the **Reminder Text** page.</span><span class="sxs-lookup"><span data-stu-id="a5781-145">Choose the **Beginning Text** or **Ending Text** actions respectively, and fill in the **Reminder Text** page.</span></span>
7. <span data-ttu-id="a5781-146">To automatically insert related values in the resulting reminder text, enter the following placeholders in the **Text** field .</span><span class="sxs-lookup"><span data-stu-id="a5781-146">To automatically insert related values in the resulting reminder text, enter the following placeholders in the **Text** field .</span></span>  

    |<span data-ttu-id="a5781-147">Placeholder</span><span class="sxs-lookup"><span data-stu-id="a5781-147">Placeholder</span></span>|<span data-ttu-id="a5781-148">Value</span><span class="sxs-lookup"><span data-stu-id="a5781-148">Value</span></span>|  
    |-----------------|-----------|  
    |<span data-ttu-id="a5781-149">%1</span><span class="sxs-lookup"><span data-stu-id="a5781-149">%1</span></span>|<span data-ttu-id="a5781-150">Content of the **Document Date** field on the reminder header</span><span class="sxs-lookup"><span data-stu-id="a5781-150">Content of the **Document Date** field on the reminder header</span></span>|  
    |<span data-ttu-id="a5781-151">%2</span><span class="sxs-lookup"><span data-stu-id="a5781-151">%2</span></span>|<span data-ttu-id="a5781-152">Content of the **Due Date** field on the reminder header</span><span class="sxs-lookup"><span data-stu-id="a5781-152">Content of the **Due Date** field on the reminder header</span></span>|  
    |<span data-ttu-id="a5781-153">%3</span><span class="sxs-lookup"><span data-stu-id="a5781-153">%3</span></span>|<span data-ttu-id="a5781-154">Content of the **Interest Rate** field on the related finance charge terms</span><span class="sxs-lookup"><span data-stu-id="a5781-154">Content of the **Interest Rate** field on the related finance charge terms</span></span>|  
    |<span data-ttu-id="a5781-155">%4</span><span class="sxs-lookup"><span data-stu-id="a5781-155">%4</span></span>|<span data-ttu-id="a5781-156">Content of the **Remaining Amount** field on the reminder header</span><span class="sxs-lookup"><span data-stu-id="a5781-156">Content of the **Remaining Amount** field on the reminder header</span></span>|  
    |<span data-ttu-id="a5781-157">%5</span><span class="sxs-lookup"><span data-stu-id="a5781-157">%5</span></span>|<span data-ttu-id="a5781-158">Content of the **Interest Amount** field on the reminder header</span><span class="sxs-lookup"><span data-stu-id="a5781-158">Content of the **Interest Amount** field on the reminder header</span></span>|  
    |<span data-ttu-id="a5781-159">%6</span><span class="sxs-lookup"><span data-stu-id="a5781-159">%6</span></span>|<span data-ttu-id="a5781-160">Content of the **Additional Fee** field on the reminder header</span><span class="sxs-lookup"><span data-stu-id="a5781-160">Content of the **Additional Fee** field on the reminder header</span></span>|  
    |<span data-ttu-id="a5781-161">%7</span><span class="sxs-lookup"><span data-stu-id="a5781-161">%7</span></span>|<span data-ttu-id="a5781-162">The total amount of the reminder</span><span class="sxs-lookup"><span data-stu-id="a5781-162">The total amount of the reminder</span></span>|  
    |<span data-ttu-id="a5781-163">%8</span><span class="sxs-lookup"><span data-stu-id="a5781-163">%8</span></span>|<span data-ttu-id="a5781-164">Content of the **Reminder Level** field on the reminder header</span><span class="sxs-lookup"><span data-stu-id="a5781-164">Content of the **Reminder Level** field on the reminder header</span></span>|  
    |<span data-ttu-id="a5781-165">%9</span><span class="sxs-lookup"><span data-stu-id="a5781-165">%9</span></span>|<span data-ttu-id="a5781-166">Content of the **Currency Code** field on the reminder header</span><span class="sxs-lookup"><span data-stu-id="a5781-166">Content of the **Currency Code** field on the reminder header</span></span>|  
    |<span data-ttu-id="a5781-167">%10</span><span class="sxs-lookup"><span data-stu-id="a5781-167">%10</span></span>|<span data-ttu-id="a5781-168">Content of the **Posting Date** field on the reminder header</span><span class="sxs-lookup"><span data-stu-id="a5781-168">Content of the **Posting Date** field on the reminder header</span></span>|  
    |<span data-ttu-id="a5781-169">%11</span><span class="sxs-lookup"><span data-stu-id="a5781-169">%11</span></span>|<span data-ttu-id="a5781-170">The company name</span><span class="sxs-lookup"><span data-stu-id="a5781-170">The company name</span></span>|  
    |<span data-ttu-id="a5781-171">%12</span><span class="sxs-lookup"><span data-stu-id="a5781-171">%12</span></span>|<span data-ttu-id="a5781-172">Content of the **Add. Fee per Line** field on the reminder header</span><span class="sxs-lookup"><span data-stu-id="a5781-172">Content of the **Add. Fee per Line** field on the reminder header</span></span>|  

    <span data-ttu-id="a5781-173">For example, if you write **You owe %9 %7 due on %2.**, then the resulting reminder will contain the following text: **You owe NZD 1.200,50 due on 02-02-2014.**.</span><span class="sxs-lookup"><span data-stu-id="a5781-173">For example, if you write **You owe %9 %7 due on %2.**, then the resulting reminder will contain the following text: **You owe USD 1.200,50 due on 02-02-2014.**.</span></span>

    > [!NOTE]
    > <span data-ttu-id="a5781-174">The due date is calculated according to the date formula that you enter.</span><span class="sxs-lookup"><span data-stu-id="a5781-174">The due date is calculated according to the date formula that you enter.</span></span> <span data-ttu-id="a5781-175">For more information, see [Using Date Formulas](ui-enter-date-ranges.md#using-date-formulas).</span><span class="sxs-lookup"><span data-stu-id="a5781-175">For more information, see [Using Date Formulas](ui-enter-date-ranges.md#using-date-formulas).</span></span>

<span data-ttu-id="a5781-176">After you have set up the reminder terms, with additional levels and text, enter one of the codes on each of the customer cards.</span><span class="sxs-lookup"><span data-stu-id="a5781-176">After you have set up the reminder terms, with additional levels and text, enter one of the codes on each of the customer cards.</span></span> <span data-ttu-id="a5781-177">For more information, see [Register New Customers](sales-how-register-new-customers.md).</span><span class="sxs-lookup"><span data-stu-id="a5781-177">For more information, see [Register New Customers](sales-how-register-new-customers.md).</span></span>  

## <a name="see-also"></a><span data-ttu-id="a5781-178">See also</span><span class="sxs-lookup"><span data-stu-id="a5781-178">See also</span></span>

[<span data-ttu-id="a5781-179">Collect Outstanding Balances</span><span class="sxs-lookup"><span data-stu-id="a5781-179">Collect Outstanding Balances</span></span>](receivables-collect-outstanding-balances.md)  
[<span data-ttu-id="a5781-180">Set Up Finance Charge Terms</span><span class="sxs-lookup"><span data-stu-id="a5781-180">Set Up Finance Charge Terms</span></span>](finance-setup-finance-charges.md)  
[<span data-ttu-id="a5781-181">Setting Up Finance</span><span class="sxs-lookup"><span data-stu-id="a5781-181">Setting Up Finance</span></span>](finance-setup-finance.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]