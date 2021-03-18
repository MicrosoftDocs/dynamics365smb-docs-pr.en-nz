---
title: How to Create Service Quotes | Microsoft Docs
description: You can use the **Service Quote** page to create documents where you enter information about a service, such as repairs and maintenance, on service items by customer request. You can use a service quote as a preliminary draft for a service order, and then convert the quote to a service order.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 92c93b2e0b876920f1c259d31b4d839a5b2ecbc0
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "5388815"
---
# <a name="create-service-quotes"></a><span data-ttu-id="ace2c-104">Create Service Quotes</span><span class="sxs-lookup"><span data-stu-id="ace2c-104">Create Service Quotes</span></span>
<span data-ttu-id="ace2c-105">You can think of service quotes as the basis for service orders.</span><span class="sxs-lookup"><span data-stu-id="ace2c-105">You can think of service quotes as the basis for service orders.</span></span> <span data-ttu-id="ace2c-106">In fact, they are almost identical.</span><span class="sxs-lookup"><span data-stu-id="ace2c-106">In fact, they are almost identical.</span></span> <span data-ttu-id="ace2c-107">They both contain information such as who the customer is, the type of order, the item that needs service, billing and shipping information, and information about the actual service work.</span><span class="sxs-lookup"><span data-stu-id="ace2c-107">They both contain information such as who the customer is, the type of order, the item that needs service, billing and shipping information, and information about the actual service work.</span></span>
 
<span data-ttu-id="ace2c-108">You can use a service quote as a preliminary draft for a service order, and then convert the quote to a service order.</span><span class="sxs-lookup"><span data-stu-id="ace2c-108">You can use a service quote as a preliminary draft for a service order, and then convert the quote to a service order.</span></span>  
  
## <a name="to-create-a-service-quote"></a><span data-ttu-id="ace2c-109">To create a service quote</span><span class="sxs-lookup"><span data-stu-id="ace2c-109">To create a service quote</span></span>  
1. <span data-ttu-id="ace2c-110">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Service Quotes**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="ace2c-110">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Service Quotes**, and then choose the related link.</span></span>  
2. <span data-ttu-id="ace2c-111">Create a new service quote.</span><span class="sxs-lookup"><span data-stu-id="ace2c-111">Create a new service quote.</span></span>  
3. <span data-ttu-id="ace2c-112">In the **No.**</span><span class="sxs-lookup"><span data-stu-id="ace2c-112">In the **No.**</span></span> <span data-ttu-id="ace2c-113">field, enter a number for the service quote.</span><span class="sxs-lookup"><span data-stu-id="ace2c-113">field, enter a number for the service quote.</span></span> <span data-ttu-id="ace2c-114">Alternatively, if you have set up a number series for service quotes on the **Service Mgt. Setup** page, you can press Enter to select the next available service quote number.</span><span class="sxs-lookup"><span data-stu-id="ace2c-114">Alternatively, if you have set up a number series for service quotes on the **Service Mgt. Setup** page, you can press Enter to select the next available service quote number.</span></span>  
4. <span data-ttu-id="ace2c-115">In the **Customer No.**</span><span class="sxs-lookup"><span data-stu-id="ace2c-115">In the **Customer No.**</span></span>  <span data-ttu-id="ace2c-116">field, select the relevant customer from the list.</span><span class="sxs-lookup"><span data-stu-id="ace2c-116">field, select the relevant customer from the list.</span></span>  

  > [!Note]  
  >  <span data-ttu-id="ace2c-117">The customer fields are filled in automatically with information from the **Customer** card.</span><span class="sxs-lookup"><span data-stu-id="ace2c-117">The customer fields are filled in automatically with information from the **Customer** card.</span></span> <span data-ttu-id="ace2c-118">If a **Customer** card does not exist for the customer, and you have set up a customer template, you can create the customer from the service quote.</span><span class="sxs-lookup"><span data-stu-id="ace2c-118">If a **Customer** card does not exist for the customer, and you have set up a customer template, you can create the customer from the service quote.</span></span> <span data-ttu-id="ace2c-119">Fill in the relevant fields, and then choose the **Create Customer** action.</span><span class="sxs-lookup"><span data-stu-id="ace2c-119">Fill in the relevant fields, and then choose the **Create Customer** action.</span></span>  
  
5. <span data-ttu-id="ace2c-120">Depending on the settings on the **Mandatory Fields** FastTab on the **Service Mgt. Setup** page, you may need to fill in the **Service Order Type** field and the **Salesperson Code** field.</span><span class="sxs-lookup"><span data-stu-id="ace2c-120">Depending on the settings on the **Mandatory Fields** FastTab on the **Service Mgt. Setup** page, you may need to fill in the **Service Order Type** field and the **Salesperson Code** field.</span></span>  
6. <span data-ttu-id="ace2c-121">Fill in the service item lines.</span><span class="sxs-lookup"><span data-stu-id="ace2c-121">Fill in the service item lines.</span></span>  
7. <span data-ttu-id="ace2c-122">Register estimated costs on the service lines.</span><span class="sxs-lookup"><span data-stu-id="ace2c-122">Register estimated costs on the service lines.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="ace2c-123">See Also</span><span class="sxs-lookup"><span data-stu-id="ace2c-123">See Also</span></span>  
[<span data-ttu-id="ace2c-124">Create Service Orders</span><span class="sxs-lookup"><span data-stu-id="ace2c-124">Create Service Orders</span></span>](service-how-to-create-service-orders.md)  
[<span data-ttu-id="ace2c-125">Work on Service tasks</span><span class="sxs-lookup"><span data-stu-id="ace2c-125">Work on Service tasks</span></span>](service-how-to-work-on-service-tasks.md)  

 

[!INCLUDE[footer-include](includes/footer-banner.md)]