---
title: Set Up Web Sources for Contact Companies| Microsoft Docs
description: You can define internet or web sources and assign them to a contact company to help identify how you want to search for information about your contacts.
services: project-madeira
documentationcenter: 
author: jswymer
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: internet
ms.date: 06/06/2017
ms.author: jswymer
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: b81deefcdf79a93cc988d216f80b08794efb8ab6
ms.contentlocale: en-nz
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-set-up-web-sources-for-contact-companies"></a><span data-ttu-id="63d05-103">How to: Set Up Web Sources for Contact Companies</span><span class="sxs-lookup"><span data-stu-id="63d05-103">How to: Set Up Web Sources for Contact Companies</span></span>
<span data-ttu-id="63d05-104">You can use web sources with your contact companies to identify, for example, search engines and web sites, on the Internet that you want to use to search for information about the contacts.</span><span class="sxs-lookup"><span data-stu-id="63d05-104">You can use web sources with your contact companies to identify, for example, search engines and web sites, on the Internet that you want to use to search for information about the contacts.</span></span> <span data-ttu-id="63d05-105">When assigning web sources, you specify which search engine and search word the application will use to find the requested information.</span><span class="sxs-lookup"><span data-stu-id="63d05-105">When assigning web sources, you specify which search engine and search word the application will use to find the requested information.</span></span>

<span data-ttu-id="63d05-106">Using web sources on contacts is a two-step process.</span><span class="sxs-lookup"><span data-stu-id="63d05-106">Using web sources on contacts is a two-step process.</span></span> <span data-ttu-id="63d05-107">First, you define the web source code.</span><span class="sxs-lookup"><span data-stu-id="63d05-107">First, you define the web source code.</span></span> <span data-ttu-id="63d05-108">You only have to perform this step one time for each web source.</span><span class="sxs-lookup"><span data-stu-id="63d05-108">You only have to perform this step one time for each web source.</span></span> <span data-ttu-id="63d05-109">Once you have a web source code, you can start to assign the code to contact persons.</span><span class="sxs-lookup"><span data-stu-id="63d05-109">Once you have a web source code, you can start to assign the code to contact persons.</span></span>

## <a name="to-define-a-web-source-code"></a><span data-ttu-id="63d05-110">To define a web source code</span><span class="sxs-lookup"><span data-stu-id="63d05-110">To define a web source code</span></span>
1. <span data-ttu-id="63d05-111">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Web Sources**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="63d05-111">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Web Sources**, and then choose the related link.</span></span>
2. <span data-ttu-id="63d05-112">Choose the **New** actions.</span><span class="sxs-lookup"><span data-stu-id="63d05-112">Choose the **New** actions.</span></span>
3. <span data-ttu-id="63d05-113">Fill in the **Code**, **Description**, and **URL** fields.</span><span class="sxs-lookup"><span data-stu-id="63d05-113">Fill in the **Code**, **Description**, and **URL** fields.</span></span>

    <span data-ttu-id="63d05-114">Type %1 in the **URL** field to insert a placeholder for a search word in the URL.</span><span class="sxs-lookup"><span data-stu-id="63d05-114">Type %1 in the **URL** field to insert a placeholder for a search word in the URL.</span></span> <span data-ttu-id="63d05-115">When you launch the web source from a contact, the %1 is replaced with the search word, for example, the name of the company that you have entered in the **Contact Web Sources** window.</span><span class="sxs-lookup"><span data-stu-id="63d05-115">When you launch the web source from a contact, the %1 is replaced with the search word, for example, the name of the company that you have entered in the **Contact Web Sources** window.</span></span>

<span data-ttu-id="63d05-116">Repeat these steps to set up as many web sources as you want.</span><span class="sxs-lookup"><span data-stu-id="63d05-116">Repeat these steps to set up as many web sources as you want.</span></span>

## <a name="to-assign-web-sources-to-a-contact-company"></a><span data-ttu-id="63d05-117">To assign web sources to a contact company</span><span class="sxs-lookup"><span data-stu-id="63d05-117">To assign web sources to a contact company</span></span>
<span data-ttu-id="63d05-118">When assigning web sources, you specify which search engine and search word that the application will use to find the requested information.</span><span class="sxs-lookup"><span data-stu-id="63d05-118">When assigning web sources, you specify which search engine and search word that the application will use to find the requested information.</span></span>

1. <span data-ttu-id="63d05-119">Open the contact.</span><span class="sxs-lookup"><span data-stu-id="63d05-119">Open the contact.</span></span>
2. <span data-ttu-id="63d05-120">Choose the **Company** action, and then choose the **Web Sources** action.</span><span class="sxs-lookup"><span data-stu-id="63d05-120">Choose the **Company** action, and then choose the **Web Sources** action.</span></span> <span data-ttu-id="63d05-121">The **Contact Web Sources** window opens.</span><span class="sxs-lookup"><span data-stu-id="63d05-121">The **Contact Web Sources** window opens.</span></span>
3. <span data-ttu-id="63d05-122">In the **Web Source Code** field, choose the web source you want to assign.</span><span class="sxs-lookup"><span data-stu-id="63d05-122">In the **Web Source Code** field, choose the web source you want to assign.</span></span>
4. <span data-ttu-id="63d05-123">In the **Search Word** field, enter the search word that you want to use to find the information.</span><span class="sxs-lookup"><span data-stu-id="63d05-123">In the **Search Word** field, enter the search word that you want to use to find the information.</span></span>

<span data-ttu-id="63d05-124">Repeat these steps to assign as many web sources as you want.</span><span class="sxs-lookup"><span data-stu-id="63d05-124">Repeat these steps to assign as many web sources as you want.</span></span>

<span data-ttu-id="63d05-125">You can also assign web sources from the **Contact List** window by following the same procedure.</span><span class="sxs-lookup"><span data-stu-id="63d05-125">You can also assign web sources from the **Contact List** window by following the same procedure.</span></span>

## <a name="see-also"></a><span data-ttu-id="63d05-126">See Also</span><span class="sxs-lookup"><span data-stu-id="63d05-126">See Also</span></span>
[<span data-ttu-id="63d05-127">Creating Contact Companies</span><span class="sxs-lookup"><span data-stu-id="63d05-127">Creating Contact Companies</span></span>](marketing-create-contact-companies.md)  
<span data-ttu-id="63d05-128">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="63d05-128">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

