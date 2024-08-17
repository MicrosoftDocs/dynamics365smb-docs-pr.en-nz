---
title: Synchronisation and data integration
description: 'The synchronisation copies data between Microsoft Dataverse tables and Business Central records, and keeps the data in both systems up-to-date.'
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bholtorf
ms.topic: conceptual
ms.date: 05/07/2024
ms.custom: bap-template
ms.search.keywords: 'Dataverse, integration, sync, synchronize, mapping'
ms.saerch.form: 5372_Primary
ms.service: dynamics-365-business-central
---

# <a name="synchronizing-data-in-business-central-with-microsoft-dataverse"></a>Synchronising data in Business Central with Microsoft Dataverse

When you integrate [!INCLUDE[prod_short](includes/cds_long_md.md)] with [!INCLUDE[prod_short](includes/prod_short.md)], you can decide whether to synchronise data in selected fields of [!INCLUDE[prod_short](includes/prod_short.md)] (such as customers, contacts, and sales people) with equivalent rows in [!INCLUDE[prod_short](includes/cds_long_md.md)] (such as accounts, contacts, and users). Depending on the type of row, you can synchronise data from [!INCLUDE[prod_short](includes/cds_long_md.md)] to [!INCLUDE[prod_short](includes/prod_short.md)], or vice versa. For more information, see [Integrating with Dynamics 365 Sales](admin-prepare-dynamics-365-for-sales-for-integration.md).  

Synchronisation uses the following elements:

* Integration table mappings
* Integration field mappings
* Synchronisation rules
* Coupled records

When synchronisation is set up you can couple [!INCLUDE[prod_short](includes/prod_short.md)] records to [!INCLUDE[prod_short](includes/cds_long_md.md)] rows to synchronise their data. You can start a synchronisation manually, or based on a schedule. The following table provides an overview of the ways you can synchronise.  

