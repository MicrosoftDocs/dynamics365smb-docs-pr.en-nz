---
title: Create Number Series | Microsoft Docs
description: Learn how to set up number series that assign unique ID codes to accounts and documents in Business Central .
documentationcenter: 
author: SusanneWindfeldPedersen
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: numbers, numbering
ms.date: 06/02/2017
ms.author: solsen
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 151e585b0a809b1b537b52089fce297f222a60dc
ms.contentlocale: en-nz
ms.lasthandoff: 03/22/2018

---
# <a name="create-number-series"></a><span data-ttu-id="2516f-103">Create Number Series</span><span class="sxs-lookup"><span data-stu-id="2516f-103">Create Number Series</span></span>
<span data-ttu-id="2516f-104">For each company that you set up, you need to assign unique identification codes to things such as general ledger accounts, customer and vendor accounts, invoices, and other documents.</span><span class="sxs-lookup"><span data-stu-id="2516f-104">For each company that you set up, you need to assign unique identification codes to things such as general ledger accounts, customer and vendor accounts, invoices, and other documents.</span></span> <span data-ttu-id="2516f-105">Numbering is important not only for identification.</span><span class="sxs-lookup"><span data-stu-id="2516f-105">Numbering is important not only for identification.</span></span> <span data-ttu-id="2516f-106">A well-designed numbering system also makes the company more manageable and easy to analyse, and can reduce the number of errors that occur in data entry.</span><span class="sxs-lookup"><span data-stu-id="2516f-106">A well-designed numbering system also makes the company more manageable and easy to analyze, and can reduce the number of errors that occur in data entry.</span></span>

> [!NOTE]  
>   <span data-ttu-id="2516f-107">We recommend that you use the same number series codes as you see listed in the **No. Series List** window in the CRONUS demonstration company.</span><span class="sxs-lookup"><span data-stu-id="2516f-107">We recommend that you use the same number series codes as you see listed in the **No. Series List** window in the CRONUS demonstration company.</span></span> <span data-ttu-id="2516f-108">Codes such as *P-INV+* might not make immediate sense to you, but [!INCLUDE[d365fin](includes/d365fin_md.md)] has a number of default settings that depend on these number series codes.</span><span class="sxs-lookup"><span data-stu-id="2516f-108">Codes such as *P-INV+* might not make immediate sense to you, but [!INCLUDE[d365fin](includes/d365fin_md.md)] has a number of default settings that depend on these number series codes.</span></span>

<span data-ttu-id="2516f-109">You create a numbering system by setting up one or more codes for each type of master data or document.</span><span class="sxs-lookup"><span data-stu-id="2516f-109">You create a numbering system by setting up one or more codes for each type of master data or document.</span></span> <span data-ttu-id="2516f-110">For example, you can set up one code for numbering customers, another code for numbering sales invoices, and another code for numbering documents in general journals.</span><span class="sxs-lookup"><span data-stu-id="2516f-110">For example, you can set up one code for numbering customers, another code for numbering sales invoices, and another code for numbering documents in general journals.</span></span> <span data-ttu-id="2516f-111">After you have set up a code, you set must set up at least one number series line.</span><span class="sxs-lookup"><span data-stu-id="2516f-111">After you have set up a code, you set must set up at least one number series line.</span></span> <span data-ttu-id="2516f-112">The number series line contains information such as the first and last number in the series and the starting date.</span><span class="sxs-lookup"><span data-stu-id="2516f-112">The number series line contains information such as the first and last number in the series and the starting date.</span></span> <span data-ttu-id="2516f-113">You can set up more than one number series line per number series code, with a different starting date for each line.</span><span class="sxs-lookup"><span data-stu-id="2516f-113">You can set up more than one number series line per number series code, with a different starting date for each line.</span></span> <span data-ttu-id="2516f-114">The series will be used consecutively, starting each series on the respective starting date.</span><span class="sxs-lookup"><span data-stu-id="2516f-114">The series will be used consecutively, starting each series on the respective starting date.</span></span>

<span data-ttu-id="2516f-115">You typically set up your number series to automatically insert the next consecutive number on new cards or documents that you create.</span><span class="sxs-lookup"><span data-stu-id="2516f-115">You typically set up your number series to automatically insert the next consecutive number on new cards or documents that you create.</span></span> <span data-ttu-id="2516f-116">However, you can also set a number series up to allow that you manually enter the new number.</span><span class="sxs-lookup"><span data-stu-id="2516f-116">However, you can also set a number series up to allow that you manually enter the new number.</span></span> <span data-ttu-id="2516f-117">You specify this with the **Manual Nos.** check box.</span><span class="sxs-lookup"><span data-stu-id="2516f-117">You specify this with the **Manual Nos.** check box.</span></span>

<span data-ttu-id="2516f-118">If you want to use more than one number series code for one type of master data - for example, if you want to use different number series for different categories of items - you can use number series relationships.</span><span class="sxs-lookup"><span data-stu-id="2516f-118">If you want to use more than one number series code for one type of master data - for example, if you want to use different number series for different categories of items - you can use number series relationships.</span></span>

