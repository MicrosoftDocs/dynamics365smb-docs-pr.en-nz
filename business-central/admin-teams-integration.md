---
title: Managing Microsoft Teams Integration with Business Central| Microsoft Docs
description: Manage Business Central integration with Microsoft Teams.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: Teams, MS Teams, Microsoft Teams, Skype, Link, Microsoft 365, collaborate, collaboration, teamwork
ms.date: 01/20/2021
ms.author: jswymer
ms.openlocfilehash: 5fc5957695145ad3bbc4225c7c7e18dd7ca0c728
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "5386315"
---
# <a name="managing-microsoft-teams-integration-with-prod_short"></a><span data-ttu-id="572b6-103">Managing Microsoft Teams Integration with [!INCLUDE [prod_short](includes/prod_short.md)]</span><span class="sxs-lookup"><span data-stu-id="572b6-103">Managing Microsoft Teams Integration with [!INCLUDE [prod_short](includes/prod_short.md)]</span></span>

[!INCLUDE [online_only](includes/online_only.md)]

<span data-ttu-id="572b6-104">This article provides an overview of what you can do as an administrator to control Microsoft Teams integration with [!INCLUDE [prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="572b6-104">This article provides an overview of what you can do as an administrator to control Microsoft Teams integration with [!INCLUDE [prod_short](includes/prod_short.md)].</span></span>

## <a name="in-microsoft-teams"></a><span data-ttu-id="572b6-105">In Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="572b6-105">In Microsoft Teams</span></span>

### <a name="minimum-requirements"></a><span data-ttu-id="572b6-106">Minimum requirements</span><span class="sxs-lookup"><span data-stu-id="572b6-106">Minimum requirements</span></span>

<span data-ttu-id="572b6-107">This section describes the minimum requirements for the [!INCLUDE [prod_short](includes/prod_short.md)] app features to work in Teams.</span><span class="sxs-lookup"><span data-stu-id="572b6-107">This section describes the minimum requirements for the [!INCLUDE [prod_short](includes/prod_short.md)] app features to work in Teams.</span></span>

- <span data-ttu-id="572b6-108">Required licences</span><span class="sxs-lookup"><span data-stu-id="572b6-108">Required licenses</span></span>

    <span data-ttu-id="572b6-109">This table gives you an overview of the licences needed for the [!INCLUDE [prod_short](includes/prod_short.md)] app features to work in Teams.</span><span class="sxs-lookup"><span data-stu-id="572b6-109">This table gives you an overview of the licenses needed for the [!INCLUDE [prod_short](includes/prod_short.md)] app features to work in Teams.</span></span>

    |<span data-ttu-id="572b6-110">What</span><span class="sxs-lookup"><span data-stu-id="572b6-110">What</span></span>|<span data-ttu-id="572b6-111">Teams licence</span><span class="sxs-lookup"><span data-stu-id="572b6-111">Teams license</span></span>|<span data-ttu-id="572b6-112">[!INCLUDE [prod_short](includes/prod_short.md)] licence</span><span class="sxs-lookup"><span data-stu-id="572b6-112">[!INCLUDE [prod_short](includes/prod_short.md)] license</span></span>|
    |----|---|---|
    |<span data-ttu-id="572b6-113">Paste a link to a [!INCLUDE [prod_short](includes/prod_short.md)] record into a conversation, and send it as a card.</span><span class="sxs-lookup"><span data-stu-id="572b6-113">Paste a link to a [!INCLUDE [prod_short](includes/prod_short.md)] record into a conversation, and send it as a card.</span></span>|<span data-ttu-id="572b6-114">![check mark](media/check.png "cheque")</span><span class="sxs-lookup"><span data-stu-id="572b6-114">![check mark](media/check.png "check")</span></span>|<span data-ttu-id="572b6-115">![check mark](media/check.png "cheque")</span><span class="sxs-lookup"><span data-stu-id="572b6-115">![check mark](media/check.png "check")</span></span>|
    |<span data-ttu-id="572b6-116">View a card of a [!INCLUDE [prod_short](includes/prod_short.md)] record in a conversation.</span><span class="sxs-lookup"><span data-stu-id="572b6-116">View a card of a [!INCLUDE [prod_short](includes/prod_short.md)] record in a conversation.</span></span>|<span data-ttu-id="572b6-117">![check mark](media/check.png "cheque")</span><span class="sxs-lookup"><span data-stu-id="572b6-117">![check mark](media/check.png "check")</span></span>||
    |<span data-ttu-id="572b6-118">View more details of card for a [!INCLUDE [prod_short](includes/prod_short.md)] record in a conversation.</span><span class="sxs-lookup"><span data-stu-id="572b6-118">View more details of card for a [!INCLUDE [prod_short](includes/prod_short.md)] record in a conversation.</span></span>|<span data-ttu-id="572b6-119">![check mark](media/check.png "cheque")</span><span class="sxs-lookup"><span data-stu-id="572b6-119">![check mark](media/check.png "check")</span></span>|<span data-ttu-id="572b6-120">![check mark](media/check.png "cheque")</span><span class="sxs-lookup"><span data-stu-id="572b6-120">![check mark](media/check.png "check")</span></span>|

- <span data-ttu-id="572b6-121">Allow URL previews</span><span class="sxs-lookup"><span data-stu-id="572b6-121">Allow URL previews</span></span>

    <span data-ttu-id="572b6-122">**Allow URL previews** policy setting must be turned on.</span><span class="sxs-lookup"><span data-stu-id="572b6-122">**Allow URL previews** policy setting must be turned on.</span></span> <span data-ttu-id="572b6-123">Otherwise, a card can't be generated for [!INCLUDE [prod_short](includes/prod_short.md)] links pasted into a Teams conversation.</span><span class="sxs-lookup"><span data-stu-id="572b6-123">Otherwise, a card can't be generated for [!INCLUDE [prod_short](includes/prod_short.md)] links pasted into a Teams conversation.</span></span> <span data-ttu-id="572b6-124">For more information about this setting, see [Manage messaging policies in Teams](/microsoftteams/messaging-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="572b6-124">For more information about this setting, see [Manage messaging policies in Teams](/microsoftteams/messaging-policies-in-teams).</span></span>

### <a name="managing-the-prod_short-app-optional"></a><span data-ttu-id="572b6-125">Managing the [!INCLUDE [prod_short](includes/prod_short.md)] app (optional)</span><span class="sxs-lookup"><span data-stu-id="572b6-125">Managing the [!INCLUDE [prod_short](includes/prod_short.md)] app (optional)</span></span>

<span data-ttu-id="572b6-126">As a Teams administrator, you can manage all apps for your organisation, including the [!INCLUDE [prod_short](includes/prod_short.md)] app.</span><span class="sxs-lookup"><span data-stu-id="572b6-126">As a Teams administrator, you can manage all apps for your organization, including the [!INCLUDE [prod_short](includes/prod_short.md)] app.</span></span> <span data-ttu-id="572b6-127">You can approve or install the [!INCLUDE [prod_short](includes/prod_short.md)] app for your organisation, block user's from installing the app and more.</span><span class="sxs-lookup"><span data-stu-id="572b6-127">You can approve or install the [!INCLUDE [prod_short](includes/prod_short.md)] app for your organization, block user's from installing the app, and more.</span></span>

<span data-ttu-id="572b6-128">For more information, see the following articles in the Microsoft Teams documentation:</span><span class="sxs-lookup"><span data-stu-id="572b6-128">For more information, see the following articles in the Microsoft Teams documentation:</span></span>

- [<span data-ttu-id="572b6-129">Manage your apps in the Microsoft Teams admin centre</span><span class="sxs-lookup"><span data-stu-id="572b6-129">Manage your apps in the Microsoft Teams admin center</span></span>](https://docs.microsoft.com/MicrosoftTeams/manage-apps)
- [<span data-ttu-id="572b6-130">Manage app setup policies in Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="572b6-130">Manage app setup policies in Microsoft Teams</span></span>](https://docs.microsoft.com/microsoftteams/teams-app-setup-policies)

## <a name="in-prod_short"></a><span data-ttu-id="572b6-131">In [!INCLUDE [prod_short](includes/prod_short.md)]</span><span class="sxs-lookup"><span data-stu-id="572b6-131">In [!INCLUDE [prod_short](includes/prod_short.md)]</span></span>

### <a name="minimum-requirements"></a><span data-ttu-id="572b6-132">Minimum requirements</span><span class="sxs-lookup"><span data-stu-id="572b6-132">Minimum requirements</span></span>

- <span data-ttu-id="572b6-133">[!INCLUDE [prod_short](includes/prod_short.md)] version:</span><span class="sxs-lookup"><span data-stu-id="572b6-133">[!INCLUDE [prod_short](includes/prod_short.md)] version:</span></span>

    <span data-ttu-id="572b6-134">[!INCLUDE [prod_short](includes/prod_short.md)] 2020 release wave 2, update 17.3, or later.</span><span class="sxs-lookup"><span data-stu-id="572b6-134">[!INCLUDE [prod_short](includes/prod_short.md)] 2020 release wave 2, update 17.3, or later.</span></span> <span data-ttu-id="572b6-135">Teams integration is only supported for [!INCLUDE [prod_short](includes/prod_short.md)] online; not on-premises.</span><span class="sxs-lookup"><span data-stu-id="572b6-135">Teams integration is only supported for [!INCLUDE [prod_short](includes/prod_short.md)] online; not on-premises.</span></span>

- <span data-ttu-id="572b6-136">Codeunit **2718 Page Summary Provider** is published as a web service:</span><span class="sxs-lookup"><span data-stu-id="572b6-136">Codeunit **2718 Page Summary Provider** is published as a web service:</span></span>

    <span data-ttu-id="572b6-137">This codeunit is published as a web service by default.</span><span class="sxs-lookup"><span data-stu-id="572b6-137">This codeunit is published as a web service by default.</span></span> <span data-ttu-id="572b6-138">The codeunit is part of the [!INCLUDE [prod_short](includes/prod_short.md)] system application.</span><span class="sxs-lookup"><span data-stu-id="572b6-138">The codeunit is part of the [!INCLUDE [prod_short](includes/prod_short.md)] system application.</span></span> <span data-ttu-id="572b6-139">It's used to get the field data for a [!INCLUDE [prod_short](includes/prod_short.md)] page added to a Teams conversation.</span><span class="sxs-lookup"><span data-stu-id="572b6-139">It's used to get the field data for a [!INCLUDE [prod_short](includes/prod_short.md)] page added to a Teams conversation.</span></span> <span data-ttu-id="572b6-140">For information about publishing web services, see [Publish a Web Service](across-how-publish-web-service.md).</span><span class="sxs-lookup"><span data-stu-id="572b6-140">For information about publishing web services, see [Publish a Web Service](across-how-publish-web-service.md).</span></span>

- <a name="permissions"></a><span data-ttu-id="572b6-141">User permissions:</span><span class="sxs-lookup"><span data-stu-id="572b6-141">User permissions:</span></span>

    <span data-ttu-id="572b6-142">For the most part, the pages and data that users can view and edit in a Teams conversation is controlled by their permissions in [!INCLUDE [prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="572b6-142">For the most part, the pages and data that users can view and edit in a Teams conversation is controlled by their permissions in [!INCLUDE [prod_short](includes/prod_short.md)].</span></span>
    
    - <span data-ttu-id="572b6-143">To paste a [!INCLUDE [prod_short](includes/prod_short.md)] link into a Teams conversation and have it expand into a card, users must have at least read permission on the page and its data.</span><span class="sxs-lookup"><span data-stu-id="572b6-143">To paste a [!INCLUDE [prod_short](includes/prod_short.md)] link into a Teams conversation and have it expand into a card, users must have at least read permission on the page and its data.</span></span>
    - <span data-ttu-id="572b6-144">Once a card is submitted into a conversation, any user in that conversation can view that card without permission to [!INCLUDE [prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="572b6-144">Once a card is submitted into a conversation, any user in that conversation can view that card without permission to [!INCLUDE [prod_short](includes/prod_short.md)].</span></span>
    - <span data-ttu-id="572b6-145">To view more details for a card or open the record in [!INCLUDE [prod_short](includes/prod_short.md)], users must have read permission on the page and its data.</span><span class="sxs-lookup"><span data-stu-id="572b6-145">To view more details for a card or open the record in [!INCLUDE [prod_short](includes/prod_short.md)], users must have read permission on the page and its data.</span></span>
    - <span data-ttu-id="572b6-146">To change data, user's need modify permissions.</span><span class="sxs-lookup"><span data-stu-id="572b6-146">To change data, user's need modify permissions.</span></span>
    
    <span data-ttu-id="572b6-147">For information about permissions, see [Assign Permissions to Users and Groups](ui-define-granular-permissions.md).</span><span class="sxs-lookup"><span data-stu-id="572b6-147">For information about permissions, see [Assign Permissions to Users and Groups](ui-define-granular-permissions.md).</span></span>

## <a name="managing-privacy-and-compliance"></a><span data-ttu-id="572b6-148">Managing privacy and compliance</span><span class="sxs-lookup"><span data-stu-id="572b6-148">Managing privacy and compliance</span></span> 

<span data-ttu-id="572b6-149">Microsoft Teams provides extensive controls for compliance and management of sensitive or personally identifiable data&mdash;including data added to chats and channels by the [!INCLUDE [prod_short](includes/prod_short.md)] app.</span><span class="sxs-lookup"><span data-stu-id="572b6-149">Microsoft Teams provides extensive controls for compliance and management of sensitive or personally identifiable data&mdash;including data added to chats and channels by the [!INCLUDE [prod_short](includes/prod_short.md)] app.</span></span>

### <a name="understanding-where-prod_short-cards-are-stored"></a><span data-ttu-id="572b6-150">Understanding where [!INCLUDE [prod_short](includes/prod_short.md)] cards are stored</span><span class="sxs-lookup"><span data-stu-id="572b6-150">Understanding where [!INCLUDE [prod_short](includes/prod_short.md)] cards are stored</span></span> 

<span data-ttu-id="572b6-151">After a card is sent to a chat, the card and the fields shown on the card are copied to Teams.</span><span class="sxs-lookup"><span data-stu-id="572b6-151">After a card is sent to a chat, the card and the fields shown on the card are copied to Teams.</span></span> <span data-ttu-id="572b6-152">This information is subject to the Teams policies for your organisation, such as data retention policies.</span><span class="sxs-lookup"><span data-stu-id="572b6-152">This information is subject to the Teams policies for your organization, such as data retention policies.</span></span> <span data-ttu-id="572b6-153">When displaying card details, none of the data in the details window is stored in Teams.</span><span class="sxs-lookup"><span data-stu-id="572b6-153">When displaying card details, none of the data in the details window is stored in Teams.</span></span> <span data-ttu-id="572b6-154">The data remains stored in [!INCLUDE [prod_short](includes/prod_short.md)] and will only be retrieved by Teams when the user chooses to view the details.</span><span class="sxs-lookup"><span data-stu-id="572b6-154">The data remains stored in [!INCLUDE [prod_short](includes/prod_short.md)] and will only be retrieved by Teams when the user chooses to view the details.</span></span> 

- <span data-ttu-id="572b6-155">To learn more about where Teams stores that data, see [Location of data in Microsoft Teams](/microsoftteams/location-of-data-in-teams).</span><span class="sxs-lookup"><span data-stu-id="572b6-155">To learn more about where Teams stores that data, see [Location of data in Microsoft Teams](/microsoftteams/location-of-data-in-teams).</span></span>
- <span data-ttu-id="572b6-156">To learn more about retention policies in Teams, see [Retention policies in Microsoft Teams](/microsoftteams/retention-policies).</span><span class="sxs-lookup"><span data-stu-id="572b6-156">To learn more about retention policies in Teams, see [Retention policies in Microsoft Teams](/microsoftteams/retention-policies).</span></span>

### <a name="restricting-sharing-of-cards"></a><span data-ttu-id="572b6-157">Restricting sharing of cards</span><span class="sxs-lookup"><span data-stu-id="572b6-157">Restricting sharing of cards</span></span> 

<span data-ttu-id="572b6-158">You prevent specific users or groups from sending cards to chats or channels by setting up messaging policies that turn off the **URL Previews** setting.</span><span class="sxs-lookup"><span data-stu-id="572b6-158">You prevent specific users or groups from sending cards to chats or channels by setting up messaging policies that turn off the **URL Previews** setting.</span></span> <span data-ttu-id="572b6-159">For more information about this setting, see [Manage messaging policies in Teams](/microsoftteams/messaging-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="572b6-159">For more information about this setting, see [Manage messaging policies in Teams](/microsoftteams/messaging-policies-in-teams).</span></span> 

<span data-ttu-id="572b6-160">You can also use information barriers to prevent individuals or groups from communicating with each other.</span><span class="sxs-lookup"><span data-stu-id="572b6-160">You can also use information barriers to prevent individuals or groups from communicating with each other.</span></span> <span data-ttu-id="572b6-161">To learn more, see [Information barriers in Microsoft Teams](/microsoftteams/information-barriers-in-teams).</span><span class="sxs-lookup"><span data-stu-id="572b6-161">To learn more, see [Information barriers in Microsoft Teams](/microsoftteams/information-barriers-in-teams).</span></span>

<span data-ttu-id="572b6-162">Data loss prevention features in the Microsoft 365 Security & Compliance Centre can't be applied specifically to cards.</span><span class="sxs-lookup"><span data-stu-id="572b6-162">Data loss prevention features in the Microsoft 365 Security & Compliance Center can't be applied specifically to cards.</span></span> <span data-ttu-id="572b6-163">But they can be applied to the chat messages that contain the cards.</span><span class="sxs-lookup"><span data-stu-id="572b6-163">But they can be applied to the chat messages that contain the cards.</span></span> <span data-ttu-id="572b6-164">To track upcoming advanced features that include enabling DLP for cards, see [https://www.microsoft.com/en-us/microsoft-365/roadmap?featureid=67093](https://www.microsoft.com/en-us/microsoft-365/roadmap?featureid=67093).</span><span class="sxs-lookup"><span data-stu-id="572b6-164">To track upcoming advanced features that include enabling DLP for cards, see [https://www.microsoft.com/en-us/microsoft-365/roadmap?featureid=67093](https://www.microsoft.com/en-us/microsoft-365/roadmap?featureid=67093).</span></span>

### <a name="responding-to-data-requests"></a><span data-ttu-id="572b6-165">Responding to data requests</span><span class="sxs-lookup"><span data-stu-id="572b6-165">Responding to data requests</span></span>

<span data-ttu-id="572b6-166">You allow team members and team owners to delete messages that contain sensitive cards by setting up messaging policies, like: **Owners can delete sent messages** and **Users can delete sent messages**.</span><span class="sxs-lookup"><span data-stu-id="572b6-166">You allow team members and team owners to delete messages that contain sensitive cards by setting up messaging policies, like: **Owners can delete sent messages** and **Users can delete sent messages**.</span></span> <span data-ttu-id="572b6-167">For more information, see [Manage messaging policies in Teams](/microsoftteams/messaging-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="572b6-167">For more information, see [Manage messaging policies in Teams](/microsoftteams/messaging-policies-in-teams).</span></span>

<span data-ttu-id="572b6-168">Content search and eDiscovery compliance features in the Microsoft 365 Security & Compliance Centre can't be applied specifically to cards.</span><span class="sxs-lookup"><span data-stu-id="572b6-168">Content search and eDiscovery compliance features in the Microsoft 365 Security & Compliance Center can't be applied specifically to cards.</span></span> <span data-ttu-id="572b6-169">But they can be applied to the chat messages that contain cards.</span><span class="sxs-lookup"><span data-stu-id="572b6-169">But they can be applied to the chat messages that contain cards.</span></span> <span data-ttu-id="572b6-170">To track upcoming compliance features for cards, see [https://www.microsoft.com/microsoft-365/roadmap?featureid=68875](https://www.microsoft.com/microsoft-365/roadmap?featureid=68875).</span><span class="sxs-lookup"><span data-stu-id="572b6-170">To track upcoming compliance features for cards, see [https://www.microsoft.com/microsoft-365/roadmap?featureid=68875](https://www.microsoft.com/microsoft-365/roadmap?featureid=68875).</span></span>

<span data-ttu-id="572b6-171">Because card data in Teams is a copy of data in [!INCLUDE [prod_short](includes/prod_short.md)], you can also use [!INCLUDE [prod_short](includes/prod_short.md)] features to export a customer’s data if requested.</span><span class="sxs-lookup"><span data-stu-id="572b6-171">Because card data in Teams is a copy of data in [!INCLUDE [prod_short](includes/prod_short.md)], you can also use [!INCLUDE [prod_short](includes/prod_short.md)] features to export a customer’s data if requested.</span></span> <span data-ttu-id="572b6-172">For more information about privacy in [!INCLUDE [prod_short](includes/prod_short.md)], see [Privacy FAQ for Business Central Customers](/dynamics365/business-central/dev-itpro/security/privacyfaq).</span><span class="sxs-lookup"><span data-stu-id="572b6-172">For more information about privacy in [!INCLUDE [prod_short](includes/prod_short.md)], see [Privacy FAQ for Business Central Customers](/dynamics365/business-central/dev-itpro/security/privacyfaq).</span></span>

## <a name="see-also"></a><span data-ttu-id="572b6-173">See Also</span><span class="sxs-lookup"><span data-stu-id="572b6-173">See Also</span></span>
<span data-ttu-id="572b6-174">[[!INCLUDE [prod_short](includes/prod_short.md)] and Microsoft Teams Integration Overview](across-teams-overview.md)</span><span class="sxs-lookup"><span data-stu-id="572b6-174">[[!INCLUDE [prod_short](includes/prod_short.md)] and Microsoft Teams Integration Overview](across-teams-overview.md)</span></span>  
<span data-ttu-id="572b6-175">[Install the [!INCLUDE [prod_short](includes/prod_short.md)] App for Microsoft Teams](across-install-app-for-teams.md)</span><span class="sxs-lookup"><span data-stu-id="572b6-175">[Install the [!INCLUDE [prod_short](includes/prod_short.md)] App for Microsoft Teams](across-install-app-for-teams.md)</span></span>  
[<span data-ttu-id="572b6-176">Teams FAQ</span><span class="sxs-lookup"><span data-stu-id="572b6-176">Teams FAQ</span></span>](teams-faq.md)  
[<span data-ttu-id="572b6-177">Troubleshooting Teams</span><span class="sxs-lookup"><span data-stu-id="572b6-177">Troubleshooting Teams</span></span>](admin-teams-troubleshooting.md)  
[<span data-ttu-id="572b6-178">Developing for Teams Integration</span><span class="sxs-lookup"><span data-stu-id="572b6-178">Developing for Teams Integration</span></span>](/dynamics365/business-central/dev-itpro/developer/devenv-develop-for-teams)  

## [!INCLUDE[prod_short](includes/free_trial_md.md)]  


[!INCLUDE[footer-include](includes/footer-banner.md)]