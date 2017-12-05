---
title: Setting up Cash Flow Analysis| Microsoft Docs
description: Set up the charts on the Accounts Role Centre to help analyse the flow of money in your business, including expenses and income, liquidity, and cash receipts minus cash payments.
services: project-madeira
documentationcenter: 
author: bholtorf
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: money flow, expense and income, liquidity, cash receipts minus cash payments, Cartera, funds
ms.date: 06/02/2017
ms.author: bholtorf
ms.translationtype: HT
ms.sourcegitcommit: ba26b354d235981bd7291f9ac6402779f554ac7a
ms.openlocfilehash: 7d78333c5a7151ad60f07433ba32cfea142a2445
ms.contentlocale: en-nz
ms.lasthandoff: 11/10/2017

---
# <a name="setting-up-cash-flow-analysis"></a>Setting Up Cash Flow Analysis
If you want some help to decide what to do with your cash, have a look at the charts on the Accountant Role Centre:  

* **Cash Cycle**  
* **Income & Expense**  
* **Cash Flow**  
* **Cash Flow Forecasts**  

This topic describes where the data in the charts comes from and, if necessary, what to do to start using the charts.  

## <a name="the-cash-cycle-and-income--expense-charts"></a>The Cash Cycle and Income & Expense charts
The **Cash Cycle** and **Income & Expense** charts are ready to go, based on the Chart of Accounts and account schedules. The accounts are where the data comes from, and account schedules calculate the relationship between sales and receivables. Some accounts and account schedules are provided. You can use them as-is, change them, and add new ones. If you add G/L accounts to your chart of accounts, for example, by importing them from QuickBooks, you'll need to map to the accounts on the **Account Schedules** page for the following account schedule names:  

| Account Schedule Name | Where it's used |
| --- | --- |
| **I_CACYCLE** |Cash Cycle |
| **I_CASHFLOW** |Cash Flow |
| **I_INCEXP** |Income & Expense |
| **I_MINTRIAL** |As an income statement if you don't use the chart of accounts |

**Note** It's a good idea to keep the calculations that are provided for the account schedule.  

Enter accounts in the **Totaling** field for **Total Revenue**, **Total Receivables**, **Total Payables**, and **Total Inventory**. To map to a range of accounts, or more than one specific account, enter the account numbers separated by ".." or by a vertical bar, respectively. For example, **1111..4444** or **2222|3333|5555**.  

**Tip** Verify your mapping by choosing the **Overview** action.  

## <a name="set-up-the-cash-flow-chart"></a>Set up the Cash Flow chart
The Cash Flow chart is based on the following:  

* A chart of cash flow accounts.
* One or more cash flow setups. These specify the accounts to use for general ledger, purchases, sales, services, and fixed assets.  

To help you get going, some accounts and cash flow setups are provided. You can add, change, or remove them.  

To set these up, search for **cash flow accounts**, choose the link, and then fill in the fields. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)] Repeat these steps for **cash flow setup**.  

## <a name="set-up-cash-flow-forecasts"></a>Set up cash flow forecasts
The **Cash Flow Forecast** chart uses cash flow accounts, cash flow setups, and cash flow forecasts. Some are provided, however, you can set up your own by using an assisted setup guide. The guide helps you specify things like how often to update the forecast, the accounts to base it on, information about when you pay taxes, and whether to turn on [Cortana Intelligence](https://www.microsoft.com/en-us/cloud-platform/what-is-cortana-intelligence-suite).  

Cash flow forecasts can use Cortana Intelligence to include documents with a due date in the future. The result is a more comprehensive prediction. The connection to Cortana Intelligence is already set up for you. You just need to turn it on. When you sign in to [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)], a notification displays in a blue bar, and provides a link to the default cash flow setup. The notification displays only once. If you close it, but decide to turn on Cortana Intelligence, you can use the assisted setup guide, or a manual process.  

> [!NOTE]  
>   Alternatively, you can use your own predictive web service. For more information, see [Create and use your own predictive web service for cash flow forecasts](#AnchorText).  

To use the assisted setup guide:  

1. In the Accountant Role Center, under the **Cash Flow Forecast** chart, choose the **Open Assisted Setup** action.  
2. Fill in the fields in each step of the guide.  
3. On the Home page, choose **Cash Flow Forecast** above the chart, and then **Recalculate Forecast**.  

To use a manual process:  

1. In the Accountant Role Center, search for **Cash Flow Setup**, and then choose the related link.  
2. Expand the **Cortana Intelligence** FastTab, and then choose the **Cortana Intelligence Enabled** check box.  
3. On the Home page, choose **Cash Flow Forecast** above the chart, and then **Recalculate Forecast**.  

> [!TIP]  
>   Consider the length of the periods that the service will use in its calculations. The more data you provide, the more accurate the predictions will be. Also, watch out for large variances in periods. They will also impact predictions. If Cortana Intelligence does not find enough data, or the data varies a lot, the service will not make a prediction.  

## <a name="AnchorText"> </a>Create and use your own predictive web service for cash flow forecasts
You can also create your own predictive web service based on a public model named **Forecasting model for Microsoft Dynamics 365 Business edition **. This predictive model is available online in the Cortana Intelligence Gallery. To use the model, follow these steps:  

1. Open a browser and go to the [Cortana Intelligence Gallery](https://go.microsoft.com/fwlink/?linkid=828352).  
2. Search for **Forecasting Model for Microsoft Dynamics 365 Business edition **, and then open the model in Azure Machine Learning Studio.  
3. Use your Microsoft account to sign up for a workspace, and then copy the model.  
4. Run the model, and publish it as a web service.  
5. Make a note of the API URL and API key. You will use these credentials for a cash flow setup.  
6. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Cash Flow Setup**, and then choose the related link.  
7. Expand the **Cortana Intelligence** FastTab, and then fill in the fields.  

## <a name="see-also"></a>See Also
[Analyzing Cash Flow in Your Company](finance-analyze-cash-flow.md)  
[Setting Up Finance](finance-setup-finance.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

