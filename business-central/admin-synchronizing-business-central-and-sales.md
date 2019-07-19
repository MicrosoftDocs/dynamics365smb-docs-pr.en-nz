---
title: Synchronisation and Data Integration | Microsoft Docs
description: The synchronisation copies data between Dynamics 365 for Sales entries and Business Central records, and keeps the data in both systems up-to-date.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: sales, crm, integration, sync, synchronize
ms.date: 04/01/2019
ms.author: bholtorf
ms.openlocfilehash: b5a3b83d21390711ff0517df67bf9912ece57f6b
ms.sourcegitcommit: f2e3b571eab6e01d9f5aa8ef47056b6bd313dcbd
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 06/13/2019
ms.locfileid: "1629635"
---
# <a name="synchronizing-data-in-business-central-and-dynamics-365-for-sales"></a>Synchronising Data in Business Central and Dynamics 365 for Sales
When you integrate [!INCLUDE[crm_md](includes/crm_md.md)] with [!INCLUDE[d365fin](includes/d365fin_md.md)], you can decide whether to synchronise data in selected fields of [!INCLUDE[d365fin](includes/d365fin_md.md)] records (such as customers, contacts, and sales people) with equivalent records in [!INCLUDE[d365fin](includes/d365fin_md.md)] (such as accounts, contacts, and users). Depending on the type of record, you can synchronise data from [!INCLUDE[crm_md](includes/crm_md.md)] to [!INCLUDE[d365fin](includes/d365fin_md.md)], or vice versa. For more information, see [Integrating with Dynamics 365 for Sales](admin-prepare-dynamics-365-for-sales-for-integration.md).  

Synchronisation uses the following elements:

* Integration table mappings
* Integration field mappings
* Synchronisation rules
* Coupled records

When synchronisation is set up you can couple [!INCLUDE[d365fin](includes/d365fin_md.md)] records to [!INCLUDE[crm_md](includes/crm_md.md)] records to synchronise their data. You can start a synchronisation manually, or based on a schedule. The following table provides on overview of the ways you can synchronise records.  

