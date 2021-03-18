---
title: Report Selection in Business Central
description: Learn about how to set up the reports that you use to print various types of documents in Business Central.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.search.keywords: setup, reporting
ms.date: 01/18/2021
ms.author: edupont
ms.openlocfilehash: 9d282ea35f7b4bdf317e818504f061d4145404bd
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "5379014"
---
# <a name="report-selection-in-business-central"></a><span data-ttu-id="15731-103">Report Selection in Business Central</span><span class="sxs-lookup"><span data-stu-id="15731-103">Report Selection in Business Central</span></span>

<span data-ttu-id="15731-104">You can set up default reports that will be used to print the various documents for sales and purchases, such as orders, quotes, invoices, and credit memos.</span><span class="sxs-lookup"><span data-stu-id="15731-104">You can set up default reports that will be used to print the various documents for sales and purchases, such as orders, quotes, invoices, and credit memos.</span></span> <span data-ttu-id="15731-105">For example, if you have a specific layout for sales invoices, you can specify that report in the **Report Selections - Sales** page so that it will be used to send or print sales invoices.</span><span class="sxs-lookup"><span data-stu-id="15731-105">For example, if you have a specific layout for sales invoices, you can specify that report in the **Report Selections - Sales** page so that it will be used to send or print sales invoices.</span></span>  

<span data-ttu-id="15731-106">The **Report Selections** pages specify which report will be printed in different situations.</span><span class="sxs-lookup"><span data-stu-id="15731-106">The **Report Selections** pages specify which report will be printed in different situations.</span></span> <span data-ttu-id="15731-107">[!INCLUDE [prod_short](includes/prod_short.md)] includes default configurations, but of course you can change these defaults.</span><span class="sxs-lookup"><span data-stu-id="15731-107">[!INCLUDE [prod_short](includes/prod_short.md)] includes default configurations, but of course you can change these defaults.</span></span> <span data-ttu-id="15731-108">You can also add reports to the **Report Selection** pages if you want to print more than one report per document type, for example.</span><span class="sxs-lookup"><span data-stu-id="15731-108">You can also add reports to the **Report Selection** pages if you want to print more than one report per document type, for example.</span></span>  

## <a name="available-report-selections"></a><span data-ttu-id="15731-109">Available report selections</span><span class="sxs-lookup"><span data-stu-id="15731-109">Available report selections</span></span>

<span data-ttu-id="15731-110">[!INCLUDE [prod_short](includes/prod_short.md)] includes different **Report Selection** pages for different areas.</span><span class="sxs-lookup"><span data-stu-id="15731-110">[!INCLUDE [prod_short](includes/prod_short.md)] includes different **Report Selection** pages for different areas.</span></span> <span data-ttu-id="15731-111">The following tables describes where you can find information about the different pages.</span><span class="sxs-lookup"><span data-stu-id="15731-111">The following tables describes where you can find information about the different pages.</span></span>  

