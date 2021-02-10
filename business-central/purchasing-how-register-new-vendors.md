---
title: Create a Vendor Card to Register a New Vendor | Microsoft Docs
description: Learn how to create a vendor card to register a new vendor or supplier.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: supplier
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 8efd74c3ae6962a383e5b127056d744dd7c1892f
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 12/17/2020
ms.locfileid: "4748809"
---
# <a name="register-new-vendors"></a><span data-ttu-id="10228-103">Register New Vendors</span><span class="sxs-lookup"><span data-stu-id="10228-103">Register New Vendors</span></span>

<span data-ttu-id="10228-104">Vendors provide the products that you sell.</span><span class="sxs-lookup"><span data-stu-id="10228-104">Vendors provide the products that you sell.</span></span> <span data-ttu-id="10228-105">Each vendor that you purchase from must be registered as a vendor card.</span><span class="sxs-lookup"><span data-stu-id="10228-105">Each vendor that you purchase from must be registered as a vendor card.</span></span>

<span data-ttu-id="10228-106">Before you can register new vendors, you must set up various purchase codes that you can select from when you fill vendor cards.</span><span class="sxs-lookup"><span data-stu-id="10228-106">Before you can register new vendors, you must set up various purchase codes that you can select from when you fill vendor cards.</span></span> <span data-ttu-id="10228-107">When all of the required master data is created, you can perform additional configuration of the vendor, such as prioritise the vendor for payment purposes and list items that the vendor and other vendors can supply.</span><span class="sxs-lookup"><span data-stu-id="10228-107">When all of the required master data is created, you can perform additional configuration of the vendor, such as prioritize the vendor for payment purposes and list items that the vendor and other vendors can supply.</span></span> <span data-ttu-id="10228-108">Another group of setup tasks for vendors is to record your agreements concerning discounts, prices, and payment methods.</span><span class="sxs-lookup"><span data-stu-id="10228-108">Another group of setup tasks for vendors is to record your agreements concerning discounts, prices, and payment methods.</span></span> <span data-ttu-id="10228-109">For more information, see [Setting Up Purchasing](purchasing-setup-purchasing.md).</span><span class="sxs-lookup"><span data-stu-id="10228-109">For more information, see [Setting Up Purchasing](purchasing-setup-purchasing.md).</span></span>

<span data-ttu-id="10228-110">Vendor cards hold the information that is required to buy products from the vendor.</span><span class="sxs-lookup"><span data-stu-id="10228-110">Vendor cards hold the information that is required to buy products from the vendor.</span></span> <span data-ttu-id="10228-111">For more information, see [Record Purchases](purchasing-how-record-purchases.md) and [Register New Items](inventory-how-register-new-items.md).</span><span class="sxs-lookup"><span data-stu-id="10228-111">For more information, see [Record Purchases](purchasing-how-record-purchases.md) and [Register New Items](inventory-how-register-new-items.md).</span></span>

> [!NOTE]  
> <span data-ttu-id="10228-112">If vendor templates exist for different vendor types, then a page appears when you create a new vendor card from where you can select an appropriate template.</span><span class="sxs-lookup"><span data-stu-id="10228-112">If vendor templates exist for different vendor types, then a page appears when you create a new vendor card from where you can select an appropriate template.</span></span> <span data-ttu-id="10228-113">If only one vendor template exists, then new vendor cards always use that template.</span><span class="sxs-lookup"><span data-stu-id="10228-113">If only one vendor template exists, then new vendor cards always use that template.</span></span>
<br><br>  

