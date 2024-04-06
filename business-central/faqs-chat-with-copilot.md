---
title: Responsible AI FAQ for Chat with Copilot (preview)
description: 'This FAQ provides information about the AI technology used for chatting with Copilot in Business Central. It includes key considerations and details about how AI is used, how it was tested and evaluated, and any specific limitations.'
ms.date: 03/18/2024
ms.custom:
  - responsible-ai-faqs
ms.topic: article
author: jswymer
ms.author: jswymer
ms.reviewer: jswymer
ms.search.keywords: 'copilot, AI, chat'
---
# <a name="responsible-ai-faq-for-chat-with-copilot-preview"></a>Responsible AI FAQ for Chat with Copilot (preview)

[!INCLUDE[production-ready-preview-dynamics365](includes/production-ready-preview-dynamics365.md)]

These frequently asked questions (FAQ) describe the AI impact of Chat with Copilot in [!INCLUDE[prod_short](includes/prod_short.md)]. If you're inetersted in general questions about using the feature, go to [FAQ for chat with Copilot](chat-with-copilot-faq.md).

## <a name="what-is-chat-with-copilot"></a>What is Chat with Copilot?

Microsoft Copilot is the AI-powered assistant that helps spark creativity, boost productivity, and eliminate tedious tasks. You can chat with Copilot in Business Central to answer questions and find business data by expressing what you're looking for in natural language.

Chat with Copilot, also referred as chat, is an interactive feature that answers questions and finds business data related to [!INCLUDE[prod_short](includes/prod_short.md)], without users having to navigate the user interface or the product documentation. The Copilot pane is available from anywhere in the [!INCLUDE[prod_short](includes/prod_short.md)] client.

Users ask questions in natural language, like "How do I deliver goods to my customers directly from my vendors?" or "Do we have any office chairs in stock for under $600?" In response, Copilot provides answers in natural language. Depending on the questions, answers can include plain text, links to records or pages in [!INCLUDE[prod_short](includes/prod_short.md)], and links to [!INCLUDE[prod_short](includes/prod_short.md)] help articles on Microsoft Learn.

## <a name="what-are-capabilities-of-chat-with-copilot"></a>What are capabilities of Chat with Copilot?

You can chat with Copilot to get answers to the following classes of questions:

### <a name="explain-and-guide"></a>Explain and guide

Users can ask Copilot to explain a specific concept related to [!INCLUDE[prod_short](includes/prod_short.md)], like what are dimensions, or provide guidance on how to complete a task, like how to post a sales order. Copilot searches the official [!INCLUDE[prod_short](includes/prod_short.md)] documentation published by Microsoft, and provides an answer based on the documentation.

- Copilot uses the knowledge on Microsoft Learn (not a broad web search) to semantically search only Dynamics 365 [!INCLUDE[prod_short](includes/prod_short.md)] documentation on Microsoft Learn.

- Copilot doesn't take action, create new data, or modify any configuration. It simply summarises any paragraphs it finds on Microsoft Learn that match the question or prompt in chat.

### <a name="find-business-data-and-related-pages"></a>Find business data and related pages

Users can ask Copilot to locate pages by name or ask for records based on their fields and constraints. If Copilot finds a match, it responds with a link to the relevant record or page, which the user then can select to open.

- Copilot converts the natural language input into a query consisting of a table search, sort, and filter criteria.

  The capability uses the [!INCLUDE[prod_short](includes/prod_short.md)]'s native data search capabilities to find matching data from tables within the companies database. The search runs under the user's own identity for security and compliance. It doesn't search outside of the [!INCLUDE[prod_short](includes/prod_short.md)] database.

- Copilot doesn't take action, create new data, or modify any configuration. It only summarises the records received from the [!INCLUDE[prod_short](includes/prod_short.md)] native data search. 

## <a name="what-is-the-intended-use-of-chat-with-copilot"></a>What is the intended use of Chat with Copilot?

Chat is designed for enterprise use and answering questions that pertain to [!INCLUDE[prod_short](includes/prod_short.md)] and the business data it contains. The feature empowers people to solve common tasks such as finding records or getting guidance by expressing themselves in their own words, making it easier and more accessible to work with [!INCLUDE[prod_short](includes/prod_short.md)].

## <a name="how-was-chat-with-copilot-evaluated-what-metrics-are-used-to-measure-performance"></a>How was Chat with Copilot evaluated? What metrics are used to measure performance?

