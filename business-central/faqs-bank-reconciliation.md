---
title: FAQ for bank account reconciliation assist with Copilot (preview)
description: 'This FAQ provides information about the AI technology used for reconciling bank accounts and statements in Business Central. It includes key considerations and details about how AI is used, how it was tested and evaluated, and any specific limitations.'
ms.date: 03/27/2024
ms.custom:
  - responsible-ai-faqs
ms.topic: article
author: jswymer
ms.author: jswymer
ms.reviewer: jswymer
ms.search.keywords: 'copilot, AI'
ms.collection:
  - bap-ai-copilot
---

# <a name="faq-for-bank-account-reconciliation-assist-with-copilot-preview"></a>FAQ for bank account reconciliation assist with Copilot (preview)

[!INCLUDE [preview-banner](~/../shared-content/shared/preview-includes/preview-banner.md)]

These frequently asked questions (FAQ) describe the AI impact of Microsoft Copilot assistance with bank account reconciliation in [!INCLUDE[prod_short](includes/prod_short.md)].

[!INCLUDE [preview-note](~/../shared-content/shared/preview-includes/production-ready-preview-dynamics365.md)]

## <a name="what-is-bank-reconciliation-assist"></a>What is bank reconciliation assist?

Bank reconciliation is a common accounting task where organisations review their bank account statements to identify transactions that should be registered in [!INCLUDE[prod_short](includes/prod_short.md)]. For example, this task is used to identify periodic bank fees or small employee expenses.

Bank reconciliation is typically a multi-step process. First, bank statements are imported into [!INCLUDE[prod_short](includes/prod_short.md)]. Next, transactions are matched with ledger entries. Finally, new ledger entries are posted to reflect any residual transactions that were not previously known to your ledgers.

Copilot in [!INCLUDE[prod_short](includes/prod_short.md)] reduces the manual effort by matching more transactions and suggesting general ledger (G/L) accounts that you can post to.

## <a name="what-are-the-capabilities-of-bank-reconciliation-assist"></a>What are the capabilities of bank reconciliation assist?

Copilot provides AI-powered assistance with two distinct tasks:

- Improved matching of transactions with ledger entries

    [!INCLUDE[prod_short](includes/prod_short.md)] offers automated rules that automatically match many bank transactions with ledger entries. However, these rules are inflexible and often result in many unmatched transactions, each of which requires manual inspection and comparison. Copilot uses AI technology to inspect those unmatched transactions and identify more matches, based on the dates, amounts, and descriptions. For example, if a customer paid multiple invoices in one lump sum, Copilot reconciles the single bank statement line with the multiple invoice ledger entries.

- Suggested G/L accounts

    For residual bank transactions that can't be matched to any ledger entries, Copilot uses AI technology to compare the transaction description with G/L account names and then suggest the most likely G/L account to post to. For example, if unmatched transactions have the narrative *Fuel Stop 24*, Copilot might suggest that you post them to the *Transportation* account.

Copilot doesn't connect to your bank to retrieve or send transactions. This task remains fully within your control. It's a prerequisite for using Copilot's assistance, regardless of whether the transactions are added to [!INCLUDE[prod_short](includes/prod_short.md)] by using a digital bank connection, imported from a bank statement file, or manually entered.

## <a name="what-is-the-intended-use-of-bank-reconciliation-assist"></a>What is the intended use of bank reconciliation assist?

Bank account reconciliation assist is designed to improve the accuracy of ledgers by helping customers identify new transactions that they should account for in [!INCLUDE[prod_short](includes/prod_short.md)]. It isn't intended for fraud detection or to identify whether customers paid on time.

## <a name="how-was-bank-reconciliation-assist-evaluated-what-metrics-are-used-to-measure-performance"></a>How was bank reconciliation assist evaluated? What metrics are used to measure performance?

Bank account reconciliation assist was tested by using combinations of synthetic bank transaction data and similar G/L accounts and ledger entries that cover the typical variations and data limits for each field and in different languages. Test data represents both typical usage and usage by bad actors. Performance was measured in comparison to manual reconciliation of the same data.

