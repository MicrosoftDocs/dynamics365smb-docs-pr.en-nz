---
title: Setting Up Tax Groups, Areas, and Jurisdictions in the US and Canada | Microsoft Docs
description: Learn about how sales tax is set up, and how tax groups, tax areas (states, counties, cities, and localities), tax jurisdictions, and tax details work.
services: project-madeira
documentationcenter: 
author: edupont04
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: local
ms.date: 03/29/2017
ms.author: edupont
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: 763bb1b954b30734b0f81f121a6534c83442321a
ms.contentlocale: en-nz
ms.lasthandoff: 07/07/2017


---
# <a name="reporting-sales-tax-in-the-us-and-canada"></a>Reporting Sales Tax in the US and Canada
When you first start using [!INCLUDE[d365fin](includes/d365fin_md.md)], you can run an assisted setup guide to quickly and easily set up sales tax information for your company, customers, and vendors. In a matter of minutes, you are ready to create sales documents and purchase documents with sales tax calculated correctly. This is explained [in our blog post](https://madeira.microsoft.com/blog/sales-tax-setup-made-easy).
If you move to the empty My Company, we recommend that you start by using each of the assisted setup guides, including the one for sales tax. If you prefer to set up sales tax yourself, this article explains what you have to take into consideration.  

## <a name="tax-groups-tax-areas-and-tax-jurisdictions"></a>Tax Groups, Tax Areas, and Tax Jurisdictions
In [!INCLUDE[d365fin](includes/d365fin_md.md)], a tax group represents a group of inventory items or resources that are subject to identical tax terms. For example, you can set up a tax group for taxable items and another for nontaxable items. You must assign tax group codes to inventory items and general ledger accounts. Similarly, you must assign tax area codes to customers, locations, and to your own company settings. The assisted setup guide helps you do this.  

Each tax area is a grouping of sales tax jurisdictions based on a particular geographic location. For example, the Miami, Florida, tax area includes three sales tax jurisdictions: city (Miami), county (Dade), and state (Florida). [!INCLUDE[d365fin](includes/d365fin_md.md)] includes a limited set of tax areas with a default configuration, but you can change them and add new tax areas.  

If you set up new tax areas and tax jurisdictions, you must make sure that you fill in the fields correctly. In the United States, states, counties, cities, and localities can charge sales tax. In Canada, the federal government and provinces can charge sales tax. Companies collect and remit sales tax to these government authorities for products sold to end users. Sales tax can also be charged to existing sales tax. For example, tax can be calculated on a sales invoice amount that already includes the tax from other jurisdictions.  

In Canada, tax amounts must be detailed in documents for each tax jurisdiction. Up to four jurisdictions can be displayed in a document, and jurisdictions that have the same print order are combined when they are printed.  

## <a name="tax-details"></a>Tax Details
The **Tax Details** window shows different combinations of sales tax jurisdictions and sales tax groups to establish sales tax rates. For each tax jurisdiction, we recommend that you set up one tax group for normal sales tax, another tax group for items or services that are not taxed, and an additional tax group for every type of item or service that is handled with a different sales tax rate in that jurisdiction.  

In the United States, when you sell to a customer at a location where you do not have a *situs*—or a legal location in that state—you do not collect sales tax. For locations in which you do not have a situs, ensure that both the **Tax Below Minimum** and **Tax Above Maximum** fields are 0.00.  

## <a name="see-also"></a>See Also
[Finance](finance.md)  
[Setting Up Finance](finance-setup-finance.md)  
[Sales Tax and Goods and Services Tax in Canada](ca-finance-tax.md)  
[Sales Tax setup made easy](https://madeira.microsoft.com/blog/sales-tax-setup-made-easy)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

