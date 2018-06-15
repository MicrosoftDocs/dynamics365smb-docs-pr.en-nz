---
title: Set up the Chart of Accounts
description: You change the default accounts in the chart of accounts (COA), and you can add new accounts.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: COA, cha of acc
ms.date: 04/16/2018
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: ad1b888d475c0523c5a905e804a3f89ab4531b28
ms.openlocfilehash: 9f84af8bb4ac3be9132ab621906c463cfc9b91ff
ms.contentlocale: en-nz
ms.lasthandoff: 05/17/2018

---
# <a name="setting-up-or-changing-the-chart-of-accounts"></a><span data-ttu-id="1cf76-103">Setting Up or Changing the Chart of Accounts</span><span class="sxs-lookup"><span data-stu-id="1cf76-103">Setting Up or Changing the Chart of Accounts</span></span>
<span data-ttu-id="1cf76-104">The chart of accounts shows the ledger accounts that store your financial data.</span><span class="sxs-lookup"><span data-stu-id="1cf76-104">The chart of accounts shows the ledger accounts that store your financial data.</span></span> [!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="1cf76-105"> includes a standard chart of accounts that is ready to support your business.</span><span class="sxs-lookup"><span data-stu-id="1cf76-105"> includes a standard chart of accounts that is ready to support your business.</span></span>
<span data-ttu-id="1cf76-106">However, you can change the default accounts, and you can add new accounts.</span><span class="sxs-lookup"><span data-stu-id="1cf76-106">However, you can change the default accounts, and you can add new accounts.</span></span>  

## <a name="adding-or-changing-accounts"></a><span data-ttu-id="1cf76-107">Adding or Changing Accounts</span><span class="sxs-lookup"><span data-stu-id="1cf76-107">Adding or Changing Accounts</span></span>
<span data-ttu-id="1cf76-108">From the chart of accounts, you can open each G/L account and add or change settings.</span><span class="sxs-lookup"><span data-stu-id="1cf76-108">From the chart of accounts, you can open each G/L account and add or change settings.</span></span>

> [!NOTE]  
>   <span data-ttu-id="1cf76-109">You can delete a general ledger account.</span><span class="sxs-lookup"><span data-stu-id="1cf76-109">You can delete a general ledger account.</span></span> <span data-ttu-id="1cf76-110">However, before you delete it, the following must be true:</span><span class="sxs-lookup"><span data-stu-id="1cf76-110">However, before you delete it, the following must be true:</span></span>  

* <span data-ttu-id="1cf76-111">The balance on the account must be zero.</span><span class="sxs-lookup"><span data-stu-id="1cf76-111">The balance on the account must be zero.</span></span>  
* <span data-ttu-id="1cf76-112">The **Allow G/L Acc. Deletion Before** field must be set in the **General Ledger Setup** window, and the account must not have ledger entries on or after that date.</span><span class="sxs-lookup"><span data-stu-id="1cf76-112">The **Allow G/L Acc. Deletion Before** field must be set in the **General Ledger Setup** window, and the account must not have ledger entries on or after that date.</span></span>  
* <span data-ttu-id="1cf76-113">If the **Check G/L Account Usage** field in the **General Ledger Setup** window is selected, then the account must not be used in any posting groups or posting setup.</span><span class="sxs-lookup"><span data-stu-id="1cf76-113">If the **Check G/L Account Usage** field in the **General Ledger Setup** window is selected, then the account must not be used in any posting groups or posting setup.</span></span>  

[!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="1cf76-114"> will prevent you from deleting a general ledger account that stores data that is needed in the chart of accounts.</span><span class="sxs-lookup"><span data-stu-id="1cf76-114"> will prevent you from deleting a general ledger account that stores data that is needed in the chart of accounts.</span></span>  

## <a name="see-also"></a><span data-ttu-id="1cf76-115">See Also</span><span class="sxs-lookup"><span data-stu-id="1cf76-115">See Also</span></span>
[<span data-ttu-id="1cf76-116">The General Ledger and the Chart of Accounts</span><span class="sxs-lookup"><span data-stu-id="1cf76-116">The General Ledger and the Chart of Accounts</span></span>](finance-general-ledger.md)  
[<span data-ttu-id="1cf76-117">Managing Bank Accounts</span><span class="sxs-lookup"><span data-stu-id="1cf76-117">Managing Bank Accounts</span></span>](bank-manage-bank-accounts.md)  
[<span data-ttu-id="1cf76-118">Working with Dimensions</span><span class="sxs-lookup"><span data-stu-id="1cf76-118">Working with Dimensions</span></span>](finance-dimensions.md)  
<span data-ttu-id="1cf76-119">[Importing Data from Other Finance Systems](across-import-data-configuration-packages.md)(across-import-data-configuration-packages.md)</span><span class="sxs-lookup"><span data-stu-id="1cf76-119">[Importing Data from Other Finance Systems](across-import-data-configuration-packages.md)(across-import-data-configuration-packages.md)</span></span>  
[<span data-ttu-id="1cf76-120">Work with Account Schedules</span><span class="sxs-lookup"><span data-stu-id="1cf76-120">Work with Account Schedules</span></span>](bi-how-work-account-schedule.md)  
<span data-ttu-id="1cf76-121">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="1cf76-121">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  

## [!INCLUDE[d365fin](includes/free_trial_md.md)]

