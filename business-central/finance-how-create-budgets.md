---
title: Create G/L budgets
description: Describes how to create G/L budgets to forecast different financial activities and assign dimensions for business intelligence purposes.
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bholtorf
ms.topic: conceptual
ms.devlang: al
ms.search.keywords: postpone
ms.search.form: '113, 120, 121, 154, 350, 422, 7132, 7133, 7138, 7139, 9203, 9219, 9239, 9373, 9374'
ms.date: 08/07/2024
ms.service: dynamics-365-business-central
---

# Create G/L budgets

You can have multiple budgets for identical time periods by creating budgets with separate names. First, you set up the budget name and enter the budget figures. The budget name is then included on all the budget entries you create.  

When you create a budget, you can assign budget-specific dimensions, called budget dimensions, for it. You can use budget dimensions to set filters on a budget and to add dimension information to budget entries. Learn more at [Work with Dimensions](finance-dimensions.md).

Budgets play an important role in business intelligence. Examples include a financial statement based on financial reports that include budget entries or when analysing budgeted versus actual amounts in the chart of accounts. Learn more at [Business Intelligence](bi.md).

In cost accounting, you work with cost budgets in a similar way. Learn more at [Creating Cost Budgets](finance-create-cost-budgets.md).  

## To create a new G/L budget

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **G/L Budgets**, and then choose the related link.  
2. Choose the **Edit List** action, then fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  
3. Choose the **Edit Budget** action.
4. At the top of the **Budget** page, fill in the fields as necessary to define what is displayed.  

   The page shows only entries that contain the budget name you entered in the **Budget Name** field. Because you just created the budget name, there are no entries that match the filter. Therefore, the page is empty.  
5. To enter an amount, choose the relevant cell in the matrix. The **G/L Budget Entries** page opens.  
6. Create a new line and fill in the **Amount** field. Close the **G/L Budget Entries** page.  
7. Repeat steps 5 and 6 for all amounts in the budget.  

> [!NOTE]  
> On the **Filters** FastTab, you can filter the budget information by the budget dimensions you set up under the budget name.

## Exporting and importing G/L budgets with Excel

As for practically all other pages, you can export data on budget pages to Microsoft Excel for further processing or analysis. Learn more at [Exporting Your Business Data to Excel](about-export-data.md).

> [!NOTE]
> The chart of accounts, which general ledger (G/L) budgets are based on, has lines of the account type Heading. These lines contain the total of the lines below it. When you export a G/L budget, you export data on all lines regardless of the account type. However, you can only import data on lines of the Posting account type.

Similarly, when you import a G/L budget, any values on Heading lines are deleted. They're deleted to avoid incorrect totals after you import data that was created or edited in Excel.

### Scenario

You know that the new budgeted salaries cost is going to be local currency (LCY) 1.200.000. You want to enable the Salaries department to budget for the three specific lines (of the Posting account type) for full-time employees, part-time employees, and temp help. The three lines are grouped under a Salaries heading line.

You enter 1.200.000 on the Heading line, export the budget to Excel, then send it to the Salaries department, telling them to distribute the LCY 1.200.000.

The Salaries department distributes the amount on the three posting accounts. When you import back into the G/L budget, the three accounts are filled in with the new Excel data, summing to LCY 1.200.000, and the Heading line is blank.

## See also

[Exporting Your Business Data to Excel](about-export-data.md)    
[Finance](finance.md)    
[Business Intelligence](bi.md)    
[Setting Up Finance](finance-setup-finance.md)    
[The General Ledger and the Chart of Accounts](finance-general-ledger.md)    
[Work with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)    

[!INCLUDE[footer-include](includes/footer-banner.md)]