|  Type  |  Method  |  See  |  
|--------|----------|-------|  
|Manual synchronisation|Synchronise on a row-by-row basis.<br /><br /> You can synchronise individual records in [!INCLUDE[prod_short](includes/prod_short.md)], such as a customer, with a corresponding [!INCLUDE[prod_short](includes/cds_long_md.md)] row, such as an account. This is typically how users will work with [!INCLUDE[prod_short](includes/cds_long_md.md)] data in [!INCLUDE[prod_short](includes/prod_short.md)].|[Couple and Synchronise Records Manually](admin-manual-synchronization-of-table-mappings.md#synchronize-individual-table-mappings)|  
|  |Synchronise on a table mapping basis.<br /><br /> You can synchronise all records in a [!INCLUDE[prod_short](includes/prod_short.md)] table with an table [!INCLUDE[prod_short](includes/cds_long_md.md)] table.|[Synchronise Individual Table Mappings](admin-manual-synchronization-of-table-mappings.md#synchronize-individual-table-mappings)|  
||Synchronise all modified records for all table mappings.<br /><br /> You can synchronise all of the records that have been modified in [!INCLUDE[prod_short](includes/prod_short.md)] tables since the last synchronisation.|[Synchronising All Modified Records](admin-manual-synchronization-of-table-mappings.md#synchronizing-all-modified-records)|
||Full synchronisation of all data for all table mappings.<br /><br /> You can synchronise all of the data in [!INCLUDE[prod_short](includes/prod_short.md)] and [!INCLUDE[prod_short](includes/cds_long_md.md)] tables that are mapped, and create new records or rows in the destination solution for uncoupled records in the source solution.<br /><br /> Full synchronisation synchronises all data and ignores coupling. Typically, you do a full synchronisation when you set up the integration and only one of solutions contains data. A full synchronisation can also be useful in a demonstration environment.|[Run a Full Synchronisation](admin-manual-synchronization-of-table-mappings.md#run-a-full-synchronization)|  
|Scheduled synchronisation|Synchronise all changes to data for all table mappings.<br /><br /> You can synchronise [!INCLUDE[prod_short](includes/prod_short.md)] with [!INCLUDE[prod_short](includes/cds_long_md.md)] on scheduled intervals by setting up jobs in the job queue.|[Schedule a Synchronisation](admin-scheduled-synchronization-using-the-synchronization-job-queue-entries.md)|  

> [!NOTE]
> The synchronisation between [!INCLUDE[prod_short](includes/cds_long_md.md)] and [!INCLUDE[prod_short](includes/prod_short.md)] is based on the scheduled execution of job queue entries and does not guarantee real time data consistency between two services. For real time data conistency you should explore [Business Central Virtual Tables](/dynamics365/business-central/dev-itpro/powerplatform/powerplat-overview) or Business Central APIs.   

## <a name="standard-table-mapping-for-synchronization"></a>Standard table mapping for synchronisation

Tables in [!INCLUDE[prod_short](includes/cds_long_md.md)], such as accounts, are integrated with equivalent types of tables in [!INCLUDE[prod_short](includes/prod_short.md)], such as customers. To work with [!INCLUDE[prod_short](includes/cds_long_md.md)] data you set up links, called couplings, between tables in [!INCLUDE[prod_short](includes/prod_short.md)] and [!INCLUDE[prod_short](includes/cds_long_md.md)].

The following table lists the standard mapping between tables in [!INCLUDE[prod_short](includes/prod_short.md)] and [!INCLUDE[prod_short](includes/cds_long_md.md)].

> [!TIP]
> You can reset configuration changes made to integration table and field mappings to their default settings by selecting the mappings, then choosing **Use Default Synchronisation Setup**.

| [!INCLUDE[prod_short](includes/prod_short.md)] | [!INCLUDE[prod_short](includes/cds_long_md.md)] | Synchronisation Direction | Default Filter |
|---------------------------------------------|----------------------------------------------|---------------------------|----------------|
| Salesperson/Purchaser | User | [!INCLUDE[prod_short](includes/cds_long_md.md)] -> [!INCLUDE[prod_short](includes/prod_short.md)] | [!INCLUDE[prod_short](includes/cds_long_md.md)] contact filter: **Status** is **No**, **User Licensed** is **Yes**, Integration user mode is **No** |
| Customer | Account | [!INCLUDE[prod_short](includes/prod_short.md)] -> [!INCLUDE[prod_short](includes/cds_long_md.md)] and [!INCLUDE[prod_short](includes/cds_long_md.md)] -> [!INCLUDE[prod_short](includes/prod_short.md)] | [!INCLUDE[prod_short](includes/cds_long_md.md)] account filter: **Relationship Type** is **Customer** and **Status** is **Active**. [!INCLUDE[prod_short](includes/prod_short.md)] filter: **Blocked** is blank (Customer is not blocked). |
| Vendor | Account | [!INCLUDE[prod_short](includes/prod_short.md)] -> [!INCLUDE[prod_short](includes/cds_long_md.md)] and [!INCLUDE[prod_short](includes/cds_long_md.md)] -> [!INCLUDE[prod_short](includes/prod_short.md)] | [!INCLUDE[prod_short](includes/cds_long_md.md)] account filter: **Relationship Type** is **Vendor** and **Status** is **Active**. [!INCLUDE[prod_short](includes/prod_short.md)] filter: **Blocked** is blank (Vendor is not blocked). |
| Contact | Contact | [!INCLUDE[prod_short](includes/prod_short.md)] -> [!INCLUDE[prod_short](includes/cds_long_md.md)] and [!INCLUDE[prod_short](includes/cds_long_md.md)] -> [!INCLUDE[prod_short](includes/prod_short.md)] | [!INCLUDE[prod_short](includes/prod_short.md)] contact filter: **Type** is **Person** and the contact is assigned to a company. [!INCLUDE[prod_short](includes/cds_long_md.md)] contact filter: The contact is assigned to a company and the parent customer type is **Customer**. |
| Currency | Transaction Currency | [!INCLUDE[prod_short](includes/prod_short.md)] -> [!INCLUDE[prod_short](includes/cds_long_md.md)] |  |

> [!NOTE]
> The **Dataverse** actions will not be available on pages, for example, the Customer Card page, for records that do not respect the table filter on the integration table mapping.

### <a name="tip-for-admins-viewing-table-mappings"></a>Tip for admins: viewing table mappings

You can view the mapping between the tables in [!INCLUDE[prod_short](includes/cds_long_md.md)] and [!INCLUDE[prod_short](includes/prod_short.md)] on the **Integration Table Mappings** page, where you can also apply filters. You define the mapping between the fields in [!INCLUDE[prod_short](includes/prod_short.md)] tables and the columns in [!INCLUDE[prod_short](includes/cds_long_md.md)] tables on the **Integration Field Mapping** page, where you can add additional mapping logic. For example, this can be useful if you need to troubleshoot synchronisation.

## <a name="use-virtual-tables-to-get-more-data"></a>Use virtual tables to get more data

When you're setting up your integration, you can use virtual tables to make more data available in [!INCLUDE[prod_short](includes/cds_long_md.md)], without help from a developer.

A virtual table is a custom table that has columns and rows that contain data from an external data source, such as [!INCLUDE [prod_short](includes/prod_short.md)]. The columns and rows in a virtual table look like a regular table, however, the data isn't stored in a physical table in the [!INCLUDE[prod_short](includes/cds_long_md.md)] database. Instead, the data is retrieved at runtime.

> [!NOTE]
> [!INCLUDE [prod_short](includes/prod_short.md)] contains objects that are also called virtual tables. Those table objects are not related to the virtual tables that you use with [!INCLUDE[prod_short](includes/cds_long_md.md)].

To learn more about virtual tables, go to the following articles:

* [Create and edit virtual tables that contain data from an external data source](/power-apps/maker/data-platform/create-edit-virtual-entities) (Power Apps documentation)
* [Business Central Virtual Table for Microsoft Dataverse Admin Reference](/dynamics365/business-central/dev-itpro/powerplatform/powerplat-admin-reference) ([!INCLUDE [prod_short](includes/prod_short.md)] documentation)

To use virtual tables, you must install the **Business Central Virtual Entity** app from [AppSource](https://appsource.microsoft.com/en-US/product/dynamics-365/microsoftdynsmb.businesscentral_virtualentity). 

After you install the app, you can enable virtual tables from one of the following pages in [!INCLUDE [prod_short](includes/prod_short.md)]:

* When you run the **Set up Dataverse connection** assisted setup guide, you can use the **Dataverse Available Virtual Tables** page to select multiple virtual tables. Afterward, the tables are available in [!INCLUDE[prod_short](includes/cds_long_md.md)] and the PowerApps Maker Portal. 
* From the **Dataverse Connection Setup**, **Virtual Tables**, and **Available Virtual Tables** pages.  
* From the Power App Maker Portal.

## <a name="synchronize-data-from-multiple-companies-or-environments"></a>Synchronise data from multiple companies or environments

You can synchronise data from multiple [!INCLUDE [prod_short](includes/prod_short.md)] companies or environments with a [!INCLUDE[prod_short](includes/cds_long_md.md)] environment. In multi-company synchronisation scenarios, there are several things to consider.

### <a name="set-company-ids"></a>Set company IDs

When you synchronise records, we set a company ID on the [!INCLUDE[prod_short](includes/cds_long_md.md)] entity to clarify the [!INCLUDE [prod_short](includes/prod_short.md)] company the records came from. Integration table mappings have integration table filter fields that take the company ID into account. To include a table mapping in a multi-company setup, on the **Integration Table Mapping** page, choose the **Multi-Company Synchronisation Enabled** checkbox. The setting optimises how integration table filter fields filter company IDs in a multi-company setup.

For integration table mappings that synchronise documents, such as orders, quotes, and opportunities, if you choose the **Multi-Company Synchronisation Enabled** checkbox the integration only considers entities that have the company ID of the current [!INCLUDE [prod_short](includes/prod_short.md)] company. To synchronise documents, for example, between Business Central and Sales, users in Sales must specify the company ID on the documents. Otherwise, the documents won't synchronise.  

For all other integration table mappings, choosing the **Multi-Company Synchronisation Enabled** checkbox removes the filter on company ID. The synchronisation will consider related entities, regardless of their company ID.

### <a name="specify-the-synchronization-direction"></a>Specify the synchronisation direction

If you enable multi-company support on an integration table mapping, we recommend that you set the direction of the mapping to **FromIntegration**. If you set the direction to **ToIntegration** or **Bidirectional**, it's a good idea to use **Table Filter** and **Integration Table Filter** to control which entities synchronise with which company. It's also a good idea to use match-based coupling to avoid creating duplicate records. To learn more about match-based coupling, go to [Customise the match-based coupling](/dynamics365/business-central/admin-how-to-set-up-a-dynamics-crm-connection#customize-the-match-based-coupling).

### <a name="use-unique-numbers"></a>Use unique numbers

If your number series doesn't guarantee that primary key values are unique to each company, we recommend that you use prefixes. To start using prefixes, create a transformation rule on the integration field mapping. To learn more about transformation rules, go to [Handle differences in field values](admin-how-to-modify-table-mappings-for-synchronization.md#handle-differences-in-field-values).

## <a name="see-also"></a>See also

[Couple and Synchronise Records Manually](admin-how-to-couple-and-synchronize-records-manually.md)   
[Schedule a Synchronisation](admin-scheduled-synchronization-using-the-synchronization-job-queue-entries.md)  
[Integrating with Dynamics 365 Sales](admin-prepare-dynamics-365-for-sales-for-integration.md)

[!INCLUDE[footer-include](includes/footer-banner.md)]
