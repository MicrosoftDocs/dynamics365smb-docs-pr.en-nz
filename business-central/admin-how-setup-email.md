---
title: Set up email in Business Central | Microsoft Docs
description: Describes how to use the company's SMTP server to send and receive email messages within Business Central, or alternatively how to use the email server settings created with the Microsoft 365 subscription.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: SMTP, mail, Microsoft 365
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 8c69de24198d8682b2e106e3bf559803c2fed72c
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 10/01/2020
ms.locfileid: "3922575"
---
# <a name="set-up-email"></a>Set Up Email
To send and receive emails from within [!INCLUDE[d365fin](includes/d365fin_md.md)], you must fill in the fields on the **SMTP Mail Setup** page.

Instead of entering the SMTP server details manually, you can use the **Apply Microsoft 365 Server Settings** function to enter them with information from your Microsoft 365 subscription.

You can either set email up manually, as described below, or you can get help by using the **Email Setup** assisted setup guide. For more information, see [Getting Ready for Doing Business](ui-get-ready-business.md).  

## <a name="to-set-up-email"></a>To set up email
1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **SMTP Email Setup** , and then choose the related link.
2. Fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

    > [!NOTE]
    > If you are using an account that requires two-factor authentication, then the password that you enter in the **Password** field must be the same that you use for your Microsoft 365 subscription and it must be of type **App Password** . For more information, see [Manage app passwords for two-step verification](/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords).
3. Alternatively, choose the **Apply Microsoft 365 Server Settings** action to insert any information that is already defined for your Microsoft 365 subscription.
4. When all the fields are correctly filled in, choose the **Test Email Setup** action.
5. When the test succeeds, close the page.

## <a name="using-a-substitute-sender-address-on-outbound-email-messages"></a>Using a Substitute Sender Address on Outbound Email Messages
All outgoing email messages from [!INCLUDE[d365fin](includes/d365fin_md.md)] will use the default address for the account that you specified on the SMTP Email Setup page, as described above. You can, however, use the **Send As** or **Send on Behalf** capabilities on your Exchange server to change the sender address on outbound messages. [!INCLUDE[d365fin](includes/d365fin_md.md)] will use the default account to authenticate to Exchange, but will either substitute the sender address with the one you specify, or amend it with "on behalf of."

The following are examples of how Send As and Send on Behalf are used in [!INCLUDE[d365fin](includes/d365fin_md.md)].:

 * When you send documents such as purchase or sales orders to vendors and customers, you might want them to appear to come from a _noreply@yourcompanyname.com_ address.
 * When your workflow sends an approval request by email using the email address of the requestor.

> [!Note]
> You can only use one account to substitute sender addresses. That is, you cannot have one substitute address for purchasing processes, and another for sales processes.

### <a name="to-set-up-the-substitute-sender-address-for-all-outbound-email-messages"></a>To set up the substitute sender address for all outbound email messages
1. In the **Exchange admin centre** for your Microsoft 365 account, find the mailbox to use as the substitute address, then copy or make a note of the address. If you need a new address, go to your Microsoft 365 admin centre to create a new user and set up their mailbox.
2. In [!INCLUDE[d365fin](includes/d365fin_md.md)] choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **SMTP Email Setup** , and then choose the related link.
3. In the **Send As** field, enter the substitute address.
4. Copy or make a note of the address in the **User ID** field.
5. In the **Exchange admin centre** , find the mailbox to use as the substitute address, and then enter the address from the **User ID** field in the **Send As** field. For more information, see [Use the EAC to assign permissions to individual mailboxes](/Exchange/recipients/mailbox-permissions?view=exchserver-2019#use-the-eac-to-assign-permissions-to-individual-mailboxes).

### <a name="to-use-the-substitute-address-in-approval-workflows"></a>To use the substitute address in approval workflows
1. In [!INCLUDE[d365fin](includes/d365fin_md.md)] choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **SMTP Email Setup** , and then choose the related link.
2. Copy or make a note of the address in the **User ID** field.
3. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Approval User Setup** , and then choose the related link.
4. In the **Exchange admin centre** , find the mailboxes for each user listed in the **Approval User Setup** page, and in the **Send As** field enter the address from the **User ID** field of the **SMTP Email Setup** page in [!INCLUDE[d365fin](includes/d365fin_md.md)]. For more information, see [Manage permissions for recipients](/Exchange/recipients/mailbox-permissions?view=exchserver-2019).
5. In [!INCLUDE[d365fin](includes/d365fin_md.md)] choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **SMTP Email Setup** , and then choose the related link.
6. To enable substitution, turn on the **Allow Sender Substitution** toggle.

> [!Note]
> [!INCLUDE[d365fin](includes/d365fin_md.md)] will determine which address to display in the following order: <br><br> 1. The address specified in the **E-Mail** field on the **Approval User Setup** page for messages in a workflow. <br> 2. The address specified in the **Send As** field in the **SMTP Email Setup** page. <br> 3. The address specified in the **User ID** field in the **SMTP Email Setup** page.

## <a name="set-up-public-folders-and-rules-for-email-logging-in-exchange-online"></a>Set up Public Folders and Rules for Email Logging in Exchange Online
Get more out of the communications between salespeople and your existing or potential customers by tracking email exchanges, and then turning them into actionable opportunities. For more information, see [Track Email Message Exchanges Between Salespeople and Contacts](marketing-set-up-email-logging.md).  

[!INCLUDE[admin-setup-email-public-folder](includes/admin-setup-email-public-folder.md)]

Next, you connect [!INCLUDE[prodshort](includes/prodshort.md)] with Exchange Online. For more information, see [Track Email Message Exchanges Between Salespeople and Contacts](marketing-set-up-email-logging.md).  

## <a name="see-also"></a>See Also
[Shared mailboxes in Exchange Online](/exchange/collaboration-exo/shared-mailboxes)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  
[Setting Up [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)  
[Send Documents by Email](ui-how-send-documents-email.md)  
[Customising [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions](ui-extensions.md)  
[Using [!INCLUDE[d365fin](includes/d365fin_md.md)] as Your Business Inbox in Outlook](admin-outlook.md)  
[Getting [!INCLUDE[d365fin](includes/d365fin_md.md)] on My Mobile Device](install-mobile-app.md)
