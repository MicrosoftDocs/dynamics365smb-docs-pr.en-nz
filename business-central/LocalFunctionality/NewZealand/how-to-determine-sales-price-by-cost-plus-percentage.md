---
title: How to Determine Sales Price by Cost Plus Percentage
description: Describes how to use the cost plus percentage function to set a sales price based on the cost of an item.
services: project-madeira
documentationcenter: ''
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2018
ms.author: bholtorf
ms.openlocfilehash: e4253198b89c23b7a13f2b9677ca851378585156
ms.sourcegitcommit: 1bcfaa99ea302e6b84b8361ca02730b135557fc1
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 03/08/2019
ms.locfileid: "827059"
---
# <a name="determine-sales-price-by-cost-plus-percentage"></a><span data-ttu-id="fe89d-103">Determine Sales Price by Cost Plus Percentage</span><span class="sxs-lookup"><span data-stu-id="fe89d-103">Determine Sales Price by Cost Plus Percentage</span></span>
<span data-ttu-id="fe89d-104">Use the cost plus percentage function to set a sales price based on the cost of an item.</span><span class="sxs-lookup"><span data-stu-id="fe89d-104">Use the cost plus percentage function to set a sales price based on the cost of an item.</span></span> <span data-ttu-id="fe89d-105">The cost of the item can be calculated along with cost plus calculation.</span><span class="sxs-lookup"><span data-stu-id="fe89d-105">The cost of the item can be calculated along with cost plus calculation.</span></span> <span data-ttu-id="fe89d-106">The discount will be based on this calculation.</span><span class="sxs-lookup"><span data-stu-id="fe89d-106">The discount will be based on this calculation.</span></span> <span data-ttu-id="fe89d-107">This functionality eliminates the need for the use of spreadsheets in determining percentage discounts as they correspond to cost plus percentage.</span><span class="sxs-lookup"><span data-stu-id="fe89d-107">This functionality eliminates the need for the use of spreadsheets in determining percentage discounts as they correspond to cost plus percentage.</span></span>  

## <a name="to-determine-sales-tax-by-cost-plus-percentage"></a><span data-ttu-id="fe89d-108">To determine US sales tax by cost plus percentage</span><span class="sxs-lookup"><span data-stu-id="fe89d-108">To determine sales tax by cost plus percentage</span></span>  

1.  <span data-ttu-id="fe89d-109">Choose the **Receivables** action.</span><span class="sxs-lookup"><span data-stu-id="fe89d-109">Choose the **Receivables** action.</span></span>  
3.  <span data-ttu-id="fe89d-110">Choose the **Customers** action.</span><span class="sxs-lookup"><span data-stu-id="fe89d-110">Choose the **Customers** action.</span></span>  
4.  <span data-ttu-id="fe89d-111">Open the card for a relevant customer.</span><span class="sxs-lookup"><span data-stu-id="fe89d-111">Open the card for a relevant customer.</span></span>  

     <span data-ttu-id="fe89d-112">–or–</span><span class="sxs-lookup"><span data-stu-id="fe89d-112">–or–</span></span>  

    <span data-ttu-id="fe89d-113">Choose the **New** action.</span><span class="sxs-lookup"><span data-stu-id="fe89d-113">Choose the **New** action.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="fe89d-114">For a new customer, in the **No.**</span><span class="sxs-lookup"><span data-stu-id="fe89d-114">For a new customer, in the **No.**</span></span> <span data-ttu-id="fe89d-115">field, enter the customer number.</span><span class="sxs-lookup"><span data-stu-id="fe89d-115">field, enter the customer number.</span></span>  

