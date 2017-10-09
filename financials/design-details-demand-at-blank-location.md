---
title: Design Details - Demand and Supply | Microsoft Docs
description: This topic introduces the concept of demand, which is the common term used for any kind of gross demand, such as a sales order and component need from a production order.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: design, demand, supply, inventory, planning
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 69d5e574b390fe50490ff98616983a5e9ea31d94
ms.contentlocale: en-nz
ms.lasthandoff: 09/22/2017

---
# <a name="design-details-demand-and-supply"></a><span data-ttu-id="8a0f8-103">Design Details: Demand and Supply</span><span class="sxs-lookup"><span data-stu-id="8a0f8-103">Design Details: Demand and Supply</span></span>
<span data-ttu-id="8a0f8-104">Demand is the common term used for any kind of gross demand, such as a sales order and component need from a production order.</span><span class="sxs-lookup"><span data-stu-id="8a0f8-104">Demand is the common term used for any kind of gross demand, such as a sales order and component need from a production order.</span></span> <span data-ttu-id="8a0f8-105">In addition, the program allows more technical types of demand, such as negative inventory and purchase returns.</span><span class="sxs-lookup"><span data-stu-id="8a0f8-105">In addition, the program allows more technical types of demand, such as negative inventory and purchase returns.</span></span>  
  
<span data-ttu-id="8a0f8-106">Supply is the common term used for any kind of positive or inbound quantity, such as inventory, purchases, assembly, production, or inbound transfers.</span><span class="sxs-lookup"><span data-stu-id="8a0f8-106">Supply is the common term used for any kind of positive or inbound quantity, such as inventory, purchases, assembly, production, or inbound transfers.</span></span> <span data-ttu-id="8a0f8-107">In addition, a sales return may also represent supply.</span><span class="sxs-lookup"><span data-stu-id="8a0f8-107">In addition, a sales return may also represent supply.</span></span>  
  
<span data-ttu-id="8a0f8-108">To sort out the many sources of demand and supply, the planning system organises them on two time lines called inventory profiles.</span><span class="sxs-lookup"><span data-stu-id="8a0f8-108">To sort out the many sources of demand and supply, the planning system organizes them on two time lines called inventory profiles.</span></span> <span data-ttu-id="8a0f8-109">One profile holds demand events, and the other holds the corresponding supply events.</span><span class="sxs-lookup"><span data-stu-id="8a0f8-109">One profile holds demand events, and the other holds the corresponding supply events.</span></span> <span data-ttu-id="8a0f8-110">Each event represents one order network entity, such as a sales order line, an item ledger entry, or a production order line.</span><span class="sxs-lookup"><span data-stu-id="8a0f8-110">Each event represents one order network entity, such as a sales order line, an item ledger entry, or a production order line.</span></span>  
  
<span data-ttu-id="8a0f8-111">When inventory profiles are loaded, the different demand-supply sets are balanced to output a supply plan that fulfills the listed goals.</span><span class="sxs-lookup"><span data-stu-id="8a0f8-111">When inventory profiles are loaded, the different demand-supply sets are balanced to output a supply plan that fulfills the listed goals.</span></span>  
  
<span data-ttu-id="8a0f8-112">Planning parameters and inventory levels are other types of demand and supply respectively, which undergo integrated balancing to replenish stock items.</span><span class="sxs-lookup"><span data-stu-id="8a0f8-112">Planning parameters and inventory levels are other types of demand and supply respectively, which undergo integrated balancing to replenish stock items.</span></span> <span data-ttu-id="8a0f8-113">For more information, see [Design Details: Handling Reordering Policies](design-details-handling-reordering-policies.md).</span><span class="sxs-lookup"><span data-stu-id="8a0f8-113">For more information, see [Design Details: Handling Reordering Policies](design-details-handling-reordering-policies.md).</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="8a0f8-114">See Also</span><span class="sxs-lookup"><span data-stu-id="8a0f8-114">See Also</span></span>  
<span data-ttu-id="8a0f8-115">[Design Details: Balancing Demand and Supply](design-details-balancing-demand-and-supply.md) </span><span class="sxs-lookup"><span data-stu-id="8a0f8-115">[Design Details: Balancing Demand and Supply](design-details-balancing-demand-and-supply.md) </span></span>  
<span data-ttu-id="8a0f8-116">[Design Details: Central Concepts of the Planning System](design-details-central-concepts-of-the-planning-system.md) </span><span class="sxs-lookup"><span data-stu-id="8a0f8-116">[Design Details: Central Concepts of the Planning System](design-details-central-concepts-of-the-planning-system.md) </span></span>  
[<span data-ttu-id="8a0f8-117">Design Details: Supply Planning</span><span class="sxs-lookup"><span data-stu-id="8a0f8-117">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)
