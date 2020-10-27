---
title: Submit GST Reports to Tax Authorities| Microsoft Docs
description: Learn how to prepare reports that lists GST from sales during a period, or from sales and purchases, and submit the report to a tax authority.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: VAT, tax, report, EC sales list, statement
ms.date: 10/01/2020
ms.author: bholtorf
ms.openlocfilehash: 65331f8c60c57bd87e3a459012a9a5678d033790
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 10/01/2020
ms.locfileid: "3920602"
---
# <a name="report-vat-to-tax-authorities"></a>Report GST to Tax Authorities
This topic describes the reports in [!INCLUDE[d365fin](includes/d365fin_md.md)] that you can use to submit information about value-added tax (VAT) amounts for sales and purchases to tax authorities in your region. 

You can use the following reports :

* The **EC Sales List** European Community (EC) Sales List report lists the value added tax (VAT) amounts that you have collected for sales to VAT-registered customers in the European Union (EU) countries.  
* The **GST Return** report includes GST for sales and purchases to customers and from vendors in all countries that use GST.

If you want to view a complete history of GST entries, every posting that involves GST creates an entry on the **GST Entries** page. These entries are used to calculate your GST settlement amount, such as your payment and refund, for a specific period. To view GST entries, choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **GST Entries** , and then choose the related link.

> [!NOTE]
> Each [!INCLUDE[d365fin](includes/d365fin_md.md)] environment is meant to handle regulatory reporting in one single country. For example, the Dutch version of [!INCLUDE[d365fin](includes/d365fin_md.md)] handles GST reporting in The Netherlands but not in other countries. Similarly, the United States version of [!INCLUDE[d365fin](includes/d365fin_md.md)] handles 1099 reporting in the United States and does not support claiming GST reporting in other countries, unless brought by an extension delivered by our partner ecosystem or a customer-specific code modification.

## <a name="about-the-ec-sales-list-report"></a>About the EC Sales List report
In the UK, all companies that sell goods and services to VAT-registered customers, including customers in other European Union (EU) countries, must submit an electronic version of the European Community (EC) Sales List report in XML format through Her Majesty's Revenue and Customs (HMRC) website. The EC Sales List report works only for countries in the EU.

The report includes one line for each type of transaction with the customer, and displays the total amount for each type of transactions. There are three types of transactions that the report can include:  

* B2B Goods  
* B2B Services  
* B2B Triangulated Goods  

B2B goods and services specify whether you sold a good or a service, and are controlled by the **EU Service** setting in the GST posting setup. B2B Triangulated Goods indicate whether you engaged in trade with a 3rd party, and are controlled by the **EU 3-Party Trade** setting on sales documents, such as sales orders, invoices, credit memos, and so on.  

After the tax authority reviews your report, they will send an email to the contact person for your company. In [!INCLUDE[d365fin](includes/d365fin_md.md)], the contact person is specified on the **Company Information** page. Before you submit the report, make sure that a contact person is chosen.

## <a name="about-the-vat-return-report"></a>About the GST Return report
Use this report to submit GST for sales and purchase documents, such as purchase and sales orders, invoices, and credit memos. The information in the report is in the same format as on the declaration form from the customs and tax authorities.  

GST is calculated based on the GST posting setup and the GST posting groups that you have set up.

For the GST return, you can specify the entries to include:

* Submit open transactions only, or open and closed. For example, this is useful when you prepare your final annual GST return.
* Submit only entries from the specified periods, or also include entries from previous periods. This is useful for updating a GST return that you have already submitted, for example, if a vendor sends you a late invoice.    

## <a name="to-connect-to-your-tax-authoritys-web-service"></a>To connect to your tax authority's web service
[!INCLUDE[d365fin](includes/d365fin_md.md)] provides service connections to tax authority websites. For example, if you are in the UK, you can enable the **GovTalk** service connection to submit the EC Sales List and VAT Return reports electronically. If you want to submit the report manually, for example by entering your data on the tax authority's website, this is not required.   

To report VAT to a tax authority electronically, you need to connect [!INCLUDE[d365fin](includes/d365fin_md.md)] to the tax authority's web service. This requires that you set up an account with your tax authority. When you have an account, you can enable a service connection that we provide in [!INCLUDE[d365fin](includes/d365fin_md.md)].

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Service Connections** , and then choose appropriate link.
2. Fill in the required fields. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

    > [!NOTE]  
    > It is a good idea to test your connection. To do this, choose the **Test Mode** check box, then prepare and submit your GST report as described in the _To prepare and submit a GST report_ section. While in Test Mode, the service tests whether the tax authority can receive your report, and the status of the report will indicate whether the test submission was successful. It is important to remember that this is not an actual submission. To submit the report for real, you must clear the **Test Mode** check box, and then repeat the submission process.

