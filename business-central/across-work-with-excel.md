---
title: Viewing and Editing in Excel From Business Central | Microsoft Docs
description: Learn about how you can open the pages in Microsoft Excel from Business Central for better data analysis.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: accountant, accounting, financial report
ms.date: 07/03/2020
ms.author: jswymer
ms.openlocfilehash: f782b3ce19baa29d9268f3fdf742d2aa6112957f
ms.sourcegitcommit: 506a433298fc3629231cfa98f64a2d1428094fde
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 07/03/2020
ms.locfileid: "3534613"
---
# <a name="viewing-and-editing-in-excel-from-business-central"></a><span data-ttu-id="77e65-103">Viewing and Editing in Excel From Business Central</span><span class="sxs-lookup"><span data-stu-id="77e65-103">Viewing and Editing in Excel From Business Central</span></span>

<span data-ttu-id="77e65-104">With pages that display a list of records in rows and columns, like a list of customers, sale orders, or invoices, you can also view the records using Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="77e65-104">With pages that display a list of records in rows and columns, like a list of customers, sale orders, or invoices, you can also view the records using Microsoft Excel.</span></span> <span data-ttu-id="77e65-105">To do this, you have two options.</span><span class="sxs-lookup"><span data-stu-id="77e65-105">To do this, you have two options.</span></span> <span data-ttu-id="77e65-106">You can either select the **Open in Excel** action or the **Edit in Excel** action on the page.</span><span class="sxs-lookup"><span data-stu-id="77e65-106">You can either select the **Open in Excel** action or the **Edit in Excel** action on the page.</span></span> <span data-ttu-id="77e65-107">The differences between the two actions is as follows:</span><span class="sxs-lookup"><span data-stu-id="77e65-107">The differences between the two actions is as follows:</span></span>  

## <a name="open-in-excel"></a><span data-ttu-id="77e65-108">Open in Excel</span><span class="sxs-lookup"><span data-stu-id="77e65-108">Open in Excel</span></span>

- <span data-ttu-id="77e65-109">With this action, Excel respects any filters on the page that limit the records shown.</span><span class="sxs-lookup"><span data-stu-id="77e65-109">With this action, Excel respects any filters on the page that limit the records shown.</span></span> <span data-ttu-id="77e65-110">This means that the Excel workbook will contain the same rows and columns that appear on the page in [!INCLUDE[prodshort](includes/prodshort.md)].</span><span class="sxs-lookup"><span data-stu-id="77e65-110">This means that the Excel workbook will contain the same rows and columns that appear on the page in [!INCLUDE[prodshort](includes/prodshort.md)].</span></span>

- <span data-ttu-id="77e65-111">You can make changes to the records in Excel, but you cannot publish the changes back to [!INCLUDE[prodshort](includes/prodshort.md)].</span><span class="sxs-lookup"><span data-stu-id="77e65-111">You can make changes to the records in Excel, but you cannot publish the changes back to [!INCLUDE[prodshort](includes/prodshort.md)].</span></span> <span data-ttu-id="77e65-112">You can only save the changes to Excel file on your computer.</span><span class="sxs-lookup"><span data-stu-id="77e65-112">You can only save the changes to Excel file on your computer.</span></span>

- <span data-ttu-id="77e65-113">This action works on both on Windows and macOS.</span><span class="sxs-lookup"><span data-stu-id="77e65-113">This action works on both on Windows and macOS.</span></span>

> [!NOTE]
> <span data-ttu-id="77e65-114">For [!INCLUDE[prodshort](includes/prodshort.md)] on-premises, the **Open in Excel** action is available by default.</span><span class="sxs-lookup"><span data-stu-id="77e65-114">For [!INCLUDE[prodshort](includes/prodshort.md)] on-premises, the **Open in Excel** action is available by default.</span></span> <span data-ttu-id="77e65-115">However, if you set up [!INCLUDE[prodshort](includes/prodshort.md)] on-premises for editing data in Excel, then the **Open in Excel** action is replaced by the **Edit in Excel** action.</span><span class="sxs-lookup"><span data-stu-id="77e65-115">However, if you set up [!INCLUDE[prodshort](includes/prodshort.md)] on-premises for editing data in Excel, then the **Open in Excel** action is replaced by the **Edit in Excel** action.</span></span>

## <a name="edit-in-excel"></a><span data-ttu-id="77e65-116">Edit in Excel</span><span class="sxs-lookup"><span data-stu-id="77e65-116">Edit in Excel</span></span>

- <span data-ttu-id="77e65-117">With this action, Excel respects most filters on the page that limit the records shown.</span><span class="sxs-lookup"><span data-stu-id="77e65-117">With this action, Excel respects most filters on the page that limit the records shown.</span></span> <span data-ttu-id="77e65-118">This means that the Excel workbook will contain almost the same records and columns.</span><span class="sxs-lookup"><span data-stu-id="77e65-118">This means that the Excel workbook will contain almost the same records and columns.</span></span>

