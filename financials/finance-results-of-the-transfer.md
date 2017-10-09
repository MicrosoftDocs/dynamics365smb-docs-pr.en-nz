---
title: Results of the Transfer | Microsoft Docs
description: This topic describes what happens after you transfer general ledger entries to cost entries.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: general ledger, transfer, cost entries
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 9f1c3573137d7cd15c8b98813da514f8b8f2e1cd
ms.contentlocale: en-nz
ms.lasthandoff: 09/22/2017

---
# <a name="results-of-transferring-general-ledger-entries-to-cost-entries"></a><span data-ttu-id="56a41-103">Results of Transferring General Ledger Entries to Cost Entries</span><span class="sxs-lookup"><span data-stu-id="56a41-103">Results of Transferring General Ledger Entries to Cost Entries</span></span>
<span data-ttu-id="56a41-104">During the transfer of general ledger entries to cost entries, [!INCLUDE[d365fin](includes/d365fin_md.md)] creates connections in the entries in the **G/L Entry** table, the **Cost Entry** table, and the **Cost Register** table to make it possible to trace the connections between cost entries and general ledger entries.</span><span class="sxs-lookup"><span data-stu-id="56a41-104">During the transfer of general ledger entries to cost entries, [!INCLUDE[d365fin](includes/d365fin_md.md)] creates connections in the entries in the **G/L Entry** table, the **Cost Entry** table, and the **Cost Register** table to make it possible to trace the connections between cost entries and general ledger entries.</span></span>  

## <a name="general-ledger-entries"></a><span data-ttu-id="56a41-105">General Ledger Entries</span><span class="sxs-lookup"><span data-stu-id="56a41-105">General Ledger Entries</span></span>  
<span data-ttu-id="56a41-106">For each general ledger entry that is transferred to cost accounting, [!INCLUDE[d365fin](includes/d365fin_md.md)] fills the cost **Entry No.** field.</span><span class="sxs-lookup"><span data-stu-id="56a41-106">For each general ledger entry that is transferred to cost accounting, [!INCLUDE[d365fin](includes/d365fin_md.md)] fills the cost **Entry No.** field.</span></span>  

## <a name="cost-entries"></a><span data-ttu-id="56a41-107">Cost Entries</span><span class="sxs-lookup"><span data-stu-id="56a41-107">Cost Entries</span></span>  
<span data-ttu-id="56a41-108">For each cost entry, [!INCLUDE[d365fin](includes/d365fin_md.md)] saves the entry number of the corresponding general ledger entry in the **G/L Entry No.** field in the **Cost Entry** table.</span><span class="sxs-lookup"><span data-stu-id="56a41-108">For each cost entry, [!INCLUDE[d365fin](includes/d365fin_md.md)] saves the entry number of the corresponding general ledger entry in the **G/L Entry No.** field in the **Cost Entry** table.</span></span>  

<span data-ttu-id="56a41-109">For combined cost entries, [!INCLUDE[d365fin](includes/d365fin_md.md)] saves the entry number of the last general ledger entry, which is the entry with the highest entry number.</span><span class="sxs-lookup"><span data-stu-id="56a41-109">For combined cost entries, [!INCLUDE[d365fin](includes/d365fin_md.md)] saves the entry number of the last general ledger entry, which is the entry with the highest entry number.</span></span>  

<span data-ttu-id="56a41-110">The **G/L Account** field in the **Cost Entry** table contains the number of the general ledger account that the cost entry came from.</span><span class="sxs-lookup"><span data-stu-id="56a41-110">The **G/L Account** field in the **Cost Entry** table contains the number of the general ledger account that the cost entry came from.</span></span>  

<span data-ttu-id="56a41-111">For single cost entries, [!INCLUDE[d365fin](includes/d365fin_md.md)] transfers the posting text from the general ledger entry to the **Description** text field.</span><span class="sxs-lookup"><span data-stu-id="56a41-111">For single cost entries, [!INCLUDE[d365fin](includes/d365fin_md.md)] transfers the posting text from the general ledger entry to the **Description** text field.</span></span> <span data-ttu-id="56a41-112">For combined entries, the text field shows these entries are transferred as combined entries.</span><span class="sxs-lookup"><span data-stu-id="56a41-112">For combined entries, the text field shows these entries are transferred as combined entries.</span></span> <span data-ttu-id="56a41-113">For example, for a combined entry for the month of October in 2013, the text can be **Combined Entries, October 2013**.</span><span class="sxs-lookup"><span data-stu-id="56a41-113">For example, for a combined entry for the month of October in 2013, the text can be **Combined Entries, October 2013**.</span></span>  

## <a name="cost-register"></a><span data-ttu-id="56a41-114">Cost Register</span><span class="sxs-lookup"><span data-stu-id="56a41-114">Cost Register</span></span>  
<span data-ttu-id="56a41-115">In the **Cost Register** table, [!INCLUDE[d365fin](includes/d365fin_md.md)] creates an entry with the source transfer from general ledger.</span><span class="sxs-lookup"><span data-stu-id="56a41-115">In the **Cost Register** table, [!INCLUDE[d365fin](includes/d365fin_md.md)] creates an entry with the source transfer from general ledger.</span></span> <span data-ttu-id="56a41-116">The entry records the first and last entry numbers of the general ledger entries that are transferred, in addition to the first and last entry numbers of the cost entries that are created.</span><span class="sxs-lookup"><span data-stu-id="56a41-116">The entry records the first and last entry numbers of the general ledger entries that are transferred, in addition to the first and last entry numbers of the cost entries that are created.</span></span>  

## <a name="see-also"></a><span data-ttu-id="56a41-117">See Also</span><span class="sxs-lookup"><span data-stu-id="56a41-117">See Also</span></span>  
<span data-ttu-id="56a41-118">[How to: Transfer General Ledger Entries to Cost Entries](finance-how-to-transfer-general-ledger-entries-to-cost-entries.md) </span><span class="sxs-lookup"><span data-stu-id="56a41-118">[How to: Transfer General Ledger Entries to Cost Entries](finance-how-to-transfer-general-ledger-entries-to-cost-entries.md) </span></span>  
<span data-ttu-id="56a41-119">[Criteria for Transferring General Ledger Entries to Cost Entries](finance-criteria-for-transferring-general-ledger-entries-to-cost-entries.md) </span><span class="sxs-lookup"><span data-stu-id="56a41-119">[Criteria for Transferring General Ledger Entries to Cost Entries](finance-criteria-for-transferring-general-ledger-entries-to-cost-entries.md) </span></span>  
<span data-ttu-id="56a41-120">[Automatic Transfer and Combined Entries](finance-automatic-transfer-combined-entries.md) </span><span class="sxs-lookup"><span data-stu-id="56a41-120">[Automatic Transfer and Combined Entries](finance-automatic-transfer-combined-entries.md) </span></span>  
[<span data-ttu-id="56a41-121">Transferring and Posting Cost Entries</span><span class="sxs-lookup"><span data-stu-id="56a41-121">Transferring and Posting Cost Entries</span></span>](finance-transfer-and-post-cost-entries.md)  

