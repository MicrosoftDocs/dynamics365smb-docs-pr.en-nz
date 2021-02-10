---
title: Report Selection in Business Central
description: Learn about how to set up the reports that you use to print various types of documents in Business Central.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.search.keywords: setup, reporting
ms.date: 01/18/2021
ms.author: edupont
ms.openlocfilehash: d30baa44894658c03c3deffdf24a7923293b88fd
ms.sourcegitcommit: 32bfc2acaaf3693afc9aeb86feea505fd328caa1
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 01/19/2021
ms.locfileid: "5024653"
---
# <a name="report-selection-in-business-central"></a><span data-ttu-id="a5fc9-103">Report Selection in Business Central</span><span class="sxs-lookup"><span data-stu-id="a5fc9-103">Report Selection in Business Central</span></span>

<span data-ttu-id="a5fc9-104">You can set up default reports that will be used to print the various documents for sales and purchases, such as orders, quotes, invoices, and credit memos.</span><span class="sxs-lookup"><span data-stu-id="a5fc9-104">You can set up default reports that will be used to print the various documents for sales and purchases, such as orders, quotes, invoices, and credit memos.</span></span> <span data-ttu-id="a5fc9-105">For example, if you have a specific layout for sales invoices, you can specify that report in the **Report Selections - Sales** page so that it will be used to send or print sales invoices.</span><span class="sxs-lookup"><span data-stu-id="a5fc9-105">For example, if you have a specific layout for sales invoices, you can specify that report in the **Report Selections - Sales** page so that it will be used to send or print sales invoices.</span></span>  

<span data-ttu-id="a5fc9-106">The **Report Selections** pages specify which report will be printed in different situations.</span><span class="sxs-lookup"><span data-stu-id="a5fc9-106">The **Report Selections** pages specify which report will be printed in different situations.</span></span> <span data-ttu-id="a5fc9-107">[!INCLUDE [prod_short](includes/prod_short.md)] includes default configurations, but of course you can change these defaults.</span><span class="sxs-lookup"><span data-stu-id="a5fc9-107">[!INCLUDE [prod_short](includes/prod_short.md)] includes default configurations, but of course you can change these defaults.</span></span> <span data-ttu-id="a5fc9-108">You can also add reports to the **Report Selection** pages if you want to print more than one report per document type, for example.</span><span class="sxs-lookup"><span data-stu-id="a5fc9-108">You can also add reports to the **Report Selection** pages if you want to print more than one report per document type, for example.</span></span>  

## <a name="available-report-selections"></a><span data-ttu-id="a5fc9-109">Available report selections</span><span class="sxs-lookup"><span data-stu-id="a5fc9-109">Available report selections</span></span>

<span data-ttu-id="a5fc9-110">[!INCLUDE [prod_short](includes/prod_short.md)] includes different **Report Selection** pages for different areas.</span><span class="sxs-lookup"><span data-stu-id="a5fc9-110">[!INCLUDE [prod_short](includes/prod_short.md)] includes different **Report Selection** pages for different areas.</span></span> <span data-ttu-id="a5fc9-111">The following tables describes where you can find information about the different pages.</span><span class="sxs-lookup"><span data-stu-id="a5fc9-111">The following tables describes where you can find information about the different pages.</span></span>  

