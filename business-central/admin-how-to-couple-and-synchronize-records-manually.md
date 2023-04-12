---
title: Coupling and Synchronising (contains video)
description: Synchronising an integration table mapping enables data syncing in all records in a table in Business Central and Dynamics 365 Sales table that are coupled.
author: brentholtorf
ms.author: bholtorf
ms.reviewer: ivkoleti
ms.topic: conceptual
ms.date: 03/31/2023
ms.custom: bap-template
ms.search.keywords: 'crm, sales, couple, decouple, synchronize'
ms.search.form: '6250,'
---

# Coupling and Synchronising Records between Dataverse and Business Central

This topic describes how to couple one or more records in [!INCLUDE[prod_short](includes/prod_short.md)] with records in Dataverse or [!INCLUDE[crm_md](includes/crm_md.md)]. Coupling records lets you view Dataverse information from [!INCLUDE[prod_short](includes/prod_short.md)], and vice versa. The coupling also enables you to synchronise data between the records. You can couple existing records, or create and couple new records.

> [!NOTE]
> Coupling and synchronising data is available only if your system administrator has created a connection between [!INCLUDE[prod_short](includes/prod_short.md)] and Dataverse or [!INCLUDE[crm_md](includes/crm_md.md)]. A quick way to check is to open the **Customer** card and look for the **Set Up Coupling** action. If the action is available, the apps are connected.

## Video Example

This video shows coupling and synchronising data in the context of an integration with [!INCLUDE[crm_md](includes/crm_md.md)].

> [!VIDEO https://go.microsoft.com/fwlink/?linkid=2098376]

## To couple a record  

1. In [!INCLUDE[prod_short](includes/prod_short.md)], open the card for the record you want to couple. For example, the Customer or Contact card.  

    You can also just open the list page and select the record that you want to couple.  

2. Choose the **Set Up Coupling** action.  
3. Fill in the fields, and then choose **OK**.  

## To synchronise a single record  

1. In [!INCLUDE[prod_short](includes/prod_short.md)], open the card for the record you want to couple. For example, the Customer or Contact card.  
2. Choose the **Synchronise Now** action.  
3. If a record can be synchronised in one direction, select the option that specifies the direction of data update, and then choose **OK**.  

## To synchronise a single record from [!INCLUDE[crm_md](includes/crm_md.md)]  

1. In [!INCLUDE[crm_md](includes/crm_md.md)], open the form for the record you want to couple. For example, the Account card or Contact card form.  
2. Choose the **[!INCLUDE[prod_short](includes/prod_short.md)]** action in the ribbon to open and couple record automatically.

    > [!Note]
    > You can synchronise a single record from [!INCLUDE[crm_md](includes/crm_md.md)] automatically only when **Sync. Only Coupled Records** is disabled and the synchronisation direction is set to Bidirectional or From Integration Table on the **Integration Table Mapping** page for the record. For more information, see [Mapping the Tables and Fields to Synchronise](admin-how-to-modify-table-mappings-for-synchronization.md#create-new-records).     

## To couple multiple records using match-based coupling

Specify the data to synchronise for an entity, such as a customer or contact, by coupling records based on matches. Refine the matches by making the search case sensitive, and assigning a priority for each match. If no match is found, you can also specify that you want to create the entity in Dataverse. For more information, go to [Customise the match-based coupling](admin-how-to-set-up-a-dynamics-crm-connection.md#customize-the-match-based-coupling).  

> [!NOTE]
> The match-based coupling process skips records that are already matched. To include those records when you run match-based coupling, uncouple the records and then try again. To learn more about uncoupling records, go to [Uncoupling Records](#uncoupling-records).

1. In [!INCLUDE[prod_short](includes/prod_short.md)], open the list page for the record, such as the Customers or Contacts list pages.
2. Choose the **Match-Based Coupling** action.
3. Fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## To synchronise multiple records  

1. In [!INCLUDE[prod_short](includes/prod_short.md)], open the list page for the record, such as the Customers or Contacts pages.  
2. Select the records that you want to synchronise, and then choose the **Synchronise Now** action.  
3. If records can be synchronised in one direction, select the option that specifies the direction, and then choose **OK**.  

## Uncoupling Records

You can uncouple one or more records from list pages or the **Coupled Data Synchronisation Errors** page by choosing one or more lines and choosing **Delete Coupling**. You can also remove all couplings for one or more table mappings on the **Integration Table Mappings** page.

## See Also  

[Use Dynamics 365 Sales from Business Central](marketing-integrate-dynamicscrm.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]