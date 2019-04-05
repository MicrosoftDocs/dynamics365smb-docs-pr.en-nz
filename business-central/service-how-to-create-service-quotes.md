---
title: How to Create Service Quotes | Microsoft Docs
description: You can use the **Service Quote** page to create documents where you enter information about a service, such as repairs and maintenance, on service items by customer request. You can use a service quote as a preliminary draft for a service order, and then convert the quote to a service order.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2018
ms.author: sgroespe
ms.openlocfilehash: 1486be71b0b848aa48996f4161f8987322a09e32
ms.sourcegitcommit: 1bcfaa99ea302e6b84b8361ca02730b135557fc1
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 03/08/2019
ms.locfileid: "821714"
---
# <a name="create-service-quotes"></a><span data-ttu-id="ad96c-104">Create Service Quotes</span><span class="sxs-lookup"><span data-stu-id="ad96c-104">Create Service Quotes</span></span>
<span data-ttu-id="ad96c-105">You can think of service quotes as the basis for service orders.</span><span class="sxs-lookup"><span data-stu-id="ad96c-105">You can think of service quotes as the basis for service orders.</span></span> <span data-ttu-id="ad96c-106">In fact, they are almost identical.</span><span class="sxs-lookup"><span data-stu-id="ad96c-106">In fact, they are almost identical.</span></span> <span data-ttu-id="ad96c-107">They both contain information such as who the customer is, the type of order, the item that needs service, billing and shipping information, and information about the actual service work.</span><span class="sxs-lookup"><span data-stu-id="ad96c-107">They both contain information such as who the customer is, the type of order, the item that needs service, billing and shipping information, and information about the actual service work.</span></span>
 
<span data-ttu-id="ad96c-108">You can use a service quote as a preliminary draft for a service order, and then convert the quote to a service order.</span><span class="sxs-lookup"><span data-stu-id="ad96c-108">You can use a service quote as a preliminary draft for a service order, and then convert the quote to a service order.</span></span>  
  
## <a name="to-create-a-service-quote"></a><span data-ttu-id="ad96c-109">To create a service quote</span><span class="sxs-lookup"><span data-stu-id="ad96c-109">To create a service quote</span></span>  
1. <span data-ttu-id="ad96c-110">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Service Quotes**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="ad96c-110">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Service Quotes**, and then choose the related link.</span></span>  
2. <span data-ttu-id="ad96c-111">Create a new service quote.</span><span class="sxs-lookup"><span data-stu-id="ad96c-111">Create a new service quote.</span></span>  
3. <span data-ttu-id="ad96c-112">In the **No.**</span><span class="sxs-lookup"><span data-stu-id="ad96c-112">In the **No.**</span></span> <span data-ttu-id="ad96c-113">field, enter a number for the service quote.</span><span class="sxs-lookup"><span data-stu-id="ad96c-113">field, enter a number for the service quote.</span></span> <span data-ttu-id="ad96c-114">Alternatively, if you have set up a number series for service quotes on the **Service Mgt. Setup** page, you can press Enter to select the next available service quote number.</span><span class="sxs-lookup"><span data-stu-id="ad96c-114">Alternatively, if you have set up a number series for service quotes on the **Service Mgt. Setup** page, you can press Enter to select the next available service quote number.</span></span>  
4. <span data-ttu-id="ad96c-115">In the **Customer No.**</span><span class="sxs-lookup"><span data-stu-id="ad96c-115">In the **Customer No.**</span></span>  <span data-ttu-id="ad96c-116">field, select the relevant customer from the list.</span><span class="sxs-lookup"><span data-stu-id="ad96c-116">field, select the relevant customer from the list.</span></span>  

  > [!Note]  
  >  <span data-ttu-id="ad96c-117">The customer fields are filled in automatically with information from the **Customer** card.</span><span class="sxs-lookup"><span data-stu-id="ad96c-117">The customer fields are filled in automatically with information from the **Customer** card.</span></span> <span data-ttu-id="ad96c-118">If a **Customer** card does not exist for the customer, and you have set up a customer template, you can create the customer from the service quote.</span><span class="sxs-lookup"><span data-stu-id="ad96c-118">If a **Customer** card does not exist for the customer, and you have set up a customer template, you can create the customer from the service quote.</span></span> <span data-ttu-id="ad96c-119">Fill in the relevant fields, and then choose the **Create Customer** action.</span><span class="sxs-lookup"><span data-stu-id="ad96c-119">Fill in the relevant fields, and then choose the **Create Customer** action.</span></span>  
  
5. <span data-ttu-id="ad96c-120">Depending on the settings on the **Mandatory Fields** FastTab on the **Service Mgt. Setup** page, you may need to fill in the **Service Order Type** field and the **Salesperson Code** field.</span><span class="sxs-lookup"><span data-stu-id="ad96c-120">Depending on the settings on the **Mandatory Fields** FastTab on the **Service Mgt. Setup** page, you may need to fill in the **Service Order Type** field and the **Salesperson Code** field.</span></span>  
6. <span data-ttu-id="ad96c-121">Fill in the service item lines.</span><span class="sxs-lookup"><span data-stu-id="ad96c-121">Fill in the service item lines.</span></span>  
7. <span data-ttu-id="ad96c-122">Register estimated costs on the service lines.</span><span class="sxs-lookup"><span data-stu-id="ad96c-122">Register estimated costs on the service lines.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="ad96c-123">See Also</span><span class="sxs-lookup"><span data-stu-id="ad96c-123">See Also</span></span>  
[<span data-ttu-id="ad96c-124">Create Service Orders</span><span class="sxs-lookup"><span data-stu-id="ad96c-124">Create Service Orders</span></span>](service-how-to-create-service-orders.md)  
[<span data-ttu-id="ad96c-125">Work on Service tasks</span><span class="sxs-lookup"><span data-stu-id="ad96c-125">Work on Service tasks</span></span>](service-how-to-work-on-service-tasks.md)  

 