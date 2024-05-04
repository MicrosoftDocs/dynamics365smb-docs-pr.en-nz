---
title: Use e-documents in the purchase process
description: Learn how to use e-documents functionality that is related to purchase invoices and orders.
author: altotovi
ms.topic: conceptual
ms.devlang: al
ms.search.keywords: 'electronic document, electronic invoice, e-document, e-invoice, receive, purchase, matching, mapping, Copilot'
ms.search.form: '50, 51, 138, 6103, 6133, 6121, 6167, 9307, 9308'
ms.date: 04/03/2024
ms.author: altotovi
ms.service: dynamics-365-business-central
---

# Use E-documents in the purchases process

You can use configured electronic documents (e-documents) with the purchase documents.

You can use the following purchase documents with e-documents functionality:  

- Purchase invoices
- Purchase orders (from version 24.0)
- Purchase credit memos
- General journals

> [!NOTE]
> From [!INCLUDE[prod_short](includes/prod_short.md)] version 24.0, it is possible to connect **Purchase Orders** with the received **E-Documents**.  

## E-documents in purchases

The receipt of purchase electronic documents in Dynamics 365 Business Central can be done as a batch job or manually.  

### How to set up vendors to work with different purchase documents  

Follow the steps to configure vendors to work properly with incoming electronic invoices: 

1. Select the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Vendors**, and then select the related link. 
2. Choose the vendor you want to configure.   
3. In the **Receiving** FastTab, find the **Receive E-Document To** field to specify the default purchase document to be generated from the received E-document. 

> [!NOTE]
> In the **Receive E-Document To** field, users can either select a **Purchase Invoice** or **Purchase Order** based on what they would like to have created from the received e-invoice. This selection does not affect the creation of corrective documents; in both scenarios, the system will generate a **Credit Memo**.  

> [!NOTE]
> If the user chooses the **Purchase Order** option in the **Receive E-Document To** field, the system will try to update one of the existing purchase orders, but if the purchase order for a vendor in the received **E-Document** does not exist, the [!INCLUDE[prod_short](includes/prod_short.md)] will create a new **Purchase Order**, using the same approach as creating the new **Purchase Invoices** explained in this page later.  

4. Choose one of the options you want to use for the selected vendor. 
5. Close the page.   

### To work with purchase invoices  

#### Run the batch job  

> [!NOTE]
> This batch job is for automated collection of your incoming invoices. It can work only in a country or a region where the functionality exists.  

Every time when a **Job Queue** is selected to run, if the external service has incoming invoices that were sent from your vendor, the system collects and imports those invoices. To complete the process, follow these steps. 

1. After the batch job has been finished running, the newly imported invoices are listed on the **E-Documents** page, together with their basic detail information. 
2. To view more details, open a specific e-document.   
3. If there were no errors or issues in the e-document, the **Record** field maps the document number of the purchase invoice, if this is configured on the **Vendor Card** page (that the system automatically created). Select the link to open the document.
 
> [!NOTE]
> This system-created document isn't the posted document. 

1. To go directly to the purchase document, select the **Record** field. After you open the **Purchase Invoice** page, check the document. Then, if everything is correct, post the document.  
1. When you post the purchase document, the **Record** field on the **E-Document** is updated from **Invoice** to **Purchase Invoice**, and the number of the posted purchase document is available. You can select the number to open the posted purchase invoice. 

Details about logs are the same as they are in the sales process for e-documents.  

Because errors in the sales process are mostly related to the availability of the service, the incoming document can contain multiple reasons. The most common reason for an error is that system can't recognise the lines on the e-document that you got from your vendor. Therefore, it can't enter lines in your purchase invoice. 

There are two common errors:  

- If you want to use this specific line from your vendor invoice that was directly posted to the general ledger (G/L) account, you must have correctly configured the **Mapping Text** value. To bypass this error if you want to use G/L accounts, select the **Map Text to Account** to create a specific mapping of the **Mapping Text** value with the **Debit Acc. No.** value that you want to use. 
- If you want to track the inventory and use lines from your vendor invoice to fill in the items on your document lines, you must have correctly configured the **Item Reference No.** value. To bypass this error, map the external item with your item numbers by using the item reference list. To learn more, see [Use Item References](inventory-how-use-item-cross-refs.md). 

After you fix the errors and warnings, you can manually specify when the system should create a purchase invoice based on your setup by selecting **Create Document**.   

#### Manually import invoices  

