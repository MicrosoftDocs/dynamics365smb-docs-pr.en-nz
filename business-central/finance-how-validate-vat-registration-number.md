---
title: Validate GST Registration numbers
description: Let Business Central use the VIES service to validate GST Registration numbers for you automatically.
author: kielkenny
ms.service: dynamics365-business-central
ms.topic: article
ms.reviewer: edupont
ms.search.keywords: VAT, posting, tax, value-added tax
ms.date: 10/01/2020
ms.author: andregu
ms.openlocfilehash: 80e955e96a64c5a0bd91d0a72297b32d67ff4ab6
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 12/17/2020
ms.locfileid: "4750587"
---
# <a name="validate-vat-registration-numbers"></a>Validate GST Registration numbers

It is important that the VAT registration numbers you have for customers, vendors, and contacts are valid. For example, companies sometimes change their tax liability status, and in some countries tax authorities might ask you to provide reports, such as the EC Sales List report, that list the GST registration numbers you use when you do business.

The European Commission provides the VIES VAT Number Validation service on its website, which is public and free. [!INCLUDE[prod_short](includes/prod_short.md)] can save you a step and let you use the VIES service to validate and track VAT numbers for customers, vendors, and contacts straight from the customer, vendor, and contact cards. The service in [!INCLUDE[prod_short](includes/prod_short.md)] is named **EU VAT Reg. No. Validation Service**. The service is available on the **Service Connections** page, and you can start using it right away. The service connection is free, and sign-up is not required.

## <a name="to-verify-vat-registration-numbers"></a>To verify GST Registration numbers

In order to enable the **EU VAT Reg. No. Validation Service** open the entry in the **Service Connection** page. The **Service Endpoint** field should already be populated. If not, you can use the **Set Default Endpoint** action. Then set the **Enabled** field and you are good to go.

> [!NOTE]
> To enable the EU VAT Reg. No. Validation Service, you must have administrator permissions.

When you use our service connection, we record a history of VAT numbers and verifications for each customer, vendor, or contact, in the **VAT Registration Log**, so you can easily track them. The log is specific to each customer. For example, the log is useful for proving that you have verified that the current GST number is correct. When you verify a VAT number, the **Request Identifier** column in the log will reflect that you have taken action.

You can view the GST Registration log on the Customer, Vendor, or Contact cards, on the **Invoicing** FastTab, by choosing the lookup button in the **GST Registration No.** field.  

Our service can also save you time when you create a customer or vendor. If you know the customer's GST number, you can enter it in the **GST Registration No.** field on the Customer or Vendor cards, and we will fill out the customer name for you. Some countries also provide company addresses in a structured format. In those countries, we fill in the address too.  

There are a couple of things to note about the VIES VAT Number Validation service:

* The service uses the http protocol, which means that data transferred through the service is not encrypted.  
* You may experience downtime for this service for which Microsoft is not responsible. The service is part of a broad EU network of national VAT registers.

> [!IMPORTANT]
> It is your responsibility to check that the data is valid. On occasion, data with errors is returned by the VIES VAT Number Validation service. If validation fails, validate the GST registration numbers on the [web site](https://ec.europa.eu/taxation_customs/vies/), print the result or save it to a shared location, and then add the link to the record for your customer, vendor, or contact. For more information, see [Manage Attachments, Links, and Notes on Cards and Documents](ui-how-add-link-to-record.md).

## <a name="see-also"></a>See Also

[Set Up Value-Added Tax](finance-setup-vat.md)  
[Setting Up Unrealized Value Added Tax](finance-setup-unrealized-vat.md)  
[Report GST to a Tax Authority](finance-how-report-vat.md)  
[Work with GST on Sales and Purchases](finance-work-with-vat.md)  
[Local functionality in Business Central](about-localization.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]