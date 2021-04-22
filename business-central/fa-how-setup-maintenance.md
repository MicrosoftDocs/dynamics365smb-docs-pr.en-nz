---
title: Set Up FA Maintenance| Microsoft Docs
description: To manage fixed asset repairs and service, you specify general maintenance information, codes for the type of work, and a posting account for costs.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: repair, service
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: b437f7508537ec438bf90c3a1239e2620e9db196
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 03/31/2021
ms.locfileid: "5775566"
---
# <a name="set-up-fixed-asset-maintenance"></a><span data-ttu-id="ec648-103">Set Up Fixed Asset Maintenance</span><span class="sxs-lookup"><span data-stu-id="ec648-103">Set Up Fixed Asset Maintenance</span></span>
<span data-ttu-id="ec648-104">To manage fixed asset maintenance, you must first set up some general maintenance information, a posting account for maintenance costs, and maintenance codes for types of work, such as Routine Service or Repair.</span><span class="sxs-lookup"><span data-stu-id="ec648-104">To manage fixed asset maintenance, you must first set up some general maintenance information, a posting account for maintenance costs, and maintenance codes for types of work, such as Routine Service or Repair.</span></span>

## <a name="to-set-up-general-maintenance-information"></a><span data-ttu-id="ec648-105">To set up general maintenance information</span><span class="sxs-lookup"><span data-stu-id="ec648-105">To set up general maintenance information</span></span>
<span data-ttu-id="ec648-106">If you set up the fields for maintenance, you can post maintenance expenses from the fixed asset journal.</span><span class="sxs-lookup"><span data-stu-id="ec648-106">If you set up the fields for maintenance, you can post maintenance expenses from the fixed asset journal.</span></span>

1. <span data-ttu-id="ec648-107">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Fixed Assets**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="ec648-107">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Fixed Assets**, and then choose the related link.</span></span>
2. <span data-ttu-id="ec648-108">Select the fixed asset that you to define insurance coverage for, and then choose the **Edit** action.</span><span class="sxs-lookup"><span data-stu-id="ec648-108">Select the fixed asset that you to define insurance coverage for, and then choose the **Edit** action.</span></span>
3. <span data-ttu-id="ec648-109">On the **Maintenance** FastTab, fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="ec648-109">On the **Maintenance** FastTab, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="to-set-up-maintenance-codes"></a><span data-ttu-id="ec648-110">To set up maintenance codes</span><span class="sxs-lookup"><span data-stu-id="ec648-110">To set up maintenance codes</span></span>
<span data-ttu-id="ec648-111">When you post maintenance costs from a general journal, you fill in the **Maintenance Code** field to record what kind of maintenance has been performed, such as routine service or repair.</span><span class="sxs-lookup"><span data-stu-id="ec648-111">When you post maintenance costs from a general journal, you fill in the **Maintenance Code** field to record what kind of maintenance has been performed, such as routine service or repair.</span></span>

1. <span data-ttu-id="ec648-112">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Maintenance**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="ec648-112">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Maintenance**, and then choose the related link.</span></span>
2. <span data-ttu-id="ec648-113">On the **Maintenance** page, set up codes for different types of maintenance work.</span><span class="sxs-lookup"><span data-stu-id="ec648-113">On the **Maintenance** page, set up codes for different types of maintenance work.</span></span>

## <a name="to-set-up-maintenance-expense-accounts"></a><span data-ttu-id="ec648-114">To set up maintenance expense accounts</span><span class="sxs-lookup"><span data-stu-id="ec648-114">To set up maintenance expense accounts</span></span>
<span data-ttu-id="ec648-115">To post maintenance costs, you must first enter an account number on the **FA Posting Groups** page.</span><span class="sxs-lookup"><span data-stu-id="ec648-115">To post maintenance costs, you must first enter an account number on the **FA Posting Groups** page.</span></span>

1. <span data-ttu-id="ec648-116">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **FA Posting Groups**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="ec648-116">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **FA Posting Groups**, and then choose the related link.</span></span>
2. <span data-ttu-id="ec648-117">Fill in the **Maintenance Expense Account** field for each posting group.</span><span class="sxs-lookup"><span data-stu-id="ec648-117">Fill in the **Maintenance Expense Account** field for each posting group.</span></span>

> [!NOTE]  
>   <span data-ttu-id="ec648-118">To define that maintenance costs are allocated to departments or projects, set up an allocation keys.</span><span class="sxs-lookup"><span data-stu-id="ec648-118">To define that maintenance costs are allocated to departments or projects, set up an allocation keys.</span></span> <span data-ttu-id="ec648-119">For more information, see [Set Up General Fixed Assets Features](fa-how-setup-general.md).</span><span class="sxs-lookup"><span data-stu-id="ec648-119">For more information, see [Set Up General Fixed Assets Features](fa-how-setup-general.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="ec648-120">See Also</span><span class="sxs-lookup"><span data-stu-id="ec648-120">See Also</span></span>
[<span data-ttu-id="ec648-121">Setting Up Fixed Assets</span><span class="sxs-lookup"><span data-stu-id="ec648-121">Setting Up Fixed Assets</span></span>](fa-setup.md)  
[<span data-ttu-id="ec648-122">Fixed Assets</span><span class="sxs-lookup"><span data-stu-id="ec648-122">Fixed Assets</span></span>](fa-manage.md)  
[<span data-ttu-id="ec648-123">Finance</span><span class="sxs-lookup"><span data-stu-id="ec648-123">Finance</span></span>](finance.md)  
[<span data-ttu-id="ec648-124">Getting Ready for Doing Business</span><span class="sxs-lookup"><span data-stu-id="ec648-124">Getting Ready for Doing Business</span></span>](ui-get-ready-business.md)  
<span data-ttu-id="ec648-125">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="ec648-125">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>


[!INCLUDE[footer-include](includes/footer-banner.md)]