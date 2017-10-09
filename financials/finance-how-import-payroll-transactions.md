---
title: Import Payroll Transactions| Microsoft Docs
description: To manage salary, you import and post financial transactions from your payroll provider to the general ledger, using a payroll extension such as Ceridian or Quickbooks.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: Ceridian, Quickbooks, salary
ms.date: 06/16/2017
ms.author: SorenGP
ms.translationtype: HT
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: d53dfb26a3fea663e68a3b558579a59184e9de26
ms.contentlocale: en-nz
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-import-payroll-transactions"></a><span data-ttu-id="d5941-103">How to: Import Payroll Transactions </span><span class="sxs-lookup"><span data-stu-id="d5941-103">How to: Import Payroll Transactions</span></span>
<span data-ttu-id="d5941-104">To account for salary payments and related transactions, you must import and post financial transactions made by your payroll provider to the general ledger.</span><span class="sxs-lookup"><span data-stu-id="d5941-104">To account for salary payments and related transactions, you must import and post financial transactions made by your payroll provider to the general ledger.</span></span> <span data-ttu-id="d5941-105">To do this, you first import a file that you receive from the payroll provider into the **General Journal** window.</span><span class="sxs-lookup"><span data-stu-id="d5941-105">To do this, you first import a file that you receive from the payroll provider into the **General Journal** window.</span></span> <span data-ttu-id="d5941-106">Then you map the external accounts in the payroll file to the relevant G/L accounts.</span><span class="sxs-lookup"><span data-stu-id="d5941-106">Then you map the external accounts in the payroll file to the relevant G/L accounts.</span></span> <span data-ttu-id="d5941-107">Lastly, you post the payroll transactions according to the account mapping.</span><span class="sxs-lookup"><span data-stu-id="d5941-107">Lastly, you post the payroll transactions according to the account mapping.</span></span>

> [!NOTE]  
>   <span data-ttu-id="d5941-108">To use this functionality, an extension for payroll import must be installed and enabled.</span><span class="sxs-lookup"><span data-stu-id="d5941-108">To use this functionality, an extension for payroll import must be installed and enabled.</span></span> <span data-ttu-id="d5941-109">The Ceridian Payroll and the Quickbooks Payroll File Import extensions are pre-installed in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="d5941-109">The Ceridian Payroll and the Quickbooks Payroll File Import extensions are pre-installed in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="d5941-110">For more information, see [Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions](ui-extensions.md).</span><span class="sxs-lookup"><span data-stu-id="d5941-110">For more information, see [Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions](ui-extensions.md).</span></span>

## <a name="to-import-a-payroll-file"></a><span data-ttu-id="d5941-111">To import a payroll file</span><span class="sxs-lookup"><span data-stu-id="d5941-111">To import a payroll file</span></span>
1. <span data-ttu-id="d5941-112">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **General Journals**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="d5941-112">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **General Journals**, and then choose the related link.</span></span>
2. <span data-ttu-id="d5941-113">In the relevant general journal batch, choose the **Import Payroll Transactions** action.</span><span class="sxs-lookup"><span data-stu-id="d5941-113">In the relevant general journal batch, choose the **Import Payroll Transactions** action.</span></span> <span data-ttu-id="d5941-114">An assisted setup guide opens.</span><span class="sxs-lookup"><span data-stu-id="d5941-114">An assisted setup guide opens.</span></span>
3. <span data-ttu-id="d5941-115">Follow the steps in the **Import Payroll Transactions** window.</span><span class="sxs-lookup"><span data-stu-id="d5941-115">Follow the steps in the **Import Payroll Transactions** window.</span></span>

    > [!TIP]  
>   <span data-ttu-id="d5941-116">In the step about mapping the external payroll records to your G/L accounts, the mappings that you make will be remembered next time the same records are imported.</span><span class="sxs-lookup"><span data-stu-id="d5941-116">In the step about mapping the external payroll records to your G/L accounts, the mappings that you make will be remembered next time the same records are imported.</span></span> <span data-ttu-id="d5941-117">This will save you time as you do not have to manually fill in the **Account No.** field in the general journal every time you have imported recurring payroll transactions.</span><span class="sxs-lookup"><span data-stu-id="d5941-117">This will save you time as you do not have to manually fill in the **Account No.** field in the general journal every time you have imported recurring payroll transactions.</span></span>   

    <span data-ttu-id="d5941-118">When you choose the **OK** button in the assisted setup guide, the **General Journal** window is filled with lines representing the transactions that the payroll file contains and with the relevant accounts prefilled in the **G/L Account** fields according to mappings you made in the guide.</span><span class="sxs-lookup"><span data-stu-id="d5941-118">When you choose the **OK** button in the assisted setup guide, the **General Journal** window is filled with lines representing the transactions that the payroll file contains and with the relevant accounts prefilled in the **G/L Account** fields according to mappings you made in the guide.</span></span>
4. <span data-ttu-id="d5941-119">Edit or post the journal lines as for any other general ledger transactions.</span><span class="sxs-lookup"><span data-stu-id="d5941-119">Edit or post the journal lines as for any other general ledger transactions.</span></span> <span data-ttu-id="d5941-120">For more information, see [How to: Post Transactions Directly to the General Ledger](finance-how-post-transactions-directly.md).</span><span class="sxs-lookup"><span data-stu-id="d5941-120">For more information, see [How to: Post Transactions Directly to the General Ledger](finance-how-post-transactions-directly.md).</span></span>   

## <a name="see-also"></a><span data-ttu-id="d5941-121">See Also</span><span class="sxs-lookup"><span data-stu-id="d5941-121">See Also</span></span>
[<span data-ttu-id="d5941-122">Finance</span><span class="sxs-lookup"><span data-stu-id="d5941-122">Finance</span></span>](finance.md)  
<span data-ttu-id="d5941-123">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions](ui-extensions.md)</span><span class="sxs-lookup"><span data-stu-id="d5941-123">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions](ui-extensions.md)</span></span>  
[<span data-ttu-id="d5941-124">Working with General Journals</span><span class="sxs-lookup"><span data-stu-id="d5941-124">Working with General Journals</span></span>](ui-work-general-journals.md)  

