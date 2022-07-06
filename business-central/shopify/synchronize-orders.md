---
title: Synchronise and fulfil sales orders
description: Set up and run import and processing of sales order from Shopify.
ms.date: 05/27/2022
ms.topic: article
ms.service: dynamics365-business-central
author: edupont04
ms.author: andreipa
ms.reviewer: solsen
ms.openlocfilehash: ce11aa8766550e72cab2f811ef6602dba4271211
ms.sourcegitcommit: 00a8acc82cdc90e0d0db9d1a4f98a908944fd50a
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 06/29/2022
ms.locfileid: "9076321"
---
# <a name="synchronize-and-fulfill-sales-orders"></a>Synchronise and Fulfil Sales Orders

This article describes the necessary settings and steps that you must perform to synchronise and fulfil sales orders from Shopify in [!INCLUDE[prod_short](../includes/prod_short.md)].

## <a name="set-the-import-of-orders-on-the-shopify-shop-card"></a>Set the import of orders on the Shopify Shop Card

A regular Shopify order can have extra amounts on top, such as shipping charges or, if enabled, tips. These amounts will be posted directly to the G/L accounts. Choose the G/L account that should be used for specific transactions:

- **Shipping Cost Account**
- **Sold Gift Card Account**, for more information, see [Gift Card](synchronize-orders.md#gift-cards).
- **Tip account**  

Enable **Auto Create Orders** to automatically create sales documents in [!INCLUDE[prod_short](../includes/prod_short.md)] once the Shopify order is imported.
The sales document in [!INCLUDE[prod_short](../includes/prod_short.md)] contains a link to the Shopify order. If you select the **Shopify Order No. on Doc. Line** field, then this information will be repeated in the sales lines of type *Comment*.

In the **Tax area source** field, you can define priority on how to select tax area code or GST business posting group based on address. This step is relevant for countries with sales tax, but can be used for VAT countries. For more information, see [Tax remarks](synchronize-orders.md#tax-remarks).

### <a name="shipment-method-mapping"></a>Shipment method mapping

The **Shipment method code** for sales documents imported from Shopify can be filled in automatically. You need to configure the **Shipment Method Mapping**.

1. Choose the ![Lightbulb that opens the Tell Me feature 1.](../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Shopify Shops**, and then choose the related link.
2. Select the Shop for which you want to define mapping to open the **Shopify Shop Card** page.
3. Choose the **Shipment Method Mapping** action. The records for shipping methods defined in the [**Shipping**](https://www.shopify.com/admin/settings/payments) settings in your **Shopify admin** gets created automatically.
4. In the **Name** field, you can see the name of the shipping method from Shopify.
5. Enter the **Shipment Method Code** with the corresponding shipping method in [!INCLUDE[prod_short](../includes/prod_short.md)].

> [!NOTE]  
> If multiple shipping charges are associated with a sales order; only one will be selected as the Shipping Method and assigned to the sales document.

### <a name="payment-method-mapping"></a>Payment method mapping

To fill in the **Payment method code** for sales documents imported from Shopify automatically, you need to configure the **Payment method mapping**.

1. Choose the ![Lightbulb that opens the Tell Me feature 1.](../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Shopify Shops**, and then choose the related link.
2. Select the Shop for which you want to define mapping to open the **Shopify Shop Card** page.
3. Choose the **Payment Method Mapping** action.
4. In the **Gateway** and **Credit Card Company** fields, enter the name of the payment method from Shopify. The record gets created automatically when you import shopify orders.
5. Enter the **Payment Method Code** with the corresponding payment method in [!INCLUDE[prod_short](../includes/prod_short.md)].
6. Set the **Priority** for cases when the customer uses multiple means of payment. The payment method with the highest priority gets selected in the sales document. If both payment methods have the same priority, the payment method with the highest amount is used.

### <a name="location-mapping"></a>Location mapping

To fill in the **Location Code** for sales documents imported from Shopify automatically, you need to configure the **Shopify Shop Locations**.

1. Choose the ![Lightbulb that opens the Tell Me feature 1.](../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Shopify Shops**, and then choose the related link.
2. Select the Shop for which you want to configure the mapping of locations to open the **Shopify Shop Card** page.
3. Choose the **Locations** action to open the **Shopify Shop Locations**.
4. Choose the **Get Shopify Locations** action to import all the locations defined in Shopify. You can find them in the [**Locations**](https://www.shopify.com/admin/settings/locations) settings in your **Shopify admin** panel. Note that the location marked as *Default* will be used when importing unfulfilled Shopify orders.
5. Enter the **Default Location Code** with the corresponding location in [!INCLUDE[prod_short](../includes/prod_short.md)].

> [!NOTE]  
> You must configure the location mapping if the **Location Mandatory** toggle is enabled in the **Inventory Setup** card, otherwise you won't be able to create sales documents.

## <a name="run-the-order-synchronization"></a>Run the order synchronisation

The following procedure describes how to import and update the sales orders.

> [!NOTE]  
> Archived orders in Shopify can't be imported. Deactivate the **Automatically archive the order** option in the **Order Processing** section of the **Checkout** settings in your **Shopify admin** panel to make sure that all orders are imported to [!INCLUDE[prod_short](../includes/prod_short.md)]. If you need to import archived orders, use the **Unarchive Orders** action in the [Orders](https://www.shopify.com/admin/orders) page of the Shopify Admin panel.

1. Choose the ![Lightbulb that opens the Tell Me feature 1.](../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Shopify Shops**, and then choose the related link.
2. Select the Shop for which you want to import orders to open the **Shopify Shop Card** page.
3. Choose the **Orders** action.
4. Choose the **Sync Orders From Shopify** action.
5. Define filters on orders as necessary. For example, you can import fully paid orders or the ones with a low risk level.
6. Choose the **OK** button.

Alternatively, you can search for the **Sync Orders From Shopify** batch job.

You can schedule the task to be performed in an automated manner. For more information, see [Schedule recurring tasks](background.md#to-schedule-recurring-tasks).

## <a name="review-imported-orders"></a>Review imported orders

Once the import is completed, you can explore the Shopify order and find all related information. For example, find the payment transactions, shipping costs, risk level, or fulfillments if the order was already fulfilled in Shopify. You can also see any order confirmation that has been sent to the customer by choosing the **Shopify Status Page** action.

> [!NOTE]  
> You can navigate to the **Shopify Orders** window directly and you'll see orders with the *open* status from all shops. To review completed orders, you need to open the **Shopify Orders** page from the specific **Shopify Shop Card** window.

## <a name="create-sales-documents-in-business-central"></a>Create sales documents in Business Central

If the **Auto Create Orders** toggle is enabled on the **Shopify Shop Card**, [!INCLUDE[prod_short](../includes/prod_short.md)] tries to create a sales document once the order is imported. If the process runs into issues, such as if a customer or product is missing, you'll need to fix the problem. Then you can try to create the sales order again.

### <a name="to-create-sales-documents"></a>To create sales documents

1. Choose the ![Lightbulb that opens the Tell Me feature 1.](../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Shopify Shops**, and then choose the related link.
2. Select the Shop for which you want to synchronise orders to open the **Shopify Shop Card** page.
3. Choose the **Orders** action.
4. Select the order for which you want to create a sales document and choose the **Create Sales Documents** action.
5. Choose **Yes**.

If the Shopify order requires fulfillment, a **Sales Order** will be created. For fulfilled Shopify orders, such as those orders that contain only a gift card or which are already handled in Shopify, a **Sales Invoice** gets created.

A sales document is now created and can be managed by using the standard [!INCLUDE[prod_short](../includes/prod_short.md)] functionalities.

### <a name="manage-missing-customers"></a>Manage missing customers

If your settings prevent creating a customer automatically and a proper existing customer can't be found, you'll assign a customer to Shopify order manually. There are a few options:

- You can assign the **Sell-to Customer No.** directly in the **Shopify Order** by choosing a customer from the list of existing customers.
- You can select a customer template code, create, and assign the customer via the **Create new customer** action in the **Shopify Orders** page.
- You can map an existing customer to the related **Shopify Customer** in the **Shopify Customers** window and then choose the **Find Mapping** action in the **Shopify Orders** page.

### <a name="tax-remarks"></a>Tax remarks

While the imported Shopify order contains information about taxes, the taxes get recalculated when you create the sales document. That recalculation makes it important that the GST/tax settings are correct in [!INCLUDE[prod_short](../includes/prod_short.md)].

- Multiple product tax/GST rates. For example, some product categories are liable for reduced tax rates. Those items must exist in [!INCLUDE[prod_short](../includes/prod_short.md)] and be mapped to Shopify products. Otherwise, with automatic creation of missing items, the GST product posting group will be used.

- Address-dependent tax rates. Use the **Tax area priority** field together with **Customer Templates** table to overwrite standard logic that fills in the **Tax Area Code** in the sales document. The **Tax area priority** field specifies the priority from where the function should take the information about the country/region and state/province. Then the corresponding record in the Shopify customer templates is found and the **Tax Area Code**, **Tax Liable**, and **GST Bus. Posting Group** is used when a sales document is created.

- Price including Tax. The **Prices including Tax**/**Prices including GST** field in the created sales document doesn't depend on the customer, but on the **Customer Template** from the Shopify Shop Card or Customer template per country.

### <a name="impact-of-edits-of-orders"></a>Impact of edits of orders

|Edit|Impact|
|------|-----------|
|In Shopify, change the fulfillment location | Original location will be synched to [!INCLUDE[prod_short](../includes/prod_short.md)]. |
|In Shopify, edit an order and change quantity| Order header and supplementary tables will be updated in [!INCLUDE[prod_short](../includes/prod_short.md)], lines won't. |
|In Shopify, edit an order and add new item | Order header will be updated, lines won't. |
|In [!INCLUDE[prod_short](../includes/prod_short.md)], change the location to another location, mapped to the Shopify Locations. Post shipment. | After synchronising the fulfilment, location will be updated in Shopify. |
|In [!INCLUDE[prod_short](../includes/prod_short.md)], change the location to another location, not mapped to the Shopify Locations. Post shipment. | The fulfilment won't be synchronised to Shopify. |
|In [!INCLUDE[prod_short](../includes/prod_short.md)], change decrease quantity. Post shipment. | The Shopify order will be marked as partially fulfilled. |
|In [!INCLUDE[prod_short](../includes/prod_short.md)], add a new item. Post shipment. | The Shopify order will be marked as fulfilled. Lines won't be updated. |

## <a name="synchronize-shipments-to-shopify"></a>Synchronise shipments to Shopify

When a sales order that is created from a Shopify order is shipped, you can synchronise the shipments to Shopify.

1. Choose the ![Lightbulb that opens the Tell Me feature 1.](../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sync Shipments to Shopify**, and then choose the related link.
2. Define the filters on shipments as necessary. For example, you can update a shipment posted at a specific date.
3. Choose the **OK** button.

The order in Shopify will be marked as fulfilled. The customer automatically receives a shipment notice email or text message (SMS). If a Shipping agent and a Tracking code are specified on the shipment, the tracking information is included in the email.

> [!NOTE]  
> Remember to run **Synchronise Orders from Shopify** to update the fulfilment status of order in [!INCLUDE[prod_short](../includes/prod_short.md)]. The connector functionality also archives completely paid and fulfilled orders in both Shopify and in [!INCLUDE[prod_short](../includes/prod_short.md)] provided the conditions are met.

### <a name="shipping-agents-and-tracking-url"></a>Shipping agents and tracking URL

If the **Posted Sales Shipment** document contains the **Shipping Agent Code** and/or **Package Tracking No.**, this information will be sent to Shopify and to the end-customer in the shipping confirmation email.

The tracking company is populated based on the Shipping Agent record with the following priorities (from highest to lowest):

- **Shopify Tracking Company**
- **Name**
- **Code**

If the **Package Tracking URL** field is filled in for the Shipping agent record, then the shipping confirmation will contain a tracking URL as well.

## <a name="gift-cards"></a>Gift cards

In the Shopify shop you can sell gift cards, which can be later used to pay for real products.

When dealing with gift cards, it's important to enter a value in the **Sold Gift Card Account** field in the **Shopify Shop Card** window. The sold gift card will be synchronised together with orders in line. An applied gift card will also be imported with the order, but now as a transaction. Notice that the gift card doesn't reduce the amount to invoice.

To review the issued and applied gift cards, choose the ![Lightbulb that opens the Tell Me feature.](../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Gift Cards**, and then choose the related link.

## <a name="transactions"></a>Transactions

The payment transactions that took place at Shopify are synchronised together with the orders and can be viewed from the *Shopify Orders* page.

To review all transactions, choose the ![Lightbulb that opens the Tell Me feature 1.](../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Transactions**, and select the related link.

## <a name="payouts"></a>Payouts

If your store has Shopify payments enabled, you'll receive payments through *Shopify Payouts* when a customer pays using Shopify payments and accelerated checkouts.

1. Choose the ![Lightbulb that opens the Tell Me feature 1.](../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Shopify Shops**, and then choose the related link.
2. Select the Shop for which you want to synchronise payouts to open the **Shopify Shop Card** page.
3. Choose the **Sync Payouts** action.

To review all payouts, choose the ![Lightbulb that opens the Tell Me feature.](../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Payouts**, and select the related link.

## <a name="see-also"></a>See also

[Get Started with the Connector for Shopify](get-started.md)  
