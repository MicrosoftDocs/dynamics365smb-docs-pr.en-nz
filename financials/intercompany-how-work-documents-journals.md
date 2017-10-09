---
title: Post Intercompany Documents and Journals| Microsoft Docs
description: Use intercompany documents to post transactions with your intercompany partners.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: IC, group, consolidation, affiliate, subsidiary
ms.date: 06/21/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: eea34afbee429d14ab150894729cb4ea3843bb2b
ms.openlocfilehash: eeb070e1431d55248a762b444c2298281b0a5101
ms.contentlocale: en-nz
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-work-with-intercompany-documents-and-journals"></a><span data-ttu-id="d224b-103">How to: Work with Intercompany Documents and Journals</span><span class="sxs-lookup"><span data-stu-id="d224b-103">How to: Work with Intercompany Documents and Journals</span></span>
<span data-ttu-id="d224b-104">You use intercompany documents or journals to post transactions with your intercompany partners.</span><span class="sxs-lookup"><span data-stu-id="d224b-104">You use intercompany documents or journals to post transactions with your intercompany partners.</span></span> <span data-ttu-id="d224b-105">When you post an intercompany document or journal line in your company, a corresponding document or journal line is created in your intercompany outbox that you can transfer to your partner.</span><span class="sxs-lookup"><span data-stu-id="d224b-105">When you post an intercompany document or journal line in your company, a corresponding document or journal line is created in your intercompany outbox that you can transfer to your partner.</span></span> <span data-ttu-id="d224b-106">Your partner can then post the corresponding transaction in their company, without having to re-enter the data.</span><span class="sxs-lookup"><span data-stu-id="d224b-106">Your partner can then post the corresponding transaction in their company, without having to re-enter the data.</span></span>

<span data-ttu-id="d224b-107">For sales and purchase documents, the intercompany partner code on the involved customer or vendor ensures that all orders and invoices generated pertaining to transactions with these companies will produce corresponding documents in the partner company, resulting in correct balancing of the accounts.</span><span class="sxs-lookup"><span data-stu-id="d224b-107">For sales and purchase documents, the intercompany partner code on the involved customer or vendor ensures that all orders and invoices generated pertaining to transactions with these companies will produce corresponding documents in the partner company, resulting in correct balancing of the accounts.</span></span>

<span data-ttu-id="d224b-108">For intercompany general journal lines, you do not need to specify the accounts for an individual set of books, but simply give the identification of the partner company.</span><span class="sxs-lookup"><span data-stu-id="d224b-108">For intercompany general journal lines, you do not need to specify the accounts for an individual set of books, but simply give the identification of the partner company.</span></span> <span data-ttu-id="d224b-109">Corresponding intercompany general journal lines are then created in the partner company that result in the balancing of the books of both companies involved in a transaction.</span><span class="sxs-lookup"><span data-stu-id="d224b-109">Corresponding intercompany general journal lines are then created in the partner company that result in the balancing of the books of both companies involved in a transaction.</span></span>

## <a name="to-fill-in-and-send-an-intercompany-sales-order"></a><span data-ttu-id="d224b-110">To fill in and send an intercompany sales order</span><span class="sxs-lookup"><span data-stu-id="d224b-110">To fill in and send an intercompany sales order</span></span>
<span data-ttu-id="d224b-111">You can send sales and purchase orders and return orders before posting.</span><span class="sxs-lookup"><span data-stu-id="d224b-111">You can send sales and purchase orders and return orders before posting.</span></span> <span data-ttu-id="d224b-112">Invoices and credit memos cannot be sent until they are posted.</span><span class="sxs-lookup"><span data-stu-id="d224b-112">Invoices and credit memos cannot be sent until they are posted.</span></span>

<span data-ttu-id="d224b-113">The following procedure describes how to fill in and send an intercompany sales order.</span><span class="sxs-lookup"><span data-stu-id="d224b-113">The following procedure describes how to fill in and send an intercompany sales order.</span></span> <span data-ttu-id="d224b-114">The same steps apply to intercompany purchase orders and return orders, and to posted intercompany invoices and credit memos.</span><span class="sxs-lookup"><span data-stu-id="d224b-114">The same steps apply to intercompany purchase orders and return orders, and to posted intercompany invoices and credit memos.</span></span>  

1. <span data-ttu-id="d224b-115">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sales Orders**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="d224b-115">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sales Orders**, and then choose the related link.</span></span>  
2. <span data-ttu-id="d224b-116">Choose **New** to create a new sales order.</span><span class="sxs-lookup"><span data-stu-id="d224b-116">Choose **New** to create a new sales order.</span></span> <span data-ttu-id="d224b-117">For more information, see [How to: Sell Products](sales-how-sell-products.md).</span><span class="sxs-lookup"><span data-stu-id="d224b-117">For more information, see [How to: Sell Products](sales-how-sell-products.md).</span></span>  
3. <span data-ttu-id="d224b-118">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="d224b-118">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4. <span data-ttu-id="d224b-119">Make sure the customer is an intercompany partner.</span><span class="sxs-lookup"><span data-stu-id="d224b-119">Make sure the customer is an intercompany partner.</span></span>
5. <span data-ttu-id="d224b-120">To send the sales order before you post it, choose the **Send IC Sales Order** action.</span><span class="sxs-lookup"><span data-stu-id="d224b-120">To send the sales order before you post it, choose the **Send IC Sales Order** action.</span></span>

