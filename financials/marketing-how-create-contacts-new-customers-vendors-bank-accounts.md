---
title: Create a Customer or VendorFrom a Contact| Microsoft Docs
description: You can record an existing contact as a customer, vendor, or bank account using existing data and specifying a business relationship.
services: project-madeira
documentationcenter: 
author: jswymer
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: relationship, client, prospect
ms.date: 06/06/2017
ms.author: jswymer
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: 142c1649438ad31b604767d6b6f35a1caeb3f9e4
ms.contentlocale: en-nz
ms.lasthandoff: 07/07/2017


---
# <a name="how-to-create-a-customer-vendor-or-bank-account-from-a-contact"></a>How to: Create a Customer, Vendor, or Bank Account From a Contact
You may want to record some of your existing contacts as customers, vendors, or bank accounts. Creating a customer, vendor, or bank account from a contact enables you use existing data. When you create a customer, vendor, or bank account this way, it is synchronised with the contact. Synchronisation makes information that is common between contacts and customers, vendors, or bank account the same.

Before you can record contacts this way, you must specify a business relation code for customers, vendors, and bank accounts in the **Marketing Setup** window. If you will be recording contacts as bank accounts, you must also specify numbers series for bank accounts in the **General Ledger Setup** window.

## <a name="to-create-a-contact-as-a-customer-vendor-or-bank-account"></a>To create a contact as a customer, vendor, or bank account
1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Contacts**, and then choose the related link.
2. Select the contact you want to create as a customer, vendor, or bank account.
3. Choose the **Create As** action, and then choose either **Customer**, **Vendor**, or **Bank**.
4. Confirm the subsequent message.

The contact information is transferred from the **Contact** card to the **Bank Account** card, the **Customer** card, or the **Vendor** card. You may want to add specific information to each of the cards, such as invoicing and payment details.

## <a name="see-also"></a>See Also
[How to: Create Contact Companies](marketing-create-contact-companies.md)  
[How to: Create Contact Persons](marketing-create-contact-persons.md)  
[Setting Up Relationship Management](marketing-setup-marketing.md)  
[Synchronizing Contacts With Customers, Vendors, and Bank Accounts](marketing-synchronize-contacts-customers-vendors-bank-accounts.md)  
[How to: Link Contacts to Existing Customers, Vendors, or Bank Accounts](marketing-how-link-contact.md)  
[Assign Business Relations to a Contact](marketing-business-relations.md#AssignBusRelContact)  
[Working with Financials](ui-work-product.md)

