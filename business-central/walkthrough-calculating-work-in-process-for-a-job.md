---
title: Walkthrough - Calculating work in process for a project
description: 'Learn how to track consumption of employee hours, machine hours, inventory items, and other types of usage as a project progresses.'
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bholtorf
ms.topic: conceptual
ms.search.keywords: null
ms.date: 12/13/2023
ms.service: dynamics-365-business-central
ms.custom: bap-template
---
# <a name="walkthrough-calculating-work-in-process-for-a-project"></a>Walkthrough: Calculating work in process for a project

<!-- [!INCLUDE[complete_sample_data](includes/complete_sample_data.md)]   -->

With project, you can schedule the usage of your company's resources and keep track of the various costs associated with the usage of resources on a specific project. Project involve the consumption of employee hours, machine hours, inventory items, and other types of usage that have to be tracked as a project progresses. If a project runs over a long period, you might want to transfer these costs to a Work in Process (WIP) account on the balance sheet while the project is being completed. You can then recognise the costs and sales in your income statement accounts when it's appropriate.  

## <a name="about-this-walkthrough"></a>About this walkthrough

 This walkthrough illustrates the following tasks:  

-   Calculating WIP.  
-   Selecting a WIP calculation method.  
-   Excluding part of a project from the WIP.  
-   Posting the WIP to the general ledger.  
-   Reversing a WIP posting.  

 Each step of the process calculates the value and moves the project transactions to the general ledger. The calculation and posting steps are separated to help you review your data and to make modifications before posting to the general ledger. Therefore, you should make sure that all information is correct after you run the calculation batch jobs and before you run the posting batch jobs.  

## <a name="roles"></a>Roles

 This walkthrough uses the project team member (Tricia) as the persona.  

## <a name="prerequisites"></a>Prerequisites

 Before you can perform the tasks in the walkthrough, the [!INCLUDE[prod_short](includes/prod_short.md)] must be installed on your computer.  

## <a name="story"></a>Story

 This walkthrough focuses on CRONUS International Ltd., a design and consultancy firm that designs and fits new infrastructures, such as conference halls and offices, with furniture, accessories, and storage units. Most of the work at CRONUS is project-oriented and Tricia, a project team member, uses project to have an overview of each ongoing project that CRONUS has started and also the project that are completed. Some of the project can be lengthy and can run over months. Tricia can use a WIP account to record the work in process and to track the costs throughout the project.  

## <a name="calculating-wip"></a>Calculating WIP

 CRONUS has taken on a lengthy project that has now extended across reporting periods. Tricia, a project team member, calculates the work in process (WIP) to make sure that the financial statement of the company is accurate.  

 During this procedure, Tricia selects a specific group of tasks that is included in the WIP calculation. On the **Project Task Lines** page, Tricia can specify these lines in the **WIP-Total** column.  

 The following table describes the three options.  

|Field|Description|  
|-------------------------------------|---------------------------------------|  
|**\<blank\>**|Leave blank if the project task is a part of a group of tasks.|  
|**Total**|Defines the range or group of tasks that are included in the WIP and recognition calculation. Within the group, any project task with **Project Task Type** set to **Posting** will be included in the WIP Total, unless its **WIP-Total** field is set to **Excluded**.|  
|**Excluded**|Applies only to a task with **Project Task Type** of **Posting**. The task isn't included when WIP and recognition are calculated.|  

 In the following walkthrough, Tricia applies the Cost Value method, their company standard, to calculate WIP. Tricia specifies the part of the project to include in the WIP calculation by assigning WIP-Total values to various project task lines.  

### <a name="to-calculate-wip"></a>To calculate WIP

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Project**, and then choose the related link.  
2. In the **Projects** list, select the **Deerfield** project, and then choose the **Edit** action. This opens the Project Card in edit mode.  

     WIP can be calculated based on Cost Value, Sales Value, Cost of Sales, Percentage of Completion, or Completed Contract. In this example, CRONUS uses the Cost Value method.  

3. On the **Posting** FastTab, choose the **WIP Method** field, and then select **Cost Value**.  
4. Choose the **Project Task Lines** action and set the following values in the **WIP-Total** field.  

     The following table describes the values.  

    |Project Task No.|WIP-Total Field|  
    |------------------|----------------------|  
    |1130|Excluded|  
    |1190|Total|  
    |1210|Excluded|  
    |1310|Excluded|  

5. Choose the **WIP** action, and then choose the **Calculate WIP** action.  
6. On the **Project Calculate WIP** page, you select a project to calculate WIP for. On the **Project** FastTab, select **Deerfield** in the **No.** field.  
7. In the **Posting Date** field, enter a date that is later than the work date.
8. In the **Document No.** field, enter **1**. This creates a document that you can refer to later for traceability.  
9. Choose the **OK** button to run the batch job. A message is displayed. Choose the **OK** button to continue. Close the **Project Task Lines** page.  

    > [!NOTE]  
    >  The message states that there are warnings associated with the WIP calculation. You will review the warnings in the next procedure.  

