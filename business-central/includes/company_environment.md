---
author: edupont04
ms.service: dynamics365-accountant
ms.topic: include
ms.date: 07/03/2020
ms.author: edupont
ms.openlocfilehash: d4d7e1ce5da2a59e4a682746035684e76dd55eef
ms.sourcegitcommit: ca5bf1d934997ef8c0bc9f8ab0e5568f0ed42fa4
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 07/06/2020
ms.locfileid: "3535501"
---
People sometimes support more than one company and need to easily switch from working in one company to another in [!INCLUDE [prodshort](prodshort.md)]. For example, a business might have sales offices in cities and multiple countries, so it has created a separate business unit for each office. The offices that are in the same country are set up as separate companies in a shared environment. Other offices are created as companies in separate environments because they are geographically based in other countries.  

What's an environment? Companies in [!INCLUDE[prodshort](prodshort.md)] exist in what are referred to as *environments*. There are two types of environments, **Production** and **Sandbox**. In short, production environments contain live business data, and sandbox environments are used as a safe place to test things like new business processes or features. For more information, see [Types of environments](/dynamics365/business-central/dev-itpro/administration/tenant-admin-center-environments#types-of-environments). If you have access to a company, you have access to the environment it's in. If you have access to more than one company, and those companies are in different environments, when you sign in to [!INCLUDE[prodshort](prodshort.md)] you must specify the environment that you want to work in. Environments are particular to a given country, so if your organisation works in multiple countries, you need separate environments for each country.  

What's a company? Think of a *company* as a container that holds information about a legal entity. Using the example above, the business has a sales office in Seattle and another in New York, so it creates a company in [!INCLUDE[prodshort](prodshort.md)] for each office so that it can manage operations for each office separately.  
