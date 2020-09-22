---
title: Microsoft Pay Standard| Microsoft Docs
description: Provides information about the Microsoft Pay extension
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 04/01/2020
ms.author: edupont
ms.openlocfilehash: 82e5cc8ba4b9335b8282857b564f9dcb3050fca0
ms.sourcegitcommit: a80afd4e5075018716efad76d82a54e158f1392d
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 09/09/2020
ms.locfileid: "3784802"
---
# <a name="the-microsoft-pay-extension"></a><span data-ttu-id="caa6c-103">The Microsoft Pay Extension</span><span class="sxs-lookup"><span data-stu-id="caa6c-103">The Microsoft Pay Extension</span></span>

> [!IMPORTANT]
> <span data-ttu-id="caa6c-104">Effective February 8 2020, changes in the Microsoft Pay service will affect the Microsoft Pay extension in Microsoft [!INCLUDE[d365fin](includes/d365fin_long_md.md)].</span><span class="sxs-lookup"><span data-stu-id="caa6c-104">Effective February 8 2020, changes in the Microsoft Pay service will affect the Microsoft Pay extension in Microsoft [!INCLUDE[d365fin](includes/d365fin_long_md.md)].</span></span> <span data-ttu-id="caa6c-105">Due to the changes, after February 8, the **Pay now** payment links that the Microsoft Pay extension generates for invoices in [!INCLUDE[d365fin](includes/d365fin_md.md)] will not open Microsoft Pay.</span><span class="sxs-lookup"><span data-stu-id="caa6c-105">Due to the changes, after February 8, the **Pay now** payment links that the Microsoft Pay extension generates for invoices in [!INCLUDE[d365fin](includes/d365fin_md.md)] will not open Microsoft Pay.</span></span> <span data-ttu-id="caa6c-106">Customers who are using the extension should change their Payment Services setup to start using the PayPal extension instead.</span><span class="sxs-lookup"><span data-stu-id="caa6c-106">Customers who are using the extension should change their Payment Services setup to start using the PayPal extension instead.</span></span><br /></br>
>
> <span data-ttu-id="caa6c-107">From January 8, we will display a notification in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="caa6c-107">From January 8, we will display a notification in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="caa6c-108">The notification will contain a link to the settings that you need to change and to more information.</span><span class="sxs-lookup"><span data-stu-id="caa6c-108">The notification will contain a link to the settings that you need to change and to more information.</span></span> <span data-ttu-id="caa6c-109">After February 8, the Microsoft Pay extension will no longer be available in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="caa6c-109">After February 8, the Microsoft Pay extension will no longer be available in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span><br /></br>
>
> <span data-ttu-id="caa6c-110">The changes impact the following versions of Business Central:</span><span class="sxs-lookup"><span data-stu-id="caa6c-110">The changes impact the following versions of Business Central:</span></span>
> - <span data-ttu-id="caa6c-111">Microsoft Dynamics 365 Business Central October 2018</span><span class="sxs-lookup"><span data-stu-id="caa6c-111">Microsoft Dynamics 365 Business Central October 2018</span></span>
> - <span data-ttu-id="caa6c-112">Microsoft Dynamics 365 Business Central April 2019</span><span class="sxs-lookup"><span data-stu-id="caa6c-112">Microsoft Dynamics 365 Business Central April 2019</span></span>
> - <span data-ttu-id="caa6c-113">Microsoft Dynamics 365 Business Central 2019 Release Wave 2</span><span class="sxs-lookup"><span data-stu-id="caa6c-113">Microsoft Dynamics 365 Business Central 2019 Release Wave 2</span></span>

<span data-ttu-id="caa6c-114">Customers continuously require higher customer service, both in terms of the quality of product but also in terms of delivery and payment services.</span><span class="sxs-lookup"><span data-stu-id="caa6c-114">Customers continuously require higher customer service, both in terms of the quality of product but also in terms of delivery and payment services.</span></span> <span data-ttu-id="caa6c-115">The Microsoft Pay service helps you increase your customer service.</span><span class="sxs-lookup"><span data-stu-id="caa6c-115">The Microsoft Pay service helps you increase your customer service.</span></span>

