---
title: Suggest Vendor Payments
description: Use the Suggest Vendor Payments batch job to create payment lines for your vendors based on due dates and payment discounts.
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bnielse
ms.topic: conceptual
ms.search.keywords: 'vendor payment, creditor, debt, balance due, AP'
ms.search.form: '256,'
ms.date: 12/04/2023
ms.custom: bap-template
---
# <a name="suggest-vendor-payments"></a>Suggest Vendor Payments

On the **Payment Journal** page, you can use the **Suggest Vendor Payments** batch job to suggest payment lines. Based on your settings, [!INCLUDE [prod_short](includes/prod_short.md)] suggests lines for:

- Payments that are due soon.
- Payments where a payment discount is available.

To benefit fully from payment suggestions, you must prioritise your vendors. To learn more about prioritising vendors, go to [Prioritise Vendors](purchasing-how-prioritize-vendors.md).  

> [!NOTE]  
> The batch job excludes vendor ledger entries that are **On Hold** or that are already applied and have a value in the **Applies-to ID** field.  

> [!IMPORTANT]  
> If you want to take advantage of payment discounts, and have entered an available amount, the amount will be used for:  
>
> * Prioritised overdue vendor entries first, in order of priority.
> * Overdue vendor entries that aren't prioritised.  
> * Open vendor entries that qualify for payment discounts. The entries are arranged by vendor number.  

## <a name="use-the-suggest-vendor-payments-action"></a>Use the Suggest Vendor Payments action

1. Select the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Payment Journals**, and then select the related link.  
2. Open the journal, and then select the **Suggest Vendor Payments** action.  
3. Fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  
4. Select the **OK** button.  

## <a name="insert-the-due-date-as-posting-date-on-payment-journal-lines"></a>Insert the due date as posting date on payment journal lines

When you use the **Suggest Vendor Payments** batch job to create payment lines for your vendors, you can fill two special fields to ensure that the generated lines use the due date to calculate the posting date. These fields are **Calculate Posting Date from Applies-to-Doc Due Date** and **Applies-to-Doc Due Date Offset**.  

> [!IMPORTANT]  
> You can't use the **Calculate Posting Date from Applies-to-Doc Due Date** field together with the **Find Payment Discounts** field or the **Summarise per Vendor** field. If the posting date is based on the due date, some payment discounts might not calculate correctly because the posting date is after the payment discount date.  

Also, if the calculated posting date is in the past, then the posting date is moved up to the work date and a warning displays.  

You can also manually create payment lines using the due date to calculate the posting date. After you apply vendor ledger entries, you can use the **Calculate Posting Date** action to update the posting date on the journal line with the due date of the related purchase invoice. To learn more about this manual process, go to [Apply Purchase Transactions Manually](payables-how-apply-purchase-transactions-manually.md).  

> [!NOTE]  
> If the purchase invoice is overdue, the posting date is set to the work date and the font on the line changes to red.  

## <a name="see-also"></a>See also

- [Managing Payables](payables-manage-payables.md)  
- [Making Payments](payables-make-payments.md)  
- [Work with General Journals](ui-work-general-journals.md)  
- [Work with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
