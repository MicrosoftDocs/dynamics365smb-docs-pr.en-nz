---
title: 'Set Up Projects, Prices, and Project Posting Groups'
description: Describes how to set up general information about projects.
author: brentholtorf
ms.author: bholtorf
ms.reviewer: andreipa
ms.topic: how-to
ms.date: 02/22/2024
ms.custom: bap-template
ms.search.keywords: project management
ms.search.form: '211, 463, 1012'
ms.service: dynamics-365-business-central
---
# Set Up projects, prices, and project posting groups

As a project manager, you can set up projects that define each of the projects that you manage in [!INCLUDE[prod_short](includes/prod_short.md)]. Use the **Project Setup** page to define how you'll use project features.

For each project, specify various information:

* Prices for project items
* Project resources
* Project G/L accounts
* Project posting groups (required)

## To set general information for projects

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Project Setup**, and then choose the related link.
2. Fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

> [!NOTE]
> The **Apply Usage Link by Default** toggle on the **Projects Setup** page indicates whether project ledger entries are linked to project planning lines by default. Turn on the toggle to apply this setting to all new projects. You can enable or disable project usage tracking for a specific project by turning the **Apply Usage Link** toggle on or off on the **Project Card** page.

### Specify a default location for project items

You can save time on data entry by specifying a default location and bin for projects on the **Project Card** page. When you create project tasks, project planning lines, and project journal lines for the project, the default location and bin are automatically assigned. You can, however, change the location code and bin on tasks and lines if needed.

If you define a **To-Project Bin Code** on the location, the bin code is populated when you select the location code. If your warehouse flow requires warehouse picks, you can also define other bins from which to consume items.

These fields are the defaults when you create project tasks. Existing project tasks don't change.

There are a few things to know about using default locations:

* For project tasks, if you define a **To-Project Bin Code** on the location, the bin code is assigned when you select the location code. If your warehouse flow requires warehouse picks, you can also define other bins from which to consume items.
* For project planning lines, the **Location Code** is based on the value selected on the project planning line when you select an item. If a bin code isn't defined for the project task, the bin from the default bin content is selected. You can change both values manually.
* For project journal lines, the **Location Code** is based on the value selected on the job journal line when you select an item. If a bin code isn't defined for the project task, the bin from default bin content is selected. You can change both values manually.

### Invoice multiple customers for project tasks 