<span data-ttu-id="caa6c-116">The Microsoft Pay extension adds a Microsoft Pay link to your sales documents so customers can easily pay using Microsoft Pay.</span><span class="sxs-lookup"><span data-stu-id="caa6c-116">The Microsoft Pay extension adds a Microsoft Pay link to your sales documents so customers can easily pay using Microsoft Pay.</span></span> <span data-ttu-id="caa6c-117">Then you can send the documents by email to provide higher customer service and shorten the time it takes for customers’ payments to arrive on your bank account.</span><span class="sxs-lookup"><span data-stu-id="caa6c-117">Then you can send the documents by email to provide higher customer service and shorten the time it takes for customers’ payments to arrive on your bank account.</span></span>

<span data-ttu-id="caa6c-118">The Microsoft Pay extension provides the following benefits:</span><span class="sxs-lookup"><span data-stu-id="caa6c-118">The Microsoft Pay extension provides the following benefits:</span></span>
- <span data-ttu-id="caa6c-119">Customer payments appear faster on your bank account.</span><span class="sxs-lookup"><span data-stu-id="caa6c-119">Customer payments appear faster on your bank account.</span></span>
- <span data-ttu-id="caa6c-120">Customers have more ways to pay invoices.</span><span class="sxs-lookup"><span data-stu-id="caa6c-120">Customers have more ways to pay invoices.</span></span>
- <span data-ttu-id="caa6c-121">Microsoft Pay offers a trustworthy payment service, which customers prefer to entering credit card information on unknown web sites.</span><span class="sxs-lookup"><span data-stu-id="caa6c-121">Microsoft Pay offers a trustworthy payment service, which customers prefer to entering credit card information on unknown web sites.</span></span>
- <span data-ttu-id="caa6c-122">Microsoft Pay offers multiple ways of handling payments, including credit card processing, such as PayPal and Stripe.</span><span class="sxs-lookup"><span data-stu-id="caa6c-122">Microsoft Pay offers multiple ways of handling payments, including credit card processing, such as PayPal and Stripe.</span></span>
- <span data-ttu-id="caa6c-123">The Microsoft Pay link can be embedded automatically on every invoice document or by the user.</span><span class="sxs-lookup"><span data-stu-id="caa6c-123">The Microsoft Pay link can be embedded automatically on every invoice document or by the user.</span></span>
- <span data-ttu-id="caa6c-124">Because this functionality is built as an extension, it gives you full control to enable it when and if your business processes require it.</span><span class="sxs-lookup"><span data-stu-id="caa6c-124">Because this functionality is built as an extension, it gives you full control to enable it when and if your business processes require it.</span></span>

<span data-ttu-id="caa6c-125">Enabling payment service extensions is free in [!INCLUDE[d365fin](includes/d365fin_md.md)], however, you will need to contact the payment service to get an account.</span><span class="sxs-lookup"><span data-stu-id="caa6c-125">Enabling payment service extensions is free in [!INCLUDE[d365fin](includes/d365fin_md.md)], however, you will need to contact the payment service to get an account.</span></span> <span data-ttu-id="caa6c-126">For more information, see [Enable Customer Payment Through Payment Services](sales-how-enable-payment-service-extensions.md).</span><span class="sxs-lookup"><span data-stu-id="caa6c-126">For more information, see [Enable Customer Payment Through Payment Services](sales-how-enable-payment-service-extensions.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="caa6c-127">See Also</span><span class="sxs-lookup"><span data-stu-id="caa6c-127">See Also</span></span>
<span data-ttu-id="caa6c-128">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions](ui-extensions.md)</span><span class="sxs-lookup"><span data-stu-id="caa6c-128">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions](ui-extensions.md)</span></span>  
[<span data-ttu-id="caa6c-129">Setting Up Sales</span><span class="sxs-lookup"><span data-stu-id="caa6c-129">Setting Up Sales</span></span>](sales-setup-sales.md)  
<span data-ttu-id="caa6c-130">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="caa6c-130">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
