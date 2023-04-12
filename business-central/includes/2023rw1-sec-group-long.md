---
author: brentholtorf
ms.topic: include
ms.date: 03/03/2023
ms.author: bholtorf
---

> [!NOTE]
> Security groups are new to [!INCLUDE [prod_short](prod_short.md)] in 2023 release wave 1. They make it easier for administrators to manage user permissions by allowing them to group users by department, job function, and so on. Administrators assign the permissions to the group that its members need to do their jobs.
>
> Security groups are similar to the user groups that are currently available. However, user groups are only relevant for [!INCLUDE [prod_short](prod_short.md)]. Security groups are based on groups in Microsoft 365 admin centre or Azure portal. That benefits administrators because they can use their security groups with other Dynamics 365 apps. For example, if salespeople use [!INCLUDE [prod_short](prod_short.md)]and SharePoint, administrators don't have to recreate the group and its members.
>
> Security groups will replace user groups in a future release. You can continue using user groups to manage permissions until then. To start using security groups now, your administrator can turn on **Feature: Convert user group permissions** on the **Feature Management** page. To learn more about security groups, go to [Control Access to Business Central Using Security Groups](../ui-security-groups.md).