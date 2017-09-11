---
title: Record expenses or income directly in G/L| Microsoft Docs
description: For business activities that are not represented by a document in, such as smaller expenses or cash receipts, you can create the related transactions by posting journal lines in the General Journal window.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: direct posting, general ledger
ms.date: 06/15/2017
ms.author: sgroespe
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: 7fa0d6b604a60e000208287546d831690a914931
ms.contentlocale: en-nz
ms.lasthandoff: 07/07/2017


---
# <a name="how-to-post-transactions-directly-to-the-general-ledger"></a><span data-ttu-id="cfe3f-103">How to: Post Transactions Directly to the General Ledger</span><span class="sxs-lookup"><span data-stu-id="cfe3f-103">How to: Post Transactions Directly to the General Ledger</span></span>
<span data-ttu-id="cfe3f-104">Most financial transactions are posted to the general ledger through dedicated business documents, such as purchase invoices and sales orders.</span><span class="sxs-lookup"><span data-stu-id="cfe3f-104">Most financial transactions are posted to the general ledger through dedicated business documents, such as purchase invoices and sales orders.</span></span> <span data-ttu-id="cfe3f-105">For business activities that are not represented by a document in [!INCLUDE[d365fin](includes/d365fin_md.md)], such as smaller expenses or cash receipts, you can create the related transactions by posting journal lines in the **General Journal** window.</span><span class="sxs-lookup"><span data-stu-id="cfe3f-105">For business activities that are not represented by a document in [!INCLUDE[d365fin](includes/d365fin_md.md)], such as smaller expenses or cash receipts, you can create the related transactions by posting journal lines in the **General Journal** window.</span></span>

<span data-ttu-id="cfe3f-106">General journals post financial transactions directly to general ledger accounts and other accounts, such as bank, customer, and vendor accounts.</span><span class="sxs-lookup"><span data-stu-id="cfe3f-106">General journals post financial transactions directly to general ledger accounts and other accounts, such as bank, customer, and vendor accounts.</span></span> <span data-ttu-id="cfe3f-107">Posting with a general journal always creates entries on general ledger accounts.</span><span class="sxs-lookup"><span data-stu-id="cfe3f-107">Posting with a general journal always creates entries on general ledger accounts.</span></span> <span data-ttu-id="cfe3f-108">This is true even when, for example, you post a journal line to a customer account, because an entry is posted to a general ledger receivables account through a posting group.</span><span class="sxs-lookup"><span data-stu-id="cfe3f-108">This is true even when, for example, you post a journal line to a customer account, because an entry is posted to a general ledger receivables account through a posting group.</span></span> <span data-ttu-id="cfe3f-109">You can personalise your version of a general journal by setting up a journal batch or template.</span><span class="sxs-lookup"><span data-stu-id="cfe3f-109">You can personalize your version of a general journal by setting up a journal batch or template.</span></span> <span data-ttu-id="cfe3f-110">For more information, see [Working with General Journals](ui-work-general-journals.md).</span><span class="sxs-lookup"><span data-stu-id="cfe3f-110">For more information, see [Working with General Journals](ui-work-general-journals.md).</span></span>

<span data-ttu-id="cfe3f-111">Unlike for entries that are posted with documents, which require a credit memo process, you can correctly reverse entries that are posted with the general journal.</span><span class="sxs-lookup"><span data-stu-id="cfe3f-111">Unlike for entries that are posted with documents, which require a credit memo process, you can correctly reverse entries that are posted with the general journal.</span></span> <span data-ttu-id="cfe3f-112">For more information, see [How to: Reverse Journal Posting](finance-how-reverse-journal-posting.md).</span><span class="sxs-lookup"><span data-stu-id="cfe3f-112">For more information, see [How to: Reverse Journal Posting](finance-how-reverse-journal-posting.md).</span></span>

## <a name="to-post-a-transaction-directly-to-a-general-ledger-account"></a><span data-ttu-id="cfe3f-113">To post a transaction directly to a general ledger account</span><span class="sxs-lookup"><span data-stu-id="cfe3f-113">To post a transaction directly to a general ledger account</span></span>
1. <span data-ttu-id="cfe3f-114">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **General Journals**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="cfe3f-114">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **General Journals**, and then choose the related link.</span></span>
2. <span data-ttu-id="cfe3f-115">Open the relevant general journal batch.</span><span class="sxs-lookup"><span data-stu-id="cfe3f-115">Open the relevant general journal batch.</span></span> <span data-ttu-id="cfe3f-116">For more information, see [Working with General Journals](ui-work-general-journals.md).</span><span class="sxs-lookup"><span data-stu-id="cfe3f-116">For more information, see [Working with General Journals](ui-work-general-journals.md).</span></span>
3. <span data-ttu-id="cfe3f-117">On a new journal line, fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="cfe3f-117">On a new journal line, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]    
4. <span data-ttu-id="cfe3f-118">Repeat step 3 for all the separate transactions that you want to post.</span><span class="sxs-lookup"><span data-stu-id="cfe3f-118">Repeat step 3 for all the separate transactions that you want to post.</span></span>

    > [!TIP]  
    > <span data-ttu-id="cfe3f-119">If you want to enter multiple transaction lines above one balance-account line, for example, for one bank account, then select the **Suggest Balancing Amount** check box on the line for your batch in the **General Journal Batches** window.</span><span class="sxs-lookup"><span data-stu-id="cfe3f-119">If you want to enter multiple transaction lines above one balance-account line, for example, for one bank account, then select the **Suggest Balancing Amount** check box on the line for your batch in the **General Journal Batches** window.</span></span> <span data-ttu-id="cfe3f-120">Then the **Amount** field on the balance-account line is automatically prefilled with the value that is required to balance the transactions.</span><span class="sxs-lookup"><span data-stu-id="cfe3f-120">Then the **Amount** field on the balance-account line is automatically prefilled with the value that is required to balance the transactions.</span></span>
5. <span data-ttu-id="cfe3f-121">Choose the **Post** action to record the transactions on the specified G/L accounts.</span><span class="sxs-lookup"><span data-stu-id="cfe3f-121">Choose the **Post** action to record the transactions on the specified G/L accounts.</span></span>

## <a name="see-also"></a><span data-ttu-id="cfe3f-122">See Also</span><span class="sxs-lookup"><span data-stu-id="cfe3f-122">See Also</span></span>
[<span data-ttu-id="cfe3f-123">Working with General Journals</span><span class="sxs-lookup"><span data-stu-id="cfe3f-123">Working with General Journals</span></span>](ui-work-general-journals.md)  
[<span data-ttu-id="cfe3f-124">How to: Reverse Journal Posting</span><span class="sxs-lookup"><span data-stu-id="cfe3f-124">How to: Reverse Journal Posting</span></span>](finance-how-reverse-journal-posting.md)  
[<span data-ttu-id="cfe3f-125">Finance</span><span class="sxs-lookup"><span data-stu-id="cfe3f-125">Finance</span></span>](finance.md)  
<span data-ttu-id="cfe3f-126">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="cfe3f-126">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  

