---
title: Post SEPA Direct Debit Payments | Microsoft Docs
description: When a direct debit collection is successfully processed by your bank, you can proceed to post receipt of the payment for the involved sales invoices.
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
ms.openlocfilehash: ee07ca7ba498858fac794f1ee1f27f281de8ae02
ms.contentlocale: en-nz
ms.lasthandoff: 09/28/2018

---
# <a name="post-sepa-direct-debit-payment-receipts"></a><span data-ttu-id="05995-103">Post SEPA Direct Debit Payment Receipts</span><span class="sxs-lookup"><span data-stu-id="05995-103">Post SEPA Direct Debit Payment Receipts</span></span>
<span data-ttu-id="05995-104">When a direct debit collection is successfully processed by your bank, you can proceed to post receipt of the payment for the involved sales invoices.</span><span class="sxs-lookup"><span data-stu-id="05995-104">When a direct debit collection is successfully processed by your bank, you can proceed to post receipt of the payment for the involved sales invoices.</span></span> <span data-ttu-id="05995-105">For more information, see [Create SEPA Direct Debit Collection Entries and Export to a Bank File](finance-how-create-sepa-direct-debit-collection-entries-export-bank-file.md).</span><span class="sxs-lookup"><span data-stu-id="05995-105">For more information, see [Create SEPA Direct Debit Collection Entries and Export to a Bank File](finance-how-create-sepa-direct-debit-collection-entries-export-bank-file.md).</span></span>  

<span data-ttu-id="05995-106">You can post the payment receipt directly from the **Direct Debit Collections** window or the **Direct Debit Collect. Entries** window.</span><span class="sxs-lookup"><span data-stu-id="05995-106">You can post the payment receipt directly from the **Direct Debit Collections** window or the **Direct Debit Collect. Entries** window.</span></span> <span data-ttu-id="05995-107">Alternatively, you can relay the work to another user by preparing the related journal lines.</span><span class="sxs-lookup"><span data-stu-id="05995-107">Alternatively, you can relay the work to another user by preparing the related journal lines.</span></span>  

## <a name="to-post-a-direct-debit-payment-receipt-from-the-direct-debit-collections-window"></a><span data-ttu-id="05995-108">To post a direct-debit payment receipt from the Direct Debit Collections window</span><span class="sxs-lookup"><span data-stu-id="05995-108">To post a direct-debit payment receipt from the Direct Debit Collections window</span></span>  
1. <span data-ttu-id="05995-109">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Direct Debit Collections**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="05995-109">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Direct Debit Collections**, and then choose the related link.</span></span>  
2. <span data-ttu-id="05995-110">Select a line for a direct debit collection that has been exported to a bank file and successfully processed by the bank.</span><span class="sxs-lookup"><span data-stu-id="05995-110">Select a line for a direct debit collection that has been exported to a bank file and successfully processed by the bank.</span></span> <span data-ttu-id="05995-111">For more information, see [Create SEPA Direct Debit Collection Entries and Export to a Bank File](finance-how-create-sepa-direct-debit-collection-entries-export-bank-file.md).</span><span class="sxs-lookup"><span data-stu-id="05995-111">For more information, see [Create SEPA Direct Debit Collection Entries and Export to a Bank File](finance-how-create-sepa-direct-debit-collection-entries-export-bank-file.md).</span></span>  
3. <span data-ttu-id="05995-112">Choose the **Post Payment Receipts** action.</span><span class="sxs-lookup"><span data-stu-id="05995-112">Choose the **Post Payment Receipts** action.</span></span>  
4. <span data-ttu-id="05995-113">In the **Post Direct Debit Collection** window, fill in the fields as described in the following table.</span><span class="sxs-lookup"><span data-stu-id="05995-113">In the **Post Direct Debit Collection** window, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="05995-114">Field</span><span class="sxs-lookup"><span data-stu-id="05995-114">Field</span></span>|<span data-ttu-id="05995-115">Description</span><span class="sxs-lookup"><span data-stu-id="05995-115">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="05995-116">**Direct Debit Collection No.**</span><span class="sxs-lookup"><span data-stu-id="05995-116">**Direct Debit Collection No.**</span></span>|<span data-ttu-id="05995-117">Specify the direct debit collection that you want to post payment receipt for.</span><span class="sxs-lookup"><span data-stu-id="05995-117">Specify the direct debit collection that you want to post payment receipt for.</span></span>|  
    |<span data-ttu-id="05995-118">**General Journal Template**</span><span class="sxs-lookup"><span data-stu-id="05995-118">**General Journal Template**</span></span>|<span data-ttu-id="05995-119">Specify which general journal template to use for posting the payment receipt, such as the template for cash receipts.</span><span class="sxs-lookup"><span data-stu-id="05995-119">Specify which general journal template to use for posting the payment receipt, such as the template for cash receipts.</span></span>|  
    |<span data-ttu-id="05995-120">**General Journal Batch Name**</span><span class="sxs-lookup"><span data-stu-id="05995-120">**General Journal Batch Name**</span></span>|<span data-ttu-id="05995-121">Specify which general journal batch to use for posting the payment receipt.</span><span class="sxs-lookup"><span data-stu-id="05995-121">Specify which general journal batch to use for posting the payment receipt.</span></span>|  
    |<span data-ttu-id="05995-122">**Create Journal Only**</span><span class="sxs-lookup"><span data-stu-id="05995-122">**Create Journal Only**</span></span>|<span data-ttu-id="05995-123">Select this check box if you do not want to post the payment receipt when you choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="05995-123">Select this check box if you do not want to post the payment receipt when you choose the **OK** button.</span></span> <span data-ttu-id="05995-124">The payment receipt will be prepared in the specified journal and will not be posted until someone posts the journal lines in question.</span><span class="sxs-lookup"><span data-stu-id="05995-124">The payment receipt will be prepared in the specified journal and will not be posted until someone posts the journal lines in question.</span></span>|  

5. <span data-ttu-id="05995-125">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="05995-125">Choose the **OK** button.</span></span>  

## <a name="see-also"></a><span data-ttu-id="05995-126">See Also</span><span class="sxs-lookup"><span data-stu-id="05995-126">See Also</span></span>  
 <span data-ttu-id="05995-127">[Collecting Payments with SEPA Direct Debit](finance-collect-payments-with-sepa-direct-debit.md) </span><span class="sxs-lookup"><span data-stu-id="05995-127">[Collecting Payments with SEPA Direct Debit](finance-collect-payments-with-sepa-direct-debit.md) </span></span>  
 [<span data-ttu-id="05995-128">Sales</span><span class="sxs-lookup"><span data-stu-id="05995-128">Sales</span></span>](sales-manage-sales.md)

