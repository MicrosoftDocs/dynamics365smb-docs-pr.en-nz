---
title: How to Set Up Cash Customers | Microsoft Docs
description: This topic describes the steps to set up customer who pays in cash.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: f047876678d26e7e53bf304433f38a410ba7d7fa
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 03/31/2021
ms.locfileid: "5770407"
---
# <a name="set-up-cash-customers"></a><span data-ttu-id="2f4dd-103">Set Up Cash Customers</span><span class="sxs-lookup"><span data-stu-id="2f4dd-103">Set Up Cash Customers</span></span>
<span data-ttu-id="2f4dd-104">You cannot create an invoice without a customer number.</span><span class="sxs-lookup"><span data-stu-id="2f4dd-104">You cannot create an invoice without a customer number.</span></span> <span data-ttu-id="2f4dd-105">This is true, even if you make a cash sale and do not have anything to record in a customer account.</span><span class="sxs-lookup"><span data-stu-id="2f4dd-105">This is true, even if you make a cash sale and do not have anything to record in a customer account.</span></span>  

## <a name="to-set-up-a-cash-customer"></a><span data-ttu-id="2f4dd-106">To set up a cash customer</span><span class="sxs-lookup"><span data-stu-id="2f4dd-106">To set up a cash customer</span></span>  
1.  <span data-ttu-id="2f4dd-107">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Customer**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="2f4dd-107">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Customer**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="2f4dd-108">Create a new **Customer** card.</span><span class="sxs-lookup"><span data-stu-id="2f4dd-108">Create a new **Customer** card.</span></span> <span data-ttu-id="2f4dd-109">For more information, see [Register New Customers](sales-how-register-new-customers.md).</span><span class="sxs-lookup"><span data-stu-id="2f4dd-109">For more information, see [Register New Customers](sales-how-register-new-customers.md).</span></span>
3.  <span data-ttu-id="2f4dd-110">In the **No.**</span><span class="sxs-lookup"><span data-stu-id="2f4dd-110">In the **No.**</span></span> <span data-ttu-id="2f4dd-111">field, enter **Cash**, for example.</span><span class="sxs-lookup"><span data-stu-id="2f4dd-111">field, enter **Cash**, for example.</span></span>  
4.  <span data-ttu-id="2f4dd-112">In the **Name** field, enter **Cash Sale**, for example.</span><span class="sxs-lookup"><span data-stu-id="2f4dd-112">In the **Name** field, enter **Cash Sale**, for example.</span></span>  
5.  <span data-ttu-id="2f4dd-113">On the **Invoicing** FastTab, fill in the **Customer Posting Group** and the **Gen. Bus. Posting Group** fields.</span><span class="sxs-lookup"><span data-stu-id="2f4dd-113">On the **Invoicing** FastTab, fill in the **Customer Posting Group** and the **Gen. Bus. Posting Group** fields.</span></span>  

 <span data-ttu-id="2f4dd-114">Now you have set up a customer that contains sufficient information for invoicing.</span><span class="sxs-lookup"><span data-stu-id="2f4dd-114">Now you have set up a customer that contains sufficient information for invoicing.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="2f4dd-115">You may have chosen a posting group that is also used for domestic credit sales.</span><span class="sxs-lookup"><span data-stu-id="2f4dd-115">You may have chosen a posting group that is also used for domestic credit sales.</span></span> <span data-ttu-id="2f4dd-116">If you want to maintain separate data on cash sales, for example, with a special sales or receivables account, you can set up an extra posting group for this purpose.</span><span class="sxs-lookup"><span data-stu-id="2f4dd-116">If you want to maintain separate data on cash sales, for example, with a special sales or receivables account, you can set up an extra posting group for this purpose.</span></span>  
>   
>  <span data-ttu-id="2f4dd-117">You must enter a number for a receivables account for the posting group, even though the balance in this account will always be 0 after you post an invoice.</span><span class="sxs-lookup"><span data-stu-id="2f4dd-117">You must enter a number for a receivables account for the posting group, even though the balance in this account will always be 0 after you post an invoice.</span></span>  

## <a name="see-also"></a><span data-ttu-id="2f4dd-118">See Also</span><span class="sxs-lookup"><span data-stu-id="2f4dd-118">See Also</span></span>
[<span data-ttu-id="2f4dd-119">Managing Receivables</span><span class="sxs-lookup"><span data-stu-id="2f4dd-119">Managing Receivables</span></span>](receivables-manage-receivables.md)  
<span data-ttu-id="2f4dd-120">[Register New Customers](sales-how-register-new-customers.md)  </span><span class="sxs-lookup"><span data-stu-id="2f4dd-120">[Register New Customers](sales-how-register-new-customers.md)  </span></span>  
[<span data-ttu-id="2f4dd-121">Finance</span><span class="sxs-lookup"><span data-stu-id="2f4dd-121">Finance</span></span>](finance.md)  



[!INCLUDE[footer-include](includes/footer-banner.md)]