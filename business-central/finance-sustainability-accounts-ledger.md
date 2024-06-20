---
title: Chart of sustainability accounts and ledger
description: 'Learn how to manage the chart of sustainability accounts (CoSA), categories and subcategories, and details about sustainability ledger entries.'
author: altotovi
ms.topic: conceptual
ms.devlang: al
ms.search.keywords: 'Sustainability, ESG, emission, GHG, CSRD, CoA, Chart, Account, Ledger'
ms.search.form: '6210, 6213, 6214, 6220'
ms.date: 05/07/2024
ms.author: altotovi
ms.service: dynamics-365-business-central
ms.reviewer: bholtorf
---

# Chart of sustainability accounts and ledger

## Chart of sustainability accounts

The chart of sustainability accounts (CoSA) forms the foundational structured list that is used to record all emissions data. It serves as a framework that categorises and organises sustainability accounts based on their attributes, such as the scope or other groupings. Each account is typically assigned a unique code or number for easy reference and tracking. It has the same structure as a traditional chart of accounts but is customised specifically to monitor sustainability-related data and metrics in an organisation.

Users can add sustainability account categories and sustainability account subcategories to define how the system behaves. In this way, they can select dedicated emissions to track, emission factors, formulas, and similar configurations.

> [!NOTE]
> Based on the greenhouse gas (GHG) standards, there are three emission scopes:
>
> - **Scope 1 emissions** include emissions from stationary and mobile combustion, and from inadvertent fugitive emissions.
> - **Scope 2 emissions** include indirect emissions from the generation of energy that is purchased from utility providers.
> - **Scope 3 emissions** include a wide spectrum of emissions, from purchased goods and services and capital goods, to fuel and energy–related activities, to upstream and downstream transportation, to generated waste, to business travel and employee commuting, and so on.

From the CoSA, you can do things such as:

- View reports that show sustainability ledger entries and balances.
- Open the sustainability account card to add or change settings.
- View the category and subcategory for the account. 
- View separate balances for each emission for a single account.
- Add single or multiple dimensions to each account and set dimension filters.

You can add, change, or delete sustainability accounts. However, to prevent discrepancies, you can't delete a sustainability account if one or more ledger entries are associated with it.

### Add or change accounts

