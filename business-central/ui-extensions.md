---
title: Installing Extensions to Customise Business Central  | Microsoft Docs
description: Learn about adding functionality and customising Business Central  by installing extensions.
documentationcenter: ''
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: app, add-in, manifest, customize
ms.date: 11/27/2018
ms.author: edupont
ms.openlocfilehash: f093a9ce2a654d5ee693ee91f32e87f6546279d1
ms.sourcegitcommit: d09f5ee0e164c7716f4ccb2ed71e2f9732a1f4f9
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 03/19/2019
ms.locfileid: "852463"
---
# <a name="customizing-business-central-using-extensions"></a>Customising Business Central Using Extensions
You can change [!INCLUDE[d365fin](includes/d365fin_md.md)] by installing extensions that add functionality, changes behavior, or gives you access to new online services, for example.
When you first launch [!INCLUDE[d365fin](includes/d365fin_md.md)], some extensions are already installed for you. Over time, more extensions will be made available to you, and you can then choose if you want to use the extension or not.

For example, Microsoft provides an extension that provides integration with PayPal Payments Standard. This extension is installed by default.
But if another extension is made available that offers integration with another payment service, you can install the new extension and then choose which of the two services to use.  

You manage the extensions on the **Extension Management** page. You can access this page from Home. Alternatively, choose the **Search for Page or Report** icon ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") in the top right corner, enter **Extension**, and then choose the related link.  

> [!NOTE]  
>   If you think you should have access to an extension but you cannot find its functionality, check the **Extension Management** page - if the extension is not listed there, you can install it as described in the following section.  

## <a name="installing-an-extension"></a>Installing an Extension
You can get new extensions from the marketplace at [AppSource.microsoft.com](https://appsource.microsoft.com/en-us/marketplace/apps?src=dynamics365website&product=dynamics-365-business-central). Here, you can see all available extensions for [!INCLUDE[d365fin](includes/d365fin_md.md)], and you can get apps, extensions, and content packs for other Microsoft products. Set the relevant filters, take a look at the information for each extension, and get an extension for your [!INCLUDE[d365fin](includes/d365fin_md.md)].  
> [!NOTE]  
>   Sign in to [AppSource.microsoft.com](https://appsource.microsoft.com/) using the email account that you use for [!INCLUDE[d365fin](includes/d365fin_md.md)]. Use the same email account for other services and products for a smooth experience.  

You can also get to the marketplace from inside [!INCLUDE[d365fin](includes/d365fin_md.md)]. On the **Extension Management** page, you can see the extensions that are currently installed, and you can open the **Extension Marketplace** page that shows the [!INCLUDE[d365fin](includes/d365fin_md.md)] extensions that are currently available in AppSource. If you choose the *More apps* link, you are taken to [AppSource.microsoft.com](https://appsource.microsoft.com/en-us/marketplace/apps?product=dynamics-365%3Bdynamics-365-for-financials&page=1).  

If you choose an extension, you can read about what the extension does, and you can access Help for the extension to learn more. When you choose to get an extension, you must agree to the terms of use. If you get the extension from the AppSource website, you will be signed in to [!INCLUDE[d365fin](includes/d365fin_md.md)] to complete the installation.  

When you install an extension, you might have to set it up, such as specifying an account for use with the **PayPal Payments Standard for [!INCLUDE[d365fin](includes/d365fin_md.md)]** extension.
Other extensions simply add fields to an existing page, or they add a new page, for example.   

If you uninstall an extension, and you then change your mind, you can install it again. When you uninstall an extension that you have been using, the data is preserved so that if you install the extension again, your data is still available.  

Some extensions are provided by Microsoft, and other extensions are provided by [other companies](ui-extensions-other.md). All extensions are tested before they are made available to you, but we recommend that you access the links that are provided with each extension to learn more about the extension before you choose to install it.  

Microsoft provides the following extensions:  

* [Dynamics GP Data Migration](ui-extensions-dynamicsgp-data-migration.md)  
* [Envestnet Yodlee Bank Feeds](ui-extensions-yodlee-bank-feeds.md)  
* [Microsoft Pay](ui-extensions-microsoft-pay-payments.md)  
* [PayPal Payments Standard](ui-extensions-paypal-payments-standard.md)  
* [QuickBooks Data Migration](ui-extensions-quickbooks-data-migration.md)  
* [Sales and Inventory Forecast](ui-extensions-sales-forecast.md)  
* [Ceridian Payroll](ui-extensions-ceridian-payroll.md)  
* [Quickbooks Payroll File Import](ui-extensions-quickbooks-payroll.md)  
* [WorldPay Payments Standard](ui-extensions-worldpay-payments-standard.md)  
* [GetAddress.io UK Postcodes](ui-extensions-getaddressio.md)  
* [QuickBooks Online Data Migration](ui-extensions-quickbooks-online-data-migration.md)  
* [Accountant Portal](ui-extensions-accountant-portal.md)  
* [Image Analyser](ui-extensions-image-analyzer.md)  
* [Payments and Reconciliations (DK)](ui-extensions-payments-reconciliation-formats-dk.md)  
* [C5 Data Migration](ui-extensions-c5-data-migration.md)  
* [Essential Business Insights](ui-extensions-essential-business-insights.md)  
* [Late Payment Predictions](ui-extensions-late-payment-prediction.md  )

> [!NOTE]  
>  New extensions are not available in AppSource immediately after we announce an update. You can keep an eye out for the extensions at [AppSource.microsoft.com](https://appsource.microsoft.com/en-us/marketplace/apps?product=dynamics-365%3Bdynamics-365-for-financials&page=1).

## <a name="see-also"></a>See Also
[Extending Dynamics 365 Business Central](about-develop-extensions.md)  
[Business Central Extensions by Other Providers](ui-extensions-other.md)  
[Set Up the Envestnet Yodlee Bank Feeds Service](bank-how-setup-bank-statement-service.md)  
[Enable Customer Payment Through PayPal](sales-how-enable-payment-service-extensions.md)  
[Migrating Business Data from Other Finance Systems](across-import-data-configuration-packages.md)  
[Setting Up the GetAddress.io UK Postcode extension](LocalFunctionality/UnitedKingdom/uk-setup-postal-code-service.md)  
[[!INCLUDE[d365fin](includes/d365fin_md.md)] Extensions by Other Providers](ui-extensions-other.md)  
[Getting Started](product-get-started.md)  

## [!INCLUDE[d365fin](includes/free_trial_md.md)]  
