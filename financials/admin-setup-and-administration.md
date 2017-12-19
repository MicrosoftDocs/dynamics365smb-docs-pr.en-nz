---
title: Administrative tasks in Dynamics 365 | Microsoft Docs
description: Some tasks in Dynamics 365 requires central administration and setup. See what they are and learn what to do.
author: edupont04
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/01/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: a49e50213f808fb72b43dfa22a34833b306ef12d
ms.openlocfilehash: c7e5efe85dddcc7db84b05879f0c71990167c775
ms.contentlocale: en-nz
ms.lasthandoff: 12/14/2017

---
# <a name="setup-and-administration-in-dynamics-365-for-financials"></a>Setup and Administration in Dynamics 365 for Financials
Central administration tasks are usually performed by one role in the company. The scope of these tasks can depend on the company's size and the administrator's job responsibilities. These tasks can include managing database synchronisation of job and email queues, setting up users, customising the user interface, and managing encryption keys.  

Entering the correct setup values from the start is important to the success of any new business software. [!INCLUDE[d365fin](includes/d365fin_md.md)] includes a number of setup guides that help you set up core data. For more information, see [Setting Up Dynamics 365 for Financials](setup.md).

<!--Whether you use [!INCLUDE[rim](../../includes/rim_md.md)] to implement setup values or you manually enter them in the new company, you can support your setup decisions with some general recommendations for selected setup fields that are known to potentially cause the solution to be inefficient if defined incorrectly.-->  

A super user or an administrator can set up the Data Exchange Framework to enable users to export and import data in bank and payroll files, for example for various cash management processes.  

The following table describes a sequence of tasks, with links to the topics that describe them.   

|**To**|**See**|  
|------------|-------------|  
|Add users, manage permissions and access to data, assign roles.|[Users, Profiles, and Role Centres in Dynamics 365 for Financials](admin-users-profiles-roles.md)|  
|Track all direct modifications that users make to data in the database to identify the origin of errors and data changes.|[Logging Changes in Dynamics 365 for Financials](across-log-changes.md)|  
|Support your setup decisions with recommendations for selected fields that are known to potentially cause the solution to be inefficient if set up incorrectly|[Set Up Complex Application Areas Using Best Practices](set-up-complex-application-areas-using-best-practices.md)|  
|Expose pages, codeunits, and queries as web services.|[How to: Publish a Web Service](across-how-publish-web-service.md)|  
|Set up an SMTP server to enable e-mail communication in and out of Dynamics 365 for Financials| [How to: Set Up Email Manually or Using the Assisted Setup](madeira-how-setup-email.md)|  
|Enter single or recurring requests to run reports or codeunits.|[Use Job Queues to Schedule Tasks](admin-job-queues-schedule-tasks.md)|  
|Manage, delete, or compress documents|[Manage Documents](admin-manage-documents.md)|  
|Set up a new business unit using templates|[Creating New Companies in [!INCLUDE[d365fin](includes/d365fin_md.md)]](about-new-company.md)|  

## <a name="see-also"></a>See Also
[Business Functionality](madeira-business-functionality.md)  
[General Business Functionality](ui-across-business-areas.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  
[Welcome to [!INCLUDE[d365fin](includes/d365fin_md.md)]](index.md)  

