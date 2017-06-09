---
title: Create Contact Persons | Microsoft Docs
description: Describes how to create contact persons in Financials
services: project-madeira
documentationcenter: 
author: jswymer
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: relationship, prospect
ms.date: 03/28/2017
ms.author: jswymer
ms.translationtype: Human Translation
ms.sourcegitcommit: a31be0f9d07e2abb591e26f6bae34c6f6e4dcda6
ms.openlocfilehash: 7f35e0b2b98d45f0e28bfb9e0bd43e18d60a3b79
ms.contentlocale: en-nz
ms.lasthandoff: 05/04/2017


---
# <a name="create-contact-persons"></a>Create Contact Persons
You can create a contact card for each contact who works for the companies you interact with. For each contact company you can enter as many contact persons as you want. You can also create contact cards for the persons that you want to record as independent.

**Tip**: Before creating a contact, you may want to check the **Inheritance** settings in the **Marketing Setup** window. Setting up inheritance enables information about contact companies that is common to contact persons, such as address details, to be automatically copied from the contact company to the contact person each time you create a contact person for a recorded contact company.

## <a name="to-create-a-contact-card-for-a-person"></a>To create a contact card for a person
1. In the top right corner, choose the **Search for Page or Report** icon ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon"), enter **Contacts**, and then choose the related link.
2. Choose the **New** action.
3. In the **No.** field, enter a number for the contact.

    Alternatively, if you have set up a number series for contacts in the **Marketing Setup** window, you can press the Enter key to select the next available contact number. For more information, see [Creating Number Series](ui-create-number-series.md).
4. In the **Type** field, select **Person**.
5. Fill in the other fields on the contact card.

**Note**: The contents of the fields that you have selected in the **Inheritance** section of the **Marketing Setup** window are copied from the company to the persons within that company.

## <a name="see-also"></a>See Also
[Setting Up Relationship Management](marketing-setup-marketing.md)  
[Assigning Mailing Groups to a Contact](marketing-mailing-groups.md#AssignMailGroupContact)  
[Setting Up Job Responsibilities on Contacts](marketing-job-responsibilities.md)  
[Setting Up Organizational Levels for Contact Persons](marketing-organizational-levels.md)  
[Synchronizing Contacts With Customers, Vendors, and Bank Accounts](marketing-synchronize-contacts-customers-vendors-bank-accounts.md)  
[Working With Financials](ui-work-product.md)  

