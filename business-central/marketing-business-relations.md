---
title: Define Business Relation Codes on Contacts| Microsoft Docs
description: Use business relations in Business Central to help with marketing and to indicate the business relationship you have with your  prospects, clients, and customers, for example, a bank or service supplier.
services: project-madeira
documentationcenter: ''
author: jswymer
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: marketing, prospect, contact, client, customer
ms.date: 04/01/2019
ms.author: jswymer
redirect_url: marketing-create-contact-companies
ms.openlocfilehash: ffeb19820b29453750ca9c03258d455dddff287c
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 04/29/2019
ms.locfileid: "1239353"
---
# <a name="setting-up-business-relations-on-contacts"></a><span data-ttu-id="f477f-103">Setting Up Business Relations on Contacts</span><span class="sxs-lookup"><span data-stu-id="f477f-103">Setting Up Business Relations on Contacts</span></span>
<span data-ttu-id="f477f-104">You can use business relations to indicate the business relationship you have with your contacts, for example, a prospect, bank, consultant, service supplier, and so on.</span><span class="sxs-lookup"><span data-stu-id="f477f-104">You can use business relations to indicate the business relationship you have with your contacts, for example, a prospect, bank, consultant, service supplier, and so on.</span></span>

<span data-ttu-id="f477f-105">Using business relations on contacts is a two-step process.</span><span class="sxs-lookup"><span data-stu-id="f477f-105">Using business relations on contacts is a two-step process.</span></span> <span data-ttu-id="f477f-106">First, you define the business relation code.</span><span class="sxs-lookup"><span data-stu-id="f477f-106">First, you define the business relation code.</span></span> <span data-ttu-id="f477f-107">You only have to perform this step one time for each business relation.</span><span class="sxs-lookup"><span data-stu-id="f477f-107">You only have to perform this step one time for each business relation.</span></span> <span data-ttu-id="f477f-108">Once you have a business relation code, you can start to assign the code to contact companies.</span><span class="sxs-lookup"><span data-stu-id="f477f-108">Once you have a business relation code, you can start to assign the code to contact companies.</span></span>

> [!NOTE]  
>   <span data-ttu-id="f477f-109">If you plan to synchronise your contacts with vendors, customers, or bank accounts in other parts of the application, you may want to set up a business relation for them.</span><span class="sxs-lookup"><span data-stu-id="f477f-109">If you plan to synchronize your contacts with vendors, customers, or bank accounts in other parts of the application, you may want to set up a business relation for them.</span></span>

## <a name="to-define-a-business-relation-code"></a><span data-ttu-id="f477f-110">To define a business relation code</span><span class="sxs-lookup"><span data-stu-id="f477f-110">To define a business relation code</span></span>
<span data-ttu-id="f477f-111">The business relation code defines a category or type of the business relationship, such as BANK or Law.</span><span class="sxs-lookup"><span data-stu-id="f477f-111">The business relation code defines a category or type of the business relationship, such as BANK or Law.</span></span> <span data-ttu-id="f477f-112">You can have several business relation codes.</span><span class="sxs-lookup"><span data-stu-id="f477f-112">You can have several business relation codes.</span></span> <span data-ttu-id="f477f-113">To define the business relation, you use the **Business Relations** page.</span><span class="sxs-lookup"><span data-stu-id="f477f-113">To define the business relation, you use the **Business Relations** page.</span></span>

1. <span data-ttu-id="f477f-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Business Relations**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="f477f-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Business Relations**, and then choose the related link.</span></span>
2. <span data-ttu-id="f477f-115">Choose the **New** action, and fill in a code and description.</span><span class="sxs-lookup"><span data-stu-id="f477f-115">Choose the **New** action, and fill in a code and description.</span></span> <span data-ttu-id="f477f-116">The code can be a maximum of 11 characters, and can be any combination of numbers and letters.</span><span class="sxs-lookup"><span data-stu-id="f477f-116">The code can be a maximum of 11 characters, and can be any combination of numbers and letters.</span></span>

## <a name="AssignBusRelContact"></a> <span data-ttu-id="f477f-117">To assign business relations to a contact</span><span class="sxs-lookup"><span data-stu-id="f477f-117">To assign business relations to a contact</span></span>
<span data-ttu-id="f477f-118">You cannot assign business relations to a contact person - only companies.</span><span class="sxs-lookup"><span data-stu-id="f477f-118">You cannot assign business relations to a contact person - only companies.</span></span>

1. <span data-ttu-id="f477f-119">Open the contact.</span><span class="sxs-lookup"><span data-stu-id="f477f-119">Open the contact.</span></span>
2. <span data-ttu-id="f477f-120">Choose the **Company** action, and then the **Business Relations** action.</span><span class="sxs-lookup"><span data-stu-id="f477f-120">Choose the **Company** action, and then the **Business Relations** action.</span></span>

    <span data-ttu-id="f477f-121">The **Contact Business Relations** page opens.</span><span class="sxs-lookup"><span data-stu-id="f477f-121">The **Contact Business Relations** page opens.</span></span>
3. <span data-ttu-id="f477f-122">In the **Business Relation Code** field, select the business relation you want to assign.</span><span class="sxs-lookup"><span data-stu-id="f477f-122">In the **Business Relation Code** field, select the business relation you want to assign.</span></span>

<span data-ttu-id="f477f-123">Repeat these steps to assign as many business relations as you want.</span><span class="sxs-lookup"><span data-stu-id="f477f-123">Repeat these steps to assign as many business relations as you want.</span></span> <span data-ttu-id="f477f-124">You can also assign business relations from the contact list by following the same procedure.</span><span class="sxs-lookup"><span data-stu-id="f477f-124">You can also assign business relations from the contact list by following the same procedure.</span></span>

<span data-ttu-id="f477f-125">The number of business relations you have assigned to the contact is displayed in the **No. of Business Relations** field in the **Segmentation** section on the **Contact** page.</span><span class="sxs-lookup"><span data-stu-id="f477f-125">The number of business relations you have assigned to the contact is displayed in the **No. of Business Relations** field in the **Segmentation** section on the **Contact** page.</span></span>

<span data-ttu-id="f477f-126">After you have assigned business relations to your contacts, you can use this information to select contacts for your segments.</span><span class="sxs-lookup"><span data-stu-id="f477f-126">After you have assigned business relations to your contacts, you can use this information to select contacts for your segments.</span></span> <span data-ttu-id="f477f-127">For more information, see [Add Contacts to Segments](marketing-add-contact-segment.md).</span><span class="sxs-lookup"><span data-stu-id="f477f-127">For more information, see [Add Contacts to Segments](marketing-add-contact-segment.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="f477f-128">See Also</span><span class="sxs-lookup"><span data-stu-id="f477f-128">See Also</span></span>
<span data-ttu-id="f477f-129">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="f477f-129">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
