---
title: Set up SEPA credit transfer | Microsoft Docs
description: Learn how to set up SEPA credit transfer in Business Central .
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: sepa, credit, transfer, payment,
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: 011bae78fd3ee065e63dd0acb39a087c8742c6a8
ms.contentlocale: en-nz
ms.lasthandoff: 09/28/2018

---
# <a name="set-up-sepa-credit-transfer"></a><span data-ttu-id="048bf-103">Set Up SEPA Credit Transfer</span><span class="sxs-lookup"><span data-stu-id="048bf-103">Set Up SEPA Credit Transfer</span></span>
<span data-ttu-id="048bf-104">From the **Payment Journal** window, you can export payments to a file for upload to your electronic bank for processing of the related money transfers.</span><span class="sxs-lookup"><span data-stu-id="048bf-104">From the **Payment Journal** window, you can export payments to a file for upload to your electronic bank for processing of the related money transfers.</span></span> [!INCLUDE[d365fin](includes/d365fin_md.md)] <span data-ttu-id="048bf-105">supports the SEPA Credit Transfer format, but in your country/region, other formats for electronic payments may be available.</span><span class="sxs-lookup"><span data-stu-id="048bf-105"> supports the SEPA Credit Transfer format, but in your country/region, other formats for electronic payments may be available.</span></span>  

<span data-ttu-id="048bf-106">To enable export of a bank file formats that are not supported out of the box in [!INCLUDE[d365fin](includes/d365fin_md.md)] , you can set up a data exchange definition by using the data exchange framework.</span><span class="sxs-lookup"><span data-stu-id="048bf-106">To enable export of a bank file formats that are not supported out of the box in [!INCLUDE[d365fin](includes/d365fin_md.md)], you can set up a data exchange definition by using the data exchange framework.</span></span> <span data-ttu-id="048bf-107">For more information, see [Set Up Data Exchange Definitions](across-how-to-set-up-data-exchange-definitions.md).</span><span class="sxs-lookup"><span data-stu-id="048bf-107">For more information, see [Set Up Data Exchange Definitions](across-how-to-set-up-data-exchange-definitions.md).</span></span>  

<span data-ttu-id="048bf-108">Before you can process payment electronically by exporting payment files in the SEPA Credit Transfer format, you must perform the following setup steps:</span><span class="sxs-lookup"><span data-stu-id="048bf-108">Before you can process payment electronically by exporting payment files in the SEPA Credit Transfer format, you must perform the following setup steps:</span></span>  

* <span data-ttu-id="048bf-109">Set up the bank account in question to handle the SEPA Credit Transfer format</span><span class="sxs-lookup"><span data-stu-id="048bf-109">Set up the bank account in question to handle the SEPA Credit Transfer format</span></span>  
* <span data-ttu-id="048bf-110">Set up vendor cards to process payments by exporting files in the SEPA Credit Transfer format</span><span class="sxs-lookup"><span data-stu-id="048bf-110">Set up vendor cards to process payments by exporting files in the SEPA Credit Transfer format</span></span>  
* <span data-ttu-id="048bf-111">Set up the related general journal batch to enable payment export from the **Payment Journal** window</span><span class="sxs-lookup"><span data-stu-id="048bf-111">Set up the related general journal batch to enable payment export from the **Payment Journal** window</span></span>  
* <span data-ttu-id="048bf-112">Connect the data exchange definition for one or more payment types with the relevant payment method or methods</span><span class="sxs-lookup"><span data-stu-id="048bf-112">Connect the data exchange definition for one or more payment types with the relevant payment method or methods</span></span>  

