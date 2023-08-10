---
title: Configure AI-powered item marketing text (preview) with Copilot
description: This article explains how to get a Copilot trial version of Business Central and enable Copilot on an environment.
author: jswymer
ms.author: jswymer
ms.reviewer: jswymer
ms.topic: how-to
ms.date: 03/22/2023
ms.custom: bap-template
---

# <a name="configure-ai-powered-item-marketing-text-preview-with-copilot"></a>Configure AI-powered item marketing text (preview) with Copilot

[!INCLUDE[ai-preview](includes/ai-preview.md)]

This article explains how you can control the ability to create AI-powered item marketing text with Copilot for your organisation. This task is done by an admin. There are two requirements that you must fulfil to make the feature available to users:

- Enable the **Create AI-powered product descriptions with Copilot** feature.
- Consent to the terms and conditions of [preview](https://dynamics.microsoft.com/legaldocs/supp-dynamics365-preview/) and [Microsoft Privacy Statement](https://go.microsoft.com/fwlink/?LinkId=521839) on behalf of the organisation.

If either of these requirements isn't fulfilled, the feature won't be available for use.

## <a name="prerequisites"></a>Prerequisites

You're using a [preview version](ai-preview-getstarted.md) of Business Central that's enabled for Copilot. Enabling Copilot is done by an admin. For more information, go to [Configure AI-powered item marketing text with Copilot](enable-ai.md).

## <a name="enable-or-disable-create-ai-powered-product-descriptions-with-copilot"></a>Enable or disable Create AI-powered product descriptions with Copilot

1. In Business Central, search for and open the **Feature Management** page.
2. Set the **Enabled for** column for **Feature preview: Create AI-powered product descriptions with Copilot** to **All users** to enable the feature or **None** to disable it.

   For more information about feature management in general, go to [Feature Management](/dynamics365/business-central/dev-itpro/administration/feature-management).

## <a name="consent-to-or-reject-preview-and-privacy-terms-and-conditions-for-all-users"></a>Consent to or reject preview and privacy terms and conditions for all users

1. In Business Central, search for and open the **Privacy Notices Status** page.
2. In the **Integration Name** column, select **Azure OpenAI**, then read the terms and conditions that are presented to you.
3. In the **Azure OpenAI** row, select the **Agree for everyone** checkbox to consent or the **Disagree for everyone** checkbox to reject.

## <a name="next-steps"></a>Next steps

After you enable and consent to the feature, you're ready to try out Copilot on items in Business Central. Go to [Add marketing text to items](item-marketing-text.md).  

## <a name="see-also"></a>See also

[Overview of AI-powered item marketing text with Copilot](ai-overview.md)  
[Create marketing text to items using Copilot](item-marketing-text.md)  
[AI-powered item marketing text with Copilot FAQ](ai-faq.md)  
