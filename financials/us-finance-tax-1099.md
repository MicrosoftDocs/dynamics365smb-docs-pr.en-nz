---
title: Reporting 1099 Transactions in the US | Microsoft Docs
description: The IRS requires the 1099 tax form for payments to vendors and you can specify a purchase document is 1099 liable and specify the 1099 code for the vendor.
services: project-madeira
documentationcenter: 
author: edupont04
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: local
ms.date: 03/29/2017
ms.author: edupont
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: c20c52927aa979e56aeef7975fbcee1564ca4dd7
ms.contentlocale: en-nz
ms.lasthandoff: 09/11/2017

---
# <a name="reporting-transactions-as-1099-liable-in-the-us"></a><span data-ttu-id="4fddf-103">Reporting Transactions as 1099 Liable in the US</span><span class="sxs-lookup"><span data-stu-id="4fddf-103">Reporting Transactions as 1099 Liable in the US</span></span>

<span data-ttu-id="4fddf-104">The Internal Revenue Service (IRS) requires one or more versions of the 1099 tax form for payments to vendors.</span><span class="sxs-lookup"><span data-stu-id="4fddf-104">The Internal Revenue Service (IRS) requires one or more versions of the 1099 tax form for payments to vendors.</span></span> <span data-ttu-id="4fddf-105">Copies of these forms must be sent to vendors annually on or before the last day of January.</span><span class="sxs-lookup"><span data-stu-id="4fddf-105">Copies of these forms must be sent to vendors annually on or before the last day of January.</span></span> <span data-ttu-id="4fddf-106">On your purchase documents, you can specify that the document is 1099 liable, and you can specify the 1099 code for the vendor.</span><span class="sxs-lookup"><span data-stu-id="4fddf-106">On your purchase documents, you can specify that the document is 1099 liable, and you can specify the 1099 code for the vendor.</span></span>  

## <a name="1099-codes"></a><span data-ttu-id="4fddf-107">1099 codes</span><span class="sxs-lookup"><span data-stu-id="4fddf-107">1099 codes</span></span>
<span data-ttu-id="4fddf-108">In [!INCLUDE[d365fin](includes/d365fin_md.md)], the most common 1099 codes are already set up for you so you are ready to generate the required reports.</span><span class="sxs-lookup"><span data-stu-id="4fddf-108">In [!INCLUDE[d365fin](includes/d365fin_md.md)], the most common 1099 codes are already set up for you so you are ready to generate the required reports.</span></span> <span data-ttu-id="4fddf-109">The codes are defined in the **IRS 1099 Form Box** window where you can also add new 1099 codes.</span><span class="sxs-lookup"><span data-stu-id="4fddf-109">The codes are defined in the **IRS 1099 Form Box** window where you can also add new 1099 codes.</span></span> <span data-ttu-id="4fddf-110">For each tax liable vendor, you can then specify the relevant 1099 code on the **Payments** FastTab on the Vendor card.</span><span class="sxs-lookup"><span data-stu-id="4fddf-110">For each tax liable vendor, you can then specify the relevant 1099 code on the **Payments** FastTab on the Vendor card.</span></span>  

<span data-ttu-id="4fddf-111">With the **Vendor 1099 Information** report, you can review 1099 transactions paid during a specified period.</span><span class="sxs-lookup"><span data-stu-id="4fddf-111">With the **Vendor 1099 Information** report, you can review 1099 transactions paid during a specified period.</span></span> <span data-ttu-id="4fddf-112">At the end of the year, you can print 1099 transactions on preprinted forms.</span><span class="sxs-lookup"><span data-stu-id="4fddf-112">At the end of the year, you can print 1099 transactions on preprinted forms.</span></span>  

## <a name="printing-1099-tax-forms"></a><span data-ttu-id="4fddf-113">Printing 1099 tax forms</span><span class="sxs-lookup"><span data-stu-id="4fddf-113">Printing 1099 tax forms</span></span>
<span data-ttu-id="4fddf-114">From the **IRS 1099 Form Box** window, you can access the following tax forms:</span><span class="sxs-lookup"><span data-stu-id="4fddf-114">From the **IRS 1099 Form Box** window, you can access the following tax forms:</span></span>  

* <span data-ttu-id="4fddf-115">Vendor 1099 Div</span><span class="sxs-lookup"><span data-stu-id="4fddf-115">Vendor 1099 Div</span></span>  

  <span data-ttu-id="4fddf-116">Prints the federal form 1099-DIV for dividends and distribution.</span><span class="sxs-lookup"><span data-stu-id="4fddf-116">Prints the federal form 1099-DIV for dividends and distribution.</span></span> <span data-ttu-id="4fddf-117">You can print all or specific 1099-DIV forms.</span><span class="sxs-lookup"><span data-stu-id="4fddf-117">You can print all or specific 1099-DIV forms.</span></span> <span data-ttu-id="4fddf-118">The report uses the codes that apply to the DIV form amount boxes from the **IRS 1099 Form-Box** window.</span><span class="sxs-lookup"><span data-stu-id="4fddf-118">The report uses the codes that apply to the DIV form amount boxes from the **IRS 1099 Form-Box** window.</span></span>  