### <a name="to-set-up-a-bank-account-for-sepa-credit-transfer"></a><span data-ttu-id="048bf-113">To set up a bank account for SEPA Credit Transfer</span><span class="sxs-lookup"><span data-stu-id="048bf-113">To set up a bank account for SEPA Credit Transfer</span></span>  
1. <span data-ttu-id="048bf-114">In the **Search** box, enter **Bank Accounts**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="048bf-114">In the **Search** box, enter **Bank Accounts**, and then choose the related link.</span></span>  
2. <span data-ttu-id="048bf-115">Open the card of the bank account from which you will export payment files in the SEPA Credit Transfer format.</span><span class="sxs-lookup"><span data-stu-id="048bf-115">Open the card of the bank account from which you will export payment files in the SEPA Credit Transfer format.</span></span>  
3. <span data-ttu-id="048bf-116">On the **Transfer** FastTab, in the **Payment Export Format** field, choose **SEPADD**.</span><span class="sxs-lookup"><span data-stu-id="048bf-116">On the **Transfer** FastTab, in the **Payment Export Format** field, choose **SEPADD**.</span></span>  
4. <span data-ttu-id="048bf-117">In the **SEPA CT Msg. ID No. Series** field, choose a number series from which numbers are assigned to SEPA credit transfer entries.</span><span class="sxs-lookup"><span data-stu-id="048bf-117">In the **SEPA CT Msg. ID No. Series** field, choose a number series from which numbers are assigned to SEPA credit transfer entries.</span></span>  
5. <span data-ttu-id="048bf-118">Make sure the **IBAN** field is filled.</span><span class="sxs-lookup"><span data-stu-id="048bf-118">Make sure the **IBAN** field is filled.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="048bf-119">The **Currency Code** field must be set to **EUR**, because SEPA credit transfers can only be made in the EURO currency.</span><span class="sxs-lookup"><span data-stu-id="048bf-119">The **Currency Code** field must be set to **EUR**, because SEPA credit transfers can only be made in the EURO currency.</span></span>  

### <a name="to-set-up-a-vendor-card-for-sepa-credit-transfer"></a><span data-ttu-id="048bf-120">To set up a vendor card for SEPA Credit Transfer</span><span class="sxs-lookup"><span data-stu-id="048bf-120">To set up a vendor card for SEPA Credit Transfer</span></span>  
1. <span data-ttu-id="048bf-121">In the **Search** box, enter **Vendors**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="048bf-121">In the **Search** box, enter **Vendors**, and then choose the related link.</span></span>  
2. <span data-ttu-id="048bf-122">Open the card of the vendor whom you will pay electronically by export payment files in the SEPA Credit Transfer format.</span><span class="sxs-lookup"><span data-stu-id="048bf-122">Open the card of the vendor whom you will pay electronically by export payment files in the SEPA Credit Transfer format.</span></span>  
3. <span data-ttu-id="048bf-123">On the **Payment** FastTab, in the **Payment Method Code** field, choose **BANK**.</span><span class="sxs-lookup"><span data-stu-id="048bf-123">On the **Payment** FastTab, in the **Payment Method Code** field, choose **BANK**.</span></span>  
4. <span data-ttu-id="048bf-124">In the **Preferred Bank Account** field, choose the bank to which the money will be transferred when it is processed by your electronic bank.</span><span class="sxs-lookup"><span data-stu-id="048bf-124">In the **Preferred Bank Account** field, choose the bank to which the money will be transferred when it is processed by your electronic bank.</span></span>  

     <span data-ttu-id="048bf-125">The value in the **Preferred Bank Account** field is copied to the **Recipient Bank Account** field in the **Payment Journal** window.</span><span class="sxs-lookup"><span data-stu-id="048bf-125">The value in the **Preferred Bank Account** field is copied to the **Recipient Bank Account** field in the **Payment Journal** window.</span></span>  

### <a name="to-set-the-payment-journal-up-to-export-payment-files"></a><span data-ttu-id="048bf-126">To set the payment journal up to export payment files</span><span class="sxs-lookup"><span data-stu-id="048bf-126">To set the payment journal up to export payment files</span></span>  
1. <span data-ttu-id="048bf-127">In the **Search** box, enter **Payment Journals**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="048bf-127">In the **Search** box, enter **Payment Journals**, and then choose the related link.</span></span>  
2. <span data-ttu-id="048bf-128">Open the payment journal that you use to process payments by exporting files in the SEPA Credit Transfer format.</span><span class="sxs-lookup"><span data-stu-id="048bf-128">Open the payment journal that you use to process payments by exporting files in the SEPA Credit Transfer format.</span></span>  
3. <span data-ttu-id="048bf-129">In the **Batch Name** field, choose the drop\-down button.</span><span class="sxs-lookup"><span data-stu-id="048bf-129">In the **Batch Name** field, choose the drop\-down button.</span></span>  
4. <span data-ttu-id="048bf-130">In the **General Journal Batches** window, on the **Home** tab, in the **Manage** group, choose **Edit List**.</span><span class="sxs-lookup"><span data-stu-id="048bf-130">In the **General Journal Batches** window, on the **Home** tab, in the **Manage** group, choose **Edit List**.</span></span>  
5. <span data-ttu-id="048bf-131">On the line for the payment journal that you will use to export payments, select the **Allow Payment Export** check box.</span><span class="sxs-lookup"><span data-stu-id="048bf-131">On the line for the payment journal that you will use to export payments, select the **Allow Payment Export** check box.</span></span>  

