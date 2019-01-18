---
title: Gather Customer Setup Values | Microsoft Docs
description: You use the configuration questionnaire to help reduce your implementation workload by streamlining the task of setting up the new company. You can generate the configuration questionnaire in Business Central and then provide it to your customer as an Excel (.xls) or XML file.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 33b900f1ac9e295921e7f3d6ea72cc93939d8a1b
ms.openlocfilehash: 9231f63266ba030bbf4b3ca41641d5210bcd49b8
ms.contentlocale: en-nz
ms.lasthandoff: 11/26/2018

---
# <a name="gather-customer-setup-values"></a>Gather Customer Setup Values
You use the configuration questionnaire to help reduce your implementation workload by streamlining the task of setting up the new company. You can generate the configuration questionnaire in [!INCLUDE[d365fin](includes/d365fin_md.md)] and then provide it to your customer as an Excel or XML file.  

You can change all default values in a questionnaire to more closely match customer needs.  

> [!TIP]  
>  For more information about defining setup values in supply planning fields, see [Setup Best Practices: Supply Planning](setup-best-practices-supply-planning.md).  

When your customer completes the questionnaire, you import the file into the customer's new [!INCLUDE[d365fin](includes/d365fin_md.md)] company. You and your customer validate the questionnaire answers before you apply them to the company.

## <a name="to-create-a-configuration-questionnaire"></a>To create a configuration questionnaire
You can use a questionnaire to help you determine the scope and needs of configuration. You can create a new questionnaire, or modify an existing questionnaire by adding new questions or question areas.  

 You can create questionnaires for setup-type tables only. For example you can use the tool to provide information to the following pages:  

-   Company Information  
-   Fixed Asset Setup  
-   General Ledger Setup  
-   Inventory Setup  
-   Assembly setup
-   Manufacturing Setup  
-   Purchases and Payables Setup  
-   Marketing Setup  
-   Service Setup  
-   Sales and Receivables Setup  
-   Warehouse Setup  

> [!NOTE]  
>  To see a complete list of setup tables, choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Setup**, and then choose the related link. To determine the scope of migration of records data, use migration functionality. For more information, see [Migrating Customer Data](admin-migrate-customer-data.md).  

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Configuration Questionnaire**, and choose the related link.  
2. Choose the **New** action. The **Config. Questionnaire** page opens.  
3. Choose the **Questions Areas** action. The **Question Areas** page opens.  
4. Choose the **New** action. The **Config. Question Area** page opens.  
5. In the **Table ID** field, choose the ID of the table for which you want to collect information. The **Table Name** field is automatically filled in.  
6. Choose the **Update Questions** action. Each field in the table is added to the questionnaire with a question mark following its label.

You can rephrase the label to make it clear how the question should be answered. For example, if a field is called "Name," you could edit it to state "What is the name of <data being collected>." You can also provide guidance in the **Reference** field, including a URL to a page that provides additional information.  

You can also delete any questions that you do not want to include in the questionnaire.  

> [!NOTE]  
>  The **Answer Option** field describes the type and format of the answer of the data that is appropriate. The **Answer** field contains user-supplied information.  
>   
>  As needed, you can also define default answers in the **Answer** field. These values are used by default for custom setup. However, the person filling in the questionnaire can modify and update the answer.  

## <a name="to-complete-the-configuration-questionnaire"></a>To complete the configuration questionnaire
You use the configuration questionnaire to structure and document a detailed discussion about the customer’s specific needs. You also use it to collect setup data from the customer to configure the relevant [!INCLUDE[d365fin](includes/d365fin_md.md)] setup tables, such as the general ledger, inventory, and customers.  

> [!NOTE]  
>  You can also create your own configuration questionnaire to meet your needs.  

1. Open the company that you want to complete the questionnaire for.
2. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Configuration Questionnaire**, and then choose the related link.  
3. Select the questionnaire for the company, and then choose the **Export to Excel** action, optionally the **Export to XML** action.
4. Have the customer complete the configuration questionnaire by entering the answers in the Excel workbook. There are worksheets for each of the question areas that have been created for the questionnaire.   
5. Choose the **Import from Excel** action, and select the .xlsx file with the customer's answers.  
6. Choose the **Question Areas** action to begin the process of validating and applying the answers to the configuration questionnaire.  

## <a name="to-complete-a-questionnaire-from-the-configuration-worksheet"></a>To complete a questionnaire from the configuration worksheet  
The following procedure provides an alternative way of accessing configuration questionnaires. It assumes that the configuration package that you have been provided includes questionnaires.  

1. After you import a configuration package, open the configuration worksheet.  
2. For each table for which there is a question area, choose the **Questions** action. The questionnaire page opens.  
3. Answer the questions, and then choose the **Apply Answers** action.  
4. Choose the **OK** button to close the questionnaire.

## <a name="to-validate-the-configuration-questionnaire"></a>To validate the configuration questionnaire
It is important to validate the configuration questionnaire before you apply it to the [!INCLUDE[d365fin](includes/d365fin_md.md)] format. It is also a way to make sure that data formatting is preserved during the import from Excel.  

A common validation task is to check that text strings are not entered in date fields. This review process is necessary because the format of the answer in the questionnaire is not validated automatically when you run the **Apply Answers** function.  

> [!NOTE]  
>  In general, validation of the configuration questionnaire is a manual process. However, there are checks for regional formatting inconsistencies. In addition, you will get errors if the structure of your [!INCLUDE[d365fin](includes/d365fin_md.md)] database does not match the structure of the migration database.  

1. On the **Configuration Questionnaire** page, select the relevant questionnaire, and then choose the **Question Areas** action.  
2. Open the relevant question area.  
3. For each question, validate that the value in the **Answer** field corresponds to the format provided in the **Answer Option** field. For example, validate that the address of a company is in text format.  
4. If you find errors, you can troubleshoot and make corrections in Excel by exporting the questionnaire, and then importing it again. Alternatively, you can correct errors directly in [!INCLUDE[d365fin](includes/d365fin_md.md)] as you review the answers on the **Config. Question Area** page.  
5. Repeat these steps for each question area.  

When you have completed your validation, the data is ready to be applied to the database.  

## <a name="to-apply-answers-from-the-configuration-questionnaire"></a>To apply answers from the configuration questionnaire
After you have imported and validated information from a configuration questionnaire, you can transfer, or apply the setup data to the corresponding tables in the [!INCLUDE[d365fin](includes/d365fin_md.md)] database.  

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Configuration Questionnaire**, and then choose the related link. The **Config. Questionnaire** page opens.  
2. Select a configuration questionnaire from the list, and then choose the **Edit List** action.  
3. You can apply answers in one of two ways.  

- To apply the whole questionnaire, choose the **Apply Answers** action.  
- To apply answers for a specific **Question Area** only, choose the **Question Areas** action, select a **Question Area** in the list, and then choose the **Apply Answers** action.  

### <a name="to-verify-that-answers-have-been-applied-successfully"></a>To verify that answers have been applied successfully  
1. Check setup pages for the various functional areas of [!INCLUDE[d365fin](includes/d365fin_md.md)]. To locate the page, choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter the name of the setup page, and then choose the related link.  
2. Verify that the fields have been populated with the correct data from the various question areas in the configuration questionnaire.  

You have now configured setup with the customer’s business information and rules.

## <a name="see-also"></a>See Also  
[Setting Up a Company With RapidStart Services](admin-set-up-a-company-with-rapidstart.md)  
[Administration](admin-setup-and-administration.md)

