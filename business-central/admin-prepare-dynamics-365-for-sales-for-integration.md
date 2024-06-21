---
title: Integrating with Dynamics 365 Sales
description: Learn how to get Dynamics 365 Business Central ready to integrate with Dynamics 365 Sales.
author: brentholtorf
ms.topic: conceptual
ms.search.keywords: 'sales, crm, integration, integrating'
ms.date: 12/15/2023
ms.author: bholtorf
ms.custom: bap-template
ms.service: dynamics-365-business-central
ms.reviewer: bholtorf
---
# <a name="integrating-with-dynamics-365-sales"></a>Integrating with Dynamics 365 Sales

[!INCLUDE[azure-ad-to-microsoft-entra-id](~/../shared-content/shared/azure-ad-to-microsoft-entra-id.md)]

The sales person role is often considered as one the most outward-facing jobs in a business. However, it can be helpful for sales people to be able to look inward in the business and see what is happening on the back end. By integrating [!INCLUDE[prod_short](includes/prod_short.md)] and [!INCLUDE[crm_md](includes/crm_md.md)], you can give your sales people that insight. The integration will let people view information in [!INCLUDE[prod_short](includes/prod_short.md)] while they're working in [!INCLUDE[crm_md](includes/crm_md.md)]. For example, when preparing a sales quote it could be useful to know whether you have enough inventory to fulfil the order. For more information, see [Use Dynamics 365 Sales from Business Central](marketing-integrate-dynamicscrm.md).

> [!NOTE]
> This topic describes the process of integrating the online versions of [!INCLUDE[crm_md](includes/crm_md.md)] and [!INCLUDE[prod_short](includes/prod_short.md)] through [!INCLUDE[prod_short](includes/cds_long_md.md)]. For information about on-premises configuration, see [Preparing Dynamics 365 Sales for Integration on-premises](/dynamics365/business-central/dev-itpro/administration/prepare-dynamics-365-for-sales-for-integration).

## <a name="integrate-through-dataverse"></a>Integrate through Dataverse

To make it easy to connect and synchronise data with other Dynamics 365 applications, [!INCLUDE[prod_short](includes/prod_short.md)] also integrates with [!INCLUDE[prod_short](includes/cds_long_md.md)]. For example, you can connect to [!INCLUDE[crm_md](includes/crm_md.md)], or even apps that you build yourself. If you're integrating for the first time, you must do so through [!INCLUDE[prod_short](includes/cds_long_md.md)]. For more information, see [Integration with Dataverse](admin-common-data-service.md).

If you've already integrated [!INCLUDE[crm_md](includes/crm_md.md)] with [!INCLUDE[prod_short](includes/prod_short.md)], you can continue to synchronise data using your setup. However, if you upgrade or turn off your [!INCLUDE[crm_md](includes/crm_md.md)] integration, to turn it on again you must connect through [!INCLUDE[prod_short](includes/cds_long_md.md)]. For more information, see [Upgrading an Integration with Dynamics 365 Sales](admin-upgrade-sales-to-cds.md).

> [!NOTE]
> Reconnecting through [!INCLUDE[prod_short](includes/cds_long_md.md)] will apply default synchronisation settings, and will overwrite any configurations you have. For example, the default table mappings will be applied.

## <a name="integration-settings-that-are-specific-to-a--integration"></a>Integration settings that are specific to a [!INCLUDE[crm_md](includes/crm_md.md)] integration

Integration with [!INCLUDE[prod_short](includes/prod_short.md)] happens through [!INCLUDE[prod_short](includes/cds_long_md.md)], and many standard settings and tables are provided. In addition to the standard settings, there are some that are specific to [!INCLUDE[crm_md](includes/crm_md.md)]. The following sections list those settings.

## <a name="permissions-and-security-roles-for-user-accounts-in-sales"></a>Permissions and security roles for user accounts in Sales

When you install the Integration Solution, permissions for the integration user account are configured. If those permissions are changed, you might need to reset them. You can do that by reinstalling the Integration Solution by choosing **Redeploy Integration Solution** on the **Dynamics 365 Connection Setup** page. The following security roles are deployed:

* Dynamics 365 Business Central Integration Administrator
* Dynamics 365 Business Central Integration User
* Dynamics 365 Business Central Product Availability User

> [!NOTE]
> To use the **Open in Business Central** action in Sales, you must have the following privileges for the following tables:
>
> * You must have Read permissions for the Dynamics 365 Business Central Connection (nav_connection) table.
> * You must have Read, Write, and Delete permissions for the Default Dynamics 365 Business Central Connection (nav_defaultconnection) table.

### <a name="connection-settings-in-the-setup-guide"></a>Connection settings in the setup guide