When projects involve multiple customers, billing the right customers for the right tasks can be challenging. [!INCLUDE [prod_short](includes/prod_short.md)] makes billing less complex by letting you specify the bill-to and sell-to customers on each project task line, so you can automatically generate invoices for the correct customers. To learn more about invoicing multiple customers, go to [Invoice one or more customers for project tasks](projects-how-create-jobs.md#invoice-one-or-more-customers-for-project-tasks).

### To set up project usage tracking

When you're working on a project, you might want to know how your usage is tracking against your plan. To explore usage, you can create a link between your project planning lines and the actual usage. The link lets you track your costs and understand how much work remains. By default, the project planning line type is **Budget**, but using the line type **Both Budget and Billable** has similar effects.

After you set up usage tracking by turning on the **Apply Usage Link by Default** toggle, you can review information on the project planning line. For example, you can set the quantity of the resource, item, or general ledger account. You can also set the quantity to transfer to the project journal. The **Remaining Quantity** field on the project planning line shows what remains to transfer and post to the project journal.

>[!NOTE]
> If the **Apply Usage Link** is chosen on the project, and the **Line Type** field on the project journal line or purchase line is **Billable**, new project planning lines of the line type **Both Budget and Billable** are created when you post the project journal or purchase document.  
>
> For more information, see [Record Usage for Projects](projects-how-record-job-usage.md) and [Manage Project Supplies](projects-how-manage-project-supplies.md)

> [!IMPORTANT]
> If you don't specify a value in the **Line Type** field on the project journal line or purchase line, project planning lines aren't created when you post the project journal or purchase document.

## To set up prices for resources, items, and general ledger accounts for projects

> [!NOTE]
> In 2020 release wave 2, we released new processes for setting up and managing prices and discounts. If you're a new customer, you're using the new experience. If you're an existing customer, whether you are using the new experience depends on whether your administrator has enabled the **New sales pricing experience** feature update in **Feature Management**. For more information, see [Enabling Upcoming Features Ahead of Time](/dynamics365/business-central/dev-itpro/administration/feature-management).

You can set up prices for the items, resources, and general ledger accounts related to a project. 

#### [Current Experience](#tab/current-experience)

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Project**, and then choose the related link.  
2. Select the project, and then choose the **Resource**, **Item**, or **G/L Account** action.
3. On the **Project Resource Prices**, **Project Item Prices**, or **Project G/L Account Prices** pages, fill in the fields as necessary.

When you choose a resource, item, or general ledger account for a project, [!INCLUDE [prod_short](includes/prod_short.md)] uses information in the optional fields on project planning lines and project journals. The following table explains how.

|Column1  |Column2  |
|---------|---------|
|**Project Resources**|The **Project Task No.**, **Work Type**, **Currency Code**, **Line Discount %**, and **Unit Cost Factor** fields. The value in the **Unit Price** field for the resource is used on project planning lines and project journals when you enter a resource, or a resource assigned to the resource group. This price overrides prices specified on the **Resource Price/Resource Group Prices** page.|
|**Project Items**|The **Project Task No.**, **Currency Code**, and **Line Discount %** fields. The value in the **Unit Price** field for the item will be used on the project planning lines and project journals when this item is entered. This price overrides the regular customer price (the "best price" mechanism) for items. To use the regular customer price, don't specify project item prices for the project.|
|**General Ledger Accounts**|The information in the **Project Task No.**, **Currency Code**, **Line Discount %**, **Unit Cost Factor**, and **Unit Cost** fields will be used on the project planning lines and project journals when this general ledger account is entered and added to a project. When you choose a general ledger account, project planning lines and project journals use the value in the **Unit Price** field for the general ledger project expense.|

#### [New Experience](#tab/new-experience)

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Projects**, and then choose the related link.  
2. Select the relevant project, and then choose the **Sales Price Lists** action.

---

## To set up project posting groups

One aspect of planning projects is deciding which posting accounts to use for project costing. To be able to post projects, you set up accounts for posting for each project posting group. A posting group represents a link between the project and how it should be treated in the general ledger. When you create a project, you specify a posting group, and by default, each task you create for the project is associated with that posting group. However, as you create tasks, you can override the default and select a posting group that is more appropriate.  

> [!NOTE]  
> You must set up accounts in the chart of accounts before you set up posting groups. For more information, see [Set Up or Change the Chart of Accounts](finance-setup-chart-accounts.md).  

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Project Posting Groups**, and then choose the related link.  
2. Choose the **New** action, and then fill in the fields as described in the following table.  

| Account field | Description | Used in WIP Type |
| --- | --- |  --- |
| **Code** |An identifier for the posting group. You can enter up to 10 characters, including spaces. | |
| **WIP Costs Account** |The WIP account for the calculated cost of the project WIP, which is a balance sheet capital asset account. | Applied Cost, Recognised Costs|
| **WIP Accrued Costs Account** |An account for the Cost Value or Cost of Sales method of WIP calculation. This account is for accrued expense liability on your balance sheet. When a WIP adjustment requires you to increase the usage costs that you post to your income statement, you post to this account. | Accrued Costs|
| **Project Costs Applied Account** |A balancing account to the WIP Costs Account, which is a contra for a negative expense account. Used when **WIP Posting Method Used** is set to *Project*. | Applied Costs, Recognised Costs|
| **Item Costs Applied Account** |Same as  **Project Costs Applied Account**, but used when **WIP Posting Method Used** is set to *Project Ledger Entry*.| |
| **Resource Costs Applied Account** |Same as  **Project Costs Applied Account**, but used when **WIP Posting Method Used** is set to *Project Ledger Entry*.| |
| **G/L Costs Applied Account** |Same as  **Project Costs Applied Account**, but used when **WIP Posting Method Used** is set to *Project Ledger Entry*.| |
| **Project Costs Adjustment Account** |The balancing account to the WIP Accrued Costs account, which is an expense account. | Accrued Costs|
| **G/L Expense Acc. (Budget)** |The sales account that will be used for general ledger expenses in project tasks with this posting group. If left empty, the general ledger account entered on the project planning line is used. | |
| **WIP Accrued Sales Account** |The WIP account for the calculated sales value of the WIP, which is an accrued revenue account for your balance sheet. When a WIP adjustment requires you to increase the recognised revenue, you post to this account. | Accrued Sales, Recognised Sales|
| **WIP Invoiced Sales Account** |The account for the invoiced sales value of the WIP that is not able to be recognised. It is a balance sheet Unearned Revenue account. | Recognised Sales, Applied Sales|
| **Project Sales Applied Account** |The balancing account to the WIP Invoiced Sales account, which is a contra income account. | Applied Sales, Recognised Sales|
| **Project Sales Adjustment Account** |The balancing account to the WIP Project Sales Account, which is an income account. | Accrued Sales|
| **Recognised Costs Account** |The expense account that contains the recognised costs for the project. It is a debit expense account ordinarily. | Recognised Costs|
| **Recognised Sales Account** |The income account that contains the recognised income for the project. It is a credit income account ordinarily. | Recognised Sales|

## See also

[Set Up Project Management](projects-setup-projects.md)  
[Video: How to create a project in Dynamics 365 Business Central](https://www.youtube.com/watch?v=VqaPWr7BWmw)  
[Managing Projects](projects-manage-projects.md)  
[Finance](finance.md)  
[Purchasing](purchasing-manage-purchasing.md)  
[Sales](sales-manage-sales.md)  
[Work with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