## <a name="what-are-the-limitations-of-bank-reconciliation-assist-how-can-users-minimize-the-impact-of-these-limitations-when-they-use-the-system"></a>What are the limitations of bank reconciliation assist? How can users minimise the impact of these limitations when they use the system?

Bank account reconciliation assist performs best when G/L account names, ledger entry descriptions, and bank transaction descriptions are all in the same language. Mixed languages or mixed languages for transaction descriptions often result in fewer matches and suggestions.

Suggested ledger accounts performs best in one of the supported languages (see the next section for a list of languages). Users might experience fewer transaction matches and fewer suggested ledger accounts in other languages.

## <a name="in-which-geographies-and-languages-is-bank-reconciliation-assist-available"></a>In which geographies and languages is bank reconciliation assist available?

- Available geographies

  Bank account reconciliation assist is available in all supported [Business Central countries/regions](/dynamics365/business-central/dev-itpro/compliance/apptest-countries-and-translations). For customer environments located in countries/regions where Azure OpenAI Service isn't deployed, administrators must consent to allowing their data to move across boundaries for [!INCLUDE [prod_short](includes/prod_short.md)] to connect to Azure OpenAI service. Learn more at [Copilot data movement across geographies](ai-copilot-data-movement.md).

- Available languages

  [!INCLUDE[bank-recon-assist-language-support](includes/bank-recon-assist-language-support.md)]

For more information about languages, see the previous question about limitations.

## <a name="what-is-expected-of-system-users-when-they-operate-bank-account-reconciliation-assist"></a>What is expected of system users when they operate bank account reconciliation assist?

### <a name="during-bank-account-reconciliation"></a>During bank account reconciliation

AI-powered matches and suggestions might sometimes be incorrect or incomplete. Users of bank account reconciliation assist must review the accuracy of the matches and suggestions that Copilot provides before they choose to keep them. Copilot's matches and suggestions aren't saved to the [!INCLUDE[prod_short](includes/prod_short.md)] database until you select the **Keep it** button and close the Copilot window. You can edit and correct any matches or suggestions before you choose to keep them.

### <a name="after-bank-account-reconciliation-is-completed"></a>After bank account reconciliation is completed

We recommend that users also verify accuracy and correct any discrepancies after they close the Copilot window. This process should include the following activities:

- Review the reconciliation test report.
- Ensure that your organisation has the appropriate review and audit processes in place.
- Reopen any posted reconciliations by using the **Undo** function.
- Correct any erroneous ledger entries through reverse posting of entries.

## <a name="what-is-expected-of-administrators-and-system-users-when-they-operate-bank-account-reconciliation-assist"></a>What is expected of administrators and system users when they operate bank account reconciliation assist?

System users, such as accountants, treasurers, or other people who work on business accounting, should always review the accuracy of matches and suggestions that Copilot provides before they choose to keep them. After reconciliation with Copilot, we recommend that these users review the reconciliation test report to verify accuracy and identify any discrepancies.

Administrators should ensure that the appropriate accounting users are granted access to this capability.

## <a name="is-copilot-the-only-means-of-completing-bank-account-reconciliation"></a>Is Copilot the only means of completing bank account reconciliation?

No. Use of Copilot is optional. [!INCLUDE[prod_short](includes/prod_short.md)] offers traditional, non-AI-powered means of importing bank statements, running predefined matching rules, and manually applying matches and posting to appropriate ledger accounts. Both the traditional approach and Copilot can be used simultaneously in an organisation.

## <a name="how-do-i-give-feedback-about-ai-generated-content"></a>How do I give feedback about AI-generated content?

Each time that Copilot provides matches or suggestions, you can provide feedback to Microsoft directly from the Copilot window by using the like (thumbs up) and dislike (thumbs down) controls. Your feedback remains anonymous, and we use this data to improve the quality of the service.

## <a name="see-also"></a>See also

[Reconcile bank accounts with Copilot (preview)](bank-reconciliation-with-copilot.md)