|<span data-ttu-id="15731-112">Area or task</span><span class="sxs-lookup"><span data-stu-id="15731-112">Area or task</span></span>  |<span data-ttu-id="15731-113">Learn more</span><span class="sxs-lookup"><span data-stu-id="15731-113">Learn more</span></span>|
|--------------|----------|
|<span data-ttu-id="15731-114">Example of how report selection works (Sales)</span><span class="sxs-lookup"><span data-stu-id="15731-114">Example of how report selection works (Sales)</span></span>|[<span data-ttu-id="15731-115">Report selection for sales documents</span><span class="sxs-lookup"><span data-stu-id="15731-115">Report selection for sales documents</span></span>](#example-report-selection-for-sales-documents)|
|<span data-ttu-id="15731-116">Default layout for emails with sales and purchase documents</span><span class="sxs-lookup"><span data-stu-id="15731-116">Default layout for emails with sales and purchase documents</span></span>  |[<span data-ttu-id="15731-117">Set Up Reusable Email Texts and Layouts for Sales and Purchase Documents</span><span class="sxs-lookup"><span data-stu-id="15731-117">Set Up Reusable Email Texts and Layouts for Sales and Purchase Documents</span></span>](admin-how-setup-email.md#set-up-reusable-email-texts-and-layouts-for-sales-and-purchase-documents) |
|<span data-ttu-id="15731-118">Define cheque layouts</span><span class="sxs-lookup"><span data-stu-id="15731-118">Define check layouts</span></span>     |[<span data-ttu-id="15731-119">Select a Cheque Layout</span><span class="sxs-lookup"><span data-stu-id="15731-119">Select a Check Layout</span></span>](finance-how-define-check-layouts.md) |
|<span data-ttu-id="15731-120">Define reports for GST reporting (Germany)</span><span class="sxs-lookup"><span data-stu-id="15731-120">Define reports for VAT reporting (Germany)</span></span>|[<span data-ttu-id="15731-121">Set Up Reports for GST and Intrastat</span><span class="sxs-lookup"><span data-stu-id="15731-121">Set Up Reports for VAT and Intrastat</span></span>](LocalFunctionality/Germany/how-to-set-up-reports-for-vat-and-intrastat.md) |

> [!TIP]
> <span data-ttu-id="15731-122">Your [!INCLUDE [prod_short](includes/prod_short.md)] can include additional **Report Selection** pages, depending on your location and industry, for example.</span><span class="sxs-lookup"><span data-stu-id="15731-122">Your [!INCLUDE [prod_short](includes/prod_short.md)] can include additional **Report Selection** pages, depending on your location and industry, for example.</span></span> <span data-ttu-id="15731-123">You can always check your setup by choosing the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, entering **Report Selections**, and then choose the relevant link.</span><span class="sxs-lookup"><span data-stu-id="15731-123">You can always check your setup by choosing the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, entering **Report Selections**, and then choose the relevant link.</span></span>

<span data-ttu-id="15731-124">The default version of [!INCLUDE [prod_short](includes/prod_short.md)] includes the following **Report Section** pages:</span><span class="sxs-lookup"><span data-stu-id="15731-124">The default version of [!INCLUDE [prod_short](includes/prod_short.md)] includes the following **Report Section** pages:</span></span>

* <span data-ttu-id="15731-125">**Report Selection - Sales**</span><span class="sxs-lookup"><span data-stu-id="15731-125">**Report Selection - Sales**</span></span>  
* <span data-ttu-id="15731-126">**Report Selection - Purchase**</span><span class="sxs-lookup"><span data-stu-id="15731-126">**Report Selection - Purchase**</span></span>  
* <span data-ttu-id="15731-127">**Report Selection - Inventory**</span><span class="sxs-lookup"><span data-stu-id="15731-127">**Report Selection - Inventory**</span></span>  
* <span data-ttu-id="15731-128">**Report Selection - Cash Flow**</span><span class="sxs-lookup"><span data-stu-id="15731-128">**Report Selection - Cash Flow**</span></span>  
* <span data-ttu-id="15731-129">**Report Selection - Warehouse**</span><span class="sxs-lookup"><span data-stu-id="15731-129">**Report Selection - Warehouse**</span></span>  
* <span data-ttu-id="15731-130">**Report Selection - Bank Account**</span><span class="sxs-lookup"><span data-stu-id="15731-130">**Report Selection - Bank Account**</span></span>  
* <span data-ttu-id="15731-131">**Report Selections Reminder/Finance Charge**</span><span class="sxs-lookup"><span data-stu-id="15731-131">**Report Selections Reminder/Finance Charge**</span></span>  

## <a name="example-report-selection-for-sales-documents"></a><span data-ttu-id="15731-132">Example: Report selection for sales documents</span><span class="sxs-lookup"><span data-stu-id="15731-132">Example: Report selection for sales documents</span></span>

<span data-ttu-id="15731-133">The **Report Selection - Sales** page defines the default reports to use in different scenarios for each related document type.</span><span class="sxs-lookup"><span data-stu-id="15731-133">The **Report Selection - Sales** page defines the default reports to use in different scenarios for each related document type.</span></span> <span data-ttu-id="15731-134">Choose a document type in the **Usage** field, and then add or review the report selection.</span><span class="sxs-lookup"><span data-stu-id="15731-134">Choose a document type in the **Usage** field, and then add or review the report selection.</span></span> <span data-ttu-id="15731-135">You can set up more than one report and the order of sequence that the reports must be sent or printed in.</span><span class="sxs-lookup"><span data-stu-id="15731-135">You can set up more than one report and the order of sequence that the reports must be sent or printed in.</span></span>  

[!INCLUDE [tooltip-inline-tip_md](includes/tooltip-inline-tip_md.md)]

<span data-ttu-id="15731-136">Some types of document can be sent as email attachments, and others cannot.</span><span class="sxs-lookup"><span data-stu-id="15731-136">Some types of document can be sent as email attachments, and others cannot.</span></span> <span data-ttu-id="15731-137">Each **Report Selection** page shows additional fields if the type support email out of the box.</span><span class="sxs-lookup"><span data-stu-id="15731-137">Each **Report Selection** page shows additional fields if the type support email out of the box.</span></span>  

<span data-ttu-id="15731-138">For example, in the **Report Selection - Sales** and **Report Selection - Purchase** pages, the following fields help you set up emailing:</span><span class="sxs-lookup"><span data-stu-id="15731-138">For example, in the **Report Selection - Sales** and **Report Selection - Purchase** pages, the following fields help you set up emailing:</span></span>

|<span data-ttu-id="15731-139">Field name</span><span class="sxs-lookup"><span data-stu-id="15731-139">Field name</span></span> |<span data-ttu-id="15731-140">Description</span><span class="sxs-lookup"><span data-stu-id="15731-140">Description</span></span>  |
|-----------|-------------|
|<span data-ttu-id="15731-141">**Use for Email Body**</span><span class="sxs-lookup"><span data-stu-id="15731-141">**Use for Email Body**</span></span>| <span data-ttu-id="15731-142">Specifies that summarised information, such as invoice number, due date, and payment service link, will be inserted in the body of the email that you send.</span><span class="sxs-lookup"><span data-stu-id="15731-142">Specifies that summarized information, such as invoice number, due date, and payment service link, will be inserted in the body of the email that you send.</span></span>        |
|<span data-ttu-id="15731-143">**Use for Email Attachment**</span><span class="sxs-lookup"><span data-stu-id="15731-143">**Use for Email Attachment**</span></span>| <span data-ttu-id="15731-144">Specifies that the related document will be attached to the email.</span><span class="sxs-lookup"><span data-stu-id="15731-144">Specifies that the related document will be attached to the email.</span></span>|
|<span data-ttu-id="15731-145">**Email Body Layout Description**</span><span class="sxs-lookup"><span data-stu-id="15731-145">**Email Body Layout Description**</span></span>|<span data-ttu-id="15731-146">Specifies the email body layout that is used, typically a custom report layout.</span><span class="sxs-lookup"><span data-stu-id="15731-146">Specifies the email body layout that is used, typically a custom report layout.</span></span> |

## <a name="see-also"></a><span data-ttu-id="15731-147">See also</span><span class="sxs-lookup"><span data-stu-id="15731-147">See also</span></span>

[<span data-ttu-id="15731-148">Set Up Reusable Email Texts and Layouts for Sales and Purchase Documents</span><span class="sxs-lookup"><span data-stu-id="15731-148">Set Up Reusable Email Texts and Layouts for Sales and Purchase Documents</span></span>](admin-how-setup-email.md#set-up-reusable-email-texts-and-layouts-for-sales-and-purchase-documents)  
[<span data-ttu-id="15731-149">Select a Cheque Layout</span><span class="sxs-lookup"><span data-stu-id="15731-149">Select a Check Layout</span></span>](finance-how-define-check-layouts.md)  
[<span data-ttu-id="15731-150">Set Up Reports for GST and Intrastat (Germany)</span><span class="sxs-lookup"><span data-stu-id="15731-150">Set Up Reports for VAT and Intrastat (Germany)</span></span>](LocalFunctionality/Germany/how-to-set-up-reports-for-vat-and-intrastat.md)  
[<span data-ttu-id="15731-151">Managing Report and Document Layouts</span><span class="sxs-lookup"><span data-stu-id="15731-151">Managing Report and Document Layouts</span></span>](ui-manage-report-layouts.md)  
[<span data-ttu-id="15731-152">Define Document Layouts for Customers and Vendors</span><span class="sxs-lookup"><span data-stu-id="15731-152">Define Document Layouts for Customers and Vendors</span></span>](ui-define-customer-vendor-document-layouts.md)  
[<span data-ttu-id="15731-153">Set Up Printers</span><span class="sxs-lookup"><span data-stu-id="15731-153">Set Up Printers</span></span>](ui-specify-printer-selection-reports.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]