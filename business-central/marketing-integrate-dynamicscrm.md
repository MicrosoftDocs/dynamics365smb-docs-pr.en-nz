---
title: Manage Customers Using Dynamics 365 for Sales| Microsoft Docs
description: You can use Dynamics 365 for Sales from inside Business Central  to map data and have seamless integration and synchronisation in the lead-to-cash process.
documentationcenter: 
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: integration, synchronize, map
ms.date: 07/02/2018
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 046a42582dc66368fded90a4bb45add71a95d979
ms.openlocfilehash: 33987f37c170af9982b86baf20f0c3e0682de2cd
ms.contentlocale: en-nz
ms.lasthandoff: 07/02/2018

---
# <a name="managing-customers-and-sales-created-in-dynamics-365-for-sales"></a>Managing Customers and Sales Created in Dynamics 365 for Sales
If you use Dynamics 365 for Sales (Sales) for customer engagement, you can use [!INCLUDE[d365fin](includes/d365fin_md.md)] for order processing and finances and have seamless integration in the lead-to-cash process.

When your application is set up to integrate with Sales, you have access to Sales data from [!INCLUDE[d365fin](includes/d365fin_md.md)] and the other way around in some cases. This integration enables you to work with and synchronise data types that are common to both services, such as customers, contacts, and sales information, and keep the data up to date in both locations.  

For example, the sales person in Sales can use the price lists from [!INCLUDE[d365fin](includes/d365fin_md.md)] when they create a sales order. When they add the item to the sales order line in Sales, they are also able to see the inventory level (availability) of the item from [!INCLUDE[d365fin](includes/d365fin_md.md)].

Conversely, order processors in [!INCLUDE[d365fin](includes/d365fin_md.md)] can handle the special characteristics of sales orders transferred automatically or manually from Sales, such as automatically create and post valid sales order lines for items or resources that were entered in Sales as write-in products. For more information, see the "Handling Special Sales Order Data" section.

> [!IMPORTANT]  
> [!INCLUDE[d365fin](includes/d365fin_md.md)] integrates with Dynamics 365 for Sales only. Other applications or solutions within Dynamics 365 that change the standard workflow or data model in Sales, for example Project Service Automation, may break the integration between [!INCLUDE[d365fin](includes/d365fin_md.md)] and Sales.

## <a name="standard-sales-entity-mapping-for-synchronization"></a>Standard Sales Entity Mapping for Synchronisation
Sales entities, such as accounts, are integrated with equivalent [!INCLUDE[d365fin](includes/d365fin_md.md)] record types, such as customers. To work with Sales data, you set up mappings, called couplings, between [!INCLUDE[d365fin](includes/d365fin_md.md)] records and Sales entity records. For example, you set up a coupling between a specific customer in [!INCLUDE[d365fin](includes/d365fin_md.md)]  and a corresponding account in Sales.

The following table lists the [!INCLUDE[d365fin](includes/d365fin_md.md)] record types (tables) and corresponding Sales entities that can be synchronised out-of-the-box.

|[!INCLUDE[d365fin](includes/d365fin_md.md)]|Sales|Synchronisation Direction|Default Filter|
|-------------------------------------------|-----|-------------------------|--------------|
|Salesperson/Purchaser|User|Sales -> Business Central|Sales contact filter: **Status** is **No**, **User Licensed** is **Yes**, Integration user mode is **No**|
|Customer|Account|Business Central -> Sales and Sales -> Business Central|Sales account filter: **Relationship Type** is **Customer** and **Status** is **Active**.|
|Contact|Contact|Business Central -> Sales and Sales -> Business Central|Business Central contact filter: **Type** is **Person** and the contact is assigned to a company. Sales contact filter: The contact is assigned to a company and the parent customer type is **Account**|
|Currency|Transaction Currency|Business Central -> Sales| |
|Unit of Measure|Unit Group|Business Central -> Sales| |
|Item|Product|Business Central -> Sales and Sales -> Business Central|Sales contact filter: **Product Type** is **Sales Inventory**|
|Resource|Product|Business Central -> Sales and Sales -> Business Central|Sales contact filter: **Product Type** is **Services**|
|Customer Price Group|Price List|Business Central -> Sales| |
|Sales Price|Product Price List|Business Central -> Sales|Business Central contact filter: **Sales Code** is not blank, **Sales Type** is **Customer Price Group**|
|Opportunity|Opportunity|Business Central -> Sales and Sales -> Business Central| |
|Sales Invoice Header|Invoice|Business Central -> Sales| |
|Sales Invoice Line|Invoice Product|Business Central -> Sales| |

