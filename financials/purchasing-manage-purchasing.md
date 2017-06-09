---
title: Purchasing| Microsoft Docs
description: Describes how to manage purchasing activities.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: procurement, supply, vendor order
ms.date: 03/29/2017
ms.author: sgroespe
ms.translationtype: Human Translation
ms.sourcegitcommit: a31be0f9d07e2abb591e26f6bae34c6f6e4dcda6
ms.openlocfilehash: 4ba8ea773fa4024cfcaccd00b80bdbbfe81be8b7
ms.contentlocale: en-nz
ms.lasthandoff: 05/04/2017


---
# <a name="purchasing"></a>Purchasing
You create a purchase invoice or purchase order to record the cost of purchases and to track accounts payable. If you need to control an inventory, purchase invoices are also used to dynamically update inventory levels so that you can minimise your inventory costs and provide better customer service. The purchasing costs, including service expenses, and inventory values that result from posting purchase invoices contribute to profit figures and other financial KPIs on your Home page.

You must use purchase orders if your purchasing process requires that you record partial receipts of an order quantity, for example, because the full quantity was not available at the vendor. If you sell items by delivering directly from your vendor to your customer, as a drop shipment, then you must also use purchase orders. For more information, see [How to: Make Drop Shipments](sales-how-drop-shipment.md). In all other aspects, purchase orders work the same way as purchase invoices.

You can have purchase invoices created automatically by using the OCR (Optical Character Recognition) service to convert PDF invoices from your vendors to electronic documents, which are then converted to purchase invoices by a workflow. To use this functionality, you must first sign up for the OCR service, and then perform various setup. For more information, see [How to: Process Incoming Documents](across-process-income-documents.md).      

Products can be both inventory items and services. For more information, see [How to: Register New Items](inventory-how-register-new-items.md).

For all purchase processes, you can incorporate an approval workflow, for example, to require that large purchases are approved by the accounting manager. For more information, see [Using Approval Workflows](across-how-use-approval-workflows.md).

The following table describes a sequence of tasks, with links to the topics that describe them. These tasks are listed in the order in which they are generally performed.

| To | See |
| --- | --- |
| Create a purchase invoice to record your agreement with a vendor to purchase products on certain delivery and payment terms. |[How to: Record Purchases](purchasing-how-record-purchases.md) |
| Create a purchase invoice for all or selected lines on a sales invoice. |[How to: Purchase Products for a Sale](purchasing-how-purchase-products-sale.md) |
| Perform an action on an unpaid posted purchase invoice to automatically create a credit memo and either cancel the purchase invoice or recreate it so you can make corrections. |[How to: Correct or Cancel Unpaid Sales Invoices](purchasing-how-correct-cancel-unpaid-purchase-invoices.md) |
| Create a purchase credit memo to revert a specific posted purchase invoice to reflect which products you are returning to the vendor and which payment amount you will collect. |[How to: Process Purchase Returns or Cancellations](purchasing-how-register-new-vendors.md) |
| Create a vendor card for each vendor that you purchase from. |[How to: Register New Vendors](purchasing-how-register-new-vendors.md) |

## <a name="see-also"></a>See Also
[Setting Up Purchasing](purchasing-setup-purchasing.md)  
[Managing Payables](payables-manage-payables.md)  
[Manage Projects](projects-manage-projects.md)    
[Supply Chain](madeira-supply-chain.md)      
[Working With [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  
[General Business Functionality](ui-across-business-areas.md)

## [!INCLUDE[d365fin](includes/free_trial_md.md)]