> [!Video https://www.microsoft.com/videoplayer/embed/RE3PZtd?rel=0]

## <a name="to-create-a-new-vendor-card"></a><span data-ttu-id="10228-114">To create a new vendor card</span><span class="sxs-lookup"><span data-stu-id="10228-114">To create a new vendor card</span></span>

1. <span data-ttu-id="10228-115">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Vendors**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="10228-115">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Vendors**, and then choose the related link.</span></span>  
2. <span data-ttu-id="10228-116">On the **Vendors** page, Choose **New**.</span><span class="sxs-lookup"><span data-stu-id="10228-116">On the **Vendors** page, Choose **New**.</span></span>

    <span data-ttu-id="10228-117">If more than one vendor template exists, then a page opens from which you can select a vendor template.</span><span class="sxs-lookup"><span data-stu-id="10228-117">If more than one vendor template exists, then a page opens from which you can select a vendor template.</span></span> <span data-ttu-id="10228-118">In that case, follow the next two steps.</span><span class="sxs-lookup"><span data-stu-id="10228-118">In that case, follow the next two steps.</span></span>
3. <span data-ttu-id="10228-119">On the **Select a template for a new vendor** page, choose the template that you want to use for the new vendor card.</span><span class="sxs-lookup"><span data-stu-id="10228-119">On the **Select a template for a new vendor** page, choose the template that you want to use for the new vendor card.</span></span>
4. <span data-ttu-id="10228-120">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="10228-120">Choose the **OK** button.</span></span> <span data-ttu-id="10228-121">A new vendor card opens with some fields filled with information from the template.</span><span class="sxs-lookup"><span data-stu-id="10228-121">A new vendor card opens with some fields filled with information from the template.</span></span>
5. <span data-ttu-id="10228-122">Proceed to fill or change fields on the vendor card as necessary.</span><span class="sxs-lookup"><span data-stu-id="10228-122">Proceed to fill or change fields on the vendor card as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

> [!NOTE]  
> <span data-ttu-id="10228-123">If you do not know the invoicing address that will be used for every invoice from a vendor, do not fill in the **Vendor No.** field.</span><span class="sxs-lookup"><span data-stu-id="10228-123">If you do not know the invoicing address that will be used for every invoice from a vendor, do not fill in the **Vendor No.** field.</span></span> <span data-ttu-id="10228-124">Instead, choose the pay-to vendor number after you have set up a purchase quote, order, or invoice header.</span><span class="sxs-lookup"><span data-stu-id="10228-124">Instead, choose the pay-to vendor number after you have set up a purchase quote, order, or invoice header.</span></span>

<span data-ttu-id="10228-125">The vendor is now registered, and the vendor card is ready to be used on purchase documents.</span><span class="sxs-lookup"><span data-stu-id="10228-125">The vendor is now registered, and the vendor card is ready to be used on purchase documents.</span></span>

<span data-ttu-id="10228-126">If you want to use this vendor card as a template when you create new vendor cards, you can save it as a vendor template.</span><span class="sxs-lookup"><span data-stu-id="10228-126">If you want to use this vendor card as a template when you create new vendor cards, you can save it as a vendor template.</span></span> <span data-ttu-id="10228-127">For more information, see the following section.</span><span class="sxs-lookup"><span data-stu-id="10228-127">For more information, see the following section.</span></span>

### <a name="deleting-vendor-cards"></a><span data-ttu-id="10228-128">Deleting Vendor Cards</span><span class="sxs-lookup"><span data-stu-id="10228-128">Deleting Vendor Cards</span></span>
<span data-ttu-id="10228-129">If you have posted a transaction for a vendor, you cannot delete the card because the ledger entries may be needed for auditing.</span><span class="sxs-lookup"><span data-stu-id="10228-129">If you have posted a transaction for a vendor, you cannot delete the card because the ledger entries may be needed for auditing.</span></span> <span data-ttu-id="10228-130">To delete vendor cards with ledger entries, contact to Microsoft partner to do so through code.</span><span class="sxs-lookup"><span data-stu-id="10228-130">To delete vendor cards with ledger entries, contact to Microsoft partner to do so through code.</span></span>

## <a name="to-save-the-vendor-card-as-a-template"></a><span data-ttu-id="10228-131">To save the vendor card as a template</span><span class="sxs-lookup"><span data-stu-id="10228-131">To save the vendor card as a template</span></span>
1. <span data-ttu-id="10228-132">On the **Vendor Card** page, choose the **Save as Template** action.</span><span class="sxs-lookup"><span data-stu-id="10228-132">On the **Vendor Card** page, choose the **Save as Template** action.</span></span> <span data-ttu-id="10228-133">The **Vendor Template** page opens showing the vendor card as a template.</span><span class="sxs-lookup"><span data-stu-id="10228-133">The **Vendor Template** page opens showing the vendor card as a template.</span></span>
2. <span data-ttu-id="10228-134">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="10228-134">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. <span data-ttu-id="10228-135">To reuse dimensions in templates, choose the **Dimensions** action.</span><span class="sxs-lookup"><span data-stu-id="10228-135">To reuse dimensions in templates, choose the **Dimensions** action.</span></span> <span data-ttu-id="10228-136">The **Dimension Templates** page opens showing any dimension codes that are set up for the vendor.</span><span class="sxs-lookup"><span data-stu-id="10228-136">The **Dimension Templates** page opens showing any dimension codes that are set up for the vendor.</span></span>
4. <span data-ttu-id="10228-137">Edit or enter dimension codes that will apply to new vendor cards created by using the template.</span><span class="sxs-lookup"><span data-stu-id="10228-137">Edit or enter dimension codes that will apply to new vendor cards created by using the template.</span></span>
5. <span data-ttu-id="10228-138">When you have completed the new vendor template, choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="10228-138">When you have completed the new vendor template, choose the **OK** button.</span></span>  
   <span data-ttu-id="10228-139">The vendor template is added to the list of vendor templates, so that you can use it to create new vendor cards.</span><span class="sxs-lookup"><span data-stu-id="10228-139">The vendor template is added to the list of vendor templates, so that you can use it to create new vendor cards.</span></span>

## <a name="see-also"></a><span data-ttu-id="10228-140">See Also</span><span class="sxs-lookup"><span data-stu-id="10228-140">See Also</span></span>
[<span data-ttu-id="10228-141">Merge Duplicate Records</span><span class="sxs-lookup"><span data-stu-id="10228-141">Merge Duplicate Records</span></span>](sales-how-merge-duplicate-records.md)  
[<span data-ttu-id="10228-142">Create Number Series</span><span class="sxs-lookup"><span data-stu-id="10228-142">Create Number Series</span></span>](ui-create-number-series.md)  
[<span data-ttu-id="10228-143">Purchasing</span><span class="sxs-lookup"><span data-stu-id="10228-143">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="10228-144">[Record Purchases](purchasing-how-record-purchases.md) </span><span class="sxs-lookup"><span data-stu-id="10228-144">[Record Purchases](purchasing-how-record-purchases.md) </span></span>  
<span data-ttu-id="10228-145">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="10228-145">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>  