|<span data-ttu-id="a5fc9-112">Area or task</span><span class="sxs-lookup"><span data-stu-id="a5fc9-112">Area or task</span></span>  |<span data-ttu-id="a5fc9-113">Learn more</span><span class="sxs-lookup"><span data-stu-id="a5fc9-113">Learn more</span></span>|
|--------------|----------|
|<span data-ttu-id="a5fc9-114">Example of how report selection works (Sales)</span><span class="sxs-lookup"><span data-stu-id="a5fc9-114">Example of how report selection works (Sales)</span></span>|[<span data-ttu-id="a5fc9-115">Report selection for sales documents</span><span class="sxs-lookup"><span data-stu-id="a5fc9-115">Report selection for sales documents</span></span>](#example-report-selection-for-sales-documents)|
|<span data-ttu-id="a5fc9-116">Default layout for emails with sales and purchase documents</span><span class="sxs-lookup"><span data-stu-id="a5fc9-116">Default layout for emails with sales and purchase documents</span></span>  |[<span data-ttu-id="a5fc9-117">Set Up Reusable Email Texts and Layouts for Sales and Purchase Documents</span><span class="sxs-lookup"><span data-stu-id="a5fc9-117">Set Up Reusable Email Texts and Layouts for Sales and Purchase Documents</span></span>](admin-how-setup-email.md#set-up-reusable-email-texts-and-layouts-for-sales-and-purchase-documents) |
|<span data-ttu-id="a5fc9-118">Define cheque layouts</span><span class="sxs-lookup"><span data-stu-id="a5fc9-118">Define check layouts</span></span>     |[<span data-ttu-id="a5fc9-119">Select a Cheque Layout</span><span class="sxs-lookup"><span data-stu-id="a5fc9-119">Select a Check Layout</span></span>](finance-how-define-check-layouts.md) |
|<span data-ttu-id="a5fc9-120">Define reports for GST reporting (Germany)</span><span class="sxs-lookup"><span data-stu-id="a5fc9-120">Define reports for VAT reporting (Germany)</span></span>|[<span data-ttu-id="a5fc9-121">Set Up Reports for GST and Intrastat</span><span class="sxs-lookup"><span data-stu-id="a5fc9-121">Set Up Reports for VAT and Intrastat</span></span>](LocalFunctionality/Germany/how-to-set-up-reports-for-vat-and-intrastat.md) |

> [!TIP]
> <span data-ttu-id="a5fc9-122">Your [!INCLUDE [prod_short](includes/prod_short.md)] can include additional **Report Selection** pages, depending on your location and industry, for example.</span><span class="sxs-lookup"><span data-stu-id="a5fc9-122">Your [!INCLUDE [prod_short](includes/prod_short.md)] can include additional **Report Selection** pages, depending on your location and industry, for example.</span></span> <span data-ttu-id="a5fc9-123">You can always check your setup by choosing the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, entering **Report Selections**, and then choose the relevant link.</span><span class="sxs-lookup"><span data-stu-id="a5fc9-123">You can always check your setup by choosing the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, entering **Report Selections**, and then choose the relevant link.</span></span>

<span data-ttu-id="a5fc9-124">The default version of [!INCLUDE [prod_short](includes/prod_short.md)] includes the following **Report Section** pages:</span><span class="sxs-lookup"><span data-stu-id="a5fc9-124">The default version of [!INCLUDE [prod_short](includes/prod_short.md)] includes the following **Report Section** pages:</span></span>

* <span data-ttu-id="a5fc9-125">**Report Selection - Sales**</span><span class="sxs-lookup"><span data-stu-id="a5fc9-125">**Report Selection - Sales**</span></span>  
* <span data-ttu-id="a5fc9-126">**Report Selection - Purchase**</span><span class="sxs-lookup"><span data-stu-id="a5fc9-126">**Report Selection - Purchase**</span></span>  
* <span data-ttu-id="a5fc9-127">**Report Selection - Inventory**</span><span class="sxs-lookup"><span data-stu-id="a5fc9-127">**Report Selection - Inventory**</span></span>  
* <span data-ttu-id="a5fc9-128">**Report Selection - Cash Flow**</span><span class="sxs-lookup"><span data-stu-id="a5fc9-128">**Report Selection - Cash Flow**</span></span>  
* <span data-ttu-id="a5fc9-129">**Report Selection - Warehouse**</span><span class="sxs-lookup"><span data-stu-id="a5fc9-129">**Report Selection - Warehouse**</span></span>  
* <span data-ttu-id="a5fc9-130">**Report Selection - Bank Account**</span><span class="sxs-lookup"><span data-stu-id="a5fc9-130">**Report Selection - Bank Account**</span></span>  
* <span data-ttu-id="a5fc9-131">**Report Selections Reminder/Finance Charge**</span><span class="sxs-lookup"><span data-stu-id="a5fc9-131">**Report Selections Reminder/Finance Charge**</span></span>  

## <a name="example-report-selection-for-sales-documents"></a><span data-ttu-id="a5fc9-132">Example: Report selection for sales documents</span><span class="sxs-lookup"><span data-stu-id="a5fc9-132">Example: Report selection for sales documents</span></span>

<span data-ttu-id="a5fc9-133">The **Report Selection - Sales** page defines the default reports to use in different scenarios for each related document type.</span><span class="sxs-lookup"><span data-stu-id="a5fc9-133">The **Report Selection - Sales** page defines the default reports to use in different scenarios for each related document type.</span></span> <span data-ttu-id="a5fc9-134">Choose a document type in the **Usage** field, and then add or review the report selection.</span><span class="sxs-lookup"><span data-stu-id="a5fc9-134">Choose a document type in the **Usage** field, and then add or review the report selection.</span></span> <span data-ttu-id="a5fc9-135">You can set up more than one report and the order of sequence that the reports must be sent or printed in.</span><span class="sxs-lookup"><span data-stu-id="a5fc9-135">You can set up more than one report and the order of sequence that the reports must be sent or printed in.</span></span>  

[!INCLUDE [tooltip-inline-tip_md](includes/tooltip-inline-tip_md.md)]

<span data-ttu-id="a5fc9-136">Some types of document can be sent as email attachments, and others cannot.</span><span class="sxs-lookup"><span data-stu-id="a5fc9-136">Some types of document can be sent as email attachments, and others cannot.</span></span> <span data-ttu-id="a5fc9-137">Each **Report Selection** page shows additional fields if the type support email out of the box.</span><span class="sxs-lookup"><span data-stu-id="a5fc9-137">Each **Report Selection** page shows additional fields if the type support email out of the box.</span></span>  

<span data-ttu-id="a5fc9-138">For example, in the **Report Selection - Sales** and **Report Selection - Purchase** pages, the following fields help you set up emailing:</span><span class="sxs-lookup"><span data-stu-id="a5fc9-138">For example, in the **Report Selection - Sales** and **Report Selection - Purchase** pages, the following fields help you set up emailing:</span></span>

|<span data-ttu-id="a5fc9-139">Field name</span><span class="sxs-lookup"><span data-stu-id="a5fc9-139">Field name</span></span> |<span data-ttu-id="a5fc9-140">Description</span><span class="sxs-lookup"><span data-stu-id="a5fc9-140">Description</span></span>  |
|-----------|-------------|
|<span data-ttu-id="a5fc9-141">**Use for Email Body**</span><span class="sxs-lookup"><span data-stu-id="a5fc9-141">**Use for Email Body**</span></span>| <span data-ttu-id="a5fc9-142">Specifies that summarised information, such as invoice number, due date, and payment service link, will be inserted in the body of the email that you send.</span><span class="sxs-lookup"><span data-stu-id="a5fc9-142">Specifies that summarized information, such as invoice number, due date, and payment service link, will be inserted in the body of the email that you send.</span></span>        |
|<span data-ttu-id="a5fc9-143">**Use for Email Attachment**</span><span class="sxs-lookup"><span data-stu-id="a5fc9-143">**Use for Email Attachment**</span></span>| <span data-ttu-id="a5fc9-144">Specifies that the related document will be attached to the email.</span><span class="sxs-lookup"><span data-stu-id="a5fc9-144">Specifies that the related document will be attached to the email.</span></span>|
|<span data-ttu-id="a5fc9-145">**Email Body Layout Description**</span><span class="sxs-lookup"><span data-stu-id="a5fc9-145">**Email Body Layout Description**</span></span>|<span data-ttu-id="a5fc9-146">Specifies the email body layout that is used, typically a custom report layout.</span><span class="sxs-lookup"><span data-stu-id="a5fc9-146">Specifies the email body layout that is used, typically a custom report layout.</span></span> |

## <a name="see-also"></a><span data-ttu-id="a5fc9-147">See also</span><span class="sxs-lookup"><span data-stu-id="a5fc9-147">See also</span></span>

[<span data-ttu-id="a5fc9-148">Set Up Reusable Email Texts and Layouts for Sales and Purchase Documents</span><span class="sxs-lookup"><span data-stu-id="a5fc9-148">Set Up Reusable Email Texts and Layouts for Sales and Purchase Documents</span></span>](admin-how-setup-email.md#set-up-reusable-email-texts-and-layouts-for-sales-and-purchase-documents)  
[<span data-ttu-id="a5fc9-149">Select a Cheque Layout</span><span class="sxs-lookup"><span data-stu-id="a5fc9-149">Select a Check Layout</span></span>](finance-how-define-check-layouts.md)  
[<span data-ttu-id="a5fc9-150">Set Up Reports for GST and Intrastat (Germany)</span><span class="sxs-lookup"><span data-stu-id="a5fc9-150">Set Up Reports for VAT and Intrastat (Germany)</span></span>](LocalFunctionality/Germany/how-to-set-up-reports-for-vat-and-intrastat.md)  
[<span data-ttu-id="a5fc9-151">Managing Report and Document Layouts</span><span class="sxs-lookup"><span data-stu-id="a5fc9-151">Managing Report and Document Layouts</span></span>](ui-manage-report-layouts.md)  
[<span data-ttu-id="a5fc9-152">Define Document Layouts for Customers and Vendors</span><span class="sxs-lookup"><span data-stu-id="a5fc9-152">Define Document Layouts for Customers and Vendors</span></span>](ui-define-customer-vendor-document-layouts.md)  
[<span data-ttu-id="a5fc9-153">Set Up Printers</span><span class="sxs-lookup"><span data-stu-id="a5fc9-153">Set Up Printers</span></span>](ui-specify-printer-selection-reports.md)  