- The feature underwent extensive testing during which numerous English language texts covering a broad range of topics and styles of expressing intent were given to Copilot. The outcomes were evaluated against accuracy, relevance, and safety.
- The feature is built in accordance with Microsoft's Responsible AI Standard. [Learn more about responsible AI from Microsoft](https://aka.ms/RAI).

## <a name="how-does-microsoft-monitor-the-quality-of-generated-content"></a>How does Microsoft monitor the quality of generated content?

Microsoft has various systems in place to ensure that content generated by Copilot is of the highest quality, detect abuse, and ensure safety for our customers and their data.

Users have the opportunity to provide feedback to every Copilot response and report inaccurate or inappropriate content to help Microsoft improve this feature. 

- You provide feedback by using the like (thumbs up) or dislike (thumbs down) icon on the **Copilot** pane in [!INCLUDE[prod_short](includes/prod_short.md)].
- We analyse and utilise user feedback on the feature to help us improve responses.
- If you encounter inappropriate generated content, report it to Microsoft by using this feedback form: [Report abuse](https://go.microsoft.com/fwlink/?linkid=2249810).
- Microsoft might disable the Copilot-driven features for selected customers if abuse of the functionality is detected.

## <a name="what-are-the-limitations-of-chat-with-copilot-how-can-users-minimize-the-impact-of-the-chat-with-copilot-limitations-when-using-the-system"></a>What are the limitations of Chat with Copilot? How can users minimise the impact of the Chat with Copilot limitations when using the system?

- General limitations of AI

  AI systems are valuable tools but they're nondeterministic. The content they generate may not be completely accurate. So, it's important to use your judgment to review and verify responses Copilot before making decisions that could affect stakeholders like customers and partners. For most responses, Copilot will also include citations or reference links that you can use to quickly verify whether Copilot has come to the correct answer. For example, when asked how to perform some task, Copilot includes links to the source article. When asked to find a record based on specific criteria, Copilot includes links that describe the list page it identified as the topic of conversation, as well as any filters or sorting that was applied to reach an answer.

- Language limitations

  - Chat is only supported in English for the following locales: en-AU, en-CA, en-GB, en-IE, en-IN, en-NZ, en-PH, en-SG, en-US, en-ZA.

    If the display language in [!INCLUDE[prod_short](includes/prod_short.md)] isn't one of the these locales, chat isn't available.

  - The quality of answers can be lower under the following conditions:
    - The language locale is something other than en-US.
    - When the language setting for the user in [!INCLUDE[prod_short](includes/prod_short.md)] differs from the primary language of the data in the [!INCLUDE[prod_short](includes/prod_short.md)] database.

- Specific industry, product, and topic limitations

   Chat includes built-in safety mechanisms that prevent the undesirable generation of harmful content, such as sexually explicit content or incitement of violence. Sometimes, customers operate in industries, sell products and services, or work with processes that naturally overlap with what might be considered inappropriate in other contexts, or work with data that might trigger these safeguards. Chat might not perform as well in these cases.

<!--## What operational factors and settings allow for effective and responsible use of the feature?-->

## <a name="what-data-does-chat-with-copilot-collect-and-how-is-it-used"></a>What data does Chat with Copilot collect and how is it used

Microsoft doesn't use your company data, including the text you send to Copilot, to train the foundational AI models for the benefit of others. Company administrators have full control to govern this data that is part of their Azure subscription. Because administrators or others in your company might have access to this data as determined by your employer, we recommend users don't enter sensitive data such as passwords or other secrets.

## <a name="what-does-chat-with-copilot-offer-for-security"></a>What does Chat with Copilot offer for security

Chat is designed to be secure and executes under the user's identity, inheriting all security permissions and other restrictions and never operating outside of [!INCLUDE[prod_short](includes/prod_short.md)]'s platform security. This means that Copilot can only access data that the user has access to.

For users with SUPER permission, chat can more easily locate unsecured data that's typically harder to get to for other users. Organisations that don't apply [!INCLUDE[prod_short](includes/prod_short.md)]'s security model to restrict which tables and objects each user or user role has access to, might be at elevated risk when using chat. Therefore, we recommend that your organisation either implements [!INCLUDE[prod_short](includes/prod_short.md)]'s security model or deactivates chat.

## <a name="see-also"></a>See also

[Chat with Copilot (preview)](chat-with-copilot.md)

