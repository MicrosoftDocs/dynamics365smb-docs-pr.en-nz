---
author: edupont04
ms.topic: include
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 045f3cc062c3ffec74177f7c7bc41c3bb96c9b8c
ms.sourcegitcommit: ef80c461713fff1a75998766e7a4ed3a7c6121d0
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 02/15/2022
ms.locfileid: "8129724"
---
People sometimes support more than one company and need to easily switch from working in one company to another in [!INCLUDE [prod_short](prod_short.md)]. For example, a business might have sales offices in cities and multiple countries, so it has created a separate business unit for each office. The offices that are in the same country are set up as separate companies in a shared environment. Other offices are created as companies in separate environments because they are geographically based in other countries.<br><br>  

What's an environment? Companies in [!INCLUDE[prod_short](prod_short.md)] exist in what are referred to as *environments*. There are two types of environments, **Production** and **Sandbox**. In short, production environments contain live business data, and sandbox environments are used as a safe place to test things like new business processes or features. For more information, see [Types of environments](/dynamics365/business-central/dev-itpro/administration/tenant-admin-center-environments#types-of-environments). If you have access to a company, you have access to the environment it's in. If you have access to more than one company, and those companies are in different environments, when you sign in to [!INCLUDE[prod_short](prod_short.md)] you must specify the environment that you want to work in. Environments are particular to a given country, so if your organisation works in multiple countries, you need separate environments for each country.<br><br>  

What's a company? Think of a *company* as a container that holds information about a legal entity. Using the example above, the business has a sales office in Seattle and another in New York, so it creates a company in [!INCLUDE[prod_short](prod_short.md)] for each office so that it can manage operations for each office separately.  
