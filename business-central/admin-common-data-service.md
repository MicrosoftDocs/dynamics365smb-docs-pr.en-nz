---
title: Integrate with Microsoft Dataverse via data sync
description: Introduction to how to integrate and use Microsoft Dataverse and its components to connect to other Dynamics 365 applications.
author: brentholtorf
ms.author: bholtorf
ms.reviewer: ivkoleti
ms.topic: conceptual
ms.date: 06/28/2023
ms.custom: bap-template
---

# <a name="integrate-with-microsoft-dataverse-via-data-sync"></a>Integrate with Microsoft Dataverse via data sync

Business apps often use data from more than one source. [!INCLUDE[prod_short](includes/cds_long_md.md)] combines data into a single set of logic that makes it easier to connect [!INCLUDE[prod_short](includes/prod_short.md)] to other Dynamics 365 applications. For example, [!INCLUDE[crm_md](includes/crm_md.md)] or your own application built on [!INCLUDE[prod_short](includes/cds_long_md.md)]. To learn more about [!INCLUDE[prod_short](includes/cds_long_md.md)], go to [What is Dataverse?](/powerapps/maker/common-data-service/data-platform-intro).

The following steps provide an overview of the steps to integrate [!INCLUDE[prod_short](includes/cds_long_md.md)] with [!INCLUDE[prod_short](includes/prod_short.md)].

> [!Note]  
> These tasks require the **System Administrator** security role in [!INCLUDE[prod_short](includes/cds_long_md.md)] and [!INCLUDE[prod_short](includes/prod_short.md)].  

1. Assign licences for [!INCLUDE[prod_short](includes/cds_long_md.md)] to the [!INCLUDE[prod_short](includes/prod_short.md)] users who will use the integrated apps.

2. Set up a connection to [!INCLUDE[prod_short](includes/cds_long_md.md)]. For more information, see [Connect to Dataverse](admin-how-to-set-up-a-dynamics-crm-connection.md).  

3. Synchronise data between the apps. For more information, see [Synchronising Business Central and Dataverse](admin-synchronizing-business-central-and-sales.md). 

## <a name="get-started-with-"></a>Get started with [!INCLUDE[prod_short](includes/cds_long_md.md)]

