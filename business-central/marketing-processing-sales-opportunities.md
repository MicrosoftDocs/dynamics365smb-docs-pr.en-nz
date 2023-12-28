---
title: Process Sales Opportunities in Sales Cycles
description: This topic describes the different ways you can process sales opportunities in sales cycles and move an opportunity through the stages of a sales cycle.
author: jswymer
ms.author: jswymer
ms.reviewer: ivkoleti
ms.topic: conceptual
ms.search.keywords: 'relationship, prospect'
ms.date: 12/28/2023
ms.custom: bap-template
---
# <a name="process-sales-opportunities"></a>Process Sales Opportunities

After you create an opportunity, there are several features for managing the opportunity and moving it through to completion.

## <a name="view-opportunities"></a>View opportunities

Existing sale opportunities are available on the **Opportunity List** page. The following table describes ways to access the page to process sales opportunities.

| To view opportunities for | Then |
| --- | --- |
| All salespeople and contacts |Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Opportunity List**, and then choose the related link. |
| A specific sales person |Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Salespeople**, and then choose the related link. Select the salesperson, choose the **Opportunities** action, and then choose the **List** action. |
| A specific contact |Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Contacts**, and then choose the related link. Select the contact from the list, and then choose the **Opportunities** action. |

Each of these tasks opens the **Opportunity List** page.

## <a name="close-opportunities"></a>Close opportunities

You can close opportunities when the negotiations are over. When you close an opportunity, you can specify whether it was won or lost, and the reasons for closing it. To specify a reason, you must set up closed opportunity codes.

1. On the **Opportunity List** page, select the opportunity, and the choose the **Close** action. The **Close Opportunity** page opens.
2. Fill in the relevant fields, and then choose the **OK** button.

   The **Close Opportunity Code** and **Date Closed** fields are required fields and must be filled in before you can choose the **OK** button.

   In the **Close Opportunity Code** field, you can choose from one of the existing close opportunity codes or add a new code. To add a new code, from the drop-down list, choose **Select from full list**, and then choose **new**. On the new blank line, fill in the **Code**, **Type**, and **Description** fields, and then choose the **OK** button.

## <a name="create-quotes-for-opportunities"></a>Create quotes for opportunities

> [!NOTE]
> You can only create sales quotes from opportunities where the contact type is Company.

1. On the **Opportunity List** page, select the opportunity, and then choose the **Assign Sales Quote** action. The **Sales Quote** page opens.
2. Fill in the relevant fields.

## <a name="create-sales-orders-for-opportunities"></a>Create sales orders for opportunities

You can make sales orders from the sales quotes that you have created for your opportunities. Before you can create sales orders for your contacts, you must create the contact as a customer. For more information, see [Create Contacts](marketing-create-contact-companies.md).

1. On the **Opportunity List** page, find the opportunity that you have created a sales quote for.
2. Choose the **Assign Sales Quote** action. The **Sales Quote** page opens to show the sales quote that you have assigned to the opportunity.
3. Fill in the additional fields, and then choose the **Make Order** action.

When handling sales opportunities, you may need to create a quote for the contact that the opportunity is linked to.

## <a name="delete-opportunities"></a>Delete opportunities

You can delete opportunities, for example, after you conclude a deal. However, you can only delete closed opportunities. There are two ways to delete closed opportunities. You can delete individual closed opportunities from the **Opportunity List** page or you can run the **Delete Opportunities** batch job to delete multiple opportunities based on specified criteria.

To delete closed opportunities from the **Opportunity List** page, select the opportunity, and then choose the **Delete** action.

To delete closed opportunities by using the **Delete Opportunities** batch job, follow these steps:

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Data Administration**, and then choose the related link.
2. Choose the **Delete Opportunities** action, and then set the filters that specify the closed opportunities to delete.
3. Choose the **OK** button.

After you delete an opportunity, it's removed it from the **Opportunity List** page.

## <a name="move-an-opportunity-through-sales-cycle-stages"></a>Move an opportunity through sales cycle stages

If an opportunity follows a sales cycle, you can move it to the next or previous stage, and even skip a stage.

1. On the **Opportunity List** page, choose the **Update** action. The **Update Opportunity** opens,
2. Use the **Action Type** field to move the opportunity through the sales cycle stages:
   * **Next** moves the opportunity forward one stage.
   * **Skip** moves the opportunity forward one or several stages in the sales cycle, which you specify in the **Presentation** field. You can only skip stages that have been set up to allow skipping.
   * **Previous** moves the opportunity back one stage.
   * **Jump** moves the opportunity back one or several stages in the sales cycle, which you specify in the **Presentation** field.
   * **Update** enables you to change information (such as to modify your evaluation of their chances of success and estimated values) without moving to another stage.
3. Fill in the other fields as needed, and then choose the **OK** button.

## <a name="see-also"></a>See also

[Sales](sales-manage-sales.md)  
[Creating and Managing Contacts](marketing-contacts.md)  
[Work with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]
