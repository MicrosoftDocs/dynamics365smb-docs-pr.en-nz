---
title: Specify a Default Printer
description: Learn about the different ways to set up printers to be used by default for print jobs.
author: jswymer
ms.topic: how-to
ms.reviewer: na
ms.service: dynamics365-business-central
ms.custom: bap-template
ms.search.keywords: 'online printing, email printing, cloud printing, Universal Print'
ms.search.form: '2650, 2750, 2752, 2753, 2754, 8900,'
ms.date: 02/09/2023
ms.author: jswymer
---
# <a name="specify-a-default-printer"></a><a name="default"></a>Specify a Default Printer

After printers have been set up in Business Central, you can then specify which printer you want to use by default. There are a couple of ways to specify printers to be used by default for reports and other print jobs. A default printer is useful if you work with different reports that require different printers because of their placement in the company or their output capabilities.

> [!IMPORTANT]
> The only printers that you can specify as default are **Microsoft Print to PDF** and cloud printers that have already been set up for use in Business Central, like Email printers and Universal Print printers. Cloud printers are typically set up by an admin. For more information, see [Printer Setup and Management](admin-printer-setup-overview.md).   

## <a name="set-a-printer-as-a-default-printer-for-all-print-jobs"></a>Set a printer as a default printer for all print jobs

Through the **Printer Management** page you set up a printer as a default printer for all print jobs. You can specify the printer as default for you only or for all users.

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Printer Management**, then select the related link.

    > [!TIP]
    > You can also open the **Printer Management** page from the **Printer Selections** page by choosing **Printer Management**.  
2. On the **Printer Management** page, select a printer from the list, choose **Manage**, then choose **Set as my default printer** or **Set as default printer for all users**.

> [!NOTE]
> Setting a default printer from the **Printer Management** adds an entry in the **Printer Selections**.

## <a name="set-a-default-printer-for-specific-reports"></a>Set a default printer for specific reports

The **Printer Selections** page lets you specify the printer a report will use by default. Default printers are set on a user-account basis. You can set a default printer for just yourself, another user, or all users.

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Printer Selections**, then select the related link. Alternatively, select a printer on the **Printer Management** page, then choose the **Printer Selections** action.
2. Choose the **New** action to add a printer selection for a specific report.
3. Fill in the fields as necessary.

The specified report is now set up to print to the selected printer by default.

> [!NOTE]
> When you print the report in question, you can select a different using the **Print** field on the report request page.

> [!NOTE]
> If you do not set a report up for a specific printer on the **Printer Selections** page, then it is printed to the default printer of the company, as defined on the **Printer Management** page.

You or the administrator can also use the **Printer Selections** page to define other variations of printing for users and reports. The following table describes the combination of values to specify different printing setups for a report.

|To                                                 |Set the following values                                             |
|---------------------------------------------------|---------------------------------------------------------------------|
|Print a report to a specific printer for all users |Specify values in the **Report ID** and **Printer Name** fields and leave the **User ID** field blank.|
|Print all reports to a specific printer for a specific user|Specify values in the **User ID** and **Printer Name** fields and leave the **Report ID** field blank. This entry does the same as the **Set as my default printer** action on the **Print Management** page.|
|Set the default printer for all reports for all users|Specify a value in the **Printer Name** field and leave the **User ID** and **Report ID** fields blank. This entry does the same as the **Set as default printer for all users** action on the **Print Management** page.|
|Print a specific report to the user's default printer|Specify a value in the **Report ID** field and leave the **Printer Name** and **User ID** fields blank.|
|Print a specific report to a specific printer for a specific user|Specify values in all three fields.|

> [!NOTE]
> More specific printer selections take precedence over more general printer selections. For example, a printer selection that has values in the **User ID**, **Report ID**, and **Printer Name** fields takes precedence over a printer selection that has blank entries in the **User ID** or **Report ID** fields.

## <a name="choosing-the-printer-when-running-a-report"></a>Choosing the printer when running a report

Instead of using the default printer when running a report, you can override this setting from the request page. Simply choose the printer you want to use for this report generation in the **Printer** dropdown menu.

## <a name="sizing-print-jobs"></a>Sizing print jobs

Cloud printing is designed for documents of a reasonable size. Most cloud services, including PrintNode and HP ePrint, have a limit of 10 MB per job. If you need to print larger reports, you may have to split them in multiple printouts.

## <a name="see-also"></a>See also

[Printer Management](admin-printer-setup-overview.md)  
[Set Up Universal Print Printers](admin-printer-setup-universal-print.md)  
[Set Up Email Printers](admin-printer-setup-email.md)  
[Printing a Report](ui-work-report.md#PrintReport)  
[Work with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  
[Run Batch Jobs](ui-how-run-batch-jobs.md)  
[Send Documents by Email](ui-how-send-documents-email.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