|  Type  |  Method  |  See  |  
|--------|----------|-------|  
|Manual synchronisation|Synchronise on a record-by-record basis.<br /><br /> You can synchronise individual records in [!INCLUDE[d365fin](includes/d365fin_md.md)], such as a customer, with a corresponding [!INCLUDE[crm_md](includes/crm_md.md)] record, such as an account. This is typically how users will work with [!INCLUDE[crm_md](includes/crm_md.md)] data in [!INCLUDE[d365fin](includes/d365fin_md.md)].|[Couple and Synchronise Records Manually](admin-manual-synchronization-of-table-mappings.md#synchronize-individual-table-mappings)|  
|  |Synchronise on a table mapping basis.<br /><br /> You can synchronise all records in a [!INCLUDE[d365fin](includes/d365fin_md.md)] table with an entity [!INCLUDE[crm_md](includes/crm_md.md)] entity.|[Synchronise Individual Table Mappings](admin-manual-synchronization-of-table-mappings.md#synchronize-individual-table-mappings)|  
||Synchronise all modified records for all table mappings.<br /><br /> You can synchronise all of the records that have been modified in [!INCLUDE[d365fin](includes/d365fin_md.md)] tables since the last synchronisation.|[Synchronising All Modified Records](admin-manual-synchronization-of-table-mappings.md#synchronizing-all-modified-records)|
||Full synchronisation of all data for all table mappings.<br /><br /> You can synchronise all of the data in [!INCLUDE[d365fin](includes/d365fin_md.md)] tables and [!INCLUDE[crm_md](includes/crm_md.md)] entities that are mapped, and create new records in the destination solution for uncoupled records in the source solution.<br /><br /> Full synchronisation synchronises all data and ignores coupling. Typically, you do a full synchronisation when you set up the integration and only one of solutions contains data. A full synchronisation can also be useful in a demonstration environment.|[Run a Full Synchronisation](admin-manual-synchronization-of-table-mappings.md#run-a-full-synchronization)|  
|Scheduled synchronisation|Synchronise all changes to data for all table mappings.<br /><br /> You can synchronise [!INCLUDE[d365fin](includes/d365fin_md.md)] with [!INCLUDE[crm_md](includes/crm_md.md)] on scheduled intervals by setting up jobs in the job queue.|[Schedule a Synchronisation](admin-scheduled-synchronization-using-the-synchronization-job-queue-entries.md)|  

## <a name="standard-sales-entity-mapping-for-synchronization"></a>Standard Sales Entity Mapping for Synchronisation
Entities in [!INCLUDE[crm_md](includes/crm_md.md)], such as accounts, are integrated with equivalent types of entities in [!INCLUDE[d365fin](includes/d365fin_md.md)],such as customers. To work with [!INCLUDE[crm_md](includes/crm_md.md)] data you set up links, called couplings, between entities in [!INCLUDE[d365fin](includes/d365fin_md.md)] and [!INCLUDE[crm_md](includes/crm_md.md)].

The following table lists the standard mapping between entities in [!INCLUDE[d365fin](includes/d365fin_md.md)] and [!INCLUDE[crm_md](includes/crm_md.md)] that [!INCLUDE[d365fin](includes/d365fin_md.md)] provides.

|[!INCLUDE[d365fin](includes/d365fin_md.md)]|[!INCLUDE[crm_md](includes/crm_md.md)]|Synchronisation Direction|Default Filter|
|-------------------------------------------|-----|-------------------------|--------------|
|Salesperson/Purchaser|User|[!INCLUDE[crm_md](includes/crm_md.md)] -> [!INCLUDE[d365fin](includes/d365fin_md.md)]|Sales contact filter: **Status** is **No**, **User Licensed** is **Yes**, Integration user mode is **No**|
|Customer|Account|[!INCLUDE[d365fin](includes/d365fin_md.md)] -> [!INCLUDE[crm_md](includes/crm_md.md)] and [!INCLUDE[crm_md](includes/crm_md.md)] -> [!INCLUDE[d365fin](includes/d365fin_md.md)]|Sales account filter: **Relationship Type** is **Customer** and **Status** is **Active**.|
|Contact|Contact|[!INCLUDE[d365fin](includes/d365fin_md.md)] -> [!INCLUDE[crm_md](includes/crm_md.md)] and [!INCLUDE[crm_md](includes/crm_md.md)] -> [!INCLUDE[d365fin](includes/d365fin_md.md)]|[!INCLUDE[d365fin](includes/d365fin_md.md)] contact filter: **Type** is **Person** and the contact is assigned to a company. Sales contact filter: The contact is assigned to a company and the parent customer type is **Account**|
|Currency|Transaction Currency|[!INCLUDE[d365fin](includes/d365fin_md.md)] -> [!INCLUDE[crm_md](includes/crm_md.md)]| |
|Unit of Measure|Unit Group|[!INCLUDE[d365fin](includes/d365fin_md.md)] -> [!INCLUDE[crm_md](includes/crm_md.md)]| |
|Item|Product|[!INCLUDE[d365fin](includes/d365fin_md.md)] -> [!INCLUDE[crm_md](includes/crm_md.md)] and [!INCLUDE[crm_md](includes/crm_md.md)] -> [!INCLUDE[d365fin](includes/d365fin_md.md)]|Sales contact filter: **Product Type** is **Sales Inventory**|
|Resource|Product|[!INCLUDE[d365fin](includes/d365fin_md.md)] -> [!INCLUDE[crm_md](includes/crm_md.md)] and [!INCLUDE[crm_md](includes/crm_md.md)] -> [!INCLUDE[d365fin](includes/d365fin_md.md)]|Sales contact filter: **Product Type** is **Services**|
|Customer Price Group|Price List|[!INCLUDE[d365fin](includes/d365fin_md.md)] -> [!INCLUDE[crm_md](includes/crm_md.md)]| |
|Sales Price|Product Price List|[!INCLUDE[d365fin](includes/d365fin_md.md)] -> [!INCLUDE[crm_md](includes/crm_md.md)]|[!INCLUDE[d365fin](includes/d365fin_md.md)] contact filter: **Sales Code** is not blank, **Sales Type** is **Customer Price Group**|
|Opportunity|Opportunity|[!INCLUDE[d365fin](includes/d365fin_md.md)] -> [!INCLUDE[crm_md](includes/crm_md.md)] and [!INCLUDE[crm_md](includes/crm_md.md)] -> [!INCLUDE[d365fin](includes/d365fin_md.md)]| |
|Sales Invoice Header|Invoice|[!INCLUDE[d365fin](includes/d365fin_md.md)] -> [!INCLUDE[crm_md](includes/crm_md.md)]| |
|Sales Invoice Line|Invoice Product|[!INCLUDE[d365fin](includes/d365fin_md.md)] -> [!INCLUDE[crm_md](includes/crm_md.md)]| |
|Sales Order Header|Sales Order|[!INCLUDE[d365fin](includes/d365fin_md.md)] -> [!INCLUDE[crm_md](includes/crm_md.md)]|[!INCLUDE[d365fin](includes/d365fin_md.md)] Sales Header filter: **Document Type** is Order, **Status** is Released|
|Sales Order Notes|Sales Order Notes|[!INCLUDE[d365fin](includes/d365fin_md.md)] -> [!INCLUDE[crm_md](includes/crm_md.md)] and [!INCLUDE[crm_md](includes/crm_md.md)] -> [!INCLUDE[d365fin](includes/d365fin_md.md)]| |

### <a name="tip-for-admins-viewing-entity-mappings"></a>Tip for Admins: Viewing Entity Mappings
You can view the mapping between the entities in [!INCLUDE[crm_md](includes/crm_md.md)] and the tables in [!INCLUDE[d365fin](includes/d365fin_md.md)] on the **Integration Table Mappings** page, where you can also apply filters. You define the mapping between the fields in [!INCLUDE[d365fin](includes/d365fin_md.md)] tables and the fields in [!INCLUDE[crm_md](includes/crm_md.md)] entities on the **Integration Field Mapping** page, where you can add additional mapping logic. For example, this can be useful if you need to troubleshoot synchronisation.

### <a name="tip-for-developers-mapping-fields-in-business-central-to-the-option-sets-in-sales"></a>Tip for Developers: Mapping Fields in Business Central to the Option Sets in Sales
If you are a developer and you want to add options to the option sets in [!INCLUDE[crm_md](includes/crm_md.md)], you need to know this. There are three tables in [!INCLUDE[d365fin](includes/d365fin_md.md)] that are mapped to the option fields of the **Account** entity in [!INCLUDE[crm_md](includes/crm_md.md)]. Records in the tables that are not linked to options in [!INCLUDE[crm_md](includes/crm_md.md)] will not be synchronised. This means that the **Option** field will be blank in [!INCLUDE[crm_md](includes/crm_md.md)].

The following table shows mappings from [!INCLUDE[d365fin](includes/d365fin_md.md)] tables for the **Option** field in the **Account** entity in [!INCLUDE[crm_md](includes/crm_md.md)].

|Table|Option Field in the Account Entity|
|----------------------|-------------------------------------------|
|Payment Terms|Payment Terms|
|Shipment Method|Address 1: Freight Terms|
|Shipping Agent|Address 1: Shipping Method|

### <a name="synchronization-rules"></a>Synchronisation Rules
The following table describes rules that control the synchronisation between the apps.

> [!NOTE]  
> Changes to data in [!INCLUDE[crm_md](includes/crm_md.md)] that were made by the [!INCLUDE[crm_md](includes/crm_md.md)] connection user account are not synchronised. Therefore, we recommended that you do not change data while using that account. For more information, see [Setting Up User Accounts for Integrating with Dynamics 365 for Sales](admin-setting-up-integration-with-dynamics-sales.md).

|Table|Rule|
|-----|----|
|Customers|Before a customer can be synchronised to an account, the salesperson that is assigned to the customer must be coupled to a user in [!INCLUDE[crm_md](includes/crm_md.md)]. Therefore, when you run the CUSTOMERS - Dynamics 365 for Sales synchronisation job and you set it up to create new records, make sure that you synchronise salespeople with [!INCLUDE[crm_md](includes/crm_md.md)] users before you synchronise customers with accounts in [!INCLUDE[crm_md](includes/crm_md.md)]. <br /> <br />The CUSTOMERS - Dynamics 365 for Sales synchronisation job only synchronises Sales accounts that have the relationship type Customer.|
|Contacts|Only contacts in [!INCLUDE[crm_md](includes/crm_md.md)] that are associated with an account will be created in [!INCLUDE[d365fin](includes/d365fin_md.md)]. The Salesperson Code value defines the owner of the coupled entity in [!INCLUDE[crm_md](includes/crm_md.md)].|
|Currencies|Currencies are coupled to transaction currencies in [!INCLUDE[crm_md](includes/crm_md.md)] based on ISO codes. Only currencies that have a standard ISO code will be coupled and synchronised with transaction currencies.|
|Units of Measure|Units of measure are synchronised with unit groups in [!INCLUDE[crm_md](includes/crm_md.md)]. There can only be one unit of measure defined in the unit group.|
|Items|When synchronising items with [!INCLUDE[crm_md](includes/crm_md.md)] products, [!INCLUDE[d365fin](includes/d365fin_md.md)] automatically creates a price list in [!INCLUDE[crm_md](includes/crm_md.md)]. To avoid synchronisation errors, you should not modify this price list manually.|
|Salespersons|Salespersons are coupled to system users in [!INCLUDE[crm_md](includes/crm_md.md)]. The user must be enabled and licensed and must not be the Integration user. Note, that this is the first table that must be synchronised because it is used in customers, contacts, opportunities, and sales invoices.|
|Resources|Resources are synchronised with [!INCLUDE[crm_md](includes/crm_md.md)] products that have product type Service.|
|Customer Price Groups|Customer price groups are synchronised with Sales price lists.|
|Sales Prices|Sales prices that have sales type Customer Price Group and have a sales code defined are synchronised with [!INCLUDE[crm_md](includes/crm_md.md)] price list lines|
|Opportunities|Opportunities are synchronised with [!INCLUDE[crm_md](includes/crm_md.md)] opportunities. The Salesperson Code value defines the owner of the coupled entity in [!INCLUDE[crm_md](includes/crm_md.md)].|
|Posted Sales Invoices|Posted sales invoices are synchronised with sales invoices. Before an invoice can be synchronised, it is better to synchronise all other entities that can participate in the invoice, from salespersons to price lists. The Salesperson Code value in the invoice header defines the owner of the coupled entity in Sales.|
|Sales Orders|Released sales order (headers) are synchronised with sales order. Before an order can be synchronised, it is better to synchronise all other entities that can participate in the order, from salespersons to price lists. The Salesperson Code value in the order header defines the owner of the coupled entity in Sales.|  

## <a name="see-also"></a>See Also  
[Couple and Synchronise Records Manually](admin-how-to-couple-and-synchronize-records-manually.md)   
[Schedule a Synchronisation](admin-scheduled-synchronization-using-the-synchronization-job-queue-entries.md)   
[Integrating with Dynamics 365 for Sales](admin-prepare-dynamics-365-for-sales-for-integration.md)
