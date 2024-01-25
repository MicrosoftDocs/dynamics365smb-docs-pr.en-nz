---
title: Set Up Companies to Synchronise Master Data
description: Learn how to set up one or more companies to synchronise master data.
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bnielse
ms.service: dynamics-365-business-central
ms.topic: conceptual
ms.date: 01/25/2023
ms.custom: bap-template
ms.search.form: '7230, 7233, 5338, 7236, 672, 7234'
---

# Get Ready to Synchronise Master Data

When two or more companies use some of the same master data, you can synchronise the data rather than add it manually in each company. For example, synchronising data is useful when you're setting up new subsidiary companies.

Master data includes settings and non-transactional information about business entities. For example, customers, vendors, items, and employees. The data provides context for business transactions. The following are a few examples of master data for a customer:

* Name
* Identification number
* Address
* Payment terms
* Credit limit

You set up synchronisation in the subsidiary companies. Using a pull model, subsidiaries pull the data from the source company that they need to do business with them. After you set up synchronisation and synchronise data for the first time, you're all set. Job queue entries update coupled records in the subsidiaries when someone changes data in the source company.

## Uni-directional synchronisation only

You can synchronise data only from the source company to the subsidiary companies in a pull fashion. Subsidiaries can't push data to the source company.

> [!NOTE]
> Although it's possible, we don't recommend that you set up bi-directional synchronisation. That is, synchronising data from the source company to the subsidiaries, and from the subsidiaries to the source company. Synchronising data in both directions can lead to conflicts or unwanted overwrites.

## Before you start

The following are requirements for setting up synchronisation.

* All companies must be in the same environment.
* The user who sets up the subsidiary must have the **Essential**, **Premium**, or **Basic ISV** licence.

> [!NOTE]
> The Team Member and Internal Administrator licences let you access but not modify records, so they can't be used to set up the synchronisation. The Delegated Admin licence doesn't let you schedule background tasks, so you won't be able to complete the setup.

## Specify the source company

The first steps are to specify the company that will be the data source and enable synchronisation. Subsidiary companies pull data from the source company.

