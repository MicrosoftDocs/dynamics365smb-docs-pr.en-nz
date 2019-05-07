---
title: How to Correct Prepayments | Microsoft Docs
description: You can make a correction to an order after you have posted a prepayment invoice for the order. You can add new lines to an order after issuing a prepayment, and then you can post another prepayment invoice, but you cannot delete a line from an order after a prepayment has been invoiced for the line.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2019
ms.author: sgroespe
ms.openlocfilehash: 1fa6640dbca61a90d02182d1b938b87b157bb080
ms.sourcegitcommit: bd78a5d990c9e83174da1409076c22df8b35eafd
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 03/31/2019
ms.locfileid: "922616"
---
# <a name="correct-prepayments"></a><span data-ttu-id="21068-104">Correct Prepayments</span><span class="sxs-lookup"><span data-stu-id="21068-104">Correct Prepayments</span></span>
<span data-ttu-id="21068-105">You can make a correction to an order after you have posted a prepayment invoice for the order.</span><span class="sxs-lookup"><span data-stu-id="21068-105">You can make a correction to an order after you have posted a prepayment invoice for the order.</span></span> <span data-ttu-id="21068-106">You can add new lines to an order after issuing a prepayment, and then you can post another prepayment invoice, but you cannot delete a line from an order after a prepayment has been invoiced for the line.</span><span class="sxs-lookup"><span data-stu-id="21068-106">You can add new lines to an order after issuing a prepayment, and then you can post another prepayment invoice, but you cannot delete a line from an order after a prepayment has been invoiced for the line.</span></span>  

## <a name="to-correct-a-prepayment"></a><span data-ttu-id="21068-107">To correct a prepayment</span><span class="sxs-lookup"><span data-stu-id="21068-107">To correct a prepayment</span></span>
<span data-ttu-id="21068-108">The following procedure shows how to issue a prepayment credit memo to cancel all invoiced prepayments for a sales order.</span><span class="sxs-lookup"><span data-stu-id="21068-108">The following procedure shows how to issue a prepayment credit memo to cancel all invoiced prepayments for a sales order.</span></span>  
1. <span data-ttu-id="21068-109">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="21068-109">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.</span></span>  
2. <span data-ttu-id="21068-110">Open the relevant sales order.</span><span class="sxs-lookup"><span data-stu-id="21068-110">Open the relevant sales order.</span></span>
3. <span data-ttu-id="21068-111">Choose the **Prepayment** action, and then choose the **Post Prepayment Credit Memo** action or the **Post and Print Prepmt. Cr. Memo** action.</span><span class="sxs-lookup"><span data-stu-id="21068-111">Choose the **Prepayment** action, and then choose the **Post Prepayment Credit Memo** action or the **Post and Print Prepmt. Cr. Memo** action.</span></span>  
4. <span data-ttu-id="21068-112">On the **Sales Credit Memo** page, proceed to correct the relevant entries, as for any sales credit memo.</span><span class="sxs-lookup"><span data-stu-id="21068-112">On the **Sales Credit Memo** page, proceed to correct the relevant entries, as for any sales credit memo.</span></span> <span data-ttu-id="21068-113">For more information, see [Process Sales Returns or Cancellations](sales-how-process-sales-returns-cancellations.md).</span><span class="sxs-lookup"><span data-stu-id="21068-113">For more information, see [Process Sales Returns or Cancellations](sales-how-process-sales-returns-cancellations.md).</span></span>     

    > [!NOTE]  
    > <span data-ttu-id="21068-114">To Reduce the amount in the **Line Amount** field, you must first increase the prepayment percentage on the line so that the value in the **Prepmt. Line Amount** field is not decreased below the value in the **Prepmt. Amt. Inv.** field.</span><span class="sxs-lookup"><span data-stu-id="21068-114">To Reduce the amount in the **Line Amount** field, you must first increase the prepayment percentage on the line so that the value in the **Prepmt. Line Amount** field is not decreased below the value in the **Prepmt. Amt. Inv.** field.</span></span>

5. <span data-ttu-id="21068-115">To make a prepayment invoice for any new lines in the sales credit memo, choose the **Prepayment** action, and then choose the **Post Prepayment Invoice** action or the **Post and Print Prepmt. Invoice** action.</span><span class="sxs-lookup"><span data-stu-id="21068-115">To make a prepayment invoice for any new lines in the sales credit memo, choose the **Prepayment** action, and then choose the **Post Prepayment Invoice** action or the **Post and Print Prepmt. Invoice** action.</span></span>  
6. <span data-ttu-id="21068-116">To issue an additional prepayment invoice, increase the prepayment amount on one or more lines and post the prepayment invoice.</span><span class="sxs-lookup"><span data-stu-id="21068-116">To issue an additional prepayment invoice, increase the prepayment amount on one or more lines and post the prepayment invoice.</span></span> <span data-ttu-id="21068-117">A new invoice will be created for the difference between the prepayment amounts invoiced and the new prepayment amounts.</span><span class="sxs-lookup"><span data-stu-id="21068-117">A new invoice will be created for the difference between the prepayment amounts invoiced and the new prepayment amounts.</span></span>  

## <a name="see-also"></a><span data-ttu-id="21068-118">See Also</span><span class="sxs-lookup"><span data-stu-id="21068-118">See Also</span></span>  
[<span data-ttu-id="21068-119">Invoicing Prepayments</span><span class="sxs-lookup"><span data-stu-id="21068-119">Invoicing Prepayments</span></span>](finance-invoice-prepayments.md)  
[<span data-ttu-id="21068-120">Walkthrough: Setting Up and Invoicing Sales Prepayments</span><span class="sxs-lookup"><span data-stu-id="21068-120">Walkthrough: Setting Up and Invoicing Sales Prepayments</span></span>](walkthrough-setting-up-and-invoicing-sales-prepayments.md)  
[<span data-ttu-id="21068-121">Finance</span><span class="sxs-lookup"><span data-stu-id="21068-121">Finance</span></span>](finance.md)  
<span data-ttu-id="21068-122">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="21068-122">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