You can use an assisted setup guide to quickly set up the connection and specify advanced features, such as coupling between records.

1. Choose **Setup and Extensions**, and then choose **Assisted Setup**.
2. Choose **Set up the Dynamics 365 Sales Connection** to start the assisted setup guide.
3. Fill in the fields as necessary.
4. Optionally, there are advanced settings that can enhance security and enable more capabilities. The following table describes the advanced settings.  

| Field | Description |
|--|--|
| **Import Dynamics 365 Sales Solution** | Install and configure the integration solution in [!INCLUDE[crm_md](includes/crm_md.md)]. <!--For more information, see [About the Base CDS Integration Solution](admin-common-data-service.md#about-the-business-central-integration-solution). Need to add a new topic--> |
|**Automatically Synchronise Item Availability**|Specifies that the item availability job queue must be scheduled. The job queue runs every 30 minutes, and updates the availability of the coupled items.|
| **Enable Legacy Sales Order Integration** | When people create sales orders in [!INCLUDE[crm_md](includes/crm_md.md)] and fulfil orders in [!INCLUDE[prod_short](includes/prod_short.md)], this setting integrates the process in [!INCLUDE[crm_md](includes/crm_md.md)]. For more information, see [Enable sales order processing integration](/dynamics365/customer-engagement/sales-enterprise/developer/enable-sales-order-processing-integration).<br><br>**Note:** You can't use this option if you use the **Bidirectional Synch of Sales Orders** option. The two settings are mutually exclusive. To learn more about this option, go to [Single and bi-directional synchronisation of sales orders](#single-and-bi-directional-synchronization-of-sales-orders). |
|**Enable Dynamics 365 Sales Connection** | Enable the connection to [!INCLUDE[crm_md](includes/crm_md.md)]. |
| **Dynamics 365 SDK Version** | This is relevant only if you're integrating with an on-premises version of [!INCLUDE[crm_md](includes/crm_md.md)]. This SDK is the Dynamics 365 software development kit (also referred to as Xrm) you use to connect [!INCLUDE[prod_short](includes/prod_short.md)] to [!INCLUDE[crm_md](includes/crm_md.md)]. The version must be compatible with the SDK version that is used by [!INCLUDE[crm_md](includes/crm_md.md)], and equal to or newer than the version used by [!INCLUDE[crm_md](includes/crm_md.md)]. |
|**Bidirectional Synch of Sales Orders**|Synchronise sales orders in both directions. To learn more about this option, go go [Single and bi-directional synchronisation of sales orders](#single-and-bi-directional-synchronization-of-sales-orders).<br><br>**Note:** You can't use this option if you use the **Enable Legacy Sales Order Integration** option. The two settings are mutually exclusive.|

### <a name="connection-settings-on-the-microsoft-dynamics-365-connection-setup-page"></a>Connection settings on the Microsoft Dynamics 365 Connection Setup page

Enter the following information for the connection from [!INCLUDE[crm_md](includes/crm_md.md)] to [!INCLUDE[prod_short](includes/prod_short.md)].

| Field | Description |
|--|--|
|**Dynamics 365 Sales URL**|The URL of your [!INCLUDE[crm_md](includes/crm_md.md)] instance. This setting lets users open the records in [!INCLUDE[prod_short](includes/prod_short.md)] that correspond to records in [!INCLUDE[crm_md](includes/crm_md.md)]. For example, an account or product. The [!INCLUDE[prod_short](includes/prod_short.md)] records open in [!INCLUDE[prod_short](includes/prod_short.md)].|
|**Automatically Synchronise Item Availability**|Specifies that the item availability job queue must be scheduled. The job queue runs every 30 minutes, and updates the availability of the coupled items.|
|**Dynamics 365 SDK Version**|If you're integrating with an on-premises version of [!INCLUDE[crm_md](includes/crm_md.md)], this is the Dynamics 365 software development kit (also referred to as Xrm) you use to connect [!INCLUDE[prod_short](includes/prod_short.md)] to [!INCLUDE[crm_md](includes/crm_md.md)]. The version that you select must be compatible with the SDK version that is used by [!INCLUDE[crm_md](includes/crm_md.md)]. This version equal to or newer than the version used by [!INCLUDE[crm_md](includes/crm_md.md)].|

In addition to the settings above, enter the following settings for [!INCLUDE[crm_md](includes/crm_md.md)].

| Field | Description |
|--|--|
| **Sales Order Integration is Enabled** | Enable users to submit sales orders and activated quotes in [!INCLUDE[crm_md](includes/crm_md.md)] and then view and process them in [!INCLUDE[prod_short](includes/prod_short.md)]. This setting integrates the process in [!INCLUDE[crm_md](includes/crm_md.md)]. For more information, see [Enable sales order processing integration](/dynamics365/customer-engagement/sales-enterprise/developer/enable-sales-order-processing-integration). |
| **Automatically Create Sales Orders** | Create a sales order in [!INCLUDE[prod_short](includes/prod_short.md)] when a user creates and submits one in [!INCLUDE[crm_md](includes/crm_md.md)]. |
| **Automatically Process Sales Quotes** | Process a sales quote in [!INCLUDE[prod_short](includes/prod_short.md)] when a user creates and activates one in [!INCLUDE[crm_md](includes/crm_md.md)]. For more information, see [Handling Sales Quotes Data](/dynamics365/business-central/marketing-integrate-dynamicscrm?tabs=new-experience#handling-sales-quotes-data). |
|**Bidirectional Synch of Sales Orders**|Synchronise sales orders in both directions. To learn more about this option, go to [Single and bi-directional synchronisation of sales orders](#single-and-bi-directional-synchronization-of-sales-orders).|
<!--
### <a name="user-account-settings"></a>User Account Settings
Integration with Business Central through Dataverse requires an administrator user account and an account that is used only for the connection between the apps. This account is called the "integration user." When you install the CDS Base Integration Solution, permissions for the integration user account are configured in [!INCLUDE[crm_md](includes/crm_md.md)]. If those permissions are changed you might need to reset them. You can do that by reinstalling the Integration Solution or by manually resetting them. The following tables list the minimum permissions for the user accounts in [!INCLUDE[crm_md](includes/crm_md.md)].  -->
### <a name="single-and-bi-directional-synchronization-of-sales-orders"></a>Single and bi-directional synchronisation of sales orders

When you set up your integration, either in the setup guide or on the Microsoft Dynamics 365 Connection Setup page, there are options that control the direction in which you synchronise sales orders, and how you submit them.

The **Bidirectional Synch of Sales Orders** option lets you synchronise sales orders from Sales to [!INCLUDE [prod_short](includes/prod_short.md)], and vice versa. For example, if a customer changes their mind about the product or quantity they ordered in [!INCLUDE[crm_md](includes/crm_md.md)], you can archive the sales document and create a new one in [!INCLUDE[prod_short](includes/prod_short.md)]. The same is true for changes in [!INCLUDE[prod_short](includes/prod_short.md)]. For example, when prices, tax amounts, or expected shipment dates change, the changes synchronize to [!INCLUDE[crm_md](includes/crm_md.md)]. Bidirectional synchronisation helps keep your sellers up to date with the latest changes and the status of sales orders.

For bidirectional synchronisation, you make sales orders available for synchronisation when you change their status to **Submitted** in Sales. When you set that status, you can no longer change information on the order's lines. When you synchronise, the order is transferred to [!INCLUDE [prod_short](includes/prod_short.md)] with the status **Released**. If there's a mistake, you can revert the order to **Open** (in [!INCLUDE [prod_short](includes/prod_short.md)]) or **Active** (in Sales), and then add or delete lines to correct the mistake, and submit the order again.

> [!TIP]
> When you enable the **Bidirectional Synch of Sales Orders** option, [!INCLUDE [prod_short](includes/prod_short.md)] creates a record on the **Sales Order Archives** page when you post or change information on an order. For example, the archived versions can be useful for exploring an order's history.

The **Enable Legacy Sales Order Integration** option synchronises only from Sales to [!INCLUDE [prod_short](includes/prod_short.md)]. For this option, you use the **Submit** action in Sales to make orders available for synchronisation. When you do, you can no longer change any information on the order. When you synchronise, the order is transferred to [!INCLUDE [prod_short](includes/prod_short.md)] with the status **Released**.

To use this option, you must provide credentials for an administrator user account in [!INCLUDE[crm_md](includes/crm_md.md)]. To learn more, see [Handling Sales Order Data](marketing-integrate-dynamicscrm.md#handling-sales-order-data).

> [!NOTE]
> The **Bidirectional Synch of Sales Orders** and **Enable Legacy Sales Order Integration** options are mutually exclusive. You can't use both options at the same time.

For both options, [!INCLUDE [prod_short](includes/prod_short.md)] shows all sales orders with the **Submitted** status on the **Orders - Microsoft Dynamics 365 Sales** page.

### <a name="standard-sales-entity-mapping-for-synchronization"></a>Standard Sales entity mapping for synchronisation

Entities in [!INCLUDE[crm_md](includes/crm_md.md)], such as orders, are integrated with equivalent types of tables in [!INCLUDE[prod_short](includes/prod_short.md)],such as sales orders. To work with [!INCLUDE[crm_md](includes/crm_md.md)] data you set up links, called couplings, between tables in [!INCLUDE[prod_short](includes/prod_short.md)] and [!INCLUDE[crm_md](includes/crm_md.md)].

The following table lists the standard mapping between tables in [!INCLUDE[prod_short](includes/prod_short.md)] and [!INCLUDE[crm_md](includes/crm_md.md)] that [!INCLUDE[prod_short](includes/prod_short.md)] provides.

| [!INCLUDE[prod_short](includes/prod_short.md)] | [!INCLUDE[crm_md](includes/crm_md.md)] | Synchronisation Direction | Default Filter |
|--|--|--|--|
| Unit of Measure | Unit Group | [!INCLUDE[prod_short](includes/prod_short.md)] -> [!INCLUDE[crm_md](includes/crm_md.md)] |  |
| Item | Product | [!INCLUDE[prod_short](includes/prod_short.md)] -> [!INCLUDE[crm_md](includes/crm_md.md)] and [!INCLUDE[crm_md](includes/crm_md.md)] -> [!INCLUDE[prod_short](includes/prod_short.md)] | Sales contact filter: **Product Type** is **Sales Inventory** |
| Resource | Product | [!INCLUDE[prod_short](includes/prod_short.md)] -> [!INCLUDE[crm_md](includes/crm_md.md)] and [!INCLUDE[crm_md](includes/crm_md.md)] -> [!INCLUDE[prod_short](includes/prod_short.md)] | Sales contact filter: **Product Type** is **Services** |
| Item Unit of Measure | CRM UOM |[!INCLUDE[prod_short](includes/prod_short.md)] -> [!INCLUDE[crm_md](includes/crm_md.md)]| |
| Resource Unit of Measure | CRM UOM |[!INCLUDE[prod_short](includes/prod_short.md)] -> [!INCLUDE[crm_md](includes/crm_md.md)]||
| Unit Group | CRM Uomschedule | [!INCLUDE[prod_short](includes/prod_short.md)] -> [!INCLUDE[crm_md](includes/crm_md.md)] ||
| Customer Price Group | Price List | [!INCLUDE[prod_short](includes/prod_short.md)] -> [!INCLUDE[crm_md](includes/crm_md.md)] |  |
| Sales Price | Product Price List | [!INCLUDE[prod_short](includes/prod_short.md)] -> [!INCLUDE[crm_md](includes/crm_md.md)] | [!INCLUDE[prod_short](includes/prod_short.md)] contact filter: **Sales Code** isn't blank, **Sales Type** is **Customer Price Group** |
| Opportunity | Opportunity | [!INCLUDE[prod_short](includes/prod_short.md)] -> [!INCLUDE[prod_short](includes/cds_long_md.md)] and [!INCLUDE[crm_md](includes/crm_md.md)] -> [!INCLUDE[prod_short](includes/prod_short.md)] |  |
| Sales Invoice Header | Invoice | [!INCLUDE[prod_short](includes/prod_short.md)] -> [!INCLUDE[crm_md](includes/crm_md.md)] |  |
| Sales Invoice Line | Invoice Product | [!INCLUDE[prod_short](includes/prod_short.md)] -> [!INCLUDE[crm_md](includes/crm_md.md)] |  |
| Sales Order Header | Sales Order | [!INCLUDE[prod_short](includes/prod_short.md)] -> [!INCLUDE[crm_md](includes/crm_md.md)] and [!INCLUDE[crm_md](includes/crm_md.md)] -> [!INCLUDE[prod_short](includes/prod_short.md)] <br><br> To synchronise in both directions, you must turn on the **Bidirectional Synch of Sales Orders** toggle on the **Dynamics 365 Connection Setup** page.| [!INCLUDE[prod_short](includes/prod_short.md)] Sales Header filter: **Document Type** is Order, **Status** is Released |
| Sales Order Notes | Sales Order Notes | [!INCLUDE[prod_short](includes/prod_short.md)] -> [!INCLUDE[crm_md](includes/crm_md.md)] and [!INCLUDE[crm_md](includes/crm_md.md)] -> [!INCLUDE[prod_short](includes/prod_short.md)] |  |

> [!NOTE]
> The mappings for the Item Unit of Measure, Resource Unit of Measure, and Unit Group tables are available only if your administrator has turned on the **Unit Group Mapping** toggle on the **Microsoft Dynamics 365 Connection Setup** page. To learn more, go to [Synchronising Items and Resources with Products in Different Units of Measure](admin-prepare-dynamics-365-for-sales-for-integration.md#synchronize-items-and-resources-with-products-with-different-units-of-measure).

## <a name="synchronize-items-and-resources-with-products-with-different-units-of-measure"></a>Synchronise items and resources with products with different units of measure

Businesses often produce or purchase the items in one unit of measure, and then sell them in another. To synchronise items that use multiple units of measure, you must turn on the **Unit Group Mapping** toggle on the **Microsoft Dynamics 365 Connection Setup** page. 

When you turn on the feature update, a new Unit Group table is created and assigned to each item and resource in [!INCLUDE[prod_short](includes/prod_short.md)]. The tables let you map the Unit Group, Item Unit of Measure, and Resource Unit of Measure tables in [!INCLUDE[prod_short](includes/prod_short.md)] to the Dynamics 365 Sales Unit Group in [!INCLUDE[crm_md](includes/crm_md.md)]. The following image shows the mappings.

:::image type="content" source="media/unit group 1.png" alt-text="Table mappings for unit groups":::

You can create multiple units of measurement for each unit group, and assign the groups to products in [!INCLUDE[crm_md](includes/crm_md.md)]. Afterwards, you'll be able to synchronise the products with items and resources in [!INCLUDE[prod_short](includes/prod_short.md)]. You can manually couple item units of measurement or resource units of measurement with a unit group. When you do, if the unit group for the item or resource isn't coupled to a unit group in [!INCLUDE[crm_md](includes/crm_md.md)], for example, because the unit group didn't exist, [!INCLUDE[prod_short](includes/prod_short.md)] will automatically create the unit group in [!INCLUDE[crm_md](includes/crm_md.md)].

### <a name="map-items-and-resources-to-products"></a>Map items and resources to products

When you turn on the **Unit Group Mapping** toggle on the **Microsoft Dynamics 365 Connection Setup** page, the following happens:

* New mappings are created for items and resources.
* Existing mappings are deleted. <!--which mappings?-->
* A data upgrade creates unit groups for items and resources.

To use the new mappings, you must synchronise unit groups, item unit of measure, and resource unit of measures. You must also resynchronize items and resources. 

> [!NOTE]
> [!INCLUDE[crm_md](includes/crm_md.md)] does not allow you to change a unit group for a product. Therefore, you must retire your products and uncouple the items and resources, and then synchronise by creating new products in [!INCLUDE[crm_md](includes/crm_md.md)]. 

The following steps describe the steps to start mapping unit groups:

1. Be sure that products in [!INCLUDE[crm_md](includes/crm_md.md)] aren't coupled with items or resources in [!INCLUDE[prod_short](includes/prod_short.md)]. If they are, go to the **Items** and/or **Resources** pages and use the filter options to select the coupled records. Then choose the **Dynamics 365 Sales** action, and select **Uncouple**. This action schedules a background job to uncouple the records. While the job is running, you can check its status by using the **Synchronisation Log** action. For more information, see [Coupling and Synchronising](admin-how-to-couple-and-synchronize-records-manually.md). 
2. Because new products will be created in [!INCLUDE[crm_md](includes/crm_md.md)] with new unit groups, to avoid duplicate names, do one of the following steps:
    
  * Rename your products, and then retire them in [!INCLUDE[crm_md](includes/crm_md.md)]. For more information, see [Retire products (Sales Hub)](/dynamics365/sales-enterprise/retire-product). To bulk edit your products in Microsoft Excel, sign in to Power Apps, choose your environment, go to the **Product** table, and then choose the **Data** tab. Clear any filters that are applied. In the **Data** group, choose the **Edit Data in Excel** action. Add a prefix or suffix to the coupled products, and then retire them.
    * Retire your products and delete them. 

3. Follow these steps to synchronise **Unit Groups**, **Unit of Measures**, **Items**, and **Resources**:
    1. In [!INCLUDE[prod_short](includes/prod_short.md)], open the **Dynamics 365 Sales Connection Setup** page.
    2. Use the **Run Full Synchronisation** action to open the **Dataverse Full Synch. Review** page.
    3. For the **ITEM UOM**, **RESOURCE UOM**, AND **UNIT GROUP** mappings, choose the **Recommend Full Synchronisation** action.
    4. Choose the **Sync All** action.

    > [!NOTE]
    > For mappings that have not yet been fully synchronised, this action will fully synchronise them. To prevent those mappings from synchronising, delete the mappings from the page. This only removes them from the current full synchronisation, and does not delete the mappings.
    
5. Choose the **ITEM-PRODUCT** mapping, and then choose the **Restart** action. Restarting creates new products from the items in [!INCLUDE[crm_md](includes/crm_md.md)], and assigns a new unit group that is specific to the item.
6. Choose the **RESOURCE-PRODUCT** mapping, and then choose the **Restart** action. Restarting creates new products from the resources in [!INCLUDE[crm_md](includes/crm_md.md)], and assigns a new unit group that is specific to the resources.

### <a name="synchronization-rules"></a>Synchronisation rules

The following table lists the rules that control the synchronisation between [!INCLUDE[crm_md](includes/crm_md.md)] and [!INCLUDE[prod_short](includes/prod_short.md)]. These rules are in addition to rules defined for Dataverse, which also apply. For more information, see [Standard Entity Mapping](admin-synchronizing-business-central-and-sales.md#standard-table-mapping-for-synchronization).

> [!NOTE]  
> Changes to data in  that were made by the integration user account are not synchronised. Therefore, we recommended that you do not change data while using that account. For more information, see [Setting Up User Accounts for Integrating with Dynamics 365 Sales](admin-setting-up-integration-with-dynamics-sales.md).

|Table|Rule|
|-----|----|
|Units of Measurement|Units of measurement are synchronised with unit groups in [!INCLUDE[crm_md](includes/crm_md.md)]. There can only be one unit of measure defined in the unit group.|
|Items|When synchronising items with [!INCLUDE[crm_md](includes/crm_md.md)] products, [!INCLUDE[prod_short](includes/prod_short.md)] automatically creates a price list in [!INCLUDE[crm_md](includes/crm_md.md)]. To avoid synchronisation errors, you shouldn't modify this price list manually.|
|Resources|Resources are synchronised with [!INCLUDE[crm_md](includes/crm_md.md)] products that have product type Service.|
|Customer Price Groups|Customer price groups are synchronised with Sales price lists.|
|Sales Prices|Sales prices that have sales type Customer Price Group and have a sales code defined are synchronised with [!INCLUDE[crm_md](includes/crm_md.md)] price list lines|
|Opportunities|Opportunities are synchronised with [!INCLUDE[crm_md](includes/crm_md.md)] opportunities. The Salesperson Code value defines the owner of the coupled table in [!INCLUDE[crm_md](includes/crm_md.md)].|
|Posted Sales Invoices|Posted sales invoices are synchronised with sales invoices. Before an invoice can be synchronised, it's better to synchronise all other tables that can participate in the invoice, from salespersons to price lists. The Salesperson Code value in the invoice header defines the owner of the coupled table in Sales.|
|Sales Orders|When sales order integration is enabled, sales orders in [!INCLUDE[prod_short](includes/prod_short.md)] that are created from submitted sales orders in [!INCLUDE[crm_md](includes/crm_md.md)] are synchronised with sales orders in [!INCLUDE[crm_md](includes/crm_md.md)] when they're released. Before you synchronise orders, we recommend that you first synchronise all tables that the are involved with the order, such as sales persons and price lists. The Salesperson Code field in the order header defines the owner of the coupled table in [!INCLUDE[crm_md](includes/crm_md.md)].|

### <a name="synchronization-jobs-for-a-sales-integration"></a>Synchronisation jobs for a Sales integration

The jobs are run in the following order to avoid coupling dependencies between tables. There are more jobs available from Dataverse. For more information, see [Use Job Queues to Schedule Tasks](./admin-job-queues-schedule-tasks.md).

1. UNITOFMEASURE - Dynamics 365 Sales synchronisation job  
2. RESOURCE-PRODUCT - Dynamics 365 Sales synchronisation job  
3. ITEM-PRODUCT - Dynamics 365 Sales synchronisation job  
4. CUSTPRCGRP-PRICE - Dynamics 365 Sales synchronisation job.
5. SALESPRC-PRODPRICE - Dynamics 365 Sales synchronisation job.
6. POSTEDSALESINV-INV - Dynamics 365 Sales synchronisation job.

### <a name="default-synchronization-job-queue-entries"></a>Default synchronisation job queue entries

The following table describes the default synchronisation jobs for [!INCLUDE[crm_md](includes/crm_md.md)].  

|Job Queue Entry|Description|Direction|Integration Table Mapping|Default Synchronisation Frequency (mins)|Default inactivity sleep time (mins)|  
|---------------------|---------------------------------------|---------------|-------------------------------|-----|-----|  
|UNITOFMEASURE - Dynamics 365 Sales synchronisation job|Synchronises [!INCLUDE[crm_md](includes/crm_md.md)] unit groups with [!INCLUDE[prod_short](includes/prod_short.md)] units of measurement.|From [!INCLUDE[prod_short](includes/prod_short.md)] to [!INCLUDE[crm_md](includes/crm_md.md)]|UNIT OF MEASUREMENT|30|720<br> (12 hrs)|
|RESOURCE-PRODUCT - Dynamics 365 Sales synchronisation job|Synchronises [!INCLUDE[crm_md](includes/crm_md.md)] products with [!INCLUDE[prod_short](includes/prod_short.md)] resources.|From [!INCLUDE[prod_short](includes/prod_short.md)] to [!INCLUDE[crm_md](includes/crm_md.md)]|RESOURCE-PRODUCT|30|720<br> (12 hrs)|
|ITEM - PRODUCT - Dynamics 365 Sales synchronisation job|Synchronises [!INCLUDE[crm_md](includes/crm_md.md)] products with [!INCLUDE[prod_short](includes/prod_short.md)] items.|From [!INCLUDE[prod_short](includes/prod_short.md)] to [!INCLUDE[crm_md](includes/crm_md.md)]|ITEM-PRODUCT|30|1440<br> (24 hrs)|
|CUSTPRCGRP-PRICE - Dynamics 365 Sales synchronisation job|Synchronises [!INCLUDE[crm_md](includes/crm_md.md)] sales price lists with [!INCLUDE[prod_short](includes/prod_short.md)] customer price groups.| |CUSTOMER PRICE GROUPS-SALES PRICE LISTS|30|1440<br> (24 hrs)|
|SALESPRC-PRODUCTPRICE - Dynamics 365 Sales synchronisation job|Synchronises [!INCLUDE[crm_md](includes/crm_md.md)] product prices with [!INCLUDE[prod_short](includes/prod_short.md)] sales prices.||PRODUCT PRICE-SALES PRICE|30|1440<br> (24 hrs)|
|POSTEDSALESINV-INV - Dynamics 365 Sales synchronisation job|Synchronises [!INCLUDE[crm_md](includes/crm_md.md)] invoices with [!INCLUDE[prod_short](includes/prod_short.md)] posted sales invoices.|From [!INCLUDE[prod_short](includes/prod_short.md)] to [!INCLUDE[crm_md](includes/crm_md.md)]|INVOICES-POSTED SALES INVOICES|30|1440<br> (24 hrs)|
|Customer Statistics - Dynamics 365 Sales synchronisation|Updates [!INCLUDE[crm_md](includes/crm_md.md)] accounts with the latest [!INCLUDE[prod_short](includes/prod_short.md)] customer data. In [!INCLUDE[crm_md](includes/crm_md.md)], this information appears in **Business Central Account Statistics** quick view form of accounts that are coupled to [!INCLUDE[prod_short](includes/prod_short.md)] customers.<br /><br /> This data can also be updated manually from each customer record. For more information, see [Couple and Synchronise Records Manually](admin-how-to-couple-and-synchronize-records-manually.md). </BR></BR>**Note:**  This job queue entry is relevant only if the [!INCLUDE[prod_short](includes/prod_short.md)] integration solution is installed in [!INCLUDE[crm_md](includes/crm_md.md)]. |Not applicable|Not applicable|30|Not applicable| 

## <a name="connect-to-on-premises-versions-of-business-central-2019-release-wave-1-and-microsoft-dynamics-nav-2018"></a>Connect to on-premises versions of Business Central 2019 release wave 1 and Microsoft Dynamics NAV 2018

The Microsoft Power Platform team has [announced](/power-platform/important-changes-coming#deprecation-of-office365-authentication-type-and-organizationserviceproxy-class-for-connecting-to-dataverse) that it's deprecating the Office365 authentication type. If you're using a version of [!INCLUDE[prod_short](includes/prod_short.md)] on-premises that is earlier than Business Central 2019 release wave 1, you must use the OAuth authentication type to connect to [!INCLUDE[crm_md](includes/crm_md.md)] online. The steps in this section describe how to connect the following product versions:

* Business Central 2019 release wave 1
* Microsoft Dynamics NAV 2018

### <a name="prerequisites"></a>Prerequisites

* You must have a Microsoft Azure subscription. A trial account will work for application registration.
* [!INCLUDE[crm_md](includes/crm_md.md)] is configured to use one of the following authentication types:

   * Office365 (legacy)

     > [!IMPORTANT]
     > Effective April 2022, Office365 (legacy) will no longer be supported. For more information, see [Important changes (deprecations) coming in Power Apps, Power Automate and customer engagement apps](/power-platform/important-changes-coming#deprecation-of-office365-authentication-type-and-organizationserviceproxy-class-for-connecting-to-dataverse).

   * OAuth

### <a name="connect-business-central-2019-release-wave-1-and-dynamics-nav-2018"></a>Connect Business Central 2019 release wave 1 and Dynamics NAV 2018

1. Import the Microsoft Dynamics 365 Business Central Integration Solution into your [!INCLUDE[crm_md](includes/crm_md.md)] environment. The integration solution is available in the CrmCustomization folder on your [!INCLUDE[prod_short](includes/prod_short.md)] or Dynamics NAV 2018 installation DVD. Depending on your product version, import one of the following solutions:

   * For [!INCLUDE[prod_short](includes/prod_short.md)], the folder contains the DynamicsNAVIntegrationSolution_v9 and DynamicsNAVIntegrationSolution_v91. solutions. The solution you should import depends on the version of [!INCLUDE[crm_md](includes/crm_md.md)] you're connecting to. [!INCLUDE[crm_md](includes/crm_md.md)] online requires the DynamicsNAVIntegrationSolution_v91 integration solution.
   * For Dynamics NAV 2018, install the DynamicsNAVIntegrationSolution solution.

2. Create a non-interactive integration user in your [!INCLUDE[crm_md](includes/crm_md.md)] environment, and assign the user the following security roles. For more information, see [Create a non-interactive user account](/power-platform/admin/create-users-assign-online-security-roles#create-a-non-interactive-user-account).

   * Dynamics 365 Business Central Integration Administrator
   * Dynamics 365 Business Central Integration User

   > [!Important]
   > This user must not have the System Administrator security role. Also, you cannot use the system administrator account as the integration user.

3. In the Azure portal, create an app registration for [!INCLUDE[prod_short](includes/prod_short.md)]. For more information, see [Register an application in Microsoft Entra ID](/powerapps/developer/data-platform/walkthrough-register-app-azure-active-directory). 
  
   > [!NOTE]
   > We recommend that you register the app in the same tenant as your Dataverse environment so that you do not have to consent to letting the app access the environment. If you register the app in another environment, you must sign in to Microsoft Entra ID using the administrator account for your Dataverse environment and give consent.
   >
   > Additionally, the app that you register must not have a secret. Connecting an app with a secret to Dataverse is available only in Business Central 2020 release wave 1 and later.
  
4. Depending on your product version, do one of the following steps:

    * In [!INCLUDE[prod_short](includes/prod_short.md)], search for **Microsoft Dynamics 365 Connection Setup**, and then choose the related link. 
    * In Dynamics NAV 2018, search for **Microsoft Dynamics 365 for Sales Connection Setup**, and then choose the related link.

5. In the **Authentication Type** field, choose the option for OAuth. 
6. Choose the CRM SDK version that matches solution version you imported in step 1.

   > [!NOTE]
   > This step is only relevant for [!INCLUDE[prod_short](includes/prod_short.md)].

7. Enter the URL of your [!INCLUDE[crm_md](includes/crm_md.md)] environment, and then enter the user name and password for the integration user. 

   * In [!INCLUDE[prod_short](includes/prod_short.md)], use the **Server Address** field.
   * In Dynamics NAV 2018, use the **Dynamics 365 Sales URL** field.

8. In the **Connection String** field, specify the ID of the app registration. This field has two tokens in which the ID of your application should be specified.

   |Token           |Description  |
   |----------------|-------------|
   |**AppId**       |Set to the application ID.      |
   |**RedirectUri** |Set to the application ID, but add the **app://** prefix.         |

    **Example** The following example shows a connection string.

    ```
    AuthType=OAuth;Username=jsmith@contoso.onmicrosoft.com;Password=****;Url=https://contosotest.crm.dynamics.com;AppId=<your AppId>;RedirectUri=app://<your AppId>;TokenCacheStorePath=;LoginPrompt=Auto
    ```
9. Enable the connection.

> [!Note]
> If you want to configure a connection to a [!INCLUDE[crm_md](includes/crm_md.md)] instance with a specific authentication type, fill in the fields on the **Authentication Type Details** FastTab. For more information, see [Authentication with Microsoft Dataverse web services](/powerapps/developer/data-platform/authentication). This step is not required when connecting an online version of [!INCLUDE[prod_short](includes/prod_short.md)].

## <a name="see-also"></a>See also

[Setting Up User Accounts for Integrating with [!INCLUDE[crm_md](includes/crm_md.md)]](admin-setting-up-integration-with-dynamics-sales.md)  
[Set Up a Connection to [!INCLUDE[crm_md](includes/crm_md.md)]](admin-how-to-set-up-a-dynamics-crm-connection.md)  
[Synchronising Business Central and [!INCLUDE[crm_md](includes/crm_md.md)]](admin-synchronizing-business-central-and-sales.md)  
[Preparing Dynamics 365 Sales for Integration on-premises](/dynamics365/business-central/dev-itpro/administration/prepare-dynamics-365-for-sales-for-integration)


[!INCLUDE[footer-include](includes/footer-banner.md)]
