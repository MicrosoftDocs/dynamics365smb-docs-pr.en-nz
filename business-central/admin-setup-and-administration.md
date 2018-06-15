---
title: Administrative tasks in Business Central | Microsoft Docs
description: Some tasks in Business Central requires central administration and setup. See what they are and learn what to do.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 05/07/2018
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 75501b9402bb1c14fcfeb2fc6e61f055a2247493
ms.openlocfilehash: 93eced90155b9172595561bfc5b80c3c49ca11bc
ms.contentlocale: en-nz
ms.lasthandoff: 05/15/2018

---
# <a name="administration"></a>Administration
Central administration tasks are usually performed by one role in the company. The scope of these tasks can depend on the company's size and the administrator's job responsibilities. These tasks can include managing database synchronisation of job and email queues, setting up users, customising the user interface, and managing encryption keys.  

Entering the correct setup values from the start is important to the success of any new business software. [!INCLUDE[d365fin](includes/d365fin_md.md)] includes a number of setup guides that help you set up core data. For more information, see [Setting Up Business Central](setup.md).

Whether you use RapidStart Services to implement setup values or you manually enter them in the new company, you can support your setup decisions with some general recommendations for selected setup fields that are known to potentially cause the solution to be inefficient if defined incorrectly.  

A super user or an administrator can set up the Data Exchange Framework to enable users to export and import data in bank and payroll files, for example for various cash management processes.

> [!NOTE]
> You can set up a new company in [!INCLUDE[d365fin](includes/d365fin_md.md)] with RapidStart Services, which is a tool designed to shorten deployment times, improve quality of implementation, introduce a repeatable approach to implementations, and enhance productivity by automating and simplifying recurring tasks. For more information, see ## [Setting Up a Company With RapidStart Services](admin-set-up-a-company-with-rapidstart.md).

The following table describes a sequence of tasks, with links to the topics that describe them.   

|**To**|**See**|  
|------------|-------------|  
|Add users, manage permissions and access to data, assign roles.|[Understanding Profiles and Role Centres](admin-users-profiles-roles.md)|  
|Assign permissions to users, modify permission sets, and group users per permissions.|[Managing Users and Permissions](ui-how-users-permissions.md)|
|Classify data sensitivities for fields so that you can respond to requests from data subjects related to their personal data.|[Classifying Data Sensitivity](admin-classifying-data-sensitivity.md)|
|Respond to requests from data subjects related to their personal data.|[Responding to Requests About Personal Data](admin-responding-to-requests-about-personal-data.md)|
|Set up a new business unit using templates|[Creating New Companies](about-new-company.md)|
|Change which fields and actions are shown in the user interface to fit your company's business processes. |[Customising [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-customizing-overview.md) |
|Track all direct modifications that users make to data in the database to identify the origin of errors and data changes.|[Logging Changes](across-log-changes.md)|  
|Enter single or recurring requests to run reports or codeunits.|[Using Job Queues to Schedule Tasks](admin-job-queues-schedule-tasks.md)|  
|Manage, delete, or compress documents|[Deleting Documents](admin-manage-documents.md)|  
|Expose pages, codeunits, and queries as web services.|[Publishing a Web Service](across-how-publish-web-service.md)|
|As a part of creating Connect apps between [!INCLUDE[d365fin](includes/d365fin_md.md)] and 3rd-party solutions through REST APIs, define templates that are used to populate empty properties on an entity when you create a POST action through an API.|[Configuring API Templates](admin-configuring-api-template.md)|

## <a name="see-also"></a>See Also
[Business Functionality](across-business-functionality.md)  
[General Business Functionality](ui-across-business-areas.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  
[Getting Started](product-get-started.md)    

## [!INCLUDE[d365fin](includes/free_trial_md.md)]  
## [!INCLUDE[d365fin](includes/training_link_md.md)]

