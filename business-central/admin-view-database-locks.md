---
title: View Database Locks
description: Learn how you can view information about any database locks right from the client interface in Business Central.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 04/01/2021
ms.author: jswymer
ms.openlocfilehash: b53677ab57d6c48b015bb0dd47ea6e315f8e80c3
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 03/31/2021
ms.locfileid: "5776932"
---
# <a name="viewing-database-locks"></a><span data-ttu-id="86d93-103">Viewing Database Locks</span><span class="sxs-lookup"><span data-stu-id="86d93-103">Viewing Database Locks</span></span>

<span data-ttu-id="86d93-104">Database locking controls access by multiple users to the same data at the same time.</span><span class="sxs-lookup"><span data-stu-id="86d93-104">Database locking controls access by multiple users to the same data at the same time.</span></span> <span data-ttu-id="86d93-105">To protect a transaction against other transactions modifying the same data, the first transaction puts a lock on the data.</span><span class="sxs-lookup"><span data-stu-id="86d93-105">To protect a transaction against other transactions modifying the same data, the first transaction puts a lock on the data.</span></span> <span data-ttu-id="86d93-106">The lock remains until the transaction's done.</span><span class="sxs-lookup"><span data-stu-id="86d93-106">The lock remains until the transaction's done.</span></span>

<span data-ttu-id="86d93-107">Users may be blocked from completing transactions on the locked data.</span><span class="sxs-lookup"><span data-stu-id="86d93-107">Users may be blocked from completing transactions on the locked data.</span></span> <span data-ttu-id="86d93-108">They'll typically get a message that indicates the lock condition.</span><span class="sxs-lookup"><span data-stu-id="86d93-108">They'll typically get a message that indicates the lock condition.</span></span>

## <a name="to-view-database-locks"></a><span data-ttu-id="86d93-109">To view database locks</span><span class="sxs-lookup"><span data-stu-id="86d93-109">To view database locks</span></span>

<span data-ttu-id="86d93-110">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Database Locks**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="86d93-110">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Database Locks**, and then choose the related link.</span></span>

<span data-ttu-id="86d93-111">The **Database Locks** page gives snapshot of all current database locks.</span><span class="sxs-lookup"><span data-stu-id="86d93-111">The **Database Locks** page gives snapshot of all current database locks.</span></span>

<span data-ttu-id="86d93-112">For more information about database locking, see [Monitoring Database Locks](/dynamics365/business-central/dev-itpro/administration/monitor-database-locks) in the Business Central Developer and IT Pro help.</span><span class="sxs-lookup"><span data-stu-id="86d93-112">For more information about database locking, see [Monitoring Database Locks](/dynamics365/business-central/dev-itpro/administration/monitor-database-locks) in the Business Central Developer and IT Pro help.</span></span>

## <a name="see-also"></a><span data-ttu-id="86d93-113">See Also</span><span class="sxs-lookup"><span data-stu-id="86d93-113">See Also</span></span>

[<span data-ttu-id="86d93-114">Monitor Database Locks</span><span class="sxs-lookup"><span data-stu-id="86d93-114">Monitor Database Locks</span></span>](/dynamics365/business-central/dev-itpro/administration/monitor-database-locks) 


[!INCLUDE[footer-include](includes/footer-banner.md)]