5.  <span data-ttu-id="fe89d-116">To open the **Sales Prices** page, choose the **Prices** action.</span><span class="sxs-lookup"><span data-stu-id="fe89d-116">To open the **Sales Prices** page, choose the **Prices** action.</span></span>  
6.  <span data-ttu-id="fe89d-117">In the **General** section, fill in the fields as described in the following table.</span><span class="sxs-lookup"><span data-stu-id="fe89d-117">In the **General** section, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="fe89d-118">Field</span><span class="sxs-lookup"><span data-stu-id="fe89d-118">Field</span></span>|<span data-ttu-id="fe89d-119">Description</span><span class="sxs-lookup"><span data-stu-id="fe89d-119">Description</span></span>|  
    |-----------|-----------------|  
    |<span data-ttu-id="fe89d-120">**Sales Type Filter**</span><span class="sxs-lookup"><span data-stu-id="fe89d-120">**Sales Type Filter**</span></span>|<span data-ttu-id="fe89d-121">Select one of the following options:</span><span class="sxs-lookup"><span data-stu-id="fe89d-121">Select one of the following options:</span></span><br /><br /> <span data-ttu-id="fe89d-122">-   **Customer**</span><span class="sxs-lookup"><span data-stu-id="fe89d-122">-   **Customer**</span></span><br /><span data-ttu-id="fe89d-123">-   **Customer Price Group**</span><span class="sxs-lookup"><span data-stu-id="fe89d-123">-   **Customer Price Group**</span></span><br /><span data-ttu-id="fe89d-124">-   **All Customers**</span><span class="sxs-lookup"><span data-stu-id="fe89d-124">-   **All Customers**</span></span><br /><span data-ttu-id="fe89d-125">-   **Campaign**</span><span class="sxs-lookup"><span data-stu-id="fe89d-125">-   **Campaign**</span></span><br /><span data-ttu-id="fe89d-126">-   **None**</span><span class="sxs-lookup"><span data-stu-id="fe89d-126">-   **None**</span></span>|  
    |<span data-ttu-id="fe89d-127">**Sales Code Filter**</span><span class="sxs-lookup"><span data-stu-id="fe89d-127">**Sales Code Filter**</span></span>|<span data-ttu-id="fe89d-128">The sales code.</span><span class="sxs-lookup"><span data-stu-id="fe89d-128">The sales code.</span></span>|  
    |<span data-ttu-id="fe89d-129">**Item No. Filter**</span><span class="sxs-lookup"><span data-stu-id="fe89d-129">**Item No. Filter**</span></span>|<span data-ttu-id="fe89d-130">The item number.</span><span class="sxs-lookup"><span data-stu-id="fe89d-130">The item number.</span></span>|  
    |<span data-ttu-id="fe89d-131">**Starting Date Filter**</span><span class="sxs-lookup"><span data-stu-id="fe89d-131">**Starting Date Filter**</span></span>|<span data-ttu-id="fe89d-132">The starting date.</span><span class="sxs-lookup"><span data-stu-id="fe89d-132">The starting date.</span></span>|  
    |<span data-ttu-id="fe89d-133">**Currency Code Filter**</span><span class="sxs-lookup"><span data-stu-id="fe89d-133">**Currency Code Filter**</span></span>|<span data-ttu-id="fe89d-134">The currency code.</span><span class="sxs-lookup"><span data-stu-id="fe89d-134">The currency code.</span></span>|  

7.  <span data-ttu-id="fe89d-135">Enter information into the relevant fields.</span><span class="sxs-lookup"><span data-stu-id="fe89d-135">Enter information into the relevant fields.</span></span>  
8.  <span data-ttu-id="fe89d-136">To send the details to a recipient, choose the **Send To** action, and then select one of the following formats:</span><span class="sxs-lookup"><span data-stu-id="fe89d-136">To send the details to a recipient, choose the **Send To** action, and then select one of the following formats:</span></span>  

    - <span data-ttu-id="fe89d-137">**Recipient as Attachment**</span><span class="sxs-lookup"><span data-stu-id="fe89d-137">**Recipient as Attachment**</span></span>  
    - <span data-ttu-id="fe89d-138">**Microsoft Word**</span><span class="sxs-lookup"><span data-stu-id="fe89d-138">**Microsoft Word**</span></span>  
    - <span data-ttu-id="fe89d-139">**Microsoft Excel**</span><span class="sxs-lookup"><span data-stu-id="fe89d-139">**Microsoft Excel**</span></span>  

9. <span data-ttu-id="fe89d-140">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="fe89d-140">Choose the **OK** button.</span></span>  

## <a name="see-also"></a><span data-ttu-id="fe89d-141">See Also</span><span class="sxs-lookup"><span data-stu-id="fe89d-141">See Also</span></span>  
[<span data-ttu-id="fe89d-142">New Zealand Local Functionality</span><span class="sxs-lookup"><span data-stu-id="fe89d-142">New Zealand Local Functionality</span></span>](new-zealand-local-functionality.md)
