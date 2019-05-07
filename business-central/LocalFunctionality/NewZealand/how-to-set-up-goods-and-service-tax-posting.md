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
ms.date: 04/01/2019
ms.author: bholtorf
ms.openlocfilehash: d53b2d4a8a6078407c38424d928f6c6f32560117
ms.sourcegitcommit: bd78a5d990c9e83174da1409076c22df8b35eafd
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 03/31/2019
ms.locfileid: "931017"
---
# <a name="set-up-goods-and-service-tax-posting"></a><span data-ttu-id="00030-103">Set Up Goods and Service Tax Posting</span><span class="sxs-lookup"><span data-stu-id="00030-103">Set Up Goods and Service Tax Posting</span></span>
<span data-ttu-id="00030-104">Goods and services tax (GST) is the tax that is applied on most goods and services.</span><span class="sxs-lookup"><span data-stu-id="00030-104">Goods and services tax (GST) is the tax that is applied on most goods and services.</span></span> <span data-ttu-id="00030-105">The GST that is paid and received during a period is reported in the Business Activity Statement (BAS) that has to be submitted to the tax authority.</span><span class="sxs-lookup"><span data-stu-id="00030-105">The GST that is paid and received during a period is reported in the Business Activity Statement (BAS) that has to be submitted to the tax authority.</span></span>  

<span data-ttu-id="00030-106">To set up posting details for GST, you must define the posting groups, rate of GST, and the accounts to which GST is to be posted.</span><span class="sxs-lookup"><span data-stu-id="00030-106">To set up posting details for GST, you must define the posting groups, rate of GST, and the accounts to which GST is to be posted.</span></span> <span data-ttu-id="00030-107">You can set up this information for a particular combination business posting groups and product posting groups.</span><span class="sxs-lookup"><span data-stu-id="00030-107">You can set up this information for a particular combination business posting groups and product posting groups.</span></span>  

## <a name="to-set-up-goods-and-sales-tax-posting"></a><span data-ttu-id="00030-108">To set up goods and sales tax posting</span><span class="sxs-lookup"><span data-stu-id="00030-108">To set up goods and sales tax posting</span></span>  
1. <span data-ttu-id="00030-109">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **VAT Posting Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="00030-109">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **VAT Posting Setup**, and then choose the related link.</span></span>  
2. <span data-ttu-id="00030-110">Fill in the fields as described in the following table.</span><span class="sxs-lookup"><span data-stu-id="00030-110">Fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="00030-111">Field</span><span class="sxs-lookup"><span data-stu-id="00030-111">Field</span></span>|<span data-ttu-id="00030-112">Description</span><span class="sxs-lookup"><span data-stu-id="00030-112">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="00030-113">**GST Bus. Posting Group**</span><span class="sxs-lookup"><span data-stu-id="00030-113">**VAT Bus. Posting Group**</span></span>|<span data-ttu-id="00030-114">Specifies the GST business posting group code.</span><span class="sxs-lookup"><span data-stu-id="00030-114">Specifies the VAT business posting group code.</span></span>|  
    |<span data-ttu-id="00030-115">**GST Prod. Posting Group**</span><span class="sxs-lookup"><span data-stu-id="00030-115">**VAT Prod. Posting Group**</span></span>|<span data-ttu-id="00030-116">Specifies the GST product posting group code.</span><span class="sxs-lookup"><span data-stu-id="00030-116">Specifies the VAT product posting group code.</span></span>|  
    |<span data-ttu-id="00030-117">**GST Identifier**</span><span class="sxs-lookup"><span data-stu-id="00030-117">**VAT Identifier**</span></span>|<span data-ttu-id="00030-118">Specifies the code that is used to group similar GST setups with similar attributes.</span><span class="sxs-lookup"><span data-stu-id="00030-118">Specifies the code that is used to group similar VAT setups with similar attributes.</span></span><br /><br /> <span data-ttu-id="00030-119">For example, you can group a number of GST posting setups that have a common GST percentage.</span><span class="sxs-lookup"><span data-stu-id="00030-119">For example, you can group a number of VAT posting setups that have a common VAT percentage.</span></span>|  
    |<span data-ttu-id="00030-120">**GST %**</span><span class="sxs-lookup"><span data-stu-id="00030-120">**VAT %**</span></span>|<span data-ttu-id="00030-121">Specifies the GST rate.</span><span class="sxs-lookup"><span data-stu-id="00030-121">Specifies the VAT rate.</span></span>|  
    |<span data-ttu-id="00030-122">**GST Calculation Type**</span><span class="sxs-lookup"><span data-stu-id="00030-122">**VAT Calculation Type**</span></span>|<span data-ttu-id="00030-123">Specifies the method that is used to calculate the purchase or sale of items.</span><span class="sxs-lookup"><span data-stu-id="00030-123">Specifies the method that is used to calculate the purchase or sale of items.</span></span>|  
    |<span data-ttu-id="00030-124">**Sales GST Account**</span><span class="sxs-lookup"><span data-stu-id="00030-124">**Sales VAT Account**</span></span>|<span data-ttu-id="00030-125">Specifies the number of the general ledger account to which you want to post the sales GST.</span><span class="sxs-lookup"><span data-stu-id="00030-125">Specifies the number of the general ledger account to which you want to post the sales VAT.</span></span><br /><br /> <span data-ttu-id="00030-126">If you have selected the **Reverse Charge GST** option in the **GST Calculation Type** field, then do not enter a value in this field.</span><span class="sxs-lookup"><span data-stu-id="00030-126">If you have selected the **Reverse Charge VAT** option in the **VAT Calculation Type** field, then do not enter a value in this field.</span></span>|  
    |<span data-ttu-id="00030-127">**Purchase GST Account**</span><span class="sxs-lookup"><span data-stu-id="00030-127">**Purchase VAT Account**</span></span>|<span data-ttu-id="00030-128">Specifies the number of the general ledger account to which you want to post the purchase GST.</span><span class="sxs-lookup"><span data-stu-id="00030-128">Specifies the number of the general ledger account to which you want to post the purchase VAT.</span></span>|  
    |<span data-ttu-id="00030-129">**Reverse Chrg. GST Acc.**</span><span class="sxs-lookup"><span data-stu-id="00030-129">**Reverse Chrg. VAT Acc.**</span></span>|<span data-ttu-id="00030-130">Specifies the number of the general ledger account to which you want to post the reverse charge GST.</span><span class="sxs-lookup"><span data-stu-id="00030-130">Specifies the number of the general ledger account to which you want to post the reverse charge VAT.</span></span><br /><br /> <span data-ttu-id="00030-131">You can enter a value in this field only if you have selected the **Reverse Charge GST** option in the **GST Calculation Type** field.</span><span class="sxs-lookup"><span data-stu-id="00030-131">You can enter a value in this field only if you have selected the **Reverse Charge VAT** option in the **VAT Calculation Type** field.</span></span>|  

3.  <span data-ttu-id="00030-132">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="00030-132">Choose the **OK** button.</span></span>  

## <a name="see-also"></a><span data-ttu-id="00030-133">See Also</span><span class="sxs-lookup"><span data-stu-id="00030-133">See Also</span></span>  
[<span data-ttu-id="00030-134">Print Goods and Service Tax Settlement Reports</span><span class="sxs-lookup"><span data-stu-id="00030-134">Print Goods and Service Tax Settlement Reports</span></span>](how-to-print-goods-and-service-tax-settlement-reports.md)