* <span data-ttu-id="4fddf-119">Vendor 1099 Int</span><span class="sxs-lookup"><span data-stu-id="4fddf-119">Vendor 1099 Int</span></span>  

  <span data-ttu-id="4fddf-120">Prints the federal form 1099-INT for interest income.</span><span class="sxs-lookup"><span data-stu-id="4fddf-120">Prints the federal form 1099-INT for interest income.</span></span> <span data-ttu-id="4fddf-121">You can print all or specific 1099-INT forms.</span><span class="sxs-lookup"><span data-stu-id="4fddf-121">You can print all or specific 1099-INT forms.</span></span> <span data-ttu-id="4fddf-122">The report uses the codes that apply to the INT form amount boxes from the **IRS 1099 Form-Box** window.</span><span class="sxs-lookup"><span data-stu-id="4fddf-122">The report uses the codes that apply to the INT form amount boxes from the **IRS 1099 Form-Box** window.</span></span>  
* <span data-ttu-id="4fddf-123">Vendor 1099 Misc - Miscellaneous income</span><span class="sxs-lookup"><span data-stu-id="4fddf-123">Vendor 1099 Misc - Miscellaneous income</span></span>  

  <span data-ttu-id="4fddf-124">Prints the federal form 1099-MISC for miscellaneous income.</span><span class="sxs-lookup"><span data-stu-id="4fddf-124">Prints the federal form 1099-MISC for miscellaneous income.</span></span> <span data-ttu-id="4fddf-125">You can print all or specific 1099-MISC forms.</span><span class="sxs-lookup"><span data-stu-id="4fddf-125">You can print all or specific 1099-MISC forms.</span></span> <span data-ttu-id="4fddf-126">The report uses the codes that apply to the MISC form amount boxes from the **IRS 1099 Form-Box** window.</span><span class="sxs-lookup"><span data-stu-id="4fddf-126">The report uses the codes that apply to the MISC form amount boxes from the **IRS 1099 Form-Box** window.</span></span>  

<span data-ttu-id="4fddf-127">Regulatory changes affecting this report and the table data are generally handled in end-of-year updates.</span><span class="sxs-lookup"><span data-stu-id="4fddf-127">Regulatory changes affecting this report and the table data are generally handled in end-of-year updates.</span></span>
<span data-ttu-id="4fddf-128">It may be helpful to run the **Vendor 1099 Information** report to review the data before printing the forms.</span><span class="sxs-lookup"><span data-stu-id="4fddf-128">It may be helpful to run the **Vendor 1099 Information** report to review the data before printing the forms.</span></span>

## <a name="submitting-1099-tax-forms-electronically"></a><span data-ttu-id="4fddf-129">Submitting 1099 tax forms electronically</span><span class="sxs-lookup"><span data-stu-id="4fddf-129">Submitting 1099 tax forms electronically</span></span>
<span data-ttu-id="4fddf-130">To submit the 1099 tax forms electronically, use the **Vendor 1099 Magnetic Media** report.</span><span class="sxs-lookup"><span data-stu-id="4fddf-130">To submit the 1099 tax forms electronically, use the **Vendor 1099 Magnetic Media** report.</span></span> <span data-ttu-id="4fddf-131">Specifies the 1099 forms that can be exported.</span><span class="sxs-lookup"><span data-stu-id="4fddf-131">Specifies the 1099 forms that can be exported.</span></span> <span data-ttu-id="4fddf-132">The form information exported by this report is the same as the reports that print 1099 forms that are described in the previous section.</span><span class="sxs-lookup"><span data-stu-id="4fddf-132">The form information exported by this report is the same as the reports that print 1099 forms that are described in the previous section.</span></span>  

<span data-ttu-id="4fddf-133">The report uses the codes that apply to the form amount boxes from the **IRS 1099 Form-Box** window.</span><span class="sxs-lookup"><span data-stu-id="4fddf-133">The report uses the codes that apply to the form amount boxes from the **IRS 1099 Form-Box** window.</span></span> <span data-ttu-id="4fddf-134">The codes are mapped to the form boxes in the file layouts of this report, therefore the table data and report version for a particular tax year must be in agreement.</span><span class="sxs-lookup"><span data-stu-id="4fddf-134">The codes are mapped to the form boxes in the file layouts of this report, therefore the table data and report version for a particular tax year must be in agreement.</span></span> <span data-ttu-id="4fddf-135">If any custom codes are added to the table these must be mapped to the form boxes inside this object.</span><span class="sxs-lookup"><span data-stu-id="4fddf-135">If any custom codes are added to the table these must be mapped to the form boxes inside this object.</span></span>  

<span data-ttu-id="4fddf-136">Regulatory changes affecting this report and the table data are generally handled in end-of-year updates.</span><span class="sxs-lookup"><span data-stu-id="4fddf-136">Regulatory changes affecting this report and the table data are generally handled in end-of-year updates.</span></span>
<span data-ttu-id="4fddf-137">It may be helpful to run the **Vendor 1099 Information** report to review the data before generating the electronic file.</span><span class="sxs-lookup"><span data-stu-id="4fddf-137">It may be helpful to run the **Vendor 1099 Information** report to review the data before generating the electronic file.</span></span>  

## <a name="see-also"></a><span data-ttu-id="4fddf-138">See Also</span><span class="sxs-lookup"><span data-stu-id="4fddf-138">See Also</span></span>
[<span data-ttu-id="4fddf-139">How to: Register New Vendors</span><span class="sxs-lookup"><span data-stu-id="4fddf-139">How to: Register New Vendors</span></span>](purchasing-how-register-new-vendors.md)  
[<span data-ttu-id="4fddf-140">How to: Record Purchase</span><span class="sxs-lookup"><span data-stu-id="4fddf-140">How to: Record Purchase</span></span>](purchasing-how-record-purchases.md)  
<span data-ttu-id="4fddf-141">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="4fddf-141">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  

