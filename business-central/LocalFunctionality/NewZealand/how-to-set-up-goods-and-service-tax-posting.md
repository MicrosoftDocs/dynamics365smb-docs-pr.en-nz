---
title: How to Set Up Goods and Service Tax Posting
description: Describes how to set up posting for goods and services tax (GST) in New Zealand.
services: project-madeira
documentationcenter: ''
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2020
ms.author: bholtorf
ms.openlocfilehash: 176f314be6629bcb2ac615d6c19f1a5b7d622969
ms.sourcegitcommit: 88e4b30eaf6fa32af0c1452ce2f85ff1111c75e2
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 04/01/2020
ms.locfileid: "3181054"
---
# <a name="set-up-goods-and-service-tax-posting"></a><span data-ttu-id="811f1-103">Set Up Goods and Service Tax Posting</span><span class="sxs-lookup"><span data-stu-id="811f1-103">Set Up Goods and Service Tax Posting</span></span>
<span data-ttu-id="811f1-104">Goods and services tax (GST) is the tax that is applied on most goods and services.</span><span class="sxs-lookup"><span data-stu-id="811f1-104">Goods and services tax (GST) is the tax that is applied on most goods and services.</span></span> <span data-ttu-id="811f1-105">The GST that is paid and received during a period is reported in the Business Activity Statement (BAS) that has to be submitted to the tax authority.</span><span class="sxs-lookup"><span data-stu-id="811f1-105">The GST that is paid and received during a period is reported in the Business Activity Statement (BAS) that has to be submitted to the tax authority.</span></span>  

<span data-ttu-id="811f1-106">To set up posting details for GST, you must define the posting groups, rate of GST, and the accounts to which GST is to be posted.</span><span class="sxs-lookup"><span data-stu-id="811f1-106">To set up posting details for GST, you must define the posting groups, rate of GST, and the accounts to which GST is to be posted.</span></span> <span data-ttu-id="811f1-107">You can set up this information for a particular combination business posting groups and product posting groups.</span><span class="sxs-lookup"><span data-stu-id="811f1-107">You can set up this information for a particular combination business posting groups and product posting groups.</span></span>  