## <a name="to-create-a-new-number-series"></a><span data-ttu-id="2516f-119">To create a new number series</span><span class="sxs-lookup"><span data-stu-id="2516f-119">To create a new number series</span></span>
1. <span data-ttu-id="2516f-120">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **No. Series**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="2516f-120">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **No. Series**, and then choose the related link.</span></span>
2. <span data-ttu-id="2516f-121">Choose the **New** action.</span><span class="sxs-lookup"><span data-stu-id="2516f-121">Choose the **New** action.</span></span>
3. <span data-ttu-id="2516f-122">On the new line, fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="2516f-122">On the new line, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

<span data-ttu-id="2516f-123">**TIP**: To allow manual entry of a number on new cards or documents, deselect the **Default Nos.** check box and select the **Manual Nos.** check box.</span><span class="sxs-lookup"><span data-stu-id="2516f-123">**TIP**: To allow manual entry of a number on new cards or documents, deselect the **Default Nos.** check box and select the **Manual Nos.** check box.</span></span>

<span data-ttu-id="2516f-124">Now when you create a new card or document that is set up to use the number series in question, you can manually fill in the **No.**</span><span class="sxs-lookup"><span data-stu-id="2516f-124">Now when you create a new card or document that is set up to use the number series in question, you can manually fill in the **No.**</span></span> <span data-ttu-id="2516f-125">field with any value.</span><span class="sxs-lookup"><span data-stu-id="2516f-125">field with any value.</span></span>  

## <a name="to-set-up-where-a-number-series-is-used"></a><span data-ttu-id="2516f-126">To set up where a number series is used</span><span class="sxs-lookup"><span data-stu-id="2516f-126">To set up where a number series is used</span></span>
<span data-ttu-id="2516f-127">The following procedure shows how to set number series up for the Sales area.</span><span class="sxs-lookup"><span data-stu-id="2516f-127">The following procedure shows how to set number series up for the Sales area.</span></span> <span data-ttu-id="2516f-128">The steps are similar for other areas.</span><span class="sxs-lookup"><span data-stu-id="2516f-128">The steps are similar for other areas.</span></span>
1. <span data-ttu-id="2516f-129">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sales & Receivables**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="2516f-129">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sales & Receivables**, and then choose the related link.</span></span>
2. <span data-ttu-id="2516f-130">In the **Sales & Receivables** window, on the **Number Series** FastTab, select the desired number series for each sales card or document.</span><span class="sxs-lookup"><span data-stu-id="2516f-130">In the **Sales & Receivables** window, on the **Number Series** FastTab, select the desired number series for each sales card or document.</span></span>

<span data-ttu-id="2516f-131">The selected number will now be used to fill in the **No.**</span><span class="sxs-lookup"><span data-stu-id="2516f-131">The selected number will now be used to fill in the **No.**</span></span> <span data-ttu-id="2516f-132">field on the card or document in question, according to the settings you made on the number series line.</span><span class="sxs-lookup"><span data-stu-id="2516f-132">field on the card or document in question, according to the settings you made on the number series line.</span></span>

## <a name="to-create-relationships-between-number-series"></a><span data-ttu-id="2516f-133">To create relationships between number series</span><span class="sxs-lookup"><span data-stu-id="2516f-133">To create relationships between number series</span></span>
<span data-ttu-id="2516f-134">If you have set up more than one number series code for the same kind of basic information or transactions, you can create relationships between the codes.</span><span class="sxs-lookup"><span data-stu-id="2516f-134">If you have set up more than one number series code for the same kind of basic information or transactions, you can create relationships between the codes.</span></span> <span data-ttu-id="2516f-135">This feature can assist you in deciding among the codes when you use a number.</span><span class="sxs-lookup"><span data-stu-id="2516f-135">This feature can assist you in deciding among the codes when you use a number.</span></span>

1. <span data-ttu-id="2516f-136">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **No. Series**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="2516f-136">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **No. Series**, and then choose the related link.</span></span>
2. <span data-ttu-id="2516f-137">Select the line with the number series you want to create relationships for and then choose **Relationships**.</span><span class="sxs-lookup"><span data-stu-id="2516f-137">Select the line with the number series you want to create relationships for and then choose **Relationships**.</span></span>
3. <span data-ttu-id="2516f-138">In the **Series Code** field, enter the code for the number series that you want to relate to the series you selected in step 2.</span><span class="sxs-lookup"><span data-stu-id="2516f-138">In the **Series Code** field, enter the code for the number series that you want to relate to the series you selected in step 2.</span></span>
4. <span data-ttu-id="2516f-139">Add a line for each code that you want to relate to the selected number series.</span><span class="sxs-lookup"><span data-stu-id="2516f-139">Add a line for each code that you want to relate to the selected number series.</span></span>
5. <span data-ttu-id="2516f-140">Close the window.</span><span class="sxs-lookup"><span data-stu-id="2516f-140">Close the window.</span></span>

<span data-ttu-id="2516f-141">Now when you set up something that requires a number, you can use the relationships you created to select among the related number series.</span><span class="sxs-lookup"><span data-stu-id="2516f-141">Now when you set up something that requires a number, you can use the relationships you created to select among the related number series.</span></span>

## <a name="see-also"></a><span data-ttu-id="2516f-142">See Also</span><span class="sxs-lookup"><span data-stu-id="2516f-142">See Also</span></span>
<span data-ttu-id="2516f-143">[Setting Up [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)</span><span class="sxs-lookup"><span data-stu-id="2516f-143">[Setting Up [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)</span></span>  
<span data-ttu-id="2516f-144">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="2516f-144">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