- <span data-ttu-id="77e65-119">The advantage of the **Edit in Excel** action is that it lets you make changes to records in Excel and then publish the changes back to [!INCLUDE[prodshort](includes/prodshort.md)].</span><span class="sxs-lookup"><span data-stu-id="77e65-119">The advantage of the **Edit in Excel** action is that it lets you make changes to records in Excel and then publish the changes back to [!INCLUDE[prodshort](includes/prodshort.md)].</span></span>

- <span data-ttu-id="77e65-120">It only works on Windows; not macOS.</span><span class="sxs-lookup"><span data-stu-id="77e65-120">It only works on Windows; not macOS.</span></span>

- <span data-ttu-id="77e65-121">You can switch the company that your are working with.</span><span class="sxs-lookup"><span data-stu-id="77e65-121">You can switch the company that your are working with.</span></span> <span data-ttu-id="77e65-122">To do this, select the **Options** icon ![Excel add-in options](media/cogwheel.png "Excel add-in options") in the Excel Add-in pane, then select the company from the **Company** field.</span><span class="sxs-lookup"><span data-stu-id="77e65-122">To do this, select the **Options** icon ![Excel add-in options](media/cogwheel.png "Excel add-in options") in the Excel Add-in pane, then select the company from the **Company** field.</span></span>  

    > [!IMPORTANT]
    > <span data-ttu-id="77e65-123">When changing the company, make sure that the **Environment** field is not empty.</span><span class="sxs-lookup"><span data-stu-id="77e65-123">When changing the company, make sure that the **Environment** field is not empty.</span></span> <span data-ttu-id="77e65-124">If it is, then set it to one of the available options; otherwise, the add-in will not work correctly.</span><span class="sxs-lookup"><span data-stu-id="77e65-124">If it is, then set it to one of the available options; otherwise, the add-in will not work correctly.</span></span>  

<span data-ttu-id="77e65-125">If you make changes to the add-in, you must reload it in order to update the connection.</span><span class="sxs-lookup"><span data-stu-id="77e65-125">If you make changes to the add-in, you must reload it in order to update the connection.</span></span> <span data-ttu-id="77e65-126">To reload, use the ![Excel add-in menu](media/excel-addin-menu.png "Excel add-in menu") menu in the top-right corner of the add-in.</span><span class="sxs-lookup"><span data-stu-id="77e65-126">To reload, use the ![Excel add-in menu](media/excel-addin-menu.png "Excel add-in menu") menu in the top-right corner of the add-in.</span></span>

> [!NOTE]
> <span data-ttu-id="77e65-127">For [!INCLUDE[prodshort](includes/prodshort.md)] on-premises, the **Edit in Excel** action is only available if the Excel add-in has been configured by your administrator, and only available for the Web client.</span><span class="sxs-lookup"><span data-stu-id="77e65-127">For [!INCLUDE[prodshort](includes/prodshort.md)] on-premises, the **Edit in Excel** action is only available if the Excel add-in has been configured by your administrator, and only available for the Web client.</span></span> <span data-ttu-id="77e65-128">For administrators, if you want to learn how to install the excel add-in, see [Setting up the Excel Add-In for Editing Business Central Data](/dynamics365/business-central/dev-itpro/administration/configuring-excel-addin).</span><span class="sxs-lookup"><span data-stu-id="77e65-128">For administrators, if you want to learn how to install the excel add-in, see [Setting up the Excel Add-In for Editing Business Central Data](/dynamics365/business-central/dev-itpro/administration/configuring-excel-addin).</span></span>

### <a name="see-the-differences-between-the-options"></a><span data-ttu-id="77e65-129">See the differences between the options</span><span class="sxs-lookup"><span data-stu-id="77e65-129">See the differences between the options</span></span>
<br><br>  

> [!Video https://go.microsoft.com/fwlink/?linkid=2086039]

## <a name="see-related-training-at-microsoft-learn"></a><span data-ttu-id="77e65-130">See Related Training at [Microsoft Learn](/learn/modules/configure-powerbi-excel-dynamics-365-business-central/index)</span><span class="sxs-lookup"><span data-stu-id="77e65-130">See Related Training at [Microsoft Learn](/learn/modules/configure-powerbi-excel-dynamics-365-business-central/index)</span></span>

## <a name="see-also"></a><span data-ttu-id="77e65-131">See Also</span><span class="sxs-lookup"><span data-stu-id="77e65-131">See Also</span></span>

[<span data-ttu-id="77e65-132">Working with Business Central</span><span class="sxs-lookup"><span data-stu-id="77e65-132">Working with Business Central</span></span>](ui-work-product.md)  
[<span data-ttu-id="77e65-133">Enhancements to Excel integration in 2019 release wave 2</span><span class="sxs-lookup"><span data-stu-id="77e65-133">Enhancements to Excel integration in 2019 release wave 2</span></span>](/dynamics365-release-plan/2019wave2/dynamics365-business-central/enhancements-excel-integration)  