## <a name="to-set-up-vat-reports-in-d365fin"></a>To set up GST reports in [!INCLUDE[d365fin](includes/d365fin_md.md)]
1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **GST Report Setup** , and then choose the related link.  
2. To let users change and resubmit this report, choose the **Modify Submitted Reports** check box.  
3. Choose the number series to use for each report.  

## <a name="to-prepare-and-submit-a-vat-report"></a>To prepare and submit a GST report
1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **EC Sales List** or **GST Return** , and then choose the related link.  
2. Choose **New** , and then fill in the required fields. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. To generate the content of the report, choose the **Suggest Lines** action.  

    > [!NOTE]  
    >   For the EC Sales List report, you can review the transactions included in the report lines before you submit the report. To do that, choose the line, and then choose the **Show VAT Entries** action.  
4. To validate and prepare the report for submission, choose the **Release** action.  

    > [!NOTE]  
    > [!INCLUDE[d365fin](includes/d365fin_md.md)] validates whether the report is set up correctly. If the validation fails, the errors display under **Errors and Warnings** so that you know what to fix. Typically, if the message is about a missing setting in [!INCLUDE[d365fin](includes/d365fin_md.md)], you can click the message to open the page that contains the information to correct.  
5. To submit the report, choose the **Submit** action.  

After you submit the report, [!INCLUDE[d365fin](includes/d365fin_md.md)] monitors the service and keeps a record of your communications. The **Status** field indicates where the report is in the process. For example, when the authorities process your report, the status of the report changes to **Succeeded** . If the tax authority found mistakes in the report you submitted, the status of the report will be **Failed** . You can view the errors under **Errors and Warnings** , correct them, and then submit the report again. To view a list of all your EC Sales List reports, go to the **EC Sales List Reports** page.  

## <a name="viewing-communications-with-your-tax-authority"></a>Viewing communications with your tax authority
In some countries, you exchange messages with the tax authority when you submit reports. You can view the first and the last message you sent or received by choosing the **Download Submission Message** and **Download Response Message** actions.  

## <a name="submitting-vat-reports-manually"></a>Submitting GST reports manually
If you use another method to submit the report, for example by exporting the XML and uploading it to a tax authority website, afterward you can choose **Mark as Submitted** to close the reporting period. When you mark the report as released, it becomes non-editable. If you must change the report after you mark it as released, you must reopen it.

## <a name="vat-settlement"></a>GST settlement
Periodically, you must remit the net GST to the tax authorities. If you need to settle GST frequently, you can run the **Calc. and Post GST Settlement** batch job to close the open GST entries and transfer purchase and sales GST amounts to the GST settlement account.

When you transfer GST amounts to the settlement account, the purchase GST account is credited, and the sales GST account is debited with the amounts calculated for the specified period. The net amount is credited or debited, if the purchase GST amount is larger, to the GST settlement account. You can post the settlement immediately or print a test report first.  

> [!Note]
> When you use the **Calc. and Post GST Settlement** batch job, if you do not specify a **GST Bus. Posting Group** and a **GST Prod. Posting group** , entries with all business posting groups and product posting group codes are included.

## <a name="configuring-your-own-vat-reports"></a>Configuring your own GST reports
You can use the EC Sales List report out-of-the-box, however, you can also create your own reports. This requires that you create a few codeunits. If you need help with that, contact a Microsoft Partner.  

The following table describes the codeunits that you must create for your report.

| Codeunit | What it must do |
|----|-----|
|Suggest Lines| Fetch information from the GST Entries table, and display it in lines on the GST report.|
|Content | Control the format of the report. For example, whether it is XML or JSON. The format to use depends on the requirements of your tax authority's web service. |
|Submission | Control how, and when, you submit the report based on the requirements of your tax authority. |
|Response Handler | Handle the return from the tax authority. For example, it might send an email message to your company's contact person. |
|Cancel | Send a cancellation of a GST report that was submitted earlier to your tax authority. |  

> [!Note]
> When create codeunits for the report, pay attention to the value in the **GST Report Version** field. This field must reflect the version of the report that is, or was, required by the tax authority. For example, you might enter **2017** in the field to indicate that the report conforms to the requirements that were in place that year. To find the current version, contact your tax authority.

## <a name="see-related-training-at-microsoft-learn"></a>See Related Training at [Microsoft Learn](/learn/paths/process-vat-dynamics-365-business-central/)

## <a name="see-also"></a>See also
[Setting Up to Calculations and Posting Methods for Value-Added Tax](finance-setup-vat.md)  
[Work with GST on Sales and Purchases](finance-work-with-vat.md)  
[Setting Up Sales](sales-setup-sales.md)  
[Invoice Sales](sales-how-invoice-sales.md)  
