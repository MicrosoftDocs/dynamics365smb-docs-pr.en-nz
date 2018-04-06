---
title: How to Configure New Companies | Microsoft Docs
description: You can configure and customise a new company that you have created. To fine tune your implementation, you proceed in three phases to complete your configuration.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 03/06/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: b9e701f102f1a2fc7ccbd4882dfec37f65cfe3b7
ms.contentlocale: en-nz
ms.lasthandoff: 03/22/2018

---
# <a name="configure-new-companies"></a>Configure New Companies
To configure a new company in your solution implementation, you typically follow three phases. In the first phase, you import the configuration package, a .rapidstart file with the configuration information. In the second phase, you modify the configuration information and then apply it to your new company. In the final phase, you review and fix any errors.  

The following procedures assume that you have created and saved a configuration package. For more information, see [Prepare a Configuration Package](admin-how-to-prepare-a-configuration-package.md).  

The following procedures assume that you have initialised and opened your new company and that you are using the RapidStart Services Implementer Role Centre.

## <a name="to-import-a-configuration-package"></a>To import a configuration package  
1. Open the new company in the [!INCLUDE[d365fin](includes/d365fin_md.md)] database.  
2. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Configuration Packages**, and then select the related link.  
3. Choose the **Import Package** action.  
4. Navigate to the location where you have saved the .rapidstart configuration package file, and then choose the **Open** button.  
5. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Company Information**, and then choose the related link. Enter information about the company in the company information card. Include information, such as bank details. You can also provide a logo for the company.  

All the tables that you have designated for inclusion in the new company are imported. At this point, you can apply the package data to the database, or adjust and modify the table data to meet your customer specifications.  

## <a name="to-apply-package-data"></a>To apply package data  
1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Configuration Worksheet**, and then select the related link.  
2. Select a table that you want to modify data for, and then choose the **Apply Data** action. Choose the **Yes** button to confirm the application.
3. To confirm that the data is now in the database and that the application has succeeded, return to the **Config. Worksheet** window and choose the **Database Data** action.  

> [!NOTE]  
>  After you apply data, you can only see it in the database. It is no longer in the package.  

## <a name="to-modify-and-apply-package-data"></a>To modify and apply package data  
1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Configuration Worksheet**, and then select the related link.  
2. Select a table that you want to modify data for, and then choose the **Package Data** action.  
3. In the **Config. Package Records** window, make your modifications. For example, you can delete options that do not apply.  
4. Choose the **Apply Data** action, and then choose the **OK** button.  
5. To confirm that the data is now in the database and that the application has succeeded, return to the **Config. Worksheet** window and choose the **Database Data** action.  

## <a name="to-locate-and-identify-a-configuration-error"></a>To locate and identify a configuration error  
There are certain types of errors that may occur when you apply data to a database. The most common error is that required related tables were not included. You fix such errors in the configuration worksheet.

1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Configuration Packages**, and then select the related link.  
2. Select the package you want to review, and then choose the **Edit** action.  

    Any table that has errors is highlighted. The number of package errors is displayed in the **No. of Package Errors** field.  

3. Choose the **No. of Package Errors** field to open the **Config. Package Records** window, which lists the records with errors.  

### <a name="to-fix-an-error"></a>To fix an error  
1. Open the company that is based on your configuration package.  
2. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Configuration Worksheet**, and then select the related link.  
3. Fix errors, such as add missing related tables to the worksheet.  
4. Add the tables to the existing configuration package, or create a new package that only contains the new tables. For more information, see [Prepare a Configuration Package](admin-how-to-prepare-a-configuration-package.md).  
5. Reopen the new company that you are implementing the configuration for.  
6. Import the configuration package.  

    > [!NOTE]  
    >  If you import the same package again, you may overwrite any data modifications that you have already made. For that reason, you may want to add any new tables in a new package and import that instead.  

7. Apply the data to the database, as described in the "To modify and apply package data" section.

## <a name="see-also"></a>See Also  
[Apply Configurations to New Companies](admin-apply-configuration-to-new-companies.md)  
[Setting Up a Company With RapidStart Services](admin-set-up-a-company-with-rapidstart.md)  
[Administration](admin-setup-and-administration.md)

