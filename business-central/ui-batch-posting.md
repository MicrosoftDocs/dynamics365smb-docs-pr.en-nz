---
title: How to Post Multiple Documents at the Same Time | Microsoft Docs
description: Instead of posting individual documents one by one, you can select multiple non-posted documents in a list for batch posting, either for immediate posting or scheduled to, for example, the end of the day.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.reviewer: edupont
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 1fd25f8b07a359414f62ef4757162f8a73889c27
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 10/01/2020
ms.locfileid: "3912737"
---
# <a name="post-multiple-documents-at-the-same-time"></a>Post Multiple Documents at the Same Time

Instead of posting individual documents one by one, you can select multiple non-posted documents in a list for immediate posting or for batch posting according to a schedule, such as at the end of the day. This may be useful if only a supervisor can post documents created by other users or to avoid system performance issues from posting during work hours.

## <a name="to-post-multiple-purchase-orders-immediately"></a>To post multiple purchase orders immediately

The following procedure explains how to post multiple purchase orders immediately. The steps are similar for all purchase and sales documents.

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchase Orders** , and then choose the related link.
2. On the **Purchase Orders** page, proceed to select all orders to be posted:
3. In the **No.** field, choose the three vertical dots to open the context menu, and then choose the **Select More** action.
4. Select the check box for all the lines representing orders that you want to post at the same time.
5. Choose the **Posting** action, and then choose the **Post** action.
6. Choose the **Yes** button on the confirmation message.

## <a name="to-batch-post-multiple-purchase-orders"></a>To batch post multiple purchase orders

The following procedure explains how to batch post purchase orders. The steps are similar for all purchase and sales documents where the **Batch Post** action is available.

> [!NOTE]
> Batch posting of documents happens in the background. [!INCLUDE [prodshort](includes/prodshort.md)] online includes default jobs for background posting and batch posting. For more information, see [Use Job Queues to Schedule Tasks](admin-job-queues-schedule-tasks.md).

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchase Orders** , and then choose the related link.  
2. On the **Purchase Orders** page, proceed to select all orders to be posted:
3. In the **No.** field, choose the three vertical dots to open the context menu, and then choose the **Select More** action.
4. Select the check box for all the lines representing orders that you want to post at the same time.
5. Choose the **Posting** action, and then choose the **Post Batch** action.
6. On the **Batch Post Purchase Order** page, fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
7. Choose the **OK** button.
8. To view potential issues that occurred during batch posting of documents, open the **Error Message Register** page.

The purchase orders will now be added to a dedicated job queue entry, which defines when the documents are posted. For more information, see [Use Job Queues to Schedule Tasks](admin-job-queues-schedule-tasks.md).

If you select **PDF** in the **Report Output Type** field, successfully posted purchase orders will be available in the **Report Inbox** part on your Role Centre.

## <a name="see-also"></a>See Also

[Posting Documents and Journals](ui-post-documents-journals.md)  
[Use Job Queues to Schedule Tasks](admin-job-queues-schedule-tasks.md)  
[Edit Posted Documents](across-edit-posted-document.md)  
[Correct or Cancel Unpaid Purchase Invoices](purchasing-how-correct-cancel-unpaid-purchase-invoices.md)  
[Finding Pages and Information with Tell Me](ui-search.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
