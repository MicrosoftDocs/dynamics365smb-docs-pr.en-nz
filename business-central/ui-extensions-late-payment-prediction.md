---
title: Predict Late Payments for Sales Documents
description: This article explains how to use our predictive model to predict whether an invoice will be paid on time.
author: brentholtorf
ms.author: bholtorf
ms.reviewer: andreipa
ms.topic: conceptual
ms.search.keywords: 'customer, payment, invoice, sales, invoice, quote'
ms.search.form: '1950, 1951,'
ms.date: 12/06/2023
ms.custom: bap-template
ms.service: dynamics-365-business-central
---
# The Late Payment Prediction Extension

Effectively managing receivables is important to the overall financial health of a business. To reduce outstanding receivables and help you fine-tune your collections strategy, the extension predicts whether to expect late payments. For example, if a payment is predicted to be late, you might decide to adjust the terms of payment or the payment method for the customer.

## Get started

When you open a posted sales document, a notification displays at the top of the page. To use the Late Payment Prediction Extension, opt in by choosing **Enable** in the notification. Alternatively, you can set up the extension manually. For example, if you regret dismissing the notification.

To enable the extension manually, follow these steps:

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Late Payment Prediction Setup**, and then choose the related link.  
2. Fill in the fields as necessary.

> [!NOTE]
> If you decide to enable the extension manually, be aware that [!INCLUDE[prod_short](includes/prod_short.md)] will not allow you to do so if the quality of the model is low. The quality of the model indicates how accurate the model's predictions are likely to be. Several factors can impact the quality of a model. For example, there might not have been enough data, or there wasn't enough variation in the data. You can view the quality of the model you're currently using on the **Late Payment Prediction Setup** page. You can also specify a minimum threshold for the model quality.

## View all payment predictions

If you enable the extension, a **Payments Predicted to be Late** tile is available in the **Business Manager** Role Centre. The tile displays the number of payments that are predicted to be late, and lets you open the **Customer Ledger Entries** page where you can dig deeper into the posted invoices. There are three columns to pay attention to:  

* **Late Payment** - Indicates whether the payment for the invoice is predicted to be late.
* **Prediction Confidence** - Indicates how reliable you should consider the prediction to be. **High** means that the prediction is at least 90% sure, **Medium** is between 80% and 90%, and **Low** is below 80%.
* **Prediction Confidence %** - Shows the actual percentage behind the confidence rating. By default, this column is hidden, but you can add it if you want. For more information, see [Personalise Your Workspace](ui-personalization-user.md).

> [!TIP]
> The Customer Ledger Entries page shows a FactBox on the right. While you're reviewing predictions, the information in the **Customer Details** section can be helpful. When you choose the invoice in the list, the section shows information about the customer. It also lets you take immediate action. For example, if a customer frequently misplaces their wallet, you can open the Customer card from the FactBox and block the customer for future sales.  

## Design details

Microsoft deploys and operates predictive web services in all regions where [!INCLUDE[prod_short](includes/prod_short.md)] is available. Access to these web services is included in your [!INCLUDE[prod_short](includes/prod_short.md)] subscription. For more information, see the Microsoft Dynamics 365 Business Central Licensing Guide. The guide is available for download on the [Business Central](https://dynamics.microsoft.com/business-central/overview/) website.

The web services work in three modes:

* Train model. The web service trains the model based on the provided dataset.
* Evaluate model. The web service checks whether the model returns reliable data for the provided dataset.
* Predict. Web-service applies the model to the provided dataset to make a prediction.

These web services are stateless, meaning they use data only to calculate predictions on demand. They don't store data.

> [!NOTE]  
> You can use your own predictive web service instead of ours. For more information, see [Create and use your own predictive web service late payment prediction](#AnchorText).

### Data required to train and evaluate the model

For each **Customer ledger entry** that has a related **Posted Sales Invoice**:

* Amount (LCY) including tax
* Payment terms in days are calculated as **Due Date** minus **Posting Date**
* Whether there is an applied credit memo

Additionally, the record has aggregated data from other invoices that are related to the same customer.

- Total number and amounts on paid invoices
- Total number and amounts on invoices that were paid late
- Total number and amounts on outstanding invoices
- Total number and amounts on outstanding invoices that are already late
- Average days late
- Ratio: Number of paid late/paid invoices
- Ratio: Amount paid late/paid invoices
- Ratio: Number of outstanding late/outstanding invoices
- Ratio: Amounts on outstanding late/outstanding invoices

> [!NOTE]
> The information about the customer isn't included in the dataset.

### Standard model and My model

The Late Payment Prediction extension's predictive model is trained on data that represents a range of small to medium-sized businesses. When you start posting invoices and receiving payments, [!INCLUDE[prod_short](includes/prod_short.md)] evaluates whether the standard model fits your business flow.

If your processes don't match the standard model, you can use the extension but you'll need to get more data. Just continue to use [!INCLUDE[prod_short](includes/prod_short.md)].

> [!NOTE]
> We use a bit of your compute time each week when we evaluate and re-train the model.

[!INCLUDE[prod_short](includes/prod_short.md)] runs training and evaluation automatically when enough paid and late invoices are available. However, you can run it manually whenever you want.

#### To train and use your model

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Late Payment Prediction Setup**, and then choose the related link.  
2. In the **Selected Model** field, choose **My Model**.
3. Choose the **Create My Model** action, to train model on your data.  

## <a name="AnchorText"> </a>Create and use your own predictive web service for late payment prediction

You can also create your own predictive web service based on a public model named **Prediction Experiment for Dynamics 365 Business Central**. This predictive model is available online in the Azure AI Gallery. To use the model, follow these steps:  

1. Open a browser and go to the [Azure AI Gallery](https://go.microsoft.com/fwlink/?linkid=2086310).  
2. Search for **Prediction Experiment for Dynamics 365 Business Central**, and then open the model in Azure Machine Learning studio.  
3. Use your Microsoft account to sign up for a workspace, and then copy the model.  
4. Run the model, and publish it as a web service.  
5. Make a note of the API URL and API key. You will use these credentials for a cash flow setup.  
6. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Late Payment Prediction Setup**, and then choose the related link.  
7. Choose the **Use My Azure Subscription** check box.
8. On the **My Model Credentials** FastTab, enter the API URL and API key for your model.  

## See also

[Azure Machine Learning studio Documentation](/azure/machine-learning/classic/)  
[Customising Business Central Using Extensions](ui-extensions.md)  
[Welcome to [!INCLUDE[prod_long](includes/prod_long.md)]](welcome.md)  
[Use Artificial Intelligence in Microsoft Dynamics 365 Business Central](/training/paths/use-artificial-intelligence/)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
