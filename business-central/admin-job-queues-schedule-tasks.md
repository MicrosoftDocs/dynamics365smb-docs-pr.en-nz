---
title: Schedule jobs to run automatically | Microsoft Docs
description: Scheduled tasks are managed by the job queue. These jobs run reports and codeunits. You can set jobs to run one time, or on a recurring basis.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 5e8c611ed5d542436f470781c92d17095ecd1f5d
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 10/01/2020
ms.locfileid: "3924594"
---
# <a name="use-job-queues-to-schedule-tasks"></a>Use Job Queues to Schedule Tasks

Job queues in [!INCLUDE[d365fin](includes/d365fin_md.md)] enables users to schedule and run specific reports and codeunits. You can set jobs to run one time, or on a recurring basis. For example, you might want to run the **Salesperson * Sales Statistics** report weekly, to track sales by salesperson each week, or you might want to run the **Delegate Approval Requests** codeunit daily, to prevent documents from piling up or otherwise block the workflow.

The **Job Queue Entries** page lists all existing jobs. If you add a new job queue entry that you want to schedule, you must specify information about the type of object you want to run, such as a report or codeunit, and the name and object ID of the object that you want to run. You can also add parameters to specify the behavior of the job queue entry. For example, you can add a parameter to only send posted sales orders. You must have permission to run the particular report or codeunit, or an error will be returned when the job queue is run.  

A job queue can have many entries, which are the jobs that the queue manages and runs. Information in the entry specifies what codeunit or report is run, when and how often the entry is run, in what category the job runs, and how it runs.  

## <a name="to-set-up-background-posting-with-job-queues"></a>To set up background posting with job queues

Job queues are an effective tool to schedule the running of business processes in the background, such as when multiple users are trying to post sales orders, but only one order can be processed at a time.  

The following procedure explains how to set up background posting of sales orders. The steps are similar for purchasing.  

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales & Receivables Setup** , and then choose the related link.
2. On the **Sales & Receivables Setup** page, choose the **Post with Job Queue** check box.
3. Choose the **Job Queue Category Code** field, and then specify the **SALESPOST** code.

    > [!NOTE]
    > Some jobs change the same data and should not run at the same time because that can cause conflicts. For example, background jobs for sales documents will try to modify the same data at the same time. Job queue categories help prevent these kinds of conflicts by ensuring that when one job is running, another job that belongs to the same job queue category will not run until it finishes. For example, a job that belongs to a Sales job queue category will wait until all other sales related jobs are done. You specify a job queue category on the **Background Posting** FastTab on the **Sales & Receivables Setup** page.
    >
    > [!INCLUDE[d365fin](includes/d365fin_md.md)] provides job queue categories for sales, purchase, and general ledger posting. We recommend that one of these, or one that you create, is always specified. If you experience failures due to conflicts, consider setting up a category for all sales, purchase, and general ledger background posting.

    If you also want sales documents to be printed when they are posted, select the **Post & Print with Job Queue** check box on the **Sales & Receivables Setup** page.  

    > [!IMPORTANT]  
    > If you set up a job that will post and print documents, and the printer displays a dialogue box, such as a request for credentials or a warning about low printer ink, your document is posted but not printed. The corresponding job queue entry eventually times out and the **Status** field is set to **Error** . Accordingly, we recommend that you do not use a printer setup that requires interaction with the display of printer dialogue boxes in conjunction with background posting.

    Next time that you post sales documents, [!INCLUDE [prodshort](includes/prodshort.md)] automatically creates a job queue entry for each document and run the jobs in the background, one by one.

4. To verify that the job queue is working as expected, post a sales order. For more information, see [Sell Products](sales-how-sell-products.md).

