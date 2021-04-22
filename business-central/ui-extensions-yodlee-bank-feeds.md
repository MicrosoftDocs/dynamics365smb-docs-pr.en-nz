---
title: Payment Reconciliation With the Envestnet Yodlee Bank Feeds Extension
description: Describes the Envestnet Yodlee Bank Feeds extension, which links to bank accounts so you can and quickly reconcile payments.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: app, add-in, manifest, customize, stream, bank account link
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 9bdbcc208429bba15e30bc56cc8a4477312c1cdd
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 03/31/2021
ms.locfileid: "5771251"
---
# <a name="the-envestnet-yodlee-bank-feeds-extension"></a><span data-ttu-id="b0cc1-103">The Envestnet Yodlee Bank Feeds Extension</span><span class="sxs-lookup"><span data-stu-id="b0cc1-103">The Envestnet Yodlee Bank Feeds Extension</span></span>

<span data-ttu-id="b0cc1-104">To quickly reconcile payments made to your bank accounts, the Envestnet Yodlee Bank Feeds service allows you to link your system bank account to your online bank account.</span><span class="sxs-lookup"><span data-stu-id="b0cc1-104">To quickly reconcile payments made to your bank accounts, the Envestnet Yodlee Bank Feeds service allows you to link your system bank account to your online bank account.</span></span> <span data-ttu-id="b0cc1-105">This means that the latest bank statement is automatically or manually fed into your reconciliation journal, ensuring that you are always processing the latest payments with minimal risk of errors.</span><span class="sxs-lookup"><span data-stu-id="b0cc1-105">This means that the latest bank statement is automatically or manually fed into your reconciliation journal, ensuring that you are always processing the latest payments with minimal risk of errors.</span></span>

<span data-ttu-id="b0cc1-106">The Envestnet Yodlee Bank Feeds service is only supported in the United States and Canada.</span><span class="sxs-lookup"><span data-stu-id="b0cc1-106">The Envestnet Yodlee Bank Feeds service is only supported in the United States and Canada.</span></span>