> [!NOTE]
> When you enable synchronisation, [!INCLUDE [prod_short](includes/prod_short.md)] creates and schedules the job queue entries that synchronise the data. It might look like the entries immediately sync the data, but that isn't the case. The created job queue entries only sync coupled records, and at this point you haven't set that up yet. Synchronisation starts after you [Enable or disable tables and fields](#enable-or-disable-tables-and-fields) and [Synchronise for the first time](#synchronize-for-the-first-time).

1. In a subsidiary company, choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Master Data Management Setup**, and then choose the related link.
1. In the **Source Company** field, specify the company that you'll pull changes from.
1. Turn on the **Enable Synchronisation** toggle.
1. In the confirmation dialogue, choose **OK**. [!INCLUDE [prod_short](includes/prod_short.md)] will find the tables and fields that are available from the source company.

The next step is to enable tables and fields for synchronisation.

## Enable or disable tables and fields

To save time, [!INCLUDE [prod_short](includes/prod_short.md)] provides a list of tables that businesses often synchronise. By default, these tables are enabled for synchronisation. You can modify, disable, or delete them as you see fit. As an extra time-saver, some fields on the tables are already disabled because they probably aren't relevant for the subsidiary.

> [!NOTE]
> If one or more extensions are installed in the source company, when a subsidiary sets up synchronisation the **Synchronisation Tables** page includes tables from the extensions, and you can access their fields. However, if the source company adds an extension after synchronisation is set up, each subsidiary must manually add the tables. To learn more about adding tables, go to [Add or delete tables from the synchronisation tables list](#add-or-delete-tables-from-the-synchronization-tables-list). To learn more about extending [!INCLUDE [prod_short](includes/prod_short.md)], go to [Developing extensions in Visual Studio Code](/dynamics365/business-central/dev-itpro/developer/devenv-dev-overview#developing-extensions-in-visual-studio-code).

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Master Data Management Setup**, and then choose the related link.
1. Choose the **Synchronisation Tables** action.
1. Fill in the fields as necessary. [!INCLUDE [tooltip-inline-tip_md](../archive/SetupAndAdministration/includes/tooltip-inline-tip_md.md)]

> [!TIP]
> The **Table Filter** field is helpful for controlling what to synchronise for a table. You can set up filters to synchronise only when certain conditions are met. For example, you can add filters that specify that you synchronise only vendors in a certain region. Or, customers that use a certain currency.
>
> If the subsidiary already has data in their tables, another good way to set criteria for synchronisation is to set up match-based coupling. To learn more about matching, go to [Use match-based coupling](#use-match-based-coupling).

1. To enable fields for a table, choose the table, and then choose the **Fields** action.
1. Fill in the fields as necessary. [!INCLUDE [tooltip-inline-tip_md](../archive/SetupAndAdministration/includes/tooltip-inline-tip_md.md)]

> [!TIP]
> A fast way to enable or disable multiple fields at the same time is to select them in the list, and then use either the **Enable** or **Disable** actions.

### Use match-based coupling

You can specify the data to synchronise for a table by matching records based on criteria. On the **Master Data Management Setup** page, choose the **Match-Based Coupling** action to open the **Select Coupling Criteria** page. You can define the following criteria for your matching:

* Whether to synchronise after you couple records.
* Whether to create a new record in the subsidiary company if a unique, uncoupled match can be found by using the match criteria. To activate this capability, turn on the **Create New if Unable to Find a Match** action.
* The fields to use to match records, and whether the match is case-sensitive.
* Prioritise the order in which records are searched by specifying a match priority. [!INCLUDE [prod_short](includes/prod_short.md)] will search for a match in ascending order based on the match priority. A blank value equals priority 0, which is the highest priority. Fields with the 0 priority are considered first.

## Synchronise for the first time

When you're ready, on the **Master Data Management Setup** page, choose the **Start Initial Synchronisation** action. On the **Master Data Initial Synchronisation** page, choose the type of synchronisation that you want to use for each table.

* If you already have records in both the source and the subsidiary companies, and you want to match existing records, choose the **Use Match-Based Coupling** action. [!INCLUDE [prod_short](includes/prod_short.md)] matches records in the subsidiary company with records in the source company. The matches are based on matching criteria that you define. For several default tables, [!INCLUDE [prod_short](includes/prod_short.md)] has already matched existing records by using their primary key, but you can change that if you want. You can also let the synchronisation create new records in the subsidiary for records in the source company that the subsidiary doesn't have. To learn more about matching, go to [Use match-based coupling](#use-match-based-coupling).
* If you choose **Run Full Synchronisation**, synchronisation creates new records for all records in the source company that aren't coupled yet. For example, this option is useful in the following scenarios:

    * The subsidiary doesn't have data in the table.
    * You want to add records from the source company without matching.  

After you choose the option to use, choose the **Start All** action to start the synchronisation.

While synchronisation is running, the **Job Status** column on the **Master Data Initial Full Synchronisation** page shows the status of each job queue entry. Press **F5** on your keyboard to update the status.

> [!TIP]
> Tables synchronise in a predefined order. If synchronisation get's stuck on a table, select the table and then choose the **Restart** action to get it going again.

To access details, such as the number of records that are inserted or modified, choose the value in the **Job Status** column to open the **View - Integration Synchronisation Jobs** page. For records that were inserted, you can choose the number in the **Inserted** column to access more details about the new records.

## Add or delete tables from the synchronisation tables list

### Add a table

> [!IMPORTANT]
> Although tables that contain transactional data are available in the list, such as tables that contain ledger entries, you shouldn't choose them. Synchronisation works only for tables that contain non-transactional data.

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Synchronisation tables**, and then choose the related link.
1. Choose **New**, and then choose the table to add.
1. Fill in the fields as necessary. [!INCLUDE [tooltip-inline-tip_md](../archive/SetupAndAdministration/includes/tooltip-inline-tip_md.md)]

### Delete a table

> [!NOTE]
> If you delete a record in the source company, it isn't also deleted in the subsidiary. This helps prevented unwanted loss of data. The subsidiary can decide to delete the table if they want.

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Synchronisation tables**, and then choose the related link.
1. Choose the **Delete** action.

## Use export and import to share a synchronisation setup

If you're setting up several subsidiaries that use the same or similar synchronisation settings, there's a time saver. Set up one subsidiary company and then export its setup to an .xml file. The file contains the entire setup, including table and field mappings and filter criteria. You can then import the file to the next subsidiary. To import or export a setup, on the **Master Data Management Setup** page, use the **Import** or **Export** actions.

## See Also

[Manage Master Data Synchronisation](admin-sync-master-data.md)