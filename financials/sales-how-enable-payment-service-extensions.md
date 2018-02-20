---
title: Enable Customer Payments Through Payment Services| Microsoft Docs
description: Make it easier for customers to pay their invoices by enabling payment services.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: online payment
ms.date: 07/07/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: cfa15ee7b85f1bd01077493d295f230e836239a7
ms.contentlocale: en-nz
ms.lasthandoff: 01/30/2018

---
# <a name="enable-customer-payments-through-payment-services"></a><span data-ttu-id="e6757-103">Enable Customer Payments Through Payment Services</span><span class="sxs-lookup"><span data-stu-id="e6757-103">Enable Customer Payments Through Payment Services</span></span>
<span data-ttu-id="e6757-104">As an alternative to collecting payments through bank transfer or credit cards, your customers can pay you through their account with payment services, such as Microsoft Pay, PayPal, or WorldPay.</span><span class="sxs-lookup"><span data-stu-id="e6757-104">As an alternative to collecting payments through bank transfer or credit cards, your customers can pay you through their account with payment services, such as Microsoft Pay, PayPal, or WorldPay.</span></span>  

<span data-ttu-id="e6757-105">After you enable a payment service in [!INCLUDE[d365fin](includes/d365fin_md.md)], a link to the service is available on sales documents that you send by email to your customers.</span><span class="sxs-lookup"><span data-stu-id="e6757-105">After you enable a payment service in [!INCLUDE[d365fin](includes/d365fin_md.md)], a link to the service is available on sales documents that you send by email to your customers.</span></span> <span data-ttu-id="e6757-106">Customers can use the link to go to the payment service and pay the bill, directly from the sales document.</span><span class="sxs-lookup"><span data-stu-id="e6757-106">Customers can use the link to go to the payment service and pay the bill, directly from the sales document.</span></span> <span data-ttu-id="e6757-107">If you don't want to include the link, for example, if a customer will pay with cash, you can remove the payment service from the invoice before posting.</span><span class="sxs-lookup"><span data-stu-id="e6757-107">If you don't want to include the link, for example, if a customer will pay with cash, you can remove the payment service from the invoice before posting.</span></span>  

<span data-ttu-id="e6757-108">The Microsoft Pay, PayPal Payments Standard, and WorldPay Payments Standard extensions are installed in [!INCLUDE[d365fin](includes/d365fin_md.md)], and are ready for you to enable.</span><span class="sxs-lookup"><span data-stu-id="e6757-108">The Microsoft Pay, PayPal Payments Standard, and WorldPay Payments Standard extensions are installed in [!INCLUDE[d365fin](includes/d365fin_md.md)], and are ready for you to enable.</span></span>  

## <a name="to-enable-a-payment-service-in-included365finincludesd365finmdmd"></a><span data-ttu-id="e6757-109">To enable a payment service in [!INCLUDE[d365fin](includes/d365fin_md.md)]</span><span class="sxs-lookup"><span data-stu-id="e6757-109">To enable a payment service in [!INCLUDE[d365fin](includes/d365fin_md.md)]</span></span>
1. <span data-ttu-id="e6757-110">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Payment Services**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="e6757-110">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Payment Services**, and then choose the related link.</span></span>  
2. <span data-ttu-id="e6757-111">In the **Payment Services** window, choose the **New** action.</span><span class="sxs-lookup"><span data-stu-id="e6757-111">In the **Payment Services** window, choose the **New** action.</span></span>  
3. <span data-ttu-id="e6757-112">Select the payment service, and then close the window.</span><span class="sxs-lookup"><span data-stu-id="e6757-112">Select the payment service, and then close the window.</span></span>  
4. <span data-ttu-id="e6757-113">In the **Payment Services** window, choose the **Setup** action.</span><span class="sxs-lookup"><span data-stu-id="e6757-113">In the **Payment Services** window, choose the **Setup** action.</span></span>  
5. <span data-ttu-id="e6757-114">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="e6757-114">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  
6. <span data-ttu-id="e6757-115">Close the window.</span><span class="sxs-lookup"><span data-stu-id="e6757-115">Close the window.</span></span>  

## <a name="to-select-a-payment-service-on-a-sales-invoice"></a><span data-ttu-id="e6757-116">To select a payment service on a sales invoice</span><span class="sxs-lookup"><span data-stu-id="e6757-116">To select a payment service on a sales invoice</span></span>
1. <span data-ttu-id="e6757-117">On the Home page, choose **Sales Invoices**.</span><span class="sxs-lookup"><span data-stu-id="e6757-117">On the Home page, choose **Sales Invoices**.</span></span>  
2. <span data-ttu-id="e6757-118">Open the sales invoice that you want to pay by using the payment service.</span><span class="sxs-lookup"><span data-stu-id="e6757-118">Open the sales invoice that you want to pay by using the payment service.</span></span>  
3. <span data-ttu-id="e6757-119">In the **Payment Service** field, choose the payment service.</span><span class="sxs-lookup"><span data-stu-id="e6757-119">In the **Payment Service** field, choose the payment service.</span></span>  

    > [!NOTE]  
>   <span data-ttu-id="e6757-120">The **Payment Service** field is available only if you've enabled the payment service.</span><span class="sxs-lookup"><span data-stu-id="e6757-120">The **Payment Service** field is available only if you've enabled the payment service.</span></span>  

## <a name="see-also"></a><span data-ttu-id="e6757-121">See Also</span><span class="sxs-lookup"><span data-stu-id="e6757-121">See Also</span></span>  
[<span data-ttu-id="e6757-122">Setting Up Sales</span><span class="sxs-lookup"><span data-stu-id="e6757-122">Setting Up Sales</span></span>](sales-setup-sales.md)  
[<span data-ttu-id="e6757-123">Sales</span><span class="sxs-lookup"><span data-stu-id="e6757-123">Sales</span></span>](sales-manage-sales.md)  
<span data-ttu-id="e6757-124">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions](ui-extensions.md)</span><span class="sxs-lookup"><span data-stu-id="e6757-124">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions](ui-extensions.md)</span></span>  
<span data-ttu-id="e6757-125">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="e6757-125">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  

