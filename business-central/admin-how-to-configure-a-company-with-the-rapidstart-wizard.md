---
title: Configure a Company with the RapidStart Wizard
description: For Business Central on-premises, you can configure a new company that you have created by using the RapidStart Services configuration wizard.
author: SorenGP
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 03/28/2022
ms.author: edupont
ms.openlocfilehash: 189701aef31c5bbdc3323b753667937775d59a9d
ms.sourcegitcommit: 8a12074b170a14d98ab7ffdad77d66aed64e5783
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 03/31/2022
ms.locfileid: "8515813"
---
# <a name="configure-a-company-with-the-rapidstart-wizard"></a>Configure a Company with the RapidStart Wizard

[!INCLUDE [onprem_only_md](includes/onprem_only_md.md)]

You can quickly configure a new company that you have created by using the RapidStart Services configuration wizard.

In the following procedure, you have provided the customer with the configuration package, which is then installed on a computer. The customer opens the new company, which contains no customer data. You or the customer then follows the steps in the RapidStart Services wizard, which are described in this procedure, to provide basic information about the company. The wizard imports the configuration package and then applies the package to the company.  

## <a name="to-configure-a-new-company"></a>To configure a new company  
1. On the RapidStart Services Implementer Role Centre, choose the **RapidStart Wizard** action.  
2. Expand the **Step 1** FastTab, which contains general information about the new company. Enter the appropriate information about the new company in the fields. There is one field that you are required to fill out, **Name**. The rest of the fields are optional.  
3. Expand the **Step 2** FastTab, which contains communication and contact information for the new company. Enter the appropriate information about the new company in the fields.
4. Expand the **Step 3** FastTab, which contains bank account and payment information for the new company. Enter the appropriate information about the new company in the fields.  
5. Expand the **Step 4** FastTab. Choose the **AssistEdit** button to select the configuration package you want to apply. The name of the configuration package is displayed. You can then perform the following actions, in the listed order:  

    1. Apply the configuration by choosing the **Apply Package** action. This imports the configuration package and applies the package database data all at the same time.  

    2. Review the configuration after it has been applied. This option lets you review configuration details and questionnaires provided by the partner and import some master data that is required for your company. Choose the **Configuration Worksheet** action. For more information, see [To complete the configuration questionnaire](admin-gather-customer-setup-values.md#to-complete-the-configuration-questionnaire).  

6. Expand the **Step 5** FastTab. Specify which Role Centre that you want to be the default for the new company.  

    > [!IMPORTANT]  
    >  Only change your Role Centre after you have completed configuration of the company. If you have more setup details to consider and modify, first use the configuration worksheet to continue your work. Then, return to the wizard to update your Role Centre profile, or choose the **Complete Setup** action.

7. Choose the **OK** button.  
8. To verify that the configuration information has been applied to the new company, Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Company Information**, and then choose the related link.

The **Company Information** page contains information that you have specified.   

You have now configured the company and applied data to it.  

## <a name="see-also"></a>See Also  
[Apply Configurations to New Companies](admin-apply-configuration-to-new-companies.md)  
[Setting Up a Company With RapidStart Services](admin-set-up-a-company-with-rapidstart.md)  
[Administration](admin-setup-and-administration.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]