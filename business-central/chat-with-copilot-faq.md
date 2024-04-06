---
title: Chat with Copilot FAQ
description: This article answers some common questions about chat with Copilot in Business Central.
author: jswymer
ms.author: jswymer
ms.reviewer: jswymer
ms.topic: conceptual
ms.collection:
  - bap-ai-copilot
ms.date: 02/27/2024
ms.custom: bap-template jswymer
---
# <a name="chat-with-copilot-faq"></a>Chat with Copilot FAQ

[!INCLUDE[preview-banner](includes/preview-banner.md)]

This article answers some common questions about chatting with Copilot in [!INCLUDE[prod_short](includes/prod_short.md)]. For questions related to AI and chat, consult [Responsible AI FAQs for chat with Copilot](faqs-chat-with-copilot.md).

[!INCLUDE[production-ready-preview-dynamics365](includes/production-ready-preview-dynamics365.md)]

## <a name="can-admins-grant-or-deny-permission-to-individual-users-to-get-access-to-chat"></a>Can admins grant or deny permission to individual users to get access to chat?

No, there's no permission or permission set for chat. If chat is activated on the [Copilot and AI capabilities](enable-ai.md) page, every user in an environment has access to chat.
 
## <a name="is-chat-available-on-tablet-phone-or-other-form-factors"></a>Is chat available on tablet, phone, or other form factors?

No, the chat pane is only available on the [!INCLUDE[web_client](includes/web_client.md)] web client.

## <a name="i-dont-use-business-central-in-english-what-are-my-options"></a>I don't use Business Central in English. What are my options?

At this time, chat is only available in English. You can change your user language to English in [My Settings](ui-change-basic-settings.md#language).

## <a name="which-business-central-version-do-i-need-to-experience-chat"></a>Which Business Central version do I need to experience chat?

Chat is available in public preview from version 24.0 (2024 release wave 1).

## <a name="does-chat-work-with-my-customizations"></a>Does chat work with my customisations?

It depends on the type of question you ask Copilot. For example:

- When you ask questions to locate records, Copilot is able to find records in your custom tables that are identified using custom fields.
- When you ask for an explanation or guidance, Copilot doesn't have access to any information about your customisations or documentation for your add-ons.

## <a name="copilot-never-seems-to-open-the-record-or-page-i-asked-for-what-am-i-doing-wrong"></a>Copilot never seems to open the record or page I asked for. What am I doing wrong?

When you ask Copilot to find records in [!INCLUDE[prod_short](includes/prod_short.md)], it displays any records it finds as selectable tiles or links in the chat pane. While in preview, Copilot doesn't automatically navigate to any page.

## <a name="the-answers-i-get-from-copilot-vary-even-though-i-ask-the-same-question-is-it-a-bug"></a>The answers I get from Copilot vary even though I ask the same question. Is it a bug?

Copilot might occasionally answer in different ways. Answers aren't necessarily identical.

## <a name="when-should-i-use-the-copy-function-on-chat-messages"></a>When should I use the Copy function on chat messages?

You can use the Copy button to copy a message from earlier in your conversation with Copilot, paste it into the input box to try again or try a variation of your message to Copilot.

## <a name="how-do-i-customize-or-extend-chat"></a>How do I customise or extend chat?

While in preview, the chat pane and Copilot's responses can't be modified in any way through customisation, add-ins, or personalisation.

## <a name="does-copilot-find-data-in-other-companies-or-environments"></a>Does Copilot find data in other companies or environments?

Even if your organisation uses multiple environments or companies to segregate data, Copilot only searches for records in the company you're currently signed into.

## <a name="the-copilot-chat-pane-doesnt-show-what-can-i-do"></a>The Copilot chat pane doesn't show. What can I do?

Check that your user language in My Settings is set to English, and that your environment is of version 24.0 or later. In the Copilot and AI Capabilities page, make sure administrators have switched on consent for data across geographies and have activated chat. Make sure your environment localisation is not Canada.

If you still do not see the chat with Copilot feature, it is possible that Microsoft is still rolling this out to your region. Copilot rolls out to US customers first in April 2024, and then over the course of weeks will roll out to other country localisations.

## <a name="next-steps"></a>Next steps

[Chat with Copilot (preview)](chat-with-copilot.md)