## <a name="to-set-up-goods-and-sales-tax-posting"></a><span data-ttu-id="811f1-108">To set up goods and sales tax posting</span><span class="sxs-lookup"><span data-stu-id="811f1-108">To set up goods and sales tax posting</span></span>  
1. <span data-ttu-id="811f1-109">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **GST Posting Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="811f1-109">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **VAT Posting Setup**, and then choose the related link.</span></span>  
2. <span data-ttu-id="811f1-110">Fill in the fields as described in the following table.</span><span class="sxs-lookup"><span data-stu-id="811f1-110">Fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="811f1-111">Field</span><span class="sxs-lookup"><span data-stu-id="811f1-111">Field</span></span>|<span data-ttu-id="811f1-112">Description</span><span class="sxs-lookup"><span data-stu-id="811f1-112">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="811f1-113">**GST Bus. Posting Group**</span><span class="sxs-lookup"><span data-stu-id="811f1-113">**VAT Bus. Posting Group**</span></span>|<span data-ttu-id="811f1-114">Specifies the GST business posting group code.</span><span class="sxs-lookup"><span data-stu-id="811f1-114">Specifies the VAT business posting group code.</span></span>|  
    |<span data-ttu-id="811f1-115">**GST Prod. Posting Group**</span><span class="sxs-lookup"><span data-stu-id="811f1-115">**VAT Prod. Posting Group**</span></span>|<span data-ttu-id="811f1-116">Specifies the GST product posting group code.</span><span class="sxs-lookup"><span data-stu-id="811f1-116">Specifies the VAT product posting group code.</span></span>|  
    |<span data-ttu-id="811f1-117">**GST Identifier**</span><span class="sxs-lookup"><span data-stu-id="811f1-117">**VAT Identifier**</span></span>|<span data-ttu-id="811f1-118">Specifies the code that is used to group similar GST setups with similar attributes.</span><span class="sxs-lookup"><span data-stu-id="811f1-118">Specifies the code that is used to group similar VAT setups with similar attributes.</span></span><br /><br /> <span data-ttu-id="811f1-119">For example, you can group a number of GST posting setups that have a common GST percentage.</span><span class="sxs-lookup"><span data-stu-id="811f1-119">For example, you can group a number of VAT posting setups that have a common VAT percentage.</span></span>|  
    |<span data-ttu-id="811f1-120">**GST %**</span><span class="sxs-lookup"><span data-stu-id="811f1-120">**VAT %**</span></span>|<span data-ttu-id="811f1-121">Specifies the GST rate.</span><span class="sxs-lookup"><span data-stu-id="811f1-121">Specifies the VAT rate.</span></span>|  
    |<span data-ttu-id="811f1-122">**GST Calculation Type**</span><span class="sxs-lookup"><span data-stu-id="811f1-122">**VAT Calculation Type**</span></span>|<span data-ttu-id="811f1-123">Specifies the method that is used to calculate the purchase or sale of items.</span><span class="sxs-lookup"><span data-stu-id="811f1-123">Specifies the method that is used to calculate the purchase or sale of items.</span></span>|  
    |<span data-ttu-id="811f1-124">**Sales GST Account**</span><span class="sxs-lookup"><span data-stu-id="811f1-124">**Sales VAT Account**</span></span>|<span data-ttu-id="811f1-125">Specifies the number of the general ledger account to which you want to post the sales GST.</span><span class="sxs-lookup"><span data-stu-id="811f1-125">Specifies the number of the general ledger account to which you want to post the sales VAT.</span></span><br /><br /> <span data-ttu-id="811f1-126">If you have selected the **Reverse Charge GST** option in the **GST Calculation Type** field, then do not enter a value in this field.</span><span class="sxs-lookup"><span data-stu-id="811f1-126">If you have selected the **Reverse Charge VAT** option in the **VAT Calculation Type** field, then do not enter a value in this field.</span></span>|  
    |<span data-ttu-id="811f1-127">**Purchase GST Account**</span><span class="sxs-lookup"><span data-stu-id="811f1-127">**Purchase VAT Account**</span></span>|<span data-ttu-id="811f1-128">Specifies the number of the general ledger account to which you want to post the purchase GST.</span><span class="sxs-lookup"><span data-stu-id="811f1-128">Specifies the number of the general ledger account to which you want to post the purchase VAT.</span></span>|  
    |<span data-ttu-id="811f1-129">**Reverse Chrg. GST Acc.**</span><span class="sxs-lookup"><span data-stu-id="811f1-129">**Reverse Chrg. VAT Acc.**</span></span>|<span data-ttu-id="811f1-130">Specifies the number of the general ledger account to which you want to post the reverse charge GST.</span><span class="sxs-lookup"><span data-stu-id="811f1-130">Specifies the number of the general ledger account to which you want to post the reverse charge VAT.</span></span><br /><br /> <span data-ttu-id="811f1-131">You can enter a value in this field only if you have selected the **Reverse Charge GST** option in the **GST Calculation Type** field.</span><span class="sxs-lookup"><span data-stu-id="811f1-131">You can enter a value in this field only if you have selected the **Reverse Charge VAT** option in the **VAT Calculation Type** field.</span></span>|  

3.  <span data-ttu-id="811f1-132">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="811f1-132">Choose the **OK** button.</span></span>  

## <a name="see-also"></a><span data-ttu-id="811f1-133">See Also</span><span class="sxs-lookup"><span data-stu-id="811f1-133">See Also</span></span>  
[<span data-ttu-id="811f1-134">Print Goods and Service Tax Settlement Reports</span><span class="sxs-lookup"><span data-stu-id="811f1-134">Print Goods and Service Tax Settlement Reports</span></span>](how-to-print-goods-and-service-tax-settlement-reports.md)
