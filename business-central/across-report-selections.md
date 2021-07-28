---
title: Report Selection in Business Central
description: Learn about how to set up the reports that you use to print various types of documents in Business Central.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.search.keywords: setup, reporting
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 848b2ddc00f5006f31a0b2cff0a07d51ec305921
ms.sourcegitcommit: a7cb0be8eae6ece95f5259d7de7a48b385c9cfeb
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 07/08/2021
ms.locfileid: "6440815"
---
# <a name="report-selection-in-business-central"></a>Report Selection in Business Central

You can set up default reports that will be used to print the various documents for sales and purchases, such as orders, quotes, invoices, and credit memos. For example, if you have a specific layout for sales invoices, you can specify that report in the **Report Selections - Sales** page so that it will be used to send or print sales invoices.  

The **Report Selections** pages specify which report will be printed in different situations. [!INCLUDE [prod_short](includes/prod_short.md)] includes default configurations, but of course you can change these defaults. You can also add reports to the **Report Selection** pages if you want to print more than one report per document type, for example.  

## <a name="available-report-selections"></a>Available report selections

[!INCLUDE [prod_short](includes/prod_short.md)] includes different **Report Selection** pages for different areas. The following tables describes where you can find information about the different pages.  

|Area or task  |Learn more|
|--------------|----------|
|Example of how report selection works (Sales)|[Report selection for sales documents](#example-report-selection-for-sales-documents)|
|Default layout for emails with sales and purchase documents  |[Set Up Reusable Email Texts and Layouts for Sales and Purchase Documents](admin-how-setup-email.md#set-up-reusable-email-texts-and-layouts-for-sales-and-purchase-documents) |
|Define cheque layouts     |[Select a Cheque Layout](finance-how-define-check-layouts.md) |
|Define reports for GST reporting (Germany)|[Set Up Reports for GST and Intrastat](LocalFunctionality/Germany/how-to-set-up-reports-for-vat-and-intrastat.md) |

> [!TIP]
> Your [!INCLUDE [prod_short](includes/prod_short.md)] can include additional **Report Selection** pages, depending on your location and industry, for example. You can always check your setup by choosing the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, entering **Report Selections**, and then choose the relevant link.

The default version of [!INCLUDE [prod_short](includes/prod_short.md)] includes the following **Report Section** pages:

* **Report Selection - Sales**  
* **Report Selection - Purchase**  
* **Report Selection - Inventory**  
* **Report Selection - Cash Flow**  
* **Report Selection - Warehouse**  
* **Report Selection - Bank Account**  
* **Report Selections Reminder/Finance Charge**  

## <a name="example-report-selection-for-sales-documents"></a>Example: Report selection for sales documents

The **Report Selection - Sales** page defines the default reports to use in different scenarios for each related document type. Choose a document type in the **Usage** field, and then add or review the report selection. You can set up more than one report and the order of sequence that the reports must be sent or printed in.  

[!INCLUDE [tooltip-inline-tip_md](includes/tooltip-inline-tip_md.md)]

Some types of document can be sent as email attachments, and others cannot. Each **Report Selection** page shows additional fields if the type support email out of the box.  

For example, in the **Report Selection - Sales** and **Report Selection - Purchase** pages, the following fields help you set up emailing:

|Field name |Description  |
|-----------|-------------|
|**Use for Email Body**| Specifies that summarised information, such as invoice number, due date, and payment service link, will be inserted in the body of the email that you send.        |
|**Use for Email Attachment**| Specifies that the related document will be attached to the email.|
|**Email Body Layout Description**|Specifies the email body layout that is used, typically a custom report layout. |

## <a name="see-also"></a>See also

[Set Up Reusable Email Texts and Layouts for Sales and Purchase Documents](admin-how-setup-email.md#set-up-reusable-email-texts-and-layouts-for-sales-and-purchase-documents)  
[Select a Cheque Layout](finance-how-define-check-layouts.md)  
[Set Up Reports for GST and Intrastat (Germany)](LocalFunctionality/Germany/how-to-set-up-reports-for-vat-and-intrastat.md)  
[Managing Report and Document Layouts](ui-manage-report-layouts.md)  
[Define Document Layouts for Customers and Vendors](ui-define-customer-vendor-document-layouts.md)  
[Set Up Printers](ui-specify-printer-selection-reports.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]