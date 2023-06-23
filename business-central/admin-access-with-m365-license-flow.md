---
title: User Access Flow for Microsoft 365 Licences
description: Get an overview of what happens when a user accesses Business Central data using their Microsoft 365 licence for the first time.
author: mikebc
ms.author: mikebc
ms.reviewer: jswymer
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.date: 11/03/2022
ms.custom: bap-template
ms.search.keywords: 'License, access, Microsoft 365, collaborate, collaboration, Teams, Microsoft Teams'
---
# <a name="user-access-flow-for-microsoft-365-licenses" />User Access Flow for Microsoft 365 Licences

[!INCLUDE [2023rw1-sec-group-short](includes/2023rw1-sec-group-short.md)]

This article describes what happens when a user accesses Business Central data using their Microsoft 365 licence for the first time. Understanding this flow allows administrators to plan their approach and configure Business Central to match their business needs.

1. First, the user’s identity is authenticated 
2. Business Central verifies that all the [minimum requirements](admin-access-with-m365-license.md#minimum-requirements) are met.
3. Business Central verifies that this user does not have a greater licence, such as a Business Central licence or an administrative role such as a delegated admin role. 
4. Business Central verifies whether the user is accessing data that belongs to an environment that has enabled access with Microsoft 365 licences. 
5. The user record is provisioned in Business Central, assigning the User Group, Profile and Permission Sets defined in the Microsoft 365 licence configuration page. By default, the Teams Users user group is assigned, the Employee profile is assigned, and only the Login permission set is assigned. Any other defaulting of user settings is also applied, just like a licensed Business Central user. 
6. The full Business Central security model is applied, to determine whether the user should be able to access the record, page, in the specified company and specified environment. 

If all steps succeed, the user can now view this Business Central data in Teams. The Business Central service automatically ensures read-only access and simplifies the UI. 

The user account is now registered in Business Central and can be managed like any Business Central user.

> [!NOTE]
> Steps may vary depending on any additional security configuration that you have specified in Microsoft 365 or Business Central.

## <a name="see-also" />See also

[Business Central Access with Microsoft 365 licences](admin-access-with-m365-license.md#minimum-requirements)  
[Set Up Access with Microsoft 365 Licences](admin-access-with-m365-license-setup.md)  
