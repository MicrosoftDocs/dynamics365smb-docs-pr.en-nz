---
title: Set Up Payment Methods| Microsoft Docs
description: You use payment methods, for example, cheque, bank transfer, cash, or PayPal, to define how sales and purchase invoices will be paid.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: check, bank transfer, cash, PayPal
ms.date: 10/01/2019
ms.author: bholtorf
ms.openlocfilehash: 753b9f30648059a68c22b524008e21c6c866d19c
ms.sourcegitcommit: cfc92eefa8b06fb426482f54e393f0e6e222f712
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 12/03/2019
ms.locfileid: "2882558"
---
# <a name="defining-payment-methods"></a><span data-ttu-id="2bfe1-103">Defining Payment Methods</span><span class="sxs-lookup"><span data-stu-id="2bfe1-103">Defining Payment Methods</span></span>
<span data-ttu-id="2bfe1-104">Payment methods define the way you prefer for customers to pay you, and how you like to pay your vendors.</span><span class="sxs-lookup"><span data-stu-id="2bfe1-104">Payment methods define the way you prefer for customers to pay you, and how you like to pay your vendors.</span></span> <span data-ttu-id="2bfe1-105">The method can vary for each customer or vendor.</span><span class="sxs-lookup"><span data-stu-id="2bfe1-105">The method can vary for each customer or vendor.</span></span> <span data-ttu-id="2bfe1-106">Examples of typical payment methods are **bank**, **cash**, **cheque**, or **account**.</span><span class="sxs-lookup"><span data-stu-id="2bfe1-106">Examples of typical payment methods are **bank**, **cash**, **check**, or **account**.</span></span>

<span data-ttu-id="2bfe1-107">You can assign a payment method to customers and vendors so that the same method is always used on the sales and purchase documents you create for them.</span><span class="sxs-lookup"><span data-stu-id="2bfe1-107">You can assign a payment method to customers and vendors so that the same method is always used on the sales and purchase documents you create for them.</span></span> <span data-ttu-id="2bfe1-108">If needed, you can change the method on the sales or purchase document.</span><span class="sxs-lookup"><span data-stu-id="2bfe1-108">If needed, you can change the method on the sales or purchase document.</span></span> <span data-ttu-id="2bfe1-109">For example, if you want to pay a particular purchase invoice in cash rather than by cheque.</span><span class="sxs-lookup"><span data-stu-id="2bfe1-109">For example, if you want to pay a particular purchase invoice in cash rather than by check.</span></span> <span data-ttu-id="2bfe1-110">This does not change the default payment method assigned to the vendor.</span><span class="sxs-lookup"><span data-stu-id="2bfe1-110">This does not change the default payment method assigned to the vendor.</span></span>

<span data-ttu-id="2bfe1-111">The same payment methods are used for sales and purchase documents.</span><span class="sxs-lookup"><span data-stu-id="2bfe1-111">The same payment methods are used for sales and purchase documents.</span></span> <span data-ttu-id="2bfe1-112">For example, a _cash_ payment method is used both when you make payments and when you receive them.</span><span class="sxs-lookup"><span data-stu-id="2bfe1-112">For example, a _cash_ payment method is used both when you make payments and when you receive them.</span></span> [!INCLUDE[d365fin](includes/d365fin_md.md)] <span data-ttu-id="2bfe1-113">knows that when you are creating a sales invoice you expect to receive payment, and the opposite for purchase invoices.</span><span class="sxs-lookup"><span data-stu-id="2bfe1-113">knows that when you are creating a sales invoice you expect to receive payment, and the opposite for purchase invoices.</span></span>

<span data-ttu-id="2bfe1-114">Credit memos for returns, however, are exceptions because money is flowing in the opposite directions, from you to your customer and from your vendor to you.</span><span class="sxs-lookup"><span data-stu-id="2bfe1-114">Credit memos for returns, however, are exceptions because money is flowing in the opposite directions, from you to your customer and from your vendor to you.</span></span> <span data-ttu-id="2bfe1-115">Therefore, a default payment method is not assigned to credit memos.</span><span class="sxs-lookup"><span data-stu-id="2bfe1-115">Therefore, a default payment method is not assigned to credit memos.</span></span> <span data-ttu-id="2bfe1-116">There is, however, a workaround if you have specified terms of payment for the customer or vendor.</span><span class="sxs-lookup"><span data-stu-id="2bfe1-116">There is, however, a workaround if you have specified terms of payment for the customer or vendor.</span></span> <span data-ttu-id="2bfe1-117">Though the **Calc. Pmt. Disc. on Cr. Memos** field is not intended for this, if you choose the check box on the **Payment Terms** page a default payment method will be added when you create a credit memo.</span><span class="sxs-lookup"><span data-stu-id="2bfe1-117">Though the **Calc. Pmt. Disc. on Cr. Memos** field is not intended for this, if you choose the check box on the **Payment Terms** page a default payment method will be added when you create a credit memo.</span></span> <br><br>  

> [!Video https://www.microsoft.com/videoplayer/embed/RE476Ys]

## <a name="to-set-up-a-payment-method"></a><span data-ttu-id="2bfe1-118">To set up a payment method</span><span class="sxs-lookup"><span data-stu-id="2bfe1-118">To set up a payment method</span></span>
[!INCLUDE[d365fin](includes/d365fin_md.md)] <span data-ttu-id="2bfe1-119">provides a few payment methods that businesses often use.</span><span class="sxs-lookup"><span data-stu-id="2bfe1-119">provides a few payment methods that businesses often use.</span></span> <span data-ttu-id="2bfe1-120">You can, however, add as many as you need.</span><span class="sxs-lookup"><span data-stu-id="2bfe1-120">You can, however, add as many as you need.</span></span>

1. <span data-ttu-id="2bfe1-121">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Payment Methods**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="2bfe1-121">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Payment Methods**, and then choose the related link.</span></span>
2. <span data-ttu-id="2bfe1-122">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="2bfe1-122">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="to-assign-a-payment-method-to-a-customer-or-vendor"></a><span data-ttu-id="2bfe1-123">To assign a payment method to a customer or vendor</span><span class="sxs-lookup"><span data-stu-id="2bfe1-123">To assign a payment method to a customer or vendor</span></span>
1. <span data-ttu-id="2bfe1-124">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Customer** or **Vendor**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="2bfe1-124">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Customer** or **Vendor**, and then choose the related link.</span></span>
2. <span data-ttu-id="2bfe1-125">In the **Payment Method Code** field, choose the method to use by default for the customer or vendor.</span><span class="sxs-lookup"><span data-stu-id="2bfe1-125">In the **Payment Method Code** field, choose the method to use by default for the customer or vendor.</span></span>

## <a name="see-also"></a><span data-ttu-id="2bfe1-126">See Also</span><span class="sxs-lookup"><span data-stu-id="2bfe1-126">See Also</span></span>
[<span data-ttu-id="2bfe1-127">Register New Customers</span><span class="sxs-lookup"><span data-stu-id="2bfe1-127">Register New Customers</span></span>](sales-how-register-new-customers.md)  
[<span data-ttu-id="2bfe1-128">Finance</span><span class="sxs-lookup"><span data-stu-id="2bfe1-128">Finance</span></span>](finance.md)  
<span data-ttu-id="2bfe1-129">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="2bfe1-129">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