To manually import external e-documents, follow these steps:

1. Select the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **E-Document Service**, and then select the related link. 
2. On the **E-Document Service** page, select the active service.   
3. Select **Receive**, and upload the e-document file that you got from the vendor. 
4. If an error message occurs, open the e-document to fix the issues. 
5. When you've finished fixing the issues, in the **Import Manually** group, select **Create Document**.  
6. After the document is created in [!INCLUDE[prod_short](includes/prod_short.md)], using a batch job doesn't change the way you view it. 

### E-documents with purchase orders  

#### To link purchase orders with the received e-documents

If your **Vendor** has configured the **Receive E-Document To** field to work with **Purchase Orders**, once electronic document is created in [!INCLUDE[prod_short](includes/prod_short.md)] (manually or from external end point), [!INCLUDE[prod_short](includes/prod_short.md)] will do the following:  

1. If the **Purchase Order** for this particular vendor exists and there's a purchase order number in the receive **E-Document** file, [!INCLUDE[prod_short](includes/prod_short.md)] will automatically link this **E-Document** with the mentioned **Purchase Order**, and the **Document Status** of this **E-Document** will be **In Progress**, and the **E-Document Status** in the **Service Status** subpage will be **Order linked**. This link will be visible in the **Document** field on this specific **E-Document**. If you need to change the **Purchase Order** linked automatically, you can do it using the **Update Purchase Order Link** action and choose manually one of the existing purchase orders for this vendor. You can do it only before matching the lines between **E-Document** and **Purchase Order**.  
2. If the **Purchase Order** for this particular vendor exists but there's no a purchase order number in the receive **E-Document** file, [!INCLUDE[prod_short](includes/prod_short.md)] will offer possibilities to choose one of existing purchase orders when and if you uploaded this document manually, opening the **Purchase Orders** list with orders only for the vendor you got **E-Document**, where you need to select **Purchase Order** you want and select **OK**. If you didn’t select the proper **Purchase Order**, or you got the **E-Document** automatically from external end point using the **Job Queue**, new **E-Document** won't be linked with any purchase document and the **Document Status** will be **Error** and the **E-Document Status** in the **Service Status** subpage will be **Imported document processing error**. To finish linking with the **Purchase Order**, select the **Update Purchase Order Link** action and choose one of the existing purchase orders for this vendor. 
3. If the **Purchase Order** for this particular vendor doesn’t exist in the moment of creation new **E-Document**, [!INCLUDE[prod_short](includes/prod_short.md)] will create a new **Purchase Order**, using the same model of creation as already exists for new **Purchase Invoices**. The **Document Status** of this **E-Document** will be **Processed**, and the **E-Document Status** in the **Service Status** subpage will be **Imported document created**. This link will be visible in the **Document** field on this specific **E-Document**.   

#### Matching lines from received e-document with purchase order  

You can match your received electronic documents with purchase orders’ lines from two different places, from the **E-Document** page or from the **Purchase Order** page. The easiest way to locate the already linked **Purchase Orders** is to use the **Linked Purchase Orders** tile as a part of **E-Document Activities**. All non-linked documents can be found using the tile **Waiting Purchase E-Invoices** where you have a list of **E-Documents** that you need to review.  

> [!NOTE]
> The **E-Document Activities** with these two tiles can be found in the following **Role Centres**: Business Manager Evaluation, Business Manager, Accountant, Inventory Manager, and Shipping and Receiving.  

> [!NOTE]
> If the GST percentage differs between the incoming document and the company's GST percentage, matching documents can't be used in a multi-country environment.  

##### Matching lines from purchase order  

You can match the lines from the **Purchase Orders** list or from one of the opened **Purchase Orders**. To begin this, use the following steps:  

1. Select the **Linked Purchase Orders** tile on your Role Centre if there's any number. 
2. As there are two options for matching, choose one of them: 

    1. If you want to match the lines from the **Purchase Orders** list, select the         **Purchase Order** line that you want to match and choose the **Map E-Document Lines** action.  
    2. If you want to first open the **Purchase Order**, open the document, and then choose the **Map E-Document Lines** action. 