1. Select the ![Lightbulb that opens the Tell Me feature 3.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Chart of Sustainability Accounts**, and then select the related link.
2. On the **Chart of Sustainability Accounts** page, you can open each sustainability account, and then add or change settings. Hover over a field to read a short description.

For accounts of the **Total** account type, you must set the **Totalling** field.

For accounts of the **End-Total** type, the Indent function automatically sets the **Totalling** field. After you set up all the accounts, select the **Indent Chart of Sustainability Accounts** action to run the Indent function and set the **Totalling** field.

> [!IMPORTANT]
> The Indent function overwrites the value of all fields for **End-Total** accounts. Therefore, if you entered definitions in the **Totalling** field for **End-Total** accounts before you ran the Indent function, you must enter them again after you run it.

### Delete accounts

You can delete a sustainability account. However, you must first make sure that no ledger entries are associated with it. Business Central prevents you from deleting a sustainability account if one or more ledger entries are associated with it.

## Account categories

Users must add a sustainability account category to each sustainability account to define how the system behaves. They can select emission scopes, dedicated emissions to track, formulas, and similar configurations.

To review sustainability account categories, follow the steps:

1. Select the ![Lightbulb that opens the Tell Me feature 3.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sustainability Account Categories**, and then select the related link.
2. On the **Sustainability Account Categories** page, you can edit the existing list or create a new category. To create a new category, select the **New** action.
3. Set the **Code** and **Description** fields.
4. In the **Emission Scope** field, select one of the scope options.
5. Select the gas emissions that you want to track. Currently, the following options are available: **CO2**, **CH4**, and **N2O**. You can select any combination that you want to track, but you must select at least one emission.
6. In the **Calculation Foundation** field, you can select the calculation foundation (formula) to use for emission calculations if you don't know the accurate emission amount. You can select one of the following options: **Fuel/Electricity**, **Distance**, **Installation**, or **Custom**.

    > [!NOTE]
    > If the set of available formulas in the **Calculation Foundation** field isn't enough, you can extend the field and add more calculations to the system for use in the sustainability journals.

7. If you selected **Custom** in the **Calculation Foundation** field, you can configure a custom description in the **Custom Value** field.

If you set the **Calculation Foundation** field, the following table explains how the system calculates emissions based on the option that you selected. (In this table, *EF* represents the **Emission Factor** value that you can configure on the **Sustainability Account Subcategory** page.)

| Emission Type | Calculation Foundation | Formula | Comment |
|---------------|------------------------|---------|---------|
| **Scope 1** | | | |
| Stationary combustion | Fuel/Electricity | *Emission* = *Fuel* &times; *EF* | *Fuel* = Amount of fuel that is spent for boilers, heaters, thermal oxidizers, and so on |
| Mobile combustion | Fuel/Electricity | *Emission* = *Fuel* &times; *EF* | *Fuel* = Amount of fuel that is spent for on-road or non-road vehicles, rail, and so on |
| | | *Emission* = *Distance* &times; *EF* | *Distance* = Mileage of on-road or non-road vehicles, rail, and so on |
| Fugitive emissions | Installation | *Emission* = *Installation multiplier* &times; *Custom Amount* &divide; 100 &times; *Time Factor* | *Custom Amount* = Assembly losses, annual leak rate, and so on |
| **Scope 2** | | | |
| Utility providers | Fuel/Electricity | *Emission* = *Electricity* &times; *EF* | *Fuel/Electricity* = Electricity quantity, steam quantity, heating unit, and so on |
| | Custom | *Emission* = *Custom Amount* &times; *EF* | *Custom Amount* = Thermal unit, ton-hour, and so on |
| **Scope 3** | | | |
| Purchased goods and services, and capital goods | Custom | *Emission* = *Custom Amount* &times; *EF* | *Custom Amount* = Cost (GL), and so on |
| Upstream transportation and distribution | Distance | *Emission* = *Distance* &times; *EF* | |
| | Distance | *Emission* = *Distance* &times; *Multiplier* &times; *EF* | *Multiplier* = Tons of cargo |
| Downstream transportation and distribution | Distance | *Emission* = *Distance* &times; *EF* | |
| | Distance | *Emission* = *Distance* &times; *Multiplier* &times; *EF* | *Multiplier* = Tons of cargo |
| Waste generated in operations and end-of-life treatment of sold products | Custom | *Emission* = *Custom Amount* &times; *EF* | *Custom Amount* = Waste |
| Business travel and employee commuting | Distance | *Emission* = *Distance* &times; *EF* | *Distance* = Mileage of the used company car, rental car, train, flight, and so on |
| | Custom | *Emission* = *Custom Amount* &times; *EF* | *Custom Amount* = Hotel stays |
| | Fuel/Electricity | *Emission* = *Fuel* &times; *EF* | *Fuel* = Amount of fuel spent in the company car, rental car, and so on |

## Account subcategories

Users must add a sustainability account subcategory to each sustainability account. This subcategory defines the emission factors that are used in the formulas, based on the emission tracking choice in the sustainability account category.

To review sustainability account subcategories, follow the steps:

1. Select the ![Lightbulb that opens the Tell Me feature 3.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sustainability Account Subcategories**, and then select the related link. 
2. On the **Sustainability Account Subcategories** page, you can edit the existing list or create a new category. To create a new category, select the **New** action.
3. Set the **Code** and **Description** fields.
4. Based on the gas emissions that you want to track in the sustainability account category and connect this subcategory with, you can also set one or more emission factors: 

    - **Emission Factor CO2** – The emission factor for carbon dioxide (CO<sub>2</sub>) emission.
    - **Emission Factor CH4** – The emission factor for methane (CH<sub>4</sub>) emission.
    - **Emission Factor N2O** – The emission factor for nitrous oxide (N<sub>2</sub>O) emission.

5. If the subcategory is related to renewable energy, select the **Renewable Energy** field.

> [!NOTE]
> The **Import Data** and **Import From** fields are intended for potential integration with external systems that are used to collect emission factors. However, in **2024 release wave 1**, these fields can't be used as a feature by default.

## Sustainability ledger entries

The sustainability ledger stores the history of all posted sustainability transactions and organises all emission data according to the CoSA. When a user posts the sustainability journal, all crucial data is recorded there. All active reports are generated based on the sustainability ledger entries.

To open this ledger for one specific account, use the **Ledger Entries** action on the **Chart of Sustainability Account** page. To open all the ledger entries, select the ![Lightbulb that opens the Tell Me feature 3.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sustainability Ledger Entries**, and then select the related link. Hover over a field to read a short description.

> [!IMPORTANT]
> After you post your data to the sustainability ledger, you can't delete it. If you made a mistake, you can post a reverse transaction that has the same details but uses the negative sign for the amount.

## See also

[Finance](finance.md)  
[Sustainability management overview](finance-manage-sustainability.md)  
[Sustainability Setup](finance-sustainability-setup.md)  
[How to record emissions](finance-sustainability-journal.md)  
[Work with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
