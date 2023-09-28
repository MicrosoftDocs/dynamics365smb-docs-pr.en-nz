---
title: Troubleshooting the Shopify and Business Central Synchronisation
description: Learn what to do if something goes wrong when you synchronise data between Shopify and Business Central.
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bholtorf
ms.topic: how-to
ms.date: 04/24/2023
ms.custom: bap-template
ms.search.form: '30118, 30119, 30120, 30101, 30102'
---

# <a name="troubleshooting-the-shopify-and-business-central-synchronization"></a>Troubleshooting the Shopify and Business Central Synchronisation

You might run into situations where you need to troubleshoot issues when synchronising data between Shopify and [!INCLUDE[prod_short](../includes/prod_short.md)]. This page defines troubleshooting steps for some typical scenarios.

## <a name="run-tasks-in-the-foreground"></a>Run tasks in the foreground

1. Choose the ![Lightbulb that opens the Tell Me feature 1.](../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Shopify Shop**, and choose the related link.
2. Select the shop for which you want to troubleshoot to open the **Shopify Shop Card** page.
3. Turn off the **Allow Background Syncs** toggle.

Now, when the sync action is triggered the task will run in the foreground. If an error occurs, you'll get an error dialogue with a **Copy details** link. Use the link to copy information to a text editor for the further analysis.

## <a name="logs"></a>Logs

If a synchronisation task fails, you can turn on the **Log Enabled** toggle on the **Shopify Shop Card** page to activate logging. Then you can manually trigger the synchronisation task and review logs.

### <a name="to-enable-logging"></a>To enable logging

1. Choose the ![Lightbulb that opens the Tell Me feature 1.](../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Shopify Shop**, and choose the related link.
2. Select the shop for which you want to troubleshoot to open the **Shopify Shop Card** page.
3. Turn on the **Log Enabled** toggle.

### <a name="to-review-logs"></a>To review logs

1. Choose the ![Lightbulb that opens the Tell Me feature 1.](../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Shopify Log Entries**, and choose the related link.
2. Select the related log entry, and then open the **Shopify Log Entry** page.
3. Review the request, status code and description, and response values. You can download the request and response values as files in a text format.

Later, remember to turn off logging to avoid negative effect on performance and increase in database size.

From the **Shopify Log Entries** page, you can trigger the deletion of all log entries, or entries that are older than seven days.

## <a name="data-capture"></a>Data capture

Regardless of whether **Log Activated** is turned on, some Shopify responses are always logged. You can inspect or download the logs from the **Data Capture List** page.

Choose the **Retrieved Shopify Data** action on one of the following pages:

- **Shopify order**
- **Shopify order line**
- **Shopify fulfillments**
- **Shopify order shipping costs**
- **Shopify order transactions**
- **Shopify return**
- **Shopify return line**
- **Shopify refund**
- **Shopify refund line**
- **Shopify payouts**
- **Shopify payment transactions**
- **Shopify transactions**

## <a name="reset-sync"></a>Reset sync

For optimal performance, the connector imports only customers, products, and orders that were created or changed after the last synchronisation. On the **Shopify Shop Card** page, there are functions that change the date/time of the last synchronisation, or completely reset it. This function ensures that all data synchronises, rather than just the changes since the last sync.

This function only applies to syncs from Shopify to [!INCLUDE[prod_short](../includes/prod_short.md)]. It can be useful if you need to restore deleted data such as products, customers, or deleted orders.

## <a name="request-the-access-token"></a>Request the access token

If [!INCLUDE[prod_short](../includes/prod_short.md)] won't connect to your Shopify account, try to request the access token from Shopify. You might need to request a new token if there were changes to the security keys or required permissions (application scopes).

1. Choose the ![Lightbulb that opens the Tell Me feature 1.](../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Shopify shops**, and choose the related link.
2. Select the shop for which you want to get the access token to open the **Shopify Shop Card** page.
3. Choose the **Request Access** action.
4. If prompted, sign in to your Shopify account.

The **Has AccessKey** toggle will be activated.

## <a name="verify-and-enable-permissions-to-make-http-requests-in-a-non-production-environment"></a>Verify and enable permissions to make HTTP requests in a non-production environment

To work correctly, the Shopify Connector extension requires permission to make HTTP requests. When testing in a sandbox, HTTP requests are prohibited for all extensions.

1. Choose the ![Lightbulb that opens the Tell Me feature 1.](../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Extension Management**, and then choose the related link.
2. Select the **Shopify Connector** extension.
3. Choose the **Configure** action to open the **Extension Setting** page.
4. Make sure that the **Allow HTTPClient Requests** toggle is enabled.

## <a name="rotate-the-shopify-access-token"></a>Rotate the Shopify access token

The following procedures describe how to rotate the access token used by the Shopify connector to access your Shopify online shop.

### <a name="in-shopify"></a>In Shopify

1. From your **Shopify Admin**, go to [Apps](https://www.shopify.com/admin/apps).
2. Select **Delete** in the row with the **Dynamics 365 Business Central** app.
3. Select **Delete** in the message that appears.

### <a name="in-"></a>In [!INCLUDE[prod_short](../includes/prod_short.md)]

1. Choose the ![Lightbulb that opens the Tell Me feature 1.](../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Shopify shops**, and then choose the related link.
2. Select the shop for which you want to rotate the access token to open the **Shopify Shop Card** page.
3. Choose the **Request Access** action.
4. If prompted, sign in to your Shopify account, review privacy and permissions, and then choose the **Install App** button.

## <a name="known-issues"></a>Known issues

### <a name="error-the-sales-header-does-not-exist-identification-fields-and-values-document-typequotenoyour-shopify-store"></a>Error: The Sales Header does not exist. Identification fields and values: Document Type='Quote',No.='YOUR SHOPIFY STORE'

To calculate prices, the Shopify Connector creates a temporary sales document (quote) for a temporary customer (Shop Code) and uses the standard price calculation logic. If a third-party extension subscribes to events on a temporary sales document, the header might not be available. We recommend that you contact the extension provider. Ask them to modify their code to check for temporary records. In some cases, they just need to add the `IsTemporary` method ìn the right place. To learn more about `IsTemporary`, go to [IsTemporary](/dynamics365/business-central/dev-itpro/developer/methods-auto/record/record-istemporary-method). 

To verify that the problem is caused by a third-party extension, use the **Copy information to clipboard** link in the error message and copy the content to a text editor. The information contains an **AL call stack**, where the top line is the line where the error occurred. The following example shows an AL call stack.

AL call stack:

```AL
[Object Name]([Object type] [Object Id]).[Function Name] line [XX] - [Extension Name] by [Publisher] 
...
"Sales Line"(Table 37)."No. - OnValidate"(Trigger) line 98 - Base Application by Microsoft
"Shpfy Product Price Calc."(CodeUnit 30182).CalcPrice line 20 - Shopify Connector by Microsoft
"Shpfy Create Product"(CodeUnit 30174).CreateTempProduct line 137 - Shopify Connector by Microsoft
"Shpfy Create Product"(CodeUnit 30174).CreateProduct line 5 - Shopify Connector by Microsoft
"Shpfy Create Product"(CodeUnit 30174).OnRun(Trigger) line 12 - Shopify Connector by Microsoft
"Shpfy Add Item to Shopify"(Report 30106)."Item - OnAfterGetRecord"(Trigger) line 2 - Shopify Connector by Microsoft
"Shpfy Products"(Page 30126)."AddItems - OnAction"(Trigger) line 5 - Shopify Connector by Microsoft
```

Remember to the share AL call stack information with the supplier of the extension.

### <a name="error-gen-bus-posting-group-must-have-a-value-in-customer-your-shopify-store-it-cannot-be-zero-or-empty"></a>Error: Gen. Bus. Posting Group must have a value in Customer: 'YOUR SHOPIFY STORE'. It cannot be zero or empty

On the **Shopify Shop Card** page, in the **Customer Template Code** field, choose the template that has **Gen. Bus. Posting Group** populated. The customer template is used to create customers and to calculate sales prices on sales documents.

### <a name="error-importing-data-to-your-shopify-shop-isnt-enabled-go-to-the-shop-card-to-enable-it"></a>Error: Importing data to your Shopify shop isn't enabled. Go to the shop card to enable it

On the **Shopify Shop Card** page, turn on the **Allow Data Sync to Shopify** toggle. This setting helps protect the online shop from getting demo data from [!INCLUDE[prod_short](../includes/prod_short.md)].

### <a name="error-oauth-error-invalid_request-could-not-find-shopify-api-application-with-api_key"></a>Error: Oauth error invalid_request: Could not find Shopify API application with api_key

It seems you use the [Embed App](/dynamics365/business-central/dev-itpro/deployment/embed-app-overview), where the client URL has the format: `https://[application name].bc.dynamics.com`. The Shopify connector doesn't work for Embed Apps. To learn more, go to [Which Microsoft products are the Shopify connector available for?](shopify-faq.md#which-microsoft-products-are-the-shopify-connector-available-for).

### <a name="error-internal-error-looks-like-something-went-wrong-on-our-end-request-id-xxxxxxxx-xxxx-xxxx-xxxx-xxxx"></a>Error: Internal Error. Looks like Something Went Wrong on Our End. Request Id: XXXXXXXX-XXXX-XXXX-XXXX-XXXX

Please contact Shopify support within 7 days of experiencing this error, and provide the Request ID. To learn more, go to [Support options for Shopify](shopify-faq.md#shopify).

### <a name="error-oauth-error-invalid_request-your-account-does-not-have-permission-to-grant-the-requested-access-for-this-app"></a>Error: Oauth error invalid_request: Your account does not have permission to grant the requested access for this app.

It seems that user which requests access doesn’t have rights to manage apps (ability to manage and install apps and channels, as well as potentially approve app charges). You may be able to resolve this issue by installing the app as the account owner. Alternatively you can check the **App permission** for the user in the [**User and permissions**](https://www.shopify.com/admin/settings/account) settings in your **Shopify admin**.  

## <a name="see-also"></a>See also

[Get Started with the Connector for Shopify](get-started.md)