10. On the **Project Card** page, expand the **WIP and Recognition** FastTab to see the calculated values. You can also see the **WIP Posting Date** and the values that have been posted to the general ledger, if any.  

 Notice that the value for **Recog. Costs Amount** is 215.60 in the **To Post** column. This reflects the total costs of two of the items in the group of project tasks 1110 – 1130. The third item was set to **Excluded**, and therefore isn't included in the WIP calculation.  

### <a name="to-review-wip-warnings"></a>To review WIP warnings

1.  Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Project WIP Cockpit**, and then choose the related link.  
2.  Select the **Deerfield** project, and then choose the **Show Warnings** action.  
3.  On the **Project WIP Warnings** page, review the warning associated with the project.  

 After the accounting period ends, Tricia has to recalculate the WIP to include completed work to this point.  

### <a name="to-recalculate-wip"></a>To recalculate WIP

1. On the **Project Card** page, choose the **WIP Entries** action to view the WIP calculation.  

     The **Project WIP Entries** page shows the WIP entries that were last calculated on a project, even if WIP hasn't yet been posted to the general ledger.  

2. You can follow the steps in the procedure that explains how to calculate WIP to recalculate WIP. Every time WIP is calculated, an entry is created on the **Project WIP Entries** page.  
3. Close the page.  

> [!NOTE]  
> WIP and recognition are calculated but aren't posted to the general ledger. To do so, you must run **Post WIP to G/L** batch job after you calculate the WIP and recognition.

## <a name="posting-wip-to-general-ledger"></a>Posting WIP to general ledger

 Now that Tricia has calculated WIP for this project, they can post it to the general ledger.  

### <a name="to-post-wip-to-general-ledger"></a>To post WIP to general ledger

1. From the **Projects** list, select the **Deerfield** project.  
2. Choose the **WIP** action, and then choose the **Post WIP to G/L** action.  
3. On the **Project Post WIP to G/L** page, on the **Projects** FastTab, select **Deerfield** in the **No.** field.  
4. On the **Options** FastTab, in the **Reversal Document No.** field, enter **1**.  
5. Choose the **OK** button to post WIP to the general ledger.  
6. Choose the **OK** button to close the confirmation page.  

     After you have completed the posting, you can view the posting information on the **WIP G/L Entries** page.  

7.  In the **Projets** list, select the **Deerfield** project, and then choose the **WIP G/L Entries** action.  

     On the **Project WIP G/L Entries** page, verify that the WIP has been posted to the general ledger.  

8. Close the page.  
9. Open the **Project Card** page for the **Deerfield** project.  
10. On the **WIP and Recognition** FastTab, notice that in the **Posted** column, the **Recog. Costs G/L Amount** field is now filled in, which indicates that WIP was posted to the general ledger successfully.  
11. Choose the **OK** button to close the card.  

## <a name="reversing-a-wip-posting"></a>Reversing a WIP posting

 Tricia determines that the project tasks that were excluded from the calculation of WIP should have been calculated in WIP. Tricia can reverse the incorrect postings without having to post new WIP postings.  

### <a name="to-reverse-a-wip-posting"></a>To reverse a WIP posting

1. From the **Projects** list, select the **Deerfield** project.  
2. Choose the **WIP** action, and then choose the **Post WIP to G/L** action.  
3. On the **Project Post to WIP to G/L** page, on the **Project** FastTab, select **Deerfield** in the **No.** field.  
4. On the **Options** FastTab, in the **Reversal Document No.** field, enter **1**.  
5. In the **Reversal Posting Date** field, enter the original posting date. It should be the same date that you used to calculate WIP the first time.  
6. Select the **Reverse Only** checkbox. This reverses previously posted WIP, but does post new WIP to the general ledger.  
7. Choose the **OK** button to run the batch job, and choose the **OK** button to close the confirmation page.  
8. Open the **Project Card** page for **Deerfield**.  
9. On the **WIP and Recognition** FastTab, verify that there are no posted WIP entries.  
10. Close this page.  
11. In the **Projects** list, select the **Deerfield** project, choose the **WIP** action, and then choose the **WIP G/L Entries** action. The WIP entries have the **Reversed** checkbox selected.  
12. Close this page.  
13. Open **Project Task Lines** for the project, include the parts of the project that should be in the WIP calculation, and then recalculate and post the new value to the general ledger.  

    > [!NOTE]  
    >  Suppose Tricia calculated and posted WIP for a project with incorrect dates. Following the method that was discussed earlier, Tricia can reverse the incorrect postings, correct the dates, and repost to the general ledger.  

## <a name="next-steps"></a>Next steps

 This walkthrough has taken you through the steps of calculating WIP in [!INCLUDE[prod_short](includes/prod_short.md)]. In larger projects, it might be useful to transfer the costs to a WIP account periodically while the project is being completed. This walkthrough has shown you how to exclude task lines from a calculation. It also shows you when you would have to recalculate. And finally, this walkthrough demonstrates how to post the WIP to the general ledger. An example of how to reverse a WIP posting to the general ledger is also included.  

## <a name="see-also"></a>See also

 [Business Process Walkthroughs](walkthrough-business-process-walkthroughs.md)  
 [Walkthrough: Managing Projects](walkthrough-managing-projects-with-jobs.md)  
 [Understanding WIP Methods](projects-understanding-wip.md)  
 [Monitor Progress and Performance](projects-how-monitor-progress-performance.md)  
 [Work with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]
