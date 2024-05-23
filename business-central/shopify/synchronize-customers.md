---
title: Synchronise customers and companies
description: Import customers from or export to Shopify.
ms.date: 03/25/2024
ms.topic: article
ms.service: dynamics-365-business-central
ms.search.form: '30105, 30106, 30107, 30108, 30109,'
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bholtorf
---

# Synchronise customers and companies

When you import an order from Shopify, getting the information about the customer is essential for further processing the document in [!INCLUDE[prod_short](../includes/prod_short.md)]. There are two main options for doing so, and several combinations:

* Use a special customer for all orders.
* Import the customer information from Shopify. This option is also available when you export customers to Shopify from [!INCLUDE[prod_short](../includes/prod_short.md)].

Shopify allows you to run your business to business (B2B) and direct to customer (DTC) business from one place with the power and ease of Shopify's all-in-one platform. Shopify Connector also works with different flavors of e-commerce.

While Shopify has two entities—customer and company—[!INCLUDE[prod_short](../includes/prod_short.md)] has only the customer entity, which affects how synchronisation works.

When you run DTC, the buyer is created in Shopify as a customer. The customer is then imported to [!INCLUDE[prod_short](../includes/prod_short.md)] as a Shopify customer, and linked or converted to a customer.

If you run B2B, the buyer is created in Shopify as a customer linked to a company. The customer is imported to [!INCLUDE[prod_short](../includes/prod_short.md)] as a Shopify customer, and the company is imported to [!INCLUDE[prod_short](../includes/prod_short.md)] as a Shopify company and linked or converted to a customer.

To export a customer from [!INCLUDE[prod_short](../includes/prod_short.md)] to Shopify, the steps are different depending on what you want to do:

* Export a customer as a Shopify customer for DTC.
* Export a customer as a company and customer pair for the B2B flow.

## Important settings when importing DTC customers from Shopify

Whether you import customers from Shopify in bulk or when you import orders, use the following settings to manage the process:

|Field|Description|
|------|-----------|
|**Customer Import from Shopify**|Select **All Customers** if you plan to import customers from Shopify in bulk; either manually using the **Sync Customers** action or via the job queue for recurring updates. Regardless of the selection, the customer information will always be imported together with the order. However, the use of this information depends on the **Shopify Customer Templates** and settings in the **Customer Mapping Type** field.|
|**Customer Mapping Type**|Define how you want the connector to perform the mapping.</br></br>- **By Email/Phone** if you want the connector to use email account and telephone information to map the imported Shopify customer to a customer in Business Central.</br></br>- **By Bill-to Info** if you want the connector to use the address of the invoice recipient to map the imported Shopify customer to an existing customer in Business Central.</br></br>- **Always Take the Default Customer** if you want the system to use a customer from the **Default Customer No.** field. |
|**Shopify Can Update Customers**| Select this field if you want the connector to update the customers it finds when either of the **By Email/Phone** or **By Bill-to Info** options are selected in the **Customer Mapping Type** field.|
|**Auto Create Unknown Customers**| Select this field if you want the connector to create missing customers when the **By Email/Phone** or **By Bill-to Info** options are selected in the **Customer Mapping Type** field. A new customer is created using imported data and the **Customer Template Code** defined on the **Shopify Shop Card** or **Shopify Customer Template** pages. Notice that the Shopify customer must have at least one address. Orders created via Shopify POS sales channel are often missing address details. If this option isn't enabled, you must create a customer manually and link it to the Shopify customer.|
|**Customer.Company Template Code**|Use this field together with **Auto Create Unknown Customers**.</br></br>Choose the default template to use for automatically created customers. Make sure the selected template contains the mandatory fields such as **Gen. Business Posting Group**, **Customer Posting Group**, and Goods and Services Tax (GST) or tax-related fields.</br></br>You can define templates per country/region on the **Shopify Customer Templates** page, which helps calculate taxes correctly.</br></br>Learn more at [Set Up Taxes](setup-taxes.md).|

### Customer template per country/region