> [!NOTE]
> <span data-ttu-id="d224b-121">If you do perform step 4, then the sales order will be moved to your intercompany outbox where you can send it later.</span><span class="sxs-lookup"><span data-stu-id="d224b-121">If you do perform step 4, then the sales order will be moved to your intercompany outbox where you can send it later.</span></span> <span data-ttu-id="d224b-122">For more information, see [How to: Manage the Intercompany Inbox and Outbox](intercompany-how-manage-intercompany-inbox.md).</span><span class="sxs-lookup"><span data-stu-id="d224b-122">For more information, see [How to: Manage the Intercompany Inbox and Outbox](intercompany-how-manage-intercompany-inbox.md).</span></span>

## <a name="to-fill-in-and-post-an-intercompany-journal"></a><span data-ttu-id="d224b-123">To fill in and post an intercompany journal</span><span class="sxs-lookup"><span data-stu-id="d224b-123">To fill in and post an intercompany journal</span></span>
<span data-ttu-id="d224b-124">When you post an intercompany general journal line in your company, a corresponding journal line is created in your intercompany outbox that you can transfer to your partner.</span><span class="sxs-lookup"><span data-stu-id="d224b-124">When you post an intercompany general journal line in your company, a corresponding journal line is created in your intercompany outbox that you can transfer to your partner.</span></span> <span data-ttu-id="d224b-125">Your partner can then post the corresponding transaction in their company, without having to re-enter the data.</span><span class="sxs-lookup"><span data-stu-id="d224b-125">Your partner can then post the corresponding transaction in their company, without having to re-enter the data.</span></span>

1. <span data-ttu-id="d224b-126">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **IC General Journals**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="d224b-126">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **IC General Journals**, and then choose the related link.</span></span>  
2. <span data-ttu-id="d224b-127">Open the relevant journal batch.</span><span class="sxs-lookup"><span data-stu-id="d224b-127">Open the relevant journal batch.</span></span> <span data-ttu-id="d224b-128">For more information, see [Working with General Journals](ui-work-general-journals.md).</span><span class="sxs-lookup"><span data-stu-id="d224b-128">For more information, see [Working with General Journals](ui-work-general-journals.md).</span></span>
3. <span data-ttu-id="d224b-129">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="d224b-129">Fill in the fields as necessary.</span></span>
4. <span data-ttu-id="d224b-130">In the **IC Partner G/L Acc. No.** field, enter the intercompany general ledger account that the amount will be posted to in your partner's company.</span><span class="sxs-lookup"><span data-stu-id="d224b-130">In the **IC Partner G/L Acc. No.** field, enter the intercompany general ledger account that the amount will be posted to in your partner's company.</span></span>

    > [!NOTE]
    > <span data-ttu-id="d224b-131">This field must be filled in on a line with a bank account or general ledger account in either the **Account No.** field or the **Bal. Account No.** field.</span><span class="sxs-lookup"><span data-stu-id="d224b-131">This field must be filled in on a line with a bank account or general ledger account in either the **Account No.** field or the **Bal. Account No.** field.</span></span>  
5. <span data-ttu-id="d224b-132">Choose the **Post** action.</span><span class="sxs-lookup"><span data-stu-id="d224b-132">Choose the **Post** action.</span></span>

<span data-ttu-id="d224b-133">The involved entries are posted in your company and a journal with the corresponding entries are created in your intercompany outbox that you can send to your partner company.</span><span class="sxs-lookup"><span data-stu-id="d224b-133">The involved entries are posted in your company and a journal with the corresponding entries are created in your intercompany outbox that you can send to your partner company.</span></span> <span data-ttu-id="d224b-134">For more information, see [How to: Manage the Intercompany Inbox and Outbox](intercompany-how-manage-intercompany-inbox.md).</span><span class="sxs-lookup"><span data-stu-id="d224b-134">For more information, see [How to: Manage the Intercompany Inbox and Outbox](intercompany-how-manage-intercompany-inbox.md).</span></span> 

## <a name="see-also"></a><span data-ttu-id="d224b-135">See Also</span><span class="sxs-lookup"><span data-stu-id="d224b-135">See Also</span></span>
[<span data-ttu-id="d224b-136">Managing Intercompany Transactions</span><span class="sxs-lookup"><span data-stu-id="d224b-136">Managing Intercompany Transactions</span></span>](intercompany-manage.md)  
[<span data-ttu-id="d224b-137">Finance</span><span class="sxs-lookup"><span data-stu-id="d224b-137">Finance</span></span>](finance.md)  
[<span data-ttu-id="d224b-138">Setting Up Finance</span><span class="sxs-lookup"><span data-stu-id="d224b-138">Setting Up Finance</span></span>](finance-setup-finance.md)  
[<span data-ttu-id="d224b-139">Working with General Journals</span><span class="sxs-lookup"><span data-stu-id="d224b-139">Working with General Journals</span></span>](ui-work-general-journals.md)  
<span data-ttu-id="d224b-140">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="d224b-140">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

