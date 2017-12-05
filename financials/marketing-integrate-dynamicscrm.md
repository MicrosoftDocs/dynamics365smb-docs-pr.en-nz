---
title: Manage Customers Using Dynamics 365 for Sales| Microsoft Docs
description: You can use Dynamics 365 for Sales from inside Dynamics 365 Business edition to map data and have seamless integration and synchronisation in the lead-to-cash process.
documentationcenter: 
author: edupont04
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: integration, synchronize, map
ms.date: 06/06/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: ba26b354d235981bd7291f9ac6402779f554ac7a
ms.openlocfilehash: fde1a04c4e6f56fb425f6aef85d21b029a76fe0c
ms.contentlocale: en-nz
ms.lasthandoff: 11/10/2017

---
# <a name="managing-customers-and-sales-created-in-dynamics-365-for-sales"></a>Managing Customers and Sales Created in Dynamics 365 for Sales
If you use Dynamics 365 for Sales for customer engagement, you can use [!INCLUDE[d365fin](includes/d365fin_md.md)] for order processing and finances and have seamless integration in the lead-to-cash process.

When your application is set up to integrate with Dynamics 365 for Sales, you have access to Sales data from [!INCLUDE[d365fin](includes/d365fin_md.md)] and the other way around in some cases. This integration enables you to work with and synchronise data types that are common to both services, such as customers, contacts, and sales information, and keep the data up to date in both locations.  

For example, the sales person in Dynamics 365 for Sales can use the price lists from [!INCLUDE[d365fin](includes/d365fin_md.md)] when they create a sales order. When they add the item to the sales order line in Dynamics 365 for Sales, they are also able to see the inventory level (availability) of the item from [!INCLUDE[d365fin](includes/d365fin_md.md)].

> [!NOTE]  
>   This functionality requires that your experience is set to **Suite**. For more information, see [Customizing Your [!INCLUDE[d365fin](includes/d365fin_md.md)] Experience](ui-experiences.md).  

## <a name="setting-up-the-connection"></a>Setting up the connection
From Home, you can access the **Dynamics 365 for Sales Connection Setup** assisted setup guide that helps you set up the connection. Once that is done, you will have a seamless coupling of Dynamics 365 for Sales records with [!INCLUDE[d365fin](includes/d365fin_md.md)] records.  

> [!NOTE]  
>   The following explains the assisted setup, but you can perform the same tasks manually in the **Dynamics 365 for Sales Connection Setup** window.

In the assisted setup guide, you can choose which data to synchronise between the two services. You can also specify that you want to import your existing Dynamics 365 for Sales solution. In that case, you must specify an administrative user account.

### <a name="setting-up-the-user-account-for-importing-the-solution"></a>Setting up the user account for importing the solution
To import an existing Dynamics 365 for Sales solution, the setup guide uses an administrative account. This account must be a valid user in Dynamics 365 for Sales with the following security roles:

* System Administrator  
* Solution Customizer  

For more information, see [Create users and assign Microsoft Dynamics 365 (online) security roles](https://technet.microsoft.com/library/jj191623.aspx) on techNet and [How to: Manage Users and Permissions](ui-how-users-permissions.md).  

This account is only used during the setup. Once the solution is imported into [!INCLUDE[d365fin](includes/d365fin_md.md)], the account is no longer needed.

### <a name="setting-up-the-user-account-for-synchronization"></a>Setting up the user account for synchronisation
The integration relies on a shared user account. So in your Office 365 subscription, you must create a dedicated user that will be used for synchronisation between the two services. This account must already be a valid user in Dynamics 365 for Sales, but you do not have to assign security roles to the account because the setup guide will do that for you. You must specify this user account one or more times in the setup guide, depending how much synchronisation you want to enable. For more information, see [Create users and assign Microsoft Dynamics 365 (online) security roles](https://technet.microsoft.com/library/jj191623.aspx) on techNet.

If you choose to enable *item availability*, the integration user account must have a web services access key. This is a two-step thing in the [!INCLUDE[d365fin](includes/d365fin_md.md)] page for that user account, you must choose the **Change Web Service Key** button; and in the Dynamics 365 Connection setup guide, you must specify that user as the OData web service user.

If you choose to enable *sales order integration*, you must specify a user that can handle this synchronization - the integration user or another user account.

### <a name="coupling-records"></a>Coupling records
In the assisted setup guide, you can choose to synchronise between the two services. But later, you can also set up synchronisation of specific types of data. This is referred to as *coupling*, and this section provides recommendations for what you must take into consideration.

For example, if you want to see Dynamics 365 for Sales accounts as customers in [!INCLUDE[d365fin](includes/d365fin_md.md)], you must couple the two types of records. It is not very complicated - you open the **Customer List** window in [!INCLUDE[d365fin](includes/d365fin_md.md)], and there is an action in the ribbon to couple this data with Dynamics 365 for Sales. Then you specify which [!INCLUDE[d365fin](includes/d365fin_md.md)] customers match which accounts in Dynamics 365 for Sales.

In certain areas, the functionality relies on you couple certain sets of data before other sets of data as shown in the following list:

* Customers and accounts  
  * Couple salespeople with Dynamics 365 for Sales users first  
* Items and resources  
  * Couple units of measure with Dynamics 365 for Sales unit groups first  
* Items and resource prices  
  * Couple customer price groups with Dynamics 365 for Sales prices first  

> [!NOTE]  
>   If you are using prices in foreign currencies, make sure that you couple currencies to Dynamics 365 for Sales transaction currencies.

Dynamics 365 for Sales sales orders depends on additional information like customers, units of measure, currencies, customer price groups, items and/or resources. In order for Dynamics 365 for Sales sales orders to work seamlessly, you must couple customers, units of measure, currencies, customer price groups, items and/or resources first.

### <a name="synchronizing-records-fully"></a>Synchronising records fully
At the end of the assisted setup guide, you can choose the **Run Full Synchronisation** action to start synchronising all [!INCLUDE[d365fin](includes/d365fin_md.md)] records with all related records in the connected Dynamics 365 for Sales solution. In the **CRM Full Synch. Review** window, you choose the **Start** action. The synchronisation then begins to execute jobs according to dependencies. For example, currency records are synchronised before customer records. The full synchronization may take a long time and will therefore run in the background so that you can continue to work in [!INCLUDE[d365fin](includes/d365fin_md.md)].

To check the progress of individual jobs in a full synchronization, drill down on the **Job Queue Entry Status**, **To Int. Table Job Status**, or **From Int. Table Job Status** field in the **CRM Full Synch. Review** window.

From the **Dynamics 365 Connection Setup** window, you can get details about full synchronisation at any time. From here, you can also open the **Integration Table Mappings** window to see details about the tables in Dynamics 365 Business edition and in the Dynamics 365 for Sales solution that must be synchronised.

## <a name="see-also"></a>See Also
[Relationship Management](marketing-relationship-management.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  
[Customizing Your [!INCLUDE[d365fin](includes/d365fin_md.md)] Experience](ui-experiences.md)  
[How to: Manage Users and Permissions](ui-how-users-permissions.md)    
[Onboard your organization and users to Dynamics 365 (online)](https://www.microsoft.com/en-US/Dynamics/crm-customer-center/onboard-your-organization-and-users-to-dynamics-365-online.aspx)  

## [!INCLUDE[d365fin](includes/free_trial_md.md)]