The Sales entities and [!INCLUDE[d365fin](includes/d365fin_md.md)] tables that are synchronised are defined by table mapping entries in table 5335, **Integration Table Mapping**. You can view the mappings and set up filters from page 5335, **Integration Table Mappings**. The mapping between the fields in [!INCLUDE[d365fin](includes/d365fin_md.md)] records and the fields in Sales entities are defined by field mapping entries in table 5336, **Integration Field Mapping**, and with additional mapping logic.

### <a name="field-mapping-for-the-sales-account-option"></a>Field Mapping for the Sales Account Option
Three tables in [!INCLUDE[d365fin](includes/d365fin_md.md)] are mapped to the option fields of the **Account** entity.   

The records in the table that are not linked to the options that exist in Sales will be skipped during synchronisation. This means that the **Option** field will be blank in Sales.

The following table shows mappings from Business Central tables for the **Option** field in the **Account** entity.

|Table|Option Field in the Account Entity in Sales|
|----------------------|-------------------------------------------|
|Payment Terms|Payment Terms|
|Shipment Method|Address 1: Freight Terms|
|Shipping Agent|Address 1: Shipping Method|

### <a name="synchronization-rules"></a>Synchronisation Rules
The following table describes rules that control the synchronisation between Business Central tables and Sales entities.

> [!NOTE]  
> Modifications to data in Sales that are performed by the Sales connection account are ignored. The changes will not be synchronised. Therefore, it is recommended that you do not modify data by using the Sales connection account.

|Table|Rule|
|-----|----|
|Customers|Before a customer can be synchronised to an account, the salesperson that is assigned to the customer must be coupled to a user in Sales. Therefore, when you run the CUSTOMERS - Dynamics 365 for Sales synchronisation job and you set it up to create new records, make sure that you synchronise salespeople with Sales users before you synchronise customers with Sales accounts. <br /> <br />The CUSTOMERS - Dynamics 365 for Sales synchronisation job only synchronises Sales accounts that have the relationship type Customer.|
|Contacts|Only contacts in Sales that are associated with an account will be created in Business Central. The Salesperson Code value defines the owner of the coupled entity in Sales.|
|Currencies|Currencies are coupled to transaction currencies in Sales based on ISO codes. Only currencies that have a standard ISO code will be coupled and synchronised with transaction currencies.|
|Units of Measure|Units of measure are synchronised with unit groups in Sales. There can only be one unit of measure defined in the unit group.|
|Items|When synchronising items with Sales products, Business Central automatically creates a price list in Sales. To avoid synchronisation errors, you should not modify this price list manually.|
|Salespersons|Salespersons are coupled to system users in Sales. The user must be enabled and licensed and must not be the Integration user. Note, that this is the first table that must be synchronised because it is used in customers, contacts, opportunities, and sales invoices.|
|Resources|Resources are synchronised with Sales products that have product type Service.|
|Customer Price Groups|Customer price groups are synchronised with Sales price lists.|
|Sales Prices|Sales prices that have sales type Customer Price Group and have a sales code defined are synchronised with Sales price list lines|
|Opportunities|Opportunities are synchronised with Sales opportunities. The Salesperson Code value defines the owner of the coupled entity in Sales.|
|Posted Sales Invoices|Posted sales invoices are synchronised with sales invoices. Before an invoice can be synchronised, it is better to synchronise all other entities that can participate in the invoice, from salespersons to price lists. The Salesperson Code value in the invoice header defines the owner of the coupled entity in Sales.|

## <a name="setting-up-the-connection"></a>Setting Up the Connection
From Home, you can access the **Microsoft Dynamics 365 Connection Setup** assisted setup guide that helps you set up the connection. Once that is done, you will have a seamless coupling of Sales records with [!INCLUDE[d365fin](includes/d365fin_md.md)] records.  

> [!NOTE]  
>   The following explains the assisted setup, but you can perform the same tasks manually in the **Sales Connection Setup** window.

In the assisted setup guide, you can choose which data to synchronise between the two services. You can also specify that you want to import your existing Sales solution. In that case, you must specify an administrative user account.

### <a name="setting-up-the-user-account-for-importing-the-solution"></a>Setting Up the User Account for Importing the Solution
To import an existing Sales solution, the setup guide uses an administrative account. This account must be a valid user in Sales with the following security roles:

* System Administrator  
* Solution Customizer  

For more information, see [Create users in Microsoft Dynamics 365 (online) and assign  security roles](/dynamics365/customer-engagement/admin/create-users-assign-online-security-roles) and [Manage Users and Permissions](ui-how-users-permissions.md).  

This account is only used during the setup. Once the solution is imported into [!INCLUDE[d365fin](includes/d365fin_md.md)], the account is no longer needed.

