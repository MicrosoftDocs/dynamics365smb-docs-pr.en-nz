---
title: How to Create Service Quotes | Microsoft Docs
description: You can use the **Service Quote** window to create documents where you enter information about a service, such as repairs and maintenance, on service items by customer request. You can use a service quote as a preliminary draft for a service order, and then convert the quote to a service order.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 91928287d24c2b6199ea243bdc00e48e136adcfd
ms.contentlocale: en-nz
ms.lasthandoff: 03/22/2018

---
# <a name="create-service-quotes"></a><span data-ttu-id="4e56e-104">Create Service Quotes</span><span class="sxs-lookup"><span data-stu-id="4e56e-104">Create Service Quotes</span></span>
<span data-ttu-id="4e56e-105">You can think of service quotes as the basis for service orders.</span><span class="sxs-lookup"><span data-stu-id="4e56e-105">You can think of service quotes as the basis for service orders.</span></span> <span data-ttu-id="4e56e-106">In fact, they are almost identical.</span><span class="sxs-lookup"><span data-stu-id="4e56e-106">In fact, they are almost identical.</span></span> <span data-ttu-id="4e56e-107">They both contain information such as who the customer is, the type of order, the item that needs service, billing and shipping information, and information about the actual service work.</span><span class="sxs-lookup"><span data-stu-id="4e56e-107">They both contain information such as who the customer is, the type of order, the item that needs service, billing and shipping information, and information about the actual service work.</span></span>
 
<span data-ttu-id="4e56e-108">You can use a service quote as a preliminary draft for a service order, and then convert the quote to a service order.</span><span class="sxs-lookup"><span data-stu-id="4e56e-108">You can use a service quote as a preliminary draft for a service order, and then convert the quote to a service order.</span></span>  
  
## <a name="to-create-a-service-quote"></a><span data-ttu-id="4e56e-109">To create a service quote</span><span class="sxs-lookup"><span data-stu-id="4e56e-109">To create a service quote</span></span>  
1. <span data-ttu-id="4e56e-110">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Service Quotes**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="4e56e-110">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Service Quotes**, and then choose the related link.</span></span>  
2. <span data-ttu-id="4e56e-111">Create a new service quote.</span><span class="sxs-lookup"><span data-stu-id="4e56e-111">Create a new service quote.</span></span>  
3. <span data-ttu-id="4e56e-112">In the **No.**</span><span class="sxs-lookup"><span data-stu-id="4e56e-112">In the **No.**</span></span> <span data-ttu-id="4e56e-113">field, enter a number for the service quote.</span><span class="sxs-lookup"><span data-stu-id="4e56e-113">field, enter a number for the service quote.</span></span> <span data-ttu-id="4e56e-114">Alternatively, if you have set up a number series for service quotes in the **Service Mgt. Setup** window, you can press Enter to select the next available service quote number.</span><span class="sxs-lookup"><span data-stu-id="4e56e-114">Alternatively, if you have set up a number series for service quotes in the **Service Mgt. Setup** window, you can press Enter to select the next available service quote number.</span></span>  
4. <span data-ttu-id="4e56e-115">In the **Customer No.**</span><span class="sxs-lookup"><span data-stu-id="4e56e-115">In the **Customer No.**</span></span>  <span data-ttu-id="4e56e-116">field, select the relevant customer from the list.</span><span class="sxs-lookup"><span data-stu-id="4e56e-116">field, select the relevant customer from the list.</span></span>  

  > [!Note]  
  >  <span data-ttu-id="4e56e-117">The customer fields are filled in automatically with information from the **Customer** card.</span><span class="sxs-lookup"><span data-stu-id="4e56e-117">The customer fields are filled in automatically with information from the **Customer** card.</span></span> <span data-ttu-id="4e56e-118">If a **Customer** card does not exist for the customer, and you have set up a customer template, you can create the customer from the service quote.</span><span class="sxs-lookup"><span data-stu-id="4e56e-118">If a **Customer** card does not exist for the customer, and you have set up a customer template, you can create the customer from the service quote.</span></span> <span data-ttu-id="4e56e-119">Fill in the relevant fields, and then choose the **Create Customer** action.</span><span class="sxs-lookup"><span data-stu-id="4e56e-119">Fill in the relevant fields, and then choose the **Create Customer** action.</span></span>  
  
5. <span data-ttu-id="4e56e-120">Depending on the settings on the **Mandatory Fields** FastTab in the **Service Mgt. Setup** window, you may need to fill in the **Service Order Type** field and the **Salesperson Code** field.</span><span class="sxs-lookup"><span data-stu-id="4e56e-120">Depending on the settings on the **Mandatory Fields** FastTab in the **Service Mgt. Setup** window, you may need to fill in the **Service Order Type** field and the **Salesperson Code** field.</span></span>  
6. <span data-ttu-id="4e56e-121">Fill in the service item lines.</span><span class="sxs-lookup"><span data-stu-id="4e56e-121">Fill in the service item lines.</span></span>  
7. <span data-ttu-id="4e56e-122">Register estimated costs on the service lines.</span><span class="sxs-lookup"><span data-stu-id="4e56e-122">Register estimated costs on the service lines.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="4e56e-123">See Also</span><span class="sxs-lookup"><span data-stu-id="4e56e-123">See Also</span></span>  
[<span data-ttu-id="4e56e-124">Create Service Orders</span><span class="sxs-lookup"><span data-stu-id="4e56e-124">Create Service Orders</span></span>](service-how-to-create-service-orders.md)  
[<span data-ttu-id="4e56e-125">Work on Service tasks</span><span class="sxs-lookup"><span data-stu-id="4e56e-125">Work on Service tasks</span></span>](service-how-to-work-on-service-tasks.md)  

 
