---
title: Set Up Organisational Levels for Contact Persons| Microsoft Docs
description: You can define an organisational level and assign it to your contact to indicate the position they have in their company, for example, top management.
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
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: d101076c8a51b1c7a79606d207f79a826c89bf29
ms.contentlocale: en-nz
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-set-up-organizational-levels-for-contact-persons"></a>How to: Set Up Organisational Levels for Contact Persons
You can use organisational levels on your contacts to specify which position they have in the company, for example, top management. You can use this information when entering information about your contacts.

Using organisational levels on contacts is a two-step process. First, you define the organisational level code. You only have to perform this step one time for each organisational level. Once you have an organisational level code, you can start to assign the code to contact persons.

## <a name="to-define-an-organizational-level-code"></a>To define an organisational level code
The organisational level code defines the type or category of the organisational level, such a CEO  or CFO. You can have several organisational level codes. To define the organisational level, you use the **Organisational Levels** window.

1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Organizational Levels**, and then choose the related link.
2. Choose the **New** action, and fill in a code and description. The code can be a maximum of 11 characters, and can be any combination of numbers and letters.

## <a name="to-assign-organizational-levels-to-a-contact-person"></a>To assign organisational levels to a contact person
You can assign organisational levels to contact persons only, not contact companies. You can only assign one organisational level to each contact.

1. Open the contact.
2. In the **Organisational Levels** field, select the code you want to assign.

After you have assigned organisational levels to your contacts, you can use this information to create segments.

After you have assigned job responsibilities to your contacts, you can use this information to select contacts for your segments. For more information, see [How to: Add Contacts to Segments](marketing-add-contact-segment.md).

## <a name="see-also"></a>See Also
[Creating Contact Companies](marketing-create-contact-companies.md)  
[Creating Contact Persons](marketing-create-contact-persons.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