To get started with [!INCLUDE[prod_short](includes/cds_long_md.md)], you'll need a Microsoft Power Apps account. If you don't already have a Power Apps account, you can get one for free by visiting [powerapps.com](https://make.powerapps.com/?utm_source=padocs&utm_medium=linkinadoc&utm_campaign=referralsfromdoc) and choosing the **Get started free** link. To learn more about how to get started with [!INCLUDE[prod_short](includes/cds_long_md.md)], go to the [Get started with Dataverse](/training/modules/get-started-with-powerapps-common-data-service/) module from Microsoft training.

## <a name="bi-directional-or-uni-directional-data-synchronization"></a>Bi-directional or uni-directional data synchronisation

You can synchronise data either to or from one Dynamics 365 business app to another, or in both directions in near-real time, through [!INCLUDE[prod_short](includes/cds_long_md.md)]. For example, if you integrate [!INCLUDE[prod_short](includes/prod_short.md)] with [!INCLUDE[crm_md](includes/crm_md.md)], a salesperson can create a sales order in [!INCLUDE[crm_md](includes/crm_md.md)] and the order synchronises to [!INCLUDE[prod_short](includes/prod_short.md)]. Conversely, from [!INCLUDE[crm_md](includes/crm_md.md)], the salesperson can check the availability of the item on the order in [!INCLUDE[prod_short](includes/prod_short.md)]. 

## <a name="standard-and-custom-entities"></a>Standard and custom entities

[!INCLUDE[prod_short](includes/cds_long_md.md)] securely stores data in a set of tables, which are sets of records similar to how a table stores data within a database. [!INCLUDE[prod_short](includes/cds_long_md.md)] includes a base set of standard tables that cover typical scenarios, but you can also create custom tables specific to your organisation. In [!INCLUDE[prod_short](includes/prod_short.md)], you can view standard and custom tables being synchronised on the Integration Table Mappings page.

## <a name="about-the-business-central-base-integration-solution"></a>About the Business Central Base Integration Solution

The Base Integration Solution is a key component of the integration. The solution adds the required roles and access levels to the user accounts for the integration, and it creates tables needed to map [!INCLUDE[prod_short](includes/prod_short.md)] company to business unit in [!INCLUDE[prod_short](includes/cds_long_md.md)]. 

By default, the **Set up [!INCLUDE[prod_short](includes/cds_long_md.md)] connection** assisted setup guide imports the solution. To do that, the setup guide uses an administrator user account that you specify. This account must be a valid user in [!INCLUDE[prod_short](includes/cds_long_md.md)] with the following security role:

* System Administrator  

To learn more about user accounts, go to the following articles:

* [Setting Up User Accounts for Integrating with [!INCLUDE[prod_short](includes/cds_long_md.md)]](admin-setting-up-integration-with-dynamics-sales.md) 
* [Create users in Microsoft Dynamics 365 (online) and assign security roles](/dynamics365/customer-engagement/admin/create-users-assign-online-security-roles). 

The administrator account is used only one time during the setup for the configuration changes that the Base Integration Solution makes in [!INCLUDE[prod_short](includes/cds_long_md.md)]. After the solution imports, the account is no longer needed. Integration will continue to use the user account that is automatically created specifically for the integration.

In addition to customising [!INCLUDE[prod_short](includes/cds_long_md.md)], the solution also creates the following roles in [!INCLUDE[prod_short](includes/cds_long_md.md)] for the integration:

* **Integration Administrator** - Allows users to manage the connection between [!INCLUDE[prod_short](includes/prod_short.md)] and [!INCLUDE[prod_short](includes/cds_long_md.md)]. Typically, this role is assigned only to the user account that's automatically created for synchronisation.  
* **Integration User** - Allows users to access synchronised data. Typically, you assign this role to the following user accounts:

  * The user accounts that's automatically created for synchronisation.
  * Other users who need access to the synchronised data.

To learn more about each role, such as the permissions and access levels, go to [Setting Up User Accounts for Integrating with [!INCLUDE[prod_short](includes/cds_long_md.md)]](admin-setting-up-integration-with-dynamics-sales.md).

When you set up the connection, you create the integration table mappings that you need to synchronise data. Entities in [!INCLUDE[prod_short](includes/cds_long_md.md)] are mapped to tables and table fields in [!INCLUDE [prod_short](includes/prod_short.md)] through integration tables. To learn more about mappings, go to [Standard Entity Mapping for Synchronisation](admin-synchronizing-business-central-and-sales.md#standard-table-mapping-for-synchronization).

## <a name="handle-differences-in-local-and-base-transaction-currencies"></a>Handle differences in local and base transaction currencies

You can connect to a [!INCLUDE[prod_short](includes/cds_long_md.md)] environment that has a different base currency than the local currency in [!INCLUDE[prod_short](includes/prod_short.md)]. You make the connection in [!INCLUDE[prod_short](includes/prod_short.md)] on the **Dataverse Connection Setup** page or by using the **Set up connection to Dataverse** assisted setup guide.

To be able to connect, ensure that the base transaction currency setting in [!INCLUDE[prod_short](includes/cds_long_md.md)] has the currency that set on the **Currencies** page in [!INCLUDE [prod_short](includes/prod_short.md)], and at least one exchange rate is specified for the currency on the **Currency Exchange Rates** page.

Here's an example. You're connecting [!INCLUDE[prod_short](includes/cds_long_md.md)] with Euro (EUR) set as the local currency on the **General Ledger Setup** page to a [!INCLUDE[prod_short](includes/cds_long_md.md)] environment that has a base transaction currency set to US dollar (USD). You'll need to have USD on the **Currencies** page in [!INCLUDE [prod_short](includes/prod_short.md)] and the appropriate exchange rate. 

When you enable the connection to [!INCLUDE[prod_short](includes/cds_long_md.md)], [!INCLUDE [prod_short](includes/prod_short.md)] adds its local currency to the **Currency** entity in [!INCLUDE[prod_short](includes/cds_long_md.md)] with the exchange rate from the **Currency Factor** field on the **Currency Exchange Rates** page.

Currency synchronisation is unidirectional, from [!INCLUDE [prod_short](includes/prod_short.md)] to [!INCLUDE [!INCLUDE[prod_short](includes/cds_long_md.md)], monetary amounts convert and synchronise as follows:

* Amounts in the [!INCLUDE[prod_short](includes/cds_long_md.md)] base currency convert to the [!INCLUDE [prod_short](includes/prod_short.md)] local currency based on the latest exchange rate synchronised from [!INCLUDE [prod_short](includes/prod_short.md)].
* Amounts in the [!INCLUDE [prod_short](includes/prod_short.md)] local currency synchronise with the [!INCLUDE [prod_short](includes/prod_short.md)] local currency in one of the other (non-base) currencies in [!INCLUDE[prod_short](includes/cds_long_md.md)].

## <a name="see-also"></a>See also

[Data Ownership Models](admin-cds-company-concept.md)  
<!--needs to be removed as this is moved to dev-itpro docs[Walkthrough: Customizing an Integration with Dataverse](\dynamics365\business-central\dev-itpro\administration\administration-custom-cds-integration) -->


[!INCLUDE[footer-include](includes/footer-banner.md)]