> [!NOTE]
> <span data-ttu-id="b0cc1-107">The Envestnet Yodlee Bank Feeds service is only supported in the online version of Business Central.</span><span class="sxs-lookup"><span data-stu-id="b0cc1-107">The Envestnet Yodlee Bank Feeds service is only supported in the online version of Business Central.</span></span> <span data-ttu-id="b0cc1-108">To use this functionality on-premises, you must obtain a cobrand account from Envestnet Yodlee.</span><span class="sxs-lookup"><span data-stu-id="b0cc1-108">To use this functionality on-premises, you must obtain a cobrand account from Envestnet Yodlee.</span></span><br /><br />
> <span data-ttu-id="b0cc1-109">The Envestnet Yodlee Bank Feeds service is only supported in the United States and Canada.</span><span class="sxs-lookup"><span data-stu-id="b0cc1-109">The Envestnet Yodlee Bank Feeds service is only supported in the United States and Canada.</span></span>
> <span data-ttu-id="b0cc1-110">Only banks residing in these countries are supported, even though banks from other countries may appear in the Envestnet Yodlee Bank Feeds bank selection window in [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="b0cc1-110">Only banks residing in these countries are supported, even though banks from other countries may appear in the Envestnet Yodlee Bank Feeds bank selection window in [!INCLUDE[prod_short](includes/prod_short.md)].</span></span>

> [!IMPORTANT]
> <span data-ttu-id="b0cc1-111">Due to the new Payment Services Directive in Europe (PSD2), after September 14, 2019, you will no longer be able to automatically import bank statements from banks in the United Kingdom into [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="b0cc1-111">Due to the new Payment Services Directive in Europe (PSD2), after September 14, 2019, you will no longer be able to automatically import bank statements from banks in the United Kingdom into [!INCLUDE[prod_short](includes/prod_short.md)].</span></span> <span data-ttu-id="b0cc1-112">We are looking into the possibility of offering this feature again in the future.</span><span class="sxs-lookup"><span data-stu-id="b0cc1-112">We are looking into the possibility of offering this feature again in the future.</span></span>

<span data-ttu-id="b0cc1-113">The Envestnet Yodlee Bank Feeds service provides the following benefits:</span><span class="sxs-lookup"><span data-stu-id="b0cc1-113">The Envestnet Yodlee Bank Feeds service provides the following benefits:</span></span>

* <span data-ttu-id="b0cc1-114">Removes the need for manual entry.</span><span class="sxs-lookup"><span data-stu-id="b0cc1-114">Removes the need for manual entry.</span></span>
* <span data-ttu-id="b0cc1-115">Improves efficiency and accuracy when doing payment reconciliation.</span><span class="sxs-lookup"><span data-stu-id="b0cc1-115">Improves efficiency and accuracy when doing payment reconciliation.</span></span>
* <span data-ttu-id="b0cc1-116">Supports a large number of banks.</span><span class="sxs-lookup"><span data-stu-id="b0cc1-116">Supports a large number of banks.</span></span>
* <span data-ttu-id="b0cc1-117">Allows up-to-date information about bank transactions from within [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="b0cc1-117">Allows up-to-date information about bank transactions from within [!INCLUDE[prod_short](includes/prod_short.md)].</span></span>
* <span data-ttu-id="b0cc1-118">Supports manual as well as automatic bank feeds.</span><span class="sxs-lookup"><span data-stu-id="b0cc1-118">Supports manual as well as automatic bank feeds.</span></span>
* <span data-ttu-id="b0cc1-119">Enables outsourcing of payment reconciliation to an accountant by providing access to bank statements.</span><span class="sxs-lookup"><span data-stu-id="b0cc1-119">Enables outsourcing of payment reconciliation to an accountant by providing access to bank statements.</span></span>

## <a name="available-bank-feeds"></a><span data-ttu-id="b0cc1-120">Available Bank Feeds</span><span class="sxs-lookup"><span data-stu-id="b0cc1-120">Available Bank Feeds</span></span>
<span data-ttu-id="b0cc1-121">You can check whether a bank is supported by setting up and connecting to the Envestnet Yodlee Bank Feeds service.</span><span class="sxs-lookup"><span data-stu-id="b0cc1-121">You can check whether a bank is supported by setting up and connecting to the Envestnet Yodlee Bank Feeds service.</span></span> <span data-ttu-id="b0cc1-122">The bank will appear on the list if it is supported by Envestnet Yodlee.</span><span class="sxs-lookup"><span data-stu-id="b0cc1-122">The bank will appear on the list if it is supported by Envestnet Yodlee.</span></span>

<span data-ttu-id="b0cc1-123">For more information, see [Set Up the Envestnet Yodlee Bank Feeds Service](bank-how-setup-bank-statement-service.md).</span><span class="sxs-lookup"><span data-stu-id="b0cc1-123">For more information, see [Set Up the Envestnet Yodlee Bank Feeds Service](bank-how-setup-bank-statement-service.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="b0cc1-124">See Also</span><span class="sxs-lookup"><span data-stu-id="b0cc1-124">See Also</span></span>
<span data-ttu-id="b0cc1-125">[Customising [!INCLUDE[prod_short](includes/prod_short.md)] Using Extensions ](ui-extensions.md)  </span><span class="sxs-lookup"><span data-stu-id="b0cc1-125">[Customizing [!INCLUDE[prod_short](includes/prod_short.md)] Using Extensions ](ui-extensions.md)  </span></span>  
[<span data-ttu-id="b0cc1-126">Applying Payments Automatically and Reconciling Bank Accounts</span><span class="sxs-lookup"><span data-stu-id="b0cc1-126">Applying Payments Automatically and Reconciling Bank Accounts</span></span>](receivables-apply-payments-auto-reconcile-bank-accounts.md)  
<span data-ttu-id="b0cc1-127">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="b0cc1-127">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>


[!INCLUDE[footer-include](includes/footer-banner.md)]