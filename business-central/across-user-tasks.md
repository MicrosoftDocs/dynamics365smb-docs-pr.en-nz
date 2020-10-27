---
title: Assigning and managing tasks| Microsoft Docs
description: Learn how to assign tasks to users, including your accountant, in Business Central
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: tasks, work
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: c76751726f5cd680fafc0887fc57a1464d0ac3ca
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 10/01/2020
ms.locfileid: "3922633"
---
# <a name="define-user-tasks"></a>Define User Tasks

In [!INCLUDE[d365fin](includes/d365fin_md.md)], you can create tasks to remind you of work to be done. You can create tasks for yourself, but you can also assign tasks to others or be assigned a task by someone else in your organisation.  

## <a name="managing-user-tasks"></a>Managing User Tasks

The **User Tasks** page shows all tasks, and you can easily create and assign new tasks. When you create a task, you can specify the start date and due date, and you can add a link to the page or report in [!INCLUDE[d365fin](includes/d365fin_md.md)] where the user must do the work.  

For example, you can create a task for yourself or a coworker to view all posted sales invoices. In that case, you link the task to page 143, **Posted Sales Invoices** . In the following screenshot, someone is creating a task for MeganB to review the posted sales invoices.  

:::image type="content" source="media/across-user-tasks/sample-user-task.png" alt-text="Example of a user task":::

> [!TIP]  
> Use the look-up in the **Page** field and then use the **Search** field to find the page that you want.  
>
> You can link to any page, but you cannot link to individual entries, so make the description as explicit as possible, such as writing "Please take a look at customer no. 10000 and make sure they don't have overdue payments.".

### <a name="picking-up-user-tasks"></a>Picking Up User Tasks

In the Business Manager, Bookkeeper, and Accountant Role Centres, a tile shows pending tasks that are assigned to that user. To pick up a task, simply choose it from the list of pending user tasks. In the ribbon, the link **Go to Task Item** opens the page where you can do the work.  

When you have completed a task, simply mark it as completed.  

### <a name="deleting-user-tasks"></a>Deleting User Tasks

If you want to bulk delete all or some user tasks, you can use the **Delete User Tasks** report. In the request page, you can set filters to determine which tasks must be deleted.  

## <a name="see-also"></a>See Also

[Searching for a Page or Report](ui-search.md)  
[Accountant Experiences in [!INCLUDE[d365fin](includes/d365fin_md.md)]](finance-accounting.md)  