Some settings can be defined at the country/regional level or a state/province level. The settings can be configured in [Shipping and Delivery](https://www.shopify.com/admin/settings/shipping) in Shopify.

You can do the following for each customer using the **Shopify Customer Template**:

1. Specify the **Default Customer No.**, which takes priority over the selection in the **Customer Import from Shopify** and **Customer Mapping Type** fields. It's used in the imported sales order.
2. Define the **Customer Template Code**, which is used to create missing customers if **Auto Create Unknown Customers** is enabled. If the **Customer Template Code** is empty, then the function uses the **Customer Template Code** defined on the **Shopify Shop Card**. The system first tries to find a template for the **Country/Region Code** for the default address. If it doesn't find a template, it uses the first address.
3. In some cases, the **Customer Template Code** defined for a country/region isn't enough to ensure correct tax calculations (for example, for countries/regions with sales tax). In this case, including **Tax Area** could be a useful addition.
4. The **Tax Area** field also contains a **Country Code** and **County Name** pair. This pair is useful when the connector needs to convert a code to a name, or vice versa.

> [!NOTE]  
> The country codes are ISO 3166-1 alpha-2 country codes. Learn more at [Country Code](https://help.shopify.com/en/api/custom-storefronts/storefront-api/reference/enum/countrycode).

## Important settings when exporting DTC customers to Shopify

You can export existing customers to Shopify in bulk. In each case, a customer and one default address are created. You can manage the process using the following settings:

|Field|Description|
|------|-----------|
|**Can update Shopify Customers**| Enable this option if you want to generate updates later from Business Central for customers that already exist in Shopify.|

The following are requirements for exporting a customer:

* The customer must have a valid email address.
* When exporting customers with addresses that include provinces/states, make sure that **ISO Code** is filled in for countries/regions.|
* When a country/region is selected on the customer card, make sure that **ISO Code** is specified. For local customers with a blank country/region, Shopify Connector uses the country/region specified on the **Company Information** page.
* If the customer has a phone number, the number must be unique because Shopify won't accept a second customer with the same phone number.
* If the customer has a phone number, it must be in the E.164 format. Different formats are supported if they represent a number that can be dialed from anywhere in the world. The following formats are valid:

  * xxxxxxxxxx
  * +xxxxxxxxxxx
  * (xxx)xxx-xxxx
  * +x xxx-xxx-xxxx

After you create the customers in Shopify, you can send them direct invitations to encourage them to activate their accounts.

### Populate customer information in Shopify

A customer in Shopify has a first name, family name, email, and/or phone number. You can enter first and family names from the customer card in [!INCLUDE[prod_short](../includes/prod_short.md)].

|Priority|Field in the customer card|Description|
|------|------|-----------|
|1|**Contact Name**|Highest priority, if the **Contact Name** field is filled and the **Contact Source** field in the **Shopify Shop Card** contains either the *First Name and Last Name* or *Last Name and First Name* option to define how to split the values.|
|2|**Name 2**|If the **Name 2** field is filled in and the **Name 2 Source** field in the **Shopify Shop Card** contains either the *First Name and Last Name* or *Last Name and First Name* option to define how to split the values.|
|3|**Name**|Lowest priority, if the **Name** field is filled and the **Name Source** field in the **Shopify Shop Card** contains either the *First Name and Last Name* or *Last Name and First Name* options to define how to split the values.|

A customer in Shopify also has a default address. The address might contain a company and address in addition to their first name, family name, email, and/or phone number. You can populate the **Company** field based on data from the customer card in [!INCLUDE[prod_short](../includes/prod_short.md)].

|Priority|Field in the customer card|Description|
|------|------|-----------|
|1|**Name**|Highest priority, if the **Name Source** field in the **Shopify Shop Card** contains *Company Name*.|
|2|**Name 2**|Lowest priority, if the **Name 2 Source** field in the **Shopify Shop Card** contains *Company Name*.|

For addresses where the county/province is used, select **Code** or **Name** in the **County Source** field on the **Shopify Shop Card** page. The code or name specifies the type of data stored in [!INCLUDE[prod_short](../includes/prod_short.md)] in the **County** field. Remember to initialise customer templates per country/region so that the county code/name mapping is ready. 

## Export DTC customers to Shopify

### Initial sync of customers from Business Central to Shopify

1. Go to the search ![Lightbulb that opens the Tell Me feature.](../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Shopify Customers**, and choose the related link.
2. Choose the **Add Customer** action.
3. In the **Shop Code** field, enter the code. If you open the **Shopify Customers** window from the **Shop Card** page, the shop code is populated automatically.
4. Define filters on customers as required. For example, you can filter by Country/Region code.
5. Choose **OK**.

The resulting customers are automatically created in Shopify with addresses.

> [!NOTE]  
> The initial sync of customers from [!INCLUDE[prod_short](../includes/prod_short.md)] to Shopify doesn't consider the **Can Update Shopify Customers** settings.

### Sync customers

1. Choose the ![Lightbulb that opens the Tell Me feature 1.](../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Shopify shop**, and then choose the related link.
2. Select the specific shop for which you want to synchronise customers.
3. Choose the **Sync Customers** action.

Alternatively, use the **Start Customer Sync** action on the **Shopify Customers** window or search for the **Sync Customers** batch job.

You can schedule the task to be performed in an automated manner. Learn more at [Schedule recurring tasks](background.md#to-schedule-recurring-tasks).

## B2B Companies

If you use B2B in Shopify, you can create companies in addition to customers. You can link one or more individual customers to a company. You can also define payment terms, locations, and catalogues.

## Important settings when importing B2B companies from Shopify

Whether you import companies from Shopify in bulk or when you import orders, use the settings in the following table to manage the process.

|Field|Description|
|------|-----------|
|**Company Import from Shopify**|Select **All Companies** if you plan to import customers from Shopify in bulk, either manually using the **Sync Companies** action or via the job queue for recurring updates. Regardless of the selection, the customer information is always imported together with the order. However, the use of this information depends on the **Shopify Company Templates** and settings in the **Company Mapping Type** field.|
|**Company Mapping Type**|Define how you want the connector to do the mapping.</br></br>- **By Email/Phone** if you want the connector to map the imported Shopify companies to an existing customer in Business Central using email and phone from the main contact.</br></br>- Select **Always Take the Default Company** if you want the system to use the company in the **Default Company No.** field. |
|**Shopify Can Update Company**| Select this field if you want the connector to update the customers it finds when the **By Email/Phone** option is selected in the **Company Mapping Type** field.|
|**Auto Create Unknown Companies**| Select this field if you want the connector to create new customers when the **By Email/Phone** option is selected in the **Company Mapping Type** field. A new customer is created using the imported data and the **Customer/Company Template Code** defined on the **Shopify Shop Card** or **Shopify Customer Template** pages.|
|**Customer/Company Template Code**|Use this field together with **Auto Create Unknown Company**.</br></br>- Choose the default template to use for automatically created customers. Make sure the mandatory fields are filled in on the template, such as the **Gen. Business Posting Group**, **Customer Posting Group**, **Goods and Services Tax (GST)** or other tax-related fields.</br></br>- You can define templates per country/region on the **Shopify Customer Templates** page, which is useful for proper tax calculation.</br></br>Learn more at [Set up Taxes](setup-taxes.md).|

> [!NOTE]  
> The company must have a main contact. Otherwise, the connector skips to company.
> Only one oldest location is imported.
> Only the main contact is imported.

## Important settings when exporting B2B companies to Shopify

You can export existing customers to Shopify in bulk as a company. In each case, a company and one default location are created and one main contact. It's also possible to create a catalogue.

|Field|Description|
|------|-----------|
|**Can update Shopify Companies**| Enable this option if you want to generate updates later from Business Central for companies that already exist in Shopify.|
|**Default Contact Permissions**| Specify which permissions must be assigned to the main contact; you can choose between **None**, **Ordering only**, and **Location admin**.|
|**Auto Create Catalogue**| Enable this option if you want to create a catalogue that includes all products. A catalogue is created for each exported company.|

## Export a B2B company to Shopify

### Initial sync of B2B companies from Business Central to Shopify

1. Go to the search ![Lightbulb that opens the Tell Me feature.](../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Shopify Company**, and choose the related link.
2. Choose the **Add Company** action.
3. In the **Shop Code** field, enter the code. If you open the **Shopify Company** window from the **Shop Card** page, the shop code is populated automatically.
4. Define filters on the customer as required. For example, you can filter by Country/Region code.
5. Choose **OK**.

The resulting company and customers are automatically created in Shopify.

> [!NOTE]  
> The initial sync of companies from [!INCLUDE[prod_short](../includes/prod_short.md)] to Shopify doesn't consider **Can Update Shopify Company** settings.

### Sync B2B company

1. Choose the ![Lightbulb that opens the Tell Me feature 1.](../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Shopify shop**, and then choose the related link.
2. Select the specific shop for which you want to synchronise customers.
3. Choose the **Sync Company** action.

Alternatively, use the **Start Company Sync** action on the **Shopify Company** page or search for the **Sync Company** batch job.

You can schedule the task to run in an automated way. Learn more at [Schedule recurring tasks](background.md#to-schedule-recurring-tasks).

## See also

[Get Started with the Connector for Shopify](get-started.md)  