### <a name="to-connect-the-data-exchange-definition-for-one-or-more-payment-types-with-the-relevant-payment-method-or-methods"></a><span data-ttu-id="048bf-132">To connect the data exchange definition for one or more payment types with the relevant payment method or methods</span><span class="sxs-lookup"><span data-stu-id="048bf-132">To connect the data exchange definition for one or more payment types with the relevant payment method or methods</span></span>  
1. <span data-ttu-id="048bf-133">In the **Search** box, enter **Payment Methods**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="048bf-133">In the **Search** box, enter **Payment Methods**, and then choose the related link.</span></span>  
2. <span data-ttu-id="048bf-134">In the **Payment Methods** window, select the payment method that is used to export payments from, and then choose the **Pmt. Export Line Definition** field.</span><span class="sxs-lookup"><span data-stu-id="048bf-134">In the **Payment Methods** window, select the payment method that is used to export payments from, and then choose the **Pmt. Export Line Definition** field.</span></span>  
3. <span data-ttu-id="048bf-135">In the **Pmt. Export Line Definitions** window, select the code that you specified in the **Code** field on the **Line Definitions** FastTab in step 4 in the “To describe the formatting of lines and columns in the file” section in the [Set Up Data Exchange Definitions](across-how-to-set-up-data-exchange-definitions.md) procedure.</span><span class="sxs-lookup"><span data-stu-id="048bf-135">In the **Pmt. Export Line Definitions** window, select the code that you specified in the **Code** field on the **Line Definitions** FastTab in step 4 in the “To describe the formatting of lines and columns in the file” section in the [Set Up Data Exchange Definitions](across-how-to-set-up-data-exchange-definitions.md) procedure.</span></span>  

    <span data-ttu-id="048bf-136">The direct-debit mandate is automatically inserted in the **Direct Debit Mandate ID** field when you create a sales invoice for the customer that you selected in step 2.</span><span class="sxs-lookup"><span data-stu-id="048bf-136">The direct-debit mandate is automatically inserted in the **Direct Debit Mandate ID** field when you create a sales invoice for the customer that you selected in step 2.</span></span> <span data-ttu-id="048bf-137">For more information, see [Create Recurring Sales and Purchase Lines](sales-how-work-standard-lines.md).</span><span class="sxs-lookup"><span data-stu-id="048bf-137">For more information, see [Create Recurring Sales and Purchase Lines](sales-how-work-standard-lines.md).</span></span>  

## <a name="see-also"></a><span data-ttu-id="048bf-138">See Also</span><span class="sxs-lookup"><span data-stu-id="048bf-138">See Also</span></span>  
[<span data-ttu-id="048bf-139">Collecting Payments with SEPA Direct Debit</span><span class="sxs-lookup"><span data-stu-id="048bf-139">Collecting Payments with SEPA Direct Debit</span></span>](finance-collect-payments-with-sepa-direct-debit.md)  
[<span data-ttu-id="048bf-140">Set Up Data Exchange Definitions</span><span class="sxs-lookup"><span data-stu-id="048bf-140">Set Up Data Exchange Definitions</span></span>](across-how-to-set-up-data-exchange-definitions.md)  
[<span data-ttu-id="048bf-141">Create Recurring Sales and Purchase Lines</span><span class="sxs-lookup"><span data-stu-id="048bf-141">Create Recurring Sales and Purchase Lines</span></span>](sales-how-work-standard-lines.md)  
[<span data-ttu-id="048bf-142">Exchanging Data Electronically</span><span class="sxs-lookup"><span data-stu-id="048bf-142">Exchanging Data Electronically</span></span>](across-data-exchange.md)  

