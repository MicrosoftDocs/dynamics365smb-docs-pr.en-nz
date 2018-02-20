---
title: Automatic Transfer and Combined Entries | Microsoft Docs
description: In cost accounting, you can transfer general ledger entries to a cost type by using a combined posting. You can specify if a cost type receives combined entries in the **Combine Entries** field in the cost type definition. The following table describes the different options.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: f4796d9796788d2fbbf5706688aec75a4ed9a6d8
ms.contentlocale: en-nz
ms.lasthandoff: 01/30/2018

---
# <a name="automatic-transfer-and-combined-entries"></a><span data-ttu-id="9ad62-105">Automatic Transfer and Combined Entries</span><span class="sxs-lookup"><span data-stu-id="9ad62-105">Automatic Transfer and Combined Entries</span></span>
<span data-ttu-id="9ad62-106">In cost accounting, you can transfer general ledger entries to a cost type by using a combined posting.</span><span class="sxs-lookup"><span data-stu-id="9ad62-106">In cost accounting, you can transfer general ledger entries to a cost type by using a combined posting.</span></span> <span data-ttu-id="9ad62-107">You can specify if a cost type receives combined entries in the **Combine Entries** field in the cost type definition.</span><span class="sxs-lookup"><span data-stu-id="9ad62-107">You can specify if a cost type receives combined entries in the **Combine Entries** field in the cost type definition.</span></span> <span data-ttu-id="9ad62-108">The following table describes the different options.</span><span class="sxs-lookup"><span data-stu-id="9ad62-108">The following table describes the different options.</span></span>  

|<span data-ttu-id="9ad62-109">Combine entries</span><span class="sxs-lookup"><span data-stu-id="9ad62-109">Combine entries</span></span>|<span data-ttu-id="9ad62-110">Description</span><span class="sxs-lookup"><span data-stu-id="9ad62-110">Description</span></span>|  
|---------------------|-----------------|  
|<span data-ttu-id="9ad62-111">None</span><span class="sxs-lookup"><span data-stu-id="9ad62-111">None</span></span>|<span data-ttu-id="9ad62-112">Each general ledger entry is transferred individually to the corresponding cost type.</span><span class="sxs-lookup"><span data-stu-id="9ad62-112">Each general ledger entry is transferred individually to the corresponding cost type.</span></span>|  
|<span data-ttu-id="9ad62-113">Day</span><span class="sxs-lookup"><span data-stu-id="9ad62-113">Day</span></span>|<span data-ttu-id="9ad62-114">General ledger entries with the same posting date are transferred as one entry to the corresponding cost type.</span><span class="sxs-lookup"><span data-stu-id="9ad62-114">General ledger entries with the same posting date are transferred as one entry to the corresponding cost type.</span></span>|  
|<span data-ttu-id="9ad62-115">Month</span><span class="sxs-lookup"><span data-stu-id="9ad62-115">Month</span></span>|<span data-ttu-id="9ad62-116">All general ledger entries in the same calendar month are transferred as one entry to the corresponding cost type.</span><span class="sxs-lookup"><span data-stu-id="9ad62-116">All general ledger entries in the same calendar month are transferred as one entry to the corresponding cost type.</span></span>|  

> [!IMPORTANT]  
>  <span data-ttu-id="9ad62-117">If you have selected the **Auto Transfer from G/L** check box in the **Cost Accounting Setup** window, [!INCLUDE[d365fin](includes/d365fin_md.md)] updates the cost accounting after every posting in the general ledger.</span><span class="sxs-lookup"><span data-stu-id="9ad62-117">If you have selected the **Auto Transfer from G/L** check box in the **Cost Accounting Setup** window, [!INCLUDE[d365fin](includes/d365fin_md.md)] updates the cost accounting after every posting in the general ledger.</span></span> <span data-ttu-id="9ad62-118">Combined entries are not possible.</span><span class="sxs-lookup"><span data-stu-id="9ad62-118">Combined entries are not possible.</span></span>  

## <a name="see-also"></a><span data-ttu-id="9ad62-119">See Also</span><span class="sxs-lookup"><span data-stu-id="9ad62-119">See Also</span></span>  
 <span data-ttu-id="9ad62-120">[Transfer General Ledger Entries to Cost Entries](finance-how-to-transfer-general-ledger-entries-to-cost-entries.md) </span><span class="sxs-lookup"><span data-stu-id="9ad62-120">[Transfer General Ledger Entries to Cost Entries](finance-how-to-transfer-general-ledger-entries-to-cost-entries.md) </span></span>  
 <span data-ttu-id="9ad62-121">[Criteria for Transferring General Ledger Entries to Cost Entries](finance-criteria-for-transferring-general-ledger-entries-to-cost-entries.md) </span><span class="sxs-lookup"><span data-stu-id="9ad62-121">[Criteria for Transferring General Ledger Entries to Cost Entries](finance-criteria-for-transferring-general-ledger-entries-to-cost-entries.md) </span></span>  
 <span data-ttu-id="9ad62-122">[Results of the Transfer](finance-results-of-the-transfer.md) </span><span class="sxs-lookup"><span data-stu-id="9ad62-122">[Results of the Transfer](finance-results-of-the-transfer.md) </span></span>  
 [<span data-ttu-id="9ad62-123">Transferring and Posting Cost Entries</span><span class="sxs-lookup"><span data-stu-id="9ad62-123">Transferring and Posting Cost Entries</span></span>](finance-transfer-and-post-cost-entries.md)  
 <span data-ttu-id="9ad62-124">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="9ad62-124">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

