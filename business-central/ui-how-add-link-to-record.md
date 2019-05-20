---
title: How to Link from Records to External Information or Programs | Microsoft Docs
description: Attach a hyperlink to a document or website to a specific record, such as a customer or document.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/12/2019
ms.author: jswymer
ms.openlocfilehash: 602d520043c5192109ccc4e2605ae0e231dafc1e
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 04/29/2019
ms.locfileid: "1250358"
---
# <a name="add-links-to-websites-documents-or-programs-on-records"></a>Add Links to Websites, Documents, or Programmes on Records
On a specific record, such as a customer, document, or sales order, you can add a link to an external document, website, or programme. Or, you may want a link that opens a new empty email to a specific recipient when you select it. The card page for some records, such as customer and vendor cards, include a **Home Page** field where you can enter an Internet address (URL). To include other links, you can use the method described in this article.  

> [!IMPORTANT]
> Currently, this capability is available only in [!INCLUDE [prodshort](includes/prodshort.md)] on-premises deployments with the legacy Dynamics NAV Windows client.  

Another example could be when you receive printed invoices from vendors. You can scan them and store them as .pdf files on a SharePoint site. Then you can make a link from a purchase invoice in [!INCLUDE[d365fin_md](includes/d365fin_md.md)] to the corresponding invoice on  SharePoint. Or, you can make a link from an item card to the corresponding page in your vendor's online catalogue.

## <a name="to-add-a-link-on-a-record"></a>To add a link on a record   

1.  Open the record that you want to attach the link to, such as a customer card or sales order. If you want to attach the link to a specific line, such as a journal line, select the line.  

2.  Choose the **Links** action to open the **Links** pages that shows all the current links that are added to the record.

3. To add a new link, choose **+new**.

4.  In the **Link Address** field, enter

    -   To link to a file on your computer or network, enter the full path and file name, such as  **C:My Documentsinvoice1.doc**.
    -   To link to website, enter the Internet address (URL), such as **www.microsoft.com**.
    -   To link to website, enter the Internet address (URL), such as **www.microsoft.com**.
    -   To link to a programme, enter a specific string to open the programme. For example, to open OneNote with a specific page, enter **onenote:///C:My Documentstest.one**. Or, to open Outlook with a new empty email to a specific alias, enter **mailto:testalias**.  

5.  Fill in the **Description** field with information about the link.  

6.  Choose the **Save** button.  

## <a name="to-delete-a-link-from-a-record"></a>To delete a link from a record  

To delete a link, on the **Links** page, you can select **...** and then **Delete**.

If you delete a single record, such as a sales order line, a sales order, or a customer, then all the links attached to the record are deleted. However, if you delete records using a batch job, such as the **Delete Invoiced Sales Orders** batch job, then the links are still stored in the database. To delete the links from the database, run the **Delete Orphaned Record Links** codeunit. To do this, choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Delete Orphaned Record Links**, and then choose the related link.   

<!-- ### To run delete orphaned record links  

1.  Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Data Deletion**, and then choose the related link.  

2.  On the **Data Deletion** page, choose **Tasks**, and then choose **Delete Orphaned Record Links**.  -->

## <a name="see-also"></a>See Also  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  
