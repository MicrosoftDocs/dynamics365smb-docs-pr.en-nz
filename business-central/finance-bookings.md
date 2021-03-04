---
title: Invoice your bookings in Business Central | Microsoft Docs
description: Learn how you can do bulk invoicing from Microsoft Bookings in Business Central .
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: invoicing, bookings
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 9b683fa14801c00904c131ada5bcce1f669c9b2a
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 12/17/2020
ms.locfileid: "4751021"
---
# <a name="bulk-invoicing-for-microsoft-bookings-in-prod_short"></a>Bulk Invoicing for Microsoft Bookings in [!INCLUDE[prod_short](includes/prod_short.md)]
If your company uses the Bookings app in Microsoft 365, you can do bulk invoicing for appointments. The **Uninvoiced Bookings** page in [!INCLUDE[prod_short](includes/prod_short.md)] provides a list of the company's completed bookings. In this page you can quickly select the appointments that you want to invoice and create draft invoices for the services provided.  

## <a name="connect-to-bookings"></a>Connect to Bookings
To connect your [!INCLUDE[prod_short](includes/prod_short.md)] with Bookings, you must specify your Bookings company, what to synchronize with Bookings, how often to synchronize, and which templates to use. You set up this information on the **Booking Sync. Setup** page, which you can launch from the **Exchange Sync. Setup** page, which you can find through [Search](ui-search.md).  

For example, if you want to synchronise customers between Bookings and [!INCLUDE[prod_short](includes/prod_short.md)], you must specify the default template to use to add new customers in [!INCLUDE[prod_short](includes/prod_short.md)] based on the customers in your Bookings company.  

> [!NOTE]
> The Bookings app is designed to book appointments for individual customers rather than companies. The synchronisation with [!INCLUDE[prod_short](includes/prod_short.md)] will, therefore, only synchronise customer contacts with a Type of "Person". An email address is also required for the contact to synchronise.  

Similarly, if you want to synchronise service items between Bookings and [!INCLUDE[prod_short](includes/prod_short.md)], you must specify the default template to use to add new service items in [!INCLUDE[prod_short](includes/prod_short.md)] based on the services in our Bookings company.  

> [!NOTE]
> Only items of type *Service* will synchronise between Bookings and [!INCLUDE[prod_short](includes/prod_short.md)]. The template that you set up in the **Configuration Templates** page so it can be used for the item synchronisation must define the type as *Service*.

## <a name="invoice-appointments"></a>Invoice Appointments
When it is time to send invoices for the completed bookings, you go to the **Uninvoiced Bookings** page. Depending on how often the information is synchronised, the list is long or short. You can create invoices for all bookings in the list or one booking at a time. You can select one or more entries in the list and invoice those only.  

The support for invoicing appointments from Bookings is simpler than the fuller workflow of working with sales quotes, sales orders, and sales invoices. For more information, see [Invoice Sales](sales-how-invoice-sales.md). You can choose to sell your services using [!INCLUDE[prod_short](includes/prod_short.md)] or choose to use Bookings, depending on your business needs.  

## <a name="see-also"></a>See Also
[Finance](finance.md)  
[Invoice Sales](sales-how-invoice-sales.md)  
[Setting Up Sales](sales-setup-sales.md)  
[Microsoft Bookings](https://products.office.com/business/scheduling-and-booking-app)  


[!INCLUDE[footer-include](includes/footer-banner.md)]