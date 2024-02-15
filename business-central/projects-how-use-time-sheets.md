---
title: Use Time Sheets
description: Learn how to create time sheets and submit them for approval.
author: brentholtorf
ms.author: bholtorf
ms.reviewer: ivkoleti
ms.topic: conceptual
ms.search.keywords: 'project management, capacity, staff, resource, time sheets'
ms.search.form: '950, 951, 973'
ms.date: 07/27/2023
ms.service: dynamics-365-business-central
ms.custom: bap-template
---
# <a name="use-time-sheets"></a>Use Time Sheets

Use time sheets to track absence, and to track time and resources that are spent on a project. Tracking time helps you identify issues early and avoid delays or cost overruns. Time sheets make it easy for a resource to report time usage for an individual or a machine so that managers can review the usage and its allocation. This article describes how to work with time sheets.  

You can copy and use your job planning lines in a time sheet. In that way, you must only enter the information in one place and the line information is always correct. To learn more, go to [To copy job planning lines to a time sheet](#copy-job-planning-lines-to-a-time-sheet).

After you have approved time sheet entries for a job, you can post them to the relevant job journal or resource journal. To learn more, go to [To post time sheet lines in a job journal](#to-post-time-sheet-lines-in-a-job-journal) and [To post time sheet lines in a resource journal](#post-time-sheet-lines-in-a-resource-journal).

Before you can use time sheets, you must set up general information and specify an administrator and one or more approvers of time sheets. To learn more about setting up time sheets, go to [Set Up Time Sheets](projects-how-setup-time-sheets.md).  

> [!TIP]
> You can use time sheets on a mobile device. To do that, you might have to turn on the **Use New Time Sheet Experience** toggle on the [Resources Setup](https://businesscentral.dynamics.com/?page=462) page.

## <a name="create-time-sheets"></a>Create time sheets

You can use the **Create Time Sheets** page to set up time sheets for a specified number of time periods or weeks. Then, the time sheet owner can open it and record time that has been spent on a task. You can also [schedule the batch job to run automatically](ui-work-report.md#ScheduleReport).  

> [!IMPORTANT]
> You must have permissions to be able to create time sheets. To learn more about permissions, go to [Set Up Time Sheets](projects-how-setup-time-sheets.md).

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Create Time Sheets**, and then choose the related link.

    > [!TIP]
    > You can also use the **Create Time Sheets** action on the **Resources** list page and the **Resource Card** page.
2. Fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

    > [!NOTE]  
    > Before you create time sheets for a resource, make sure that the **Use Time Sheet** and **Time Sheet Owner User ID** fields are specified for them on the **Resource Card** page.

    Optionally, choose the **Schedule** action to specify how often to automatically run the task. For example, to configure the task to run weekly for four weeks, on the **Schedule a Report - Create Time Sheets** page, in the **Next Run Date Formula** field, enter **4W**. To learn more about how to schedule reports, go to [Scheduling a Report to Run](ui-work-report.md#ScheduleReport).  

You can view the time sheets that you have created on the **Time Sheets** page. Each time sheet consists of one or more lines that define the time that you want to submit for approval. The following table describes the types of lines that you can add to the time sheet.

| **Field** | **Description** |
|---|---|
| | Use to add a note or marker in the **Description** field of the time sheet line. For example, you can use this field to categorise time sheet entries. If you leave the **Type** field empty for a time sheet line, you can't enter time values in the weekday fields for that line. |
| Absence | Use to register the time you're absent during a work week. To complete the information for the line, specify the type of absence in the **Cause of Absence Code** field. |
| Assembly Order | Used to register time for assembly orders. A time sheet line of this type is created during the posting of assembly order lines for which the resource is set up to use time sheets. You can't manually select a line of this type. |
| Job | Use to register time usage for a project. To complete the information for the line, specify the job number and the job task number for which you want to register time. You can register time for lines that you haven't scheduled.|
| Resource | Use to register time usage for a resource. To complete the information for the line, provide a description of the work. |
| Service | Use to register time usage for a service order or service credit memo. |

For example, you want to submit a time sheet for a week where you did cleaning tasks and had a day off for a medical appointment. The following table shows how you would add lines to the time sheet.

| Type | Description | Work Type Code | Absence Type Code |
|--|--|--|--|
| Resource | Work hours | Cleaning |  |
| Absence | Time off |  | Health |
|  | I had to take off Tuesday due to a medical appointment. |  |  |

In this hypothetical example, you would then register the relevant hours across the relevant days in the fields for each weekday.  

> [!TIP]
> In most cases, your company will have predefined work types for the various types of lines. In those cases, you just choose the relevant work type from the list, and then you add your own description.  
>
> Choose the work type by choosing the :::image type="icon" source="media/assist-edit-icon.png" border="false"::: button in the **Description** field, by choosing the **Activity Details** action and then specifying it in the page that opens, or by choosing it in the **Work Type Code** field or the **Absence Type Code** field, respectively. In this case, you can ignore the [To define work types and add one to a time sheet](#define-work-types-and-add-one-to-a-time-sheet) section.  

## <a name="reuse-time-sheet-lines-in-other-time-sheets"></a>Reuse time sheet lines in other time sheets

If your time sheet information remains the same from time period to time period, you can save time by copying the lines from the previous time period. Then, you just enter your time usage for the new period.

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Time Sheets**, and then choose the related link.  
2. Open the time sheet for a period later than the period for an existing time sheet with lines.  
3. Choose the **Copy Lines from Previous Time Sheet** action.

The lines are copied, including details such as type and description. For example, if the line is related to a job, the **Job No.** is copied. All copied lines have the status **Open**. You can now modify the lines as needed.

## <a name="copy-job-planning-lines-to-a-time-sheet"></a>Copy job planning lines to a time sheet

The following procedure describes how to quickly add job planning lines to a time sheet.

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Time Sheets**, and then choose the related link.  
2. On the **Time Sheets** page, select a time sheet for the relevant time period.  
3. Choose the **Create lines from job planning** action. Any job planning lines in the time sheet time period are copied to the time sheet for the person or machine in the **Resource No.** field on the time sheet.

## <a name="define-work-types-and-add-one-to-a-time-sheet"></a>Define work types and add one to a time sheet

You can define the work type for all-time sheet lines for service orders, job orders, and resources. In this way, you can add information that you need to bill the customer for different types of work.  

1. In the **Time Sheets** page, choose the relevant time sheet.
2. On the first of the lines in the **Lines** section, choose the **Type** field, and then choose the relevant type, such as *Resource*.  
3. Choose the **Description** field, and then, in the **Time Sheet Line Resource Detail** page, fill in the fields. [!INCLUDE [tooltip-inline-tip_md](includes/tooltip-inline-tip_md.md)]  
    1. If no work types exist, choose the **New** action.
    2. On the **Work Types** page, fill in the fields as necessary, and then return to the time sheet.
4. Fill in the rest of the time sheet. For more information, see the [To fill in time sheet lines and submit for approval](#fill-in-time-sheet-lines-and-submit-for-approval) section.  

> [!TIP]
> Similar steps apply to defining absence codes.

## <a name="fill-in-time-sheet-lines-and-submit-for-approval"></a>Fill in time sheet lines and submit for approval

Time sheet registration is tracked in hours, the standard base unit of measure for resources. By default, a time sheet shows the common work days of Monday through Friday.  

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Time Sheets**, and then choose the related link.  
2. Select a time sheet for the relevant period.
3. Fill in the fields on a line as necessary. Enter the number of hours used by the resource on each day of the week.  

    In most cases, to track work, you add a line of type *Resource*, and then you register hours spent each day. If you want to register absence, you add a line of type *Absence*.  

    > [!TIP]  
    > You can review the sum of time sheet hours that you have entered in the **Actual/Budgeted Summary** FactBox.  
4. Repeat step 3 for other work types that the resource performs.  

    Next, decide whether to submit all, or selected, lines on the time sheet.  

    * To submit the time sheet for one or more lines, choose the relevant line, and then choose the **Submit** action.

        In the submission page, choose the **Selected lines only** option. The state of the line changes from **Open** to **Submitted**.
    * To submit the time sheet for all open lines, choose the **Submit** action at the top of the **Time Sheet** page.  

        Confirm that you want to submit all open lines on the current time sheet.  

    > [!NOTE]  
    > You can only submit time sheet lines for which you have entered time.  
5. To modify information on a line that has been set to **Submitted**, select the line, and then choose the **Reopen** action.

    > [!NOTE]  
    > A manager might reject a time sheet line that is submitted for approval. If a line has the status **Rejected**, you can make changes to the line, and then choose **Submit** again.  
6. Choose the **OK** button.

## <a name="approve-or-reject-a-time-sheet"></a>To approve or reject a time sheet

A time sheet must be submitted for approval before it can be used. You can approve and reject individual lines on a time sheet or send them back to the submitter. You approve a time sheet in two ways:

* A time sheet administrator can approve any time sheet.
* The person who is specified in the **Time Sheet Approver User ID** field on a resource card can approve that resource's time sheets. To learn more about setting up approval, go to [Set Up Time Sheets](projects-how-setup-time-sheets.md).

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Manager Time Sheets**, and then choose the related link.
2. Select a time sheet from the list.  
3. On the **Time Sheet** page: 
    1. Choose the **Process** action, then choose the **Approve** action.
    2. Choose the **All submitted lines** action to approve all lines or the **Selected lines only** action to approve only the lines that are selected on the **Time Sheet** page.
4. Choose the **OK** button.  
5. Alternatively, choose the **Reject** action and follow steps 4 through 5.  

> [!TIP]  
> Use the **Time Sheet Status** and **Actual/Budgeted Summary** FactBoxes to get an overview of time sheet information.

After you have approved or rejected a time sheet, it can't be modified unless it's first reopened. The following procedure explains how to reopen an approved or rejected time sheet.

## <a name="reopen-a-time-sheet"></a>Reopen a time sheet

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Manager Time Sheets** or **Time Sheets**, and then choose the related link.
2. Open a time sheet from the list.  

    > [!NOTE]  
    > You can only reopen lines that have the status **Approved**. You can't reopen lines that have the status **Rejected** or has been posted.  
3. On the **Time Sheet** page, choose the **Reopen** action, and then choose the **All submitted lines** action to reopen all lines, or the **Selected lines only** action to reopen only the lines that are selected on the **Time Sheet** page.
4. Choose the **OK** button. The status of the time sheets line or lines is changes to **Submitted**.  

## <a name="view-and-approve-time-sheets-by-job"></a>View and approve time sheets by job

On a job, you can specify a person who is responsible for the job. That information is linked to time sheet lines. The link gives project managers a list of the time sheets to approve. For example, the team's project manager might be responsible for certain jobs in your company. In that case, the manager should be designated as the **Person Responsible** on the Job Card page. This view of time sheet information shows the job tasks associated with a job and the quantity of hours used.

> [!NOTE]
> To approve time sheets on the **Manager Time Sheet by Job** page, you must first select a **Time Sheet by Job Approval** option in the **Resources Setup** page. To learn more about setting up approvals for resources, go to [Set Up Resources](projects-how-setup-resources.md).

### <a name="approve-or-reject-a-time-sheet-by-job"></a>Approve or reject a time sheet by job

1. In the **Search** box, enter **Manager Time Sheet by Job**, and then choose the related link. [!INCLUDE[prod_short](includes/prod_short.md)] displays a list of time sheet lines associated with the jobs for which you have responsibility.
2. Choose the **Approve** action, and then choose the **All submitted lines** action to approve all lines or the **Selected lines only** action to approve only the lines that are selected on the **Time Sheet** page.

    > [!NOTE]
    > You can only approve time sheets that have the status of **Submitted**.

3. To provide additional information about the approval or rejection, select the **Related** action, then **Comments**, and then **Line Comments**.
4. Choose the **OK** button.

> [!NOTE]
> After you approve or reject a time sheet line by job, you can't reopen or modify it on the **Time Sheet** page.

## <a name="post-time-sheet-lines-in-a-resource-journal"></a>Post time sheet lines in a resource journal

After you have approved time sheet entries for a resource, you can post them to the relevant resource journal.

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Resource Journals**, and then choose the related link.  
2. Choose the **Suggest Lines from Time Sheets** action.  
3. On the **Suggest Res. Jnl. Lines** page, in the fields as necessary. [!INCLUDE [tooltip-inline-tip_md](includes/tooltip-inline-tip_md.md)] 
4. Choose the **OK** button. Entries for usage are created in the resource journal, where you can modify the information as needed.  
5. Choose the **Post** action.  
6. To verify the posting, choose the **Ledger Entries** action. The **Resource Ledger Entries** page opens showing the result of posting the resource journal.

## <a name="post-time-sheet-lines-in-a-job-journal"></a>Post time sheet lines in a job journal

After you have approved time sheet entries for a job, you can post them to the relevant job journal.

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Job Journals**, and then choose the related link.  
2. Choose the **Suggest Lines from Time Sheets** action.  
3. On the **Suggest Job Jnl. Lines** page, fill in the fields as necessary. [!INCLUDE [tooltip-inline-tip_md](includes/tooltip-inline-tip_md.md)] 
4. Choose the **OK** button. Entries for usage are created in the job journal, where you can modify the information as needed.  

    > [!NOTE]  
    > Information about the work type and whether the work is chargeable is copied from the time sheet line. If needed, you can reduce the quantity of hours and do a partial posting. If you reduce the quantity, the next time you choose the **Suggest Lines From Time Sheets** action, the line will contain the remaining quantity of hours.  
5. Choose the **Post** action.  
6. To verify the posting, choose the **Ledger Entries** action. The **Job Ledger Entries** page opens showing the result of posting the resource journal.

## <a name="archive-time-sheets"></a>To archive time sheets

After you post time sheets, you can archive them for future reference. You must post all lines on a time sheet before you can archive it.

> [!NOTE]  
> When you archive a time sheet, it's removed from the lists on the **Time Sheets** and **Manager Time Sheets** pages.

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Time Sheets**, and then choose the related link.
2. Select the **Move Time Sheets to Archive** action.  
3. On the **Move Time Sheets to Archive** page, fill in the fields as necessary, and then choose the **OK** button.  
4. To review archived time sheets, choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Time Sheet Archives** or **Manager Time Sheet Archives**, and then choose the related link.

## <a name="see-also"></a>See also

[Project Management](projects-manage-projects.md)  
[Setting Up Project Management](projects-setup-projects.md)  
[Finance](finance.md)  
[Purchasing](purchasing-manage-purchasing.md)  
[Sales](sales-manage-sales.md)  
[Work with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]
