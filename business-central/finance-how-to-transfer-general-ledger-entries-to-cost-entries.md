---
title: How to Transfer General Ledger Entries to Cost Entries | Microsoft Docs
description: You can transfer general ledger entries to cost entries.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 11/13/2018
ms.author: sgroespe
redirect_url: finance-transfer-and-post-cost-entries
ms.openlocfilehash: 273a8c4341f621710819fd5fbc5cb8ce579c86f5
ms.sourcegitcommit: 1bcfaa99ea302e6b84b8361ca02730b135557fc1
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 03/08/2019
ms.locfileid: "822893"
---
# <a name="transfer-general-ledger-entries-to-cost-entries"></a><span data-ttu-id="45e48-103">Transfer General Ledger Entries to Cost Entries</span><span class="sxs-lookup"><span data-stu-id="45e48-103">Transfer General Ledger Entries to Cost Entries</span></span>
<span data-ttu-id="45e48-104">You can transfer general ledger entries to cost entries.</span><span class="sxs-lookup"><span data-stu-id="45e48-104">You can transfer general ledger entries to cost entries.</span></span>  

<span data-ttu-id="45e48-105">Before you run the process for transferring general ledger entries to cost entries, you must prepare the transfer to avoid manual correction posting.</span><span class="sxs-lookup"><span data-stu-id="45e48-105">Before you run the process for transferring general ledger entries to cost entries, you must prepare the transfer to avoid manual correction posting.</span></span>  

## <a name="to-prepare-the-transfer"></a><span data-ttu-id="45e48-106">To prepare the transfer</span><span class="sxs-lookup"><span data-stu-id="45e48-106">To prepare the transfer</span></span>  

1.  <span data-ttu-id="45e48-107">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Cost Accounting Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="45e48-107">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Cost Accounting Setup**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="45e48-108">On the **Cost Accounting Setup** page, verify that the **Starting Date for G/L Transfer** field is set to the correct value.</span><span class="sxs-lookup"><span data-stu-id="45e48-108">On the **Cost Accounting Setup** page, verify that the **Starting Date for G/L Transfer** field is set to the correct value.</span></span>  
3.  <span data-ttu-id="45e48-109">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Chart of Cost Types**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="45e48-109">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Chart of Cost Types**, and then choose the related link.</span></span>  
4.  <span data-ttu-id="45e48-110">On the **Cost Type Card** page, verify that the **G/L Account Range** field is linked correctly for each cost type to take entries from the general ledger.</span><span class="sxs-lookup"><span data-stu-id="45e48-110">On the **Cost Type Card** page, verify that the **G/L Account Range** field is linked correctly for each cost type to take entries from the general ledger.</span></span>  
5.  <span data-ttu-id="45e48-111">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Chart of Accounts**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="45e48-111">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Chart of Accounts**, and then choose the related link.</span></span>  
6.  <span data-ttu-id="45e48-112">For each relevant general ledger account, on the **G/L Account Card** page, verify that the **Cost Type No.**</span><span class="sxs-lookup"><span data-stu-id="45e48-112">For each relevant general ledger account, on the **G/L Account Card** page, verify that the **Cost Type No.**</span></span> <span data-ttu-id="45e48-113">field is linked correctly to a cost type.</span><span class="sxs-lookup"><span data-stu-id="45e48-113">field is linked correctly to a cost type.</span></span> <span data-ttu-id="45e48-114">For more information, see [Setting Up Cost Accounting](finance-set-up-cost-accounting.md).</span><span class="sxs-lookup"><span data-stu-id="45e48-114">For more information, see [Setting Up Cost Accounting](finance-set-up-cost-accounting.md).</span></span>  
7.  <span data-ttu-id="45e48-115">Verify that all relevant general ledger entries have dimension values that correspond to a cost centre and a cost object.</span><span class="sxs-lookup"><span data-stu-id="45e48-115">Verify that all relevant general ledger entries have dimension values that correspond to a cost center and a cost object.</span></span>  

## <a name="to-transfer-general-ledger-entries-to-cost-entries"></a><span data-ttu-id="45e48-116">To transfer general ledger entries to cost entries</span><span class="sxs-lookup"><span data-stu-id="45e48-116">To transfer general ledger entries to cost entries</span></span>  
1.  <span data-ttu-id="45e48-117">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Transfer GL Entries to CA**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="45e48-117">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Transfer GL Entries to CA**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="45e48-118">Choose the **Yes** button to start the transfer.</span><span class="sxs-lookup"><span data-stu-id="45e48-118">Choose the **Yes** button to start the transfer.</span></span> <span data-ttu-id="45e48-119">The process transfers all general ledger entries that have not already been transferred.</span><span class="sxs-lookup"><span data-stu-id="45e48-119">The process transfers all general ledger entries that have not already been transferred.</span></span>  

    <span data-ttu-id="45e48-120">During the transfer, the process creates connections in the entries in the **Cost Entry** table and the **Cost Register** table.</span><span class="sxs-lookup"><span data-stu-id="45e48-120">During the transfer, the process creates connections in the entries in the **Cost Entry** table and the **Cost Register** table.</span></span> <span data-ttu-id="45e48-121">This makes it possible to trace the source of cost entries.</span><span class="sxs-lookup"><span data-stu-id="45e48-121">This makes it possible to trace the source of cost entries.</span></span>  

## <a name="see-also"></a><span data-ttu-id="45e48-122">See Also</span><span class="sxs-lookup"><span data-stu-id="45e48-122">See Also</span></span>  
<span data-ttu-id="45e48-123">[Transferring and Posting Cost Entries](finance-transfer-and-post-cost-entries.md) </span><span class="sxs-lookup"><span data-stu-id="45e48-123">[Transferring and Posting Cost Entries](finance-transfer-and-post-cost-entries.md) </span></span>  
[<span data-ttu-id="45e48-124">Setting Up Cost Accounting</span><span class="sxs-lookup"><span data-stu-id="45e48-124">Setting Up Cost Accounting</span></span>](finance-set-up-cost-accounting.md)   