### <a name="setting-up-the-user-account-for-synchronization"></a>Setting Up the User Account for Synchronisation
The integration relies on a shared user account. So in your Office 365 subscription, you must create a dedicated user that will be used for synchronisation between the two services. This account must already be a valid user in Sales, but you do not have to assign security roles to the account because the setup guide will do that for you. You must specify this user account one or more times in the setup guide, depending how much synchronisation you want to enable. For more information, see [Create users in Microsoft Dynamics 365 (online) and assign security roles](/dynamics365/customer-engagement/admin/create-users-assign-online-security-roles).

If you choose to enable *item availability*, the integration user account must have a web services access key. This is a two-step thing in the [!INCLUDE[d365fin](includes/d365fin_md.md)] page for that user account, you must choose the **Change Web Service Key** button; and in the Sales Connection setup guide, you must specify that user as the OData web service user.

If you choose to enable *sales order integration*, you must specify a user that can handle this synchronization - the integration user or another user account.

### <a name="coupling-records"></a>Coupling Records
In the assisted setup guide, you can choose to synchronise between the two services. But later, you can also set up synchronisation of specific types of data. This is referred to as *coupling*, and this section provides recommendations for what you must take into consideration.

For example, if you want to see Sales accounts as customers in [!INCLUDE[d365fin](includes/d365fin_md.md)], you must couple the two types of records. It is not very complicated - you open the **Customer List** window in [!INCLUDE[d365fin](includes/d365fin_md.md)], and there is an action in the ribbon to couple this data with Sales. Then you specify which [!INCLUDE[d365fin](includes/d365fin_md.md)] customers match which accounts in Sales.

In certain areas, the functionality relies on you couple certain sets of data before other sets of data as shown in the following list:

* Customers and accounts  
  * Couple salespeople with Sales users first  
* Items and resources  
  * Couple units of measure with Sales unit groups first  
* Items and resource prices  
  * Couple customer price groups with Sales prices first  

> [!NOTE]  
>   If you are using prices in foreign currencies, make sure that you couple currencies to Sales transaction currencies.

In Sales, sales orders depends on additional information like customers, units of measure, currencies, customer price groups, items and/or resources. In order for the integration with  sales orders to work seamlessly, you must couple customers, units of measure, currencies, customer price groups, items and/or resources first.

### <a name="synchronizing-records-fully"></a>Synchronising Records Fully
At the end of the assisted setup guide, you can choose the **Run Full Synchronisation** action to start synchronising all [!INCLUDE[d365fin](includes/d365fin_md.md)] records with all related records in the connected Sales solution. In the **CRM Full Synch. Review** window, you choose the **Start** action. The synchronisation then begins to execute jobs according to dependencies. For example, currency records are synchronised before customer records. The full synchronization may take a long time and will therefore run in the background so that you can continue to work in [!INCLUDE[d365fin](includes/d365fin_md.md)].

To check the progress of individual jobs in a full synchronization, drill down on the **Job Queue Entry Status**, **To Int. Table Job Status**, or **From Int. Table Job Status** field in the **CRM Full Synch. Review** window.

From the **Microsoft Dynamics 365 Connection Setup** window, you can get details about full synchronisation at any time. From here, you can also open the **Integration Table Mappings** window to see details about the tables in [!INCLUDE[d365fin](includes/d365fin_md.md)] and in the Sales solution that must be synchronised.

## <a name="handling-special-sales-order-data"></a>Handling Special Sales Order Data
Sales orders in Sales will be transferred to [!INCLUDE[d365fin](includes/d365fin_md.md)] automatically if you select the **Automatically Create Sales Orders** check box in the **Microsoft Dynamics 365 Connection Setup** window. On such sales orders, the **Name** field on the original order is transferred and mapped to the **External Document Number** field on the sales order in [!INCLUDE[d365fin](includes/d365fin_md.md)].

This can also work if the original sales order contains write-in products, meaning items or resources that are not registered in either product. In that case, you must fill in the **Write-in Product Type** and **Write-in Product No.** fields in the **Sales & Receivables Setup** window, so that such non-registered product sales are mapped to a specified item/resource number for financial analysis.

If the item description on the original sales order is very long, then an additional sales order line of type Comment is created to hold the full text on the sales order in [!INCLUDE[d365fin](includes/d365fin_md.md)].

## <a name="see-also"></a>See Also
[Relationship Management](marketing-relationship-management.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  
[Changing Which Features are Displayed](ui-experiences.md)  
[Manage Users and Permissions](ui-how-users-permissions.md)    
[Onboard your organisation and users to Dynamics 365 (online)](/dynamics365/customer-engagement/admin/onboard-your-organization-and-users-to-dynamics-365-online)  

## [!INCLUDE[d365fin](includes/free_trial_md.md)]  