5. Review on the **Job Queue Log Entries** page if the sales order was posted successfully. For more information, see [To view status or errors in the job queue](admin-job-queues-schedule-tasks.md#to-view-status-or-errors-in-the-job-queue).

## <a name="to-create-a-job-queue-entry-for-batch-posting-of-sales-orders"></a>To create a job queue entry for batch posting of sales orders

Alternatively, you can postpone postings for when it is convenient for your organisation. For example, in your business it might make sense to run certain routines when most of the data entry for the day has concluded. You can achieve this by setting the job queue up to run various batch-posting reports, such as the **Batch Post Sales Orders** , **Batch Post Sales Invoices** , and similar reports. [!INCLUDE[d365fin](includes/d365fin_md.md)] supports background posting for all sales, purchasing, and service documents.

The following procedure shows how to set the **Batch Post Sales Orders** report up to automatically post sales orders at 4 PM on week days.  

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Job Queue Entries** , and then choose the related link.  
2. Choose the **New** action.  
3. In the **Object Type to Run** field, select **Report** .  
4. In the **Object ID to Run** field, select 296, **Batch Post Sales Orders** .

   You can also use following reports:
  
   * 900 **Batch Post Assembly Orders**
   * 497 **Batch Post Purchase Invoices**
   * 496 **Batch Post Purchase Orders**
   * 498 **Batch Post Purch. Credit Memos**
   * 6665 **Batch Post Purch. Ret. Orders**
   * 298 **Batch Post Sales Credit Memos**
   * 297 **Batch Post Sales Invoices**
   * 296 **Batch Post Sales Orders**
   * 6655 **Batch Post Sales Return Orders**
   * 6005 **Batch Post Service Cr. Memos**
   * 6004 **Batch Post Service Invoices**
   * 6001 **Batch Post Service Orders**

5. Select the **Report Request Page** check box.
6. In the **Batch Post Sales Orders** request page, define what is included during automatic posting of sales orders, and then choose the **OK** button.

    > [!IMPORTANT]
    > Remember to set strict filters; otherwise, [!INCLUDE [prodshort](includes/prodshort.md)] will post all documents, even if they are not ready. Consider setting a filter on the **Status** field for the value *Released* , and a filter on the **Posting Date** field for the value *..today* . For more information, see [Sorting, Searching, and Filtering](ui-enter-criteria-filters.md).
7. Select all check boxes from **Run on Mondays** through **Run on Fridays** .
8. In the **Starting Time** field, enter 4 PM.
9. Choose the **Set Status to Ready** action.

Sales orders that are within defined filters will now be posted every week day at 4 PM.

> [!NOTE]
> If the job queue cannot post the sales order, the status is changed to **Error** and the sales order is added to the list of sales orders that the user must handle manually. For more information, see [To view status or errors in the job queue](admin-job-queues-schedule-tasks.md#to-view-status-or-errors-in-the-job-queue).

After job queues are set up and running, the status can change as follows within each recurring period:

* **On Hold**  
* **Ready**  
* **In Process**  
* **Error**  
* **Finished**  

After a job has finished successfully, it is removed from the list of job queue entries unless it is a recurring job. If it is a recurring job, the **Earliest Start Time** field is adjusted to show the next time that the job is expected to run.  

## <a name="to-view-status-or-errors-in-the-job-queue"></a>To view status or errors in the job queue
Data that is generated when a job queue is run is stored in the database, so that you can troubleshoot job queue errors.

### <a name="to-view-status-for-any-job"></a>To view status for any job
1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Job Queue Entries** , and then choose the related link.
2. On the **Job Queue Entries** page, select a job queue entry, and then choose the **Log Entries** action.  

### <a name="to-view-status-from-a-sales-or-purchase-document"></a>To view status from a sales or purchase document
1. From the document that you have tried to post with background posting, choose the **Job Queue Status** field, which will contain **Error** .
2. Review the error message and fix the problem.

## <a name="the-my-job-queue-part"></a>The My Job Queue Part
The **My Job Queue** part on your Role Centre shows the job queues entries that you have started, but which are not yet finished. By default, the part is not visible, so you have to add it to your Role Centre. For more information, see [Personalise Your Workspace](ui-personalization-user.md).  

The part shows which documents with your ID in the **Assigned User ID** field are being processed or are queued, including those related to background posting. The part can tell you at a glance whether there has been an error in the posting of a document or if there are errors in a job queue entry. The part also lets you cancel a document posting if it is not running.

### <a name="to-view-an-error-from-the-my-job-queue-part"></a>To view an error from the My Job Queue part
1. On an entry with the status **Error** , choose the **Show Error** action.
2. Review the error message and fix the problem.

## <a name="security"></a>Security  
Job queue entries run based on permissions. Those permissions must allow the execution of the report or codeunit.  

When a job queue is activated manually, it is run with the credentials of the user. When a job queue is activated as a scheduled task, it is run with the credentials of the server instance. When a job is run, it is run with the credentials of the job queue that activates it. However, the user who created that job queue entry must also have permissions. When a job is "run in user session" (such as during background posting), it is run with the credentials of the user who created that job.  

> [!IMPORTANT]  
> If you use the SUPER permissions set that comes with [!INCLUDE[d365fin](includes/d365fin_md.md)], you and your users have permissions to run all objects. In this case, access for each user is only limited by permissions for data.  

## <a name="using-job-queues-effectively"></a>Using Job Queues Effectively  
The job queue entry record has many fields whose purpose is to carry parameters into a codeunit that you have specified to be run with a job queue. This also means that codeunits that are to be run via the job queue must be specified with the Job Queue Entry record as a parameter in the **OnRun** trigger. This helps provide an extra level of security, as this prevents users from running random codeunits via the job queue. If the user must pass parameters to a report, the only way to do this is by wrapping the report execution into a codeunit, which then parses the input parameters and enters them into the report before executing it.  

## <a name="scheduling-synchronization-between-d365fin-and-d365fin"></a>Scheduling Synchronisation Between [!INCLUDE[d365fin](includes/d365fin_md.md)] and [!INCLUDE[d365fin](includes/cds_long_md.md)]

If you have integrated [!INCLUDE[d365fin](includes/d365fin_md.md)] with [!INCLUDE[d365fin](includes/cds_long_md.md)], you can use the job queue to schedule when you want to synchronise data for the records that you have coupled in the two business apps. Depending on the direction and rules that you have defined for the integration, the synchronisation jobs can also create new records in the destination app to match those in the source. For example, if a salesperson creates a new contact in [!INCLUDE[crm_md](includes/crm_md.md)], the synchronisation job can create that contact for the coupled salesperson in [!INCLUDE[d365fin](includes/d365fin_md.md)]. For more information, see [Scheduling a synchronisation between Business Central and Dynamics 365 Sales](admin-scheduled-synchronization-using-the-synchronization-job-queue-entries.md).

## <a name="see-also"></a>See Also

[Administration](admin-setup-and-administration.md)  
[Setting Up Business Central](setup.md)  
[Change Basic Settings](ui-change-basic-settings.md)  