3. As both options have the same process, you'll open the **Purchase Order Matching** page with the following content: 

    1. In the header you can find the following information, which can help you to map the lines easier: 

    |Field name |Description |
    |--------|-----------------|
    |Vendor Name |Specifies the vendor’s name of the electronic document. |
    |E-Document No. |Specifies the linked electronic document number. |
    |E-Document Date |Specifies the linked electronic document date.  |
    |E-Document Amount |Specifies the linked e-document total amount including GST. |

    2. In the lines, you can find the lines imported from the **E-Document** file on the left side and the lines from existing **Purchase Order** on the right side.  
    3. All lines on both sides have item numbers and descriptions, together with the **Direct Unit Cost** and **Line Discount %**.  
    4. On the **Imported Lines** side, you can also locate the **Quantity** field as a total quantity from e-invoice and the **Matched Quantity** field specifying the quantity that already matched to the purchase order lines. 
    5. On the **Purchase Orders Lines** side, you can also find the **Available Quantity** as the quantity that can be matched to this line (received, but not invoiced quantity) and **Qty. to Invoice**, specifying the quantity that is already matched to this line. 
    6. To match lines, select the lines on both sides that you want to match and choose the **Match Manually** action. The matched lines will be marked with the green colour. 
    7. It's possible to match one to one, but it's also possible to match many to one or one to many, selecting more lines on one or another side before choosing the **Match Manually** action. 
    8. You can also choose the **Match Automatically** action to automatically match all lines with the same **Type**, **No.**, **Unit Price**, **Discount, and **Unit of Measure**. 
    9. If you make a mistake, you can choose the **Remove Match** action to remove the matched lines on the purchase order side or choose the **Reset Matching** action to reset all that is matching. 
    10. If your **E-Document** has many lines, during matching process, you can choose the **Show Pending Lines** action to remove all the e-document lines if they're already completely matched. If you need to see all the lines, you can always choose the **Show All Lines** action. 

4. Once you finish the matching, you need to choose the **Apply To Purchase Order** action.   
5. Once you apply the matching to the **Purchase Order**, [!INCLUDE[prod_short](includes/prod_short.md)] will update the following fields:

    1. **Vendor Invoice No.** and **Document Date** on the document header will be updated with values from the electronic document that you'd received and linked. 
    2. **Qty. to Invoice** in lines will be updated with the values from the **Qty. to Invoice** column from the **Purchase Order Matching** page based on matching you did. 
    3. Now you can post the document, by choosing the **Post** action.  
    4. Once you post the document, the **Document** field on the **E-Document** page will change the value and it will relate to the **Posted Purchase Invoice**. 
    5. Close the page.  

> [!IMPORTANT]
> By default, you can match only the lines that has the same total amount in both documents. That means **Direct Unit Cost** together with the applied Line **Discount %** must be the same, as in one document you can have an amount without discount and in another with discount.  

If you want to add some tolerance and allow the difference between lines in **E-invoice** and **Purchase Order**, follow the steps:   

1. Select the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchases & Payables Setup**, and then select the related link.  
2. You want to allow tolerance in the **E-Document Matching Difference %** field, specifying the maximum allowed percentage of cost difference when matching incoming **E-Document** line with the **Purchase Order** line. 
3. This setup will apply to all the matching lines, but again considering tolerance for the total amount, as for **Direct Unit Cost** together with applied **Line Discount %**.  
4. Close the page.   

##### To match lines from e-document  

You can match the lines on the **E-Document** page. To start with this, use the following steps:  

1. Select the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **E-Documents**, and then select the related link. 
2. Select the **E-Document** that you want to match.   
3. Choose the **Match Purchase Order** action to open the **Purchase Order Matching** page.  
4. Repeat the same steps that you used when you started matching from purchase orders.

### E-document matching assistance copilot  

> [!NOTE]
> Currently, **E-Document Matching Assistance** copilot is in the Production ready preview status, and it is available globally except in Canada. But it works in English only. 

> [!NOTE]
> Copilot is the AI-powered assistant that helps people across your organisation unlock their creativity and automate tedious tasks. The **E-Document Matching Assistance** copilot helps users to easily match their received electronic invoices with existing purchase order lines, using LLM model for matching lines between two different documents. 

#### To activate the copilot  

In case you didn't activate **E-Document Matching Assistance** copilot, you need to do it manually. To enable the **E-Document Matching Assistance** copilot, follow the steps: 

1. Select the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Copilot & AI Capabilities**, and then select the related link. 
2. In the list of capabilities choose **E-Document Matching Assistance** and change the status to **Active**.  

Once the Copilot is activated, you can begin using it.

#### Use the e-document matching assistance copilot 

