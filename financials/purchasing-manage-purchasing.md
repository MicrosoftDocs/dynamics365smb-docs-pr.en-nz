---
title: Overview of Tasks to Manage Purchasing | Microsoft Docs
description: Outlines tasks to manage your purchasing or procurement processes, including how purchase invoices and purchase orders work.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: procurement, supply, vendor order
ms.date: 08/10/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: f9a932a521cd14e52e2a73e69544d2950235ea35
ms.contentlocale: en-nz
ms.lasthandoff: 09/22/2017

---
# <a name="purchasing"></a>Purchasing
You create a purchase invoice or purchase order to record the cost of purchases and to track accounts payable. If you need to control an inventory, purchase invoices are also used to dynamically update inventory levels so that you can minimise your inventory costs and provide better customer service. The purchasing costs, including service expenses, and inventory values that result from posting purchase invoices contribute to profit figures and other financial KPIs on your Home page.

You must use purchase orders if your purchasing process requires that you record partial receipts of an order quantity, for example, because the full quantity was not available at the vendor. If you sell items by delivering directly from your vendor to your customer, as a drop shipment, then you must also use purchase orders. For more information, see [How to: Make Drop Shipments](sales-how-drop-shipment.md). In all other aspects, purchase orders work the same way as purchase invoices.

You can have purchase invoices created automatically by using the OCR (Optical Character Recognition) service to convert PDF invoices from your vendors to electronic documents, which are then converted to purchase invoices by a workflow. To use this functionality, you must first sign up for the OCR service, and then perform various setup. For more information, see [How to: Process Incoming Documents](across-process-income-documents.md).      

Products can be both inventory items and services. For more information, see [How to: Register New Items](inventory-how-register-new-items.md).

For all purchase processes, you can incorporate an approval workflow, for example, to require that large purchases are approved by the accounting manager. For more information, see [Using Approval Workflows](across-how-use-approval-workflows.md).

The following table describes a sequence of tasks, with links to the topics that describe them.

| To | See |
| --- | --- |
| Create a purchase invoice to record your agreement with a vendor to purchase products on certain delivery and payment terms. |[How to: Record Purchases](purchasing-how-record-purchases.md) |
|Create a purchase quote to reflect a request for quote from your vendor, which you can later convert to a purchase order.|[How to: Request Quotes](purchasing-how-request-quotes.md)|
| Create a purchase invoice for all or selected lines on a sales invoice. |[How to: Purchase Items for a Sale](purchasing-how-purchase-products-sale.md) |
| Perform an action on an unpaid posted purchase invoice to automatically create a credit memo and either cancel the purchase invoice or recreate it so you can make corrections. |[How to: Correct or Cancel Unpaid Sales Invoices](purchasing-how-correct-cancel-unpaid-purchase-invoices.md) |
| Create a purchase credit memo to revert a specific posted purchase invoice to reflect which products you are returning to the vendor and which payment amount you will collect. |[How to: Process Purchase Returns or Cancellations](purchasing-how-register-new-vendors.md) |
|Prepare to invoice multiple receipts from the same vendor once by combining the receipts on one invoice.|[How to: Combine Receipts on a Single Invoice](purchasing-how-to-combine-receipts.md)|
| Learn how [!INCLUDE[d365fin](includes/d365fin_md.md)] calculates when you must order an item to receive it on a certain date.|[Date Calculation for Purchases](purchasing-date-calculation-for-purchases.md)|

## <a name="see-also"></a>See Also
[Setting Up Purchasing](purchasing-setup-purchasing.md)  
[How to: Register New Vendors](purchasing-how-register-new-vendors.md)  
[Managing Payables](payables-manage-payables.md)  
[Managing Projects](projects-manage-projects.md)    
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  
[General Business Functionality](ui-across-business-areas.md)

## [!INCLUDE[d365fin](includes/free_trial_md.md)]

