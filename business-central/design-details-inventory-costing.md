---
title: Design Details - Inventory Costing | Microsoft Docs
description: This documentation provides detailed technical insight to the concepts and principles that are used within the Inventory Costing features in Business Central.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: design, inventory, costing
ms.date: 10/01/2018
ms.author: sgroespe
ms.openlocfilehash: 830c14eb96557f8852d0a4758922503fe0179b58
ms.sourcegitcommit: 1bcfaa99ea302e6b84b8361ca02730b135557fc1
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 03/08/2019
ms.locfileid: "822375"
---
# <a name="design-details-inventory-costing"></a><span data-ttu-id="091db-103">Design Details: Inventory Costing</span><span class="sxs-lookup"><span data-stu-id="091db-103">Design Details: Inventory Costing</span></span>
<span data-ttu-id="091db-104">This documentation provides detailed technical insight to the concepts and principles that are used within the Inventory Costing features in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="091db-104">This documentation provides detailed technical insight to the concepts and principles that are used within the Inventory Costing features in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  

<span data-ttu-id="091db-105">Inventory costing, also referred to as cost management, is concerned with recording and reporting business operating costs.</span><span class="sxs-lookup"><span data-stu-id="091db-105">Inventory costing, also referred to as cost management, is concerned with recording and reporting business operating costs.</span></span>  

## <a name="in-this-section"></a><span data-ttu-id="091db-106">In This Section</span><span class="sxs-lookup"><span data-stu-id="091db-106">In This Section</span></span>  
[<span data-ttu-id="091db-107">Design Details: Costing Methods</span><span class="sxs-lookup"><span data-stu-id="091db-107">Design Details: Costing Methods</span></span>](design-details-costing-methods.md)  
[<span data-ttu-id="091db-108">Design Details: Item Application</span><span class="sxs-lookup"><span data-stu-id="091db-108">Design Details: Item Application</span></span>](design-details-item-application.md)  
[<span data-ttu-id="091db-109">Design Details: Known Item Application Issue</span><span class="sxs-lookup"><span data-stu-id="091db-109">Design Details: Known Item Application Issue</span></span>](design-details-inventory-zero-level-open-item-ledger-entries.md)  
[<span data-ttu-id="091db-110">Design Details: Cost Adjustment</span><span class="sxs-lookup"><span data-stu-id="091db-110">Design Details: Cost Adjustment</span></span>](design-details-cost-adjustment.md)  
[<span data-ttu-id="091db-111">Design Details: Posting Date on Adjustment Value Entry</span><span class="sxs-lookup"><span data-stu-id="091db-111">Design Details: Posting Date on Adjustment Value Entry</span></span>](design-details-inventory-adjustment-value-entry-posting-date.md)  
[<span data-ttu-id="091db-112">Design Details: Expected Cost Posting</span><span class="sxs-lookup"><span data-stu-id="091db-112">Design Details: Expected Cost Posting</span></span>](design-details-expected-cost-posting.md)  
[<span data-ttu-id="091db-113">Design Details: Average Cost</span><span class="sxs-lookup"><span data-stu-id="091db-113">Design Details: Average Cost</span></span>](design-details-average-cost.md)  
[<span data-ttu-id="091db-114">Design Details: Variance</span><span class="sxs-lookup"><span data-stu-id="091db-114">Design Details: Variance</span></span>](design-details-variance.md)  
[<span data-ttu-id="091db-115">Design Details: Rounding</span><span class="sxs-lookup"><span data-stu-id="091db-115">Design Details: Rounding</span></span>](design-details-rounding.md)  
[<span data-ttu-id="091db-116">Design Details: Cost Components</span><span class="sxs-lookup"><span data-stu-id="091db-116">Design Details: Cost Components</span></span>](design-details-cost-components.md)  
[<span data-ttu-id="091db-117">Design Details: Inventory Periods</span><span class="sxs-lookup"><span data-stu-id="091db-117">Design Details: Inventory Periods</span></span>](design-details-inventory-periods.md)  
[<span data-ttu-id="091db-118">Design Details: Inventory Posting</span><span class="sxs-lookup"><span data-stu-id="091db-118">Design Details: Inventory Posting</span></span>](design-details-inventory-posting.md)  
[<span data-ttu-id="091db-119">Design Details: Production Order Posting</span><span class="sxs-lookup"><span data-stu-id="091db-119">Design Details: Production Order Posting</span></span>](design-details-production-order-posting.md)  
[<span data-ttu-id="091db-120">Design Details: Assembly Order Posting</span><span class="sxs-lookup"><span data-stu-id="091db-120">Design Details: Assembly Order Posting</span></span>](design-details-assembly-order-posting.md)  
[<span data-ttu-id="091db-121">Design Details: Reconciliation with the General Ledger</span><span class="sxs-lookup"><span data-stu-id="091db-121">Design Details: Reconciliation with the General Ledger</span></span>](design-details-reconciliation-with-the-general-ledger.md)  
<span data-ttu-id="091db-122">[Design Details: Accounts in the General Ledger](design-details-accounts-in-the-general-ledger.md)
[Design Details: Inventory Valuation](design-details-inventory-valuation.md)</span><span class="sxs-lookup"><span data-stu-id="091db-122">[Design Details: Accounts in the General Ledger](design-details-accounts-in-the-general-ledger.md)
[Design Details: Inventory Valuation](design-details-inventory-valuation.md)</span></span>  
[<span data-ttu-id="091db-123">Design Details: Revaluation</span><span class="sxs-lookup"><span data-stu-id="091db-123">Design Details: Revaluation</span></span>](design-details-revaluation.md)