If the Copilot is activated, existing actions **Map E-Document Lines** on purchased orders and **Match Purchase Order** on the **E-Document** page will get different icons, symbolising AI capability. You can run these actions (absolutely the same as in previous examples from the list of purchase orders), from one of the **Purchase Orders**, or from **E-Document**. All steps for running are the same, but when you run this action, the result will be different, and you need to follow the steps:  

1. Choose the **Map E-Document Lines** or **Match Purchase Order** action, for already linked documents.  
2. You can notice that **E-Document Match Order Lines with Copilot** prompt is working and  you have the **Purchase Order Matching** page in the background. That means the same process is happening but with the automatic support of **Copilot**, who runs the process of matching instead of you. 
3. After a few seconds, the **E-Document Match Order Lines with Copilot** will suggest lines for matching with some additional details: 

    1. In the prompt header, you can find the following information: 

    |Field name |Description |
    |--------|-----------------|
    |Auto-matched | Specifies the number of matches proposed automatically. This is based on a string comparison and if there's 80% or more description overlapping, the system will match these descriptions automatically without using GPT capabilities. |
    |Copilot matched | Specifies the number of matches proposed by Copilot using both string and semantical comparison. |
    |E-Document No. | Specifies the linked E-Document number. |
    |Invoice Total Amount Excl. GST | Specifies the total invoice amount excluding GST. |
    |Matched Total Amount Incl. GST | Specifies the matched amount excluding GST. |
    
    2. If all lines are matched, you'll see the green text in the upper right corner: **All lines (100%) are matched. Review match proposals**.  
    3. In the **Matched proposal** lines, you can find the following information:  

    |Field name |Description |
    |--------|-----------------|
    |E-Document Line No. | Specifies the E-Document line number (coming from the original e-document file). |
    |E-Document Line Description | Specifies the E-Document line description (coming from the original e-document file). |
    |Matched Quantity | Specifies the quantity that will be applied to the purchase order line. |
    |Proposal | Specifies the action proposed by AI, and these suggested actions are related to matching the purchase order lines. |

    4. All fully suggested and matched lines are marked with green colour. If there's any issue, i.e., different price, but in the allowed price range, this line will be marked as yellow, and if there's any similarity between the description fields but price difference is bigger than allowed, this line will be marked as red. 
    5. If you aren't satisfied with some suggestions, you can delete them using the **Delete Line** action.  
    6. If you want to see proposal matchings, you can select the link in the **Proposal** column to open the **E-Document Match Details** page. 
    7. On the **E-Document Match Details** page you can compare details from the **E-Document** and **Purchase Order**, to be sure about the suggested matching before confirming it. 
    8. After reviewing, close the page.   

4. If you aren't satisfied with most of the suggestions, or in a case you don't want to use the **E-Document Match Order Lines with Copilot** feature, select **Discard it**, and you can continue with the manual matching as explained previously.  
5. If you want to keep suggestions, choose the **Keep it** button and the system will save all suggestions made by **Copilot**.  
6. [!INCLUDE[prod_short](includes/prod_short.md)] will close the Copilot prompt and lines on the **Purchase Order Matching** page will be marked as green, as they're already matched.  
7. From this moment, you can continue to work as you're doing manual matching, and that means you can remove matches, manual matches, reset matching or if there are no changes you want to make, just choose the **Apply To Purchase Order** action and continue working with the **Purchase Order**. 

> [!NOTE]
> If you want you can choose the **Match with Copilot** action fon the **Purchase Order Matching** page again, but in this case, you will be asked if you want to overwrite the existing matches, as all lines have been matched already.  

> [!NOTE]
> Price/Cost analyse, and the available quantity check is a part of preprocessing activity.   

## Overview of e-document statuses

To get a better overview of all e-documents in the company, you can select the **Accountant** role centre where e-document statuses exist. There, you can find e-document activities that have the following statuses:

- **Incoming e-documents:**

    - Processed
    - In Progress
    - Error


## See also

[How to set up e-documents in [!INCLUDE[prod_short](includes/prod_short.md)]](finance-how-setup-edocuments.md)    
[How to use e-document in the sales process](finance-how-use-edocuments.md)   
[How to extend e-documents in [!INCLUDE[prod_short](includes/prod_short.md)]](/dynamics365/business-central/dev-itpro/developer/devenv-extend-edocuments)    
[Financial Management](finance.md)    
[Invoice Sales](sales-how-invoice-sales.md)    
[Record Purchases with Purchase Invoices and Orders](purchasing-how-record-purchases.md)    
[Work with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]

