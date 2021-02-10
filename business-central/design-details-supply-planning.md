---
title: Design Details - Supply Planning | Microsoft Docs
description: This topic provides an overview of the the concepts and principles that are used within the Supply Planning features in Business Central.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: design, supply, planning, reordering, replenishment
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: ed874c647dd5c3526df38a3c4d6ee43293737786
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 12/17/2020
ms.locfileid: "4751096"
---
# <a name="design-details-supply-planning"></a><span data-ttu-id="fb352-103">Design Details: Supply Planning</span><span class="sxs-lookup"><span data-stu-id="fb352-103">Design Details: Supply Planning</span></span>
<span data-ttu-id="fb352-104">This documentation provides detailed technical insight to the concepts and principles that are used within the Supply Planning features in [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="fb352-104">This documentation provides detailed technical insight to the concepts and principles that are used within the Supply Planning features in [!INCLUDE[prod_short](includes/prod_short.md)].</span></span>  

<span data-ttu-id="fb352-105">It explains how the planning system works and how to adjust the algorithms to meet planning requirements in different environments.</span><span class="sxs-lookup"><span data-stu-id="fb352-105">It explains how the planning system works and how to adjust the algorithms to meet planning requirements in different environments.</span></span> <span data-ttu-id="fb352-106">It first introduces central solution concepts and then describes the logic of the central mechanism, supply balancing, before proceeding to explain how inventory planning is performed with the use of reordering policies.</span><span class="sxs-lookup"><span data-stu-id="fb352-106">It first introduces central solution concepts and then describes the logic of the central mechanism, supply balancing, before proceeding to explain how inventory planning is performed with the use of reordering policies.</span></span>  

## <a name="in-this-section"></a><span data-ttu-id="fb352-107">In This Section</span><span class="sxs-lookup"><span data-stu-id="fb352-107">In This Section</span></span>  
[<span data-ttu-id="fb352-108">Design Details: Central Concepts of the Planning System</span><span class="sxs-lookup"><span data-stu-id="fb352-108">Design Details: Central Concepts of the Planning System</span></span>](design-details-central-concepts-of-the-planning-system.md)  
[<span data-ttu-id="fb352-109">Design Details: Reservation, Order Tracking, and Action Messaging</span><span class="sxs-lookup"><span data-stu-id="fb352-109">Design Details: Reservation, Order Tracking, and Action Messaging</span></span>](design-details-reservation-order-tracking-and-action-messaging.md)  
[<span data-ttu-id="fb352-110">Design Details: Balancing Demand and Supply</span><span class="sxs-lookup"><span data-stu-id="fb352-110">Design Details: Balancing Demand and Supply</span></span>](design-details-balancing-demand-and-supply.md)  
[<span data-ttu-id="fb352-111">Design Details: Handling Reordering Policies</span><span class="sxs-lookup"><span data-stu-id="fb352-111">Design Details: Handling Reordering Policies</span></span>](design-details-handling-reordering-policies.md)  
[<span data-ttu-id="fb352-112">Design Details: Planning Parameters</span><span class="sxs-lookup"><span data-stu-id="fb352-112">Design Details: Planning Parameters</span></span>](design-details-planning-parameters.md)  
[<span data-ttu-id="fb352-113">Design Details: Planning Assignment Table</span><span class="sxs-lookup"><span data-stu-id="fb352-113">Design Details: Planning Assignment Table</span></span>](design-details-planning-assignment-table.md)  
[<span data-ttu-id="fb352-114">Design Details: Demand at Blank Location</span><span class="sxs-lookup"><span data-stu-id="fb352-114">Design Details: Demand at Blank Location</span></span>](design-details-demand-at-blank-location.md)  
[<span data-ttu-id="fb352-115">Design Details: Transfers in Planning</span><span class="sxs-lookup"><span data-stu-id="fb352-115">Design Details: Transfers in Planning</span></span>](design-details-transfers-in-planning.md)
