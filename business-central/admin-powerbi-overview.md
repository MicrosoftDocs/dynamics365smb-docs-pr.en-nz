---
title: Power BI Integration Component and Architecture Overview for Business Central| Microsoft Docs
description: Getting insight, business intelligence, and KPIs from your Business Central data is easy with the Business Central apps for Power BI.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: account schedule, analysis, reporting, financial report, business intelligence, KPI
ms.reviewer: edupont
ms.date: 04/01/2020
ms.author: jswymer
ms.openlocfilehash: 9514f0355932c1b1cbd30acfdb9f6dab46db8a0a
ms.sourcegitcommit: aeaa0dc64e54432a70c4b0e1faf325cd17d01389
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 08/17/2020
ms.locfileid: "3697842"
---
# <a name="power-bi-integration-component-and-architecture-overview-for-prodshort"></a>Power BI Integration Component and Architecture Overview for [!INCLUDE[prodshort](includes/prodshort.md)]

In this article, you'll learn about the different aspects of Power BI integration with [!INCLUDE[prodshort](includes/prodshort.md)] to help you understand its implementation and use.

## <a name="components"></a>Components

The following table describes the major components involved with Power BI integration.

|Component|Description|
|---------|-----------|
|Power BI|A cloud-based report hosting and management service.|
|Power BI Desktop|An authoring tool for building reports and dashboards, and allows you to run reports. It's available as a free download on Microsoft Store and is installed locally.|
|[!INCLUDE[prodshort](includes/prodshort.md)]|Online or on-premises solution with connectors exposed to Power BI and the ability to embed a Power BI part.|

## <a name="whats-available-from-the-start"></a>What's available from the start

The following table describes available features.

|Feature|[!INCLUDE[prodshort](includes/prodshort.md)] online or on-premises support|
|-------|---------------------|
|Power BI connectors|Both. Different connectors for online and on-premises. Same connector used for Power BI Desktop and Power BI Service |
|Embedded experience for viewing a given report inside a FactBox in [!INCLUDE[prodshort](includes/prodshort.md)]|Both. Requires configuration to display reports for on-premises.|
|Power BI report management from [!INCLUDE[prodshort](includes/prodshort.md)]|Online|
|Default Power BI reports on role centres deployed to Power BI|Online|
|Power BI Apps on Microsoft AppSource|Online.|

## <a name="architecture"></a>Architecture

[!INCLUDE[prodshort](includes/prodshort.md)] integrates with Power BI through a connector using OData. The data source for Power BI reports is exposed as OData web services.

![Power BI architecture for integration with Business Central](./media/power-bi-architecture.png)

## <a name="general-flow"></a>General Flow

The following diagram illustrates the basic workflow for users when connecting [!INCLUDE[prodshort](includes/prodshort.md)] to Power BI.

![Power BI workflow  for integration with Business Central](./media/power-bi-flow.png)

1. User signs up for a Power BI account.
2. User connects to Power BI from [!INCLUDE[prodshort](includes/prodshort.md)].
3. [!INCLUDE[prodshort](includes/prodshort.md)] verifies the licence.
4. [!INCLUDE[prodshort](includes/prodshort.md)] deploys default reports to the Power BI service. This step only happens for [!INCLUDE[prodshort](includes/prodshort.md)] online.
5. [!INCLUDE[prodshort](includes/prodshort.md)] makes reports in Power BI available for selection in [!INCLUDE[prodshort](includes/prodshort.md)]. Default reports are automatically displayed in Power BI parts.
6. User creates a report in Power BI Desktop.
7. User publishes the report to the Power BI service. The reports are then available for selection in [!INCLUDE[prodshort](includes/prodshort.md)].

## <a name="see-related-training-at-microsoft-learn"></a>See Related Training at [Microsoft Learn](/learn/modules/configure-powerbi-excel-dynamics-365-business-central/index)

## <a name="see-also"></a>See Also

[Business Central and Power BI](admin-powerbi.md)  
[Power BI for consumers](/power-bi/consumer/end-user-consumer)  
[The 'new look' of the Power BI service](/power-bi/service-new-look)  
[Quickstart: Connect to data in Power BI Desktop](/power-bi/desktop-quickstart-connect-to-data)  
[Power BI documentation](/power-bi/)  
[Business Intelligence](bi.md)  
[Getting Started](product-get-started.md)  
[Importing Business Data from Other Finance Systems](across-import-data-configuration-packages.md)  
[Setting Up [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)  
[Using [!INCLUDE[d365fin](includes/d365fin_md.md)] as a Power BI Data Source](across-how-use-financials-data-source-powerbi.md)  
[Using [!INCLUDE[d365fin](includes/d365fin_md.md)] as a Power Apps Data Source](across-how-use-financials-data-source-powerapps.md)  
[Using [!INCLUDE[d365fin](includes/d365fin_md.md)] in Power Automate](across-how-use-financials-data-source-flow.md)  

## [!INCLUDE[d365fin](includes/free_trial_md.md)]  
