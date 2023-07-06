---
title: Sharing Data
description: Learn about the different ways to share business data from Business Central.
author: jswymer
ms.topic: conceptual
ms.workload: na
ms.search.keywords: null
ms.date: 09/21/2022
ms.author: jswymer
---
# <a name="sharing-business-data-from-business-central"></a><a name="sharing-business-data-from-business-central"></a><a name="sharing-business-data-from-business-central"></a>Sharing Business Data from Business Central

Collaboration among people inside and outside an organisation is integral part of most businesses. [!INCLUDE[prod_short](includes/prod_short.md)] offers several features for sharing business data, like a list of records, specific records, or documents. <!--, with others&mdash;even those people who don't have a Business Central license in some cases.-->

With all these features, access to data is protected by the licence and permissions of Business Central.

## <a name="copying-a-link"></a><a name="copying-a-link"></a><a name="copying-a-link"></a>Copying a link

![Supported](media/check.png) Business Central Online ![Supported](media/check.png) Business Central On-premises

From any page, you can copy the page's URL, then paste and distribute it in other forms of media like emails, Teams chats, or text messages. The easiest way to copy a link is by selecting **Share** > **Copy Link** from the top of the page. Another way is to copy the URL directly from the browser's address box.

### <a name="modify-the-page-link"></a><a name="modify-the-page-link"></a><a name="modify-the-page-link"></a>Modify the page link

After you copy a link, before you send it, you can modify the URL to manipulate what shows when the page opens. You can, for example, add filters or specify a different company.

For more information, see [Web Client URL](/dynamics365/business-central/dev-itpro/developer/devenv-web-client-urls).

### <a name="about-filtered-lists"></a><a name="about-filtered-lists"></a><a name="about-filtered-lists"></a>About filtered lists

Using the filter pane on list pages, you can apply filters to narrow-down the records shown in the list. If you use the **Copy Link** action or copy the URL from the browser, the page link won't include your filter changes. Users that open the link will see the full collection. The way to keep the filtering on a collection page link is to save the filtered page as a **View** first. Then, open the view and copy the link from there.

For more information, see [Sorting, Searching, and Filtering](ui-enter-criteria-filters.md).

## <a name="sharing-to-teams"></a><a name="sharing-to-teams"></a><a name="sharing-to-teams"></a>Sharing to Teams

![Supported](media/check.png) Business Central Online ![Not Supported](media/x-icon.png) Business Central On-premises

Directly from most collection pages and details pages, you can send a link to the page to people, group chats or channels. For example, share a link to a filtered view of your records. If you've installed the [!INCLUDE[prod_short](includes/prod_short.md)] app for Teams, the link will automatically expand into a compact card for you to include with your message. Recipients then select the link or card to open the page in Business Central.

For more information, see [Sharing Records and Page Links in Teams](across-working-with-teams.md).

## <a name="sharing-through-onedrive"></a><a name="sharing-through-onedrive"></a><a name="sharing-through-onedrive"></a>Sharing Through OneDrive

![Supported](media/check.png) Business Central Online ![Supported](media/check.png) Business Central On-premises

Business Central makes it easy to store, manage, and share files with other people through OneDrive for Business. On most pages where files are available, such as the Report Inbox or files that are attached to records, you'll find the **Open in OneDrive** and **Share** actions. Both actions save a copy of a file to OneDrive. Once in OneDrive, you can use its sharing and contribution features on the file. The difference in the actions is that **Open in OneDrive** opens the file in OneDrive. **Share** opens a page the let's you select who you want to share the file with. Recipients will get a notification email to access the file from your OneDrive.

For more information, see [Sharing Files in OneDrive](across-share-onedrive.md).

## <a name="opening-in-excel"></a><a name="opening-in-excel"></a><a name="opening-in-excel"></a>Opening in Excel

![Supported](media/check.png) Business Central Online ![Supported](media/check.png) Business Central On-premises

For list pages and lists embedded on a page, you can use the **Open in Excel** action. This action exports the list of records to an Excel workbook (.xlsx file), which you can share with others. In the workbook, you can also use the Share feature that's part of Excel.

For more information, see [Viewing and Editing in Excel](across-work-with-excel.md).

## <a name="sharing-rows-or-tables"></a><a name="sharing-rows-or-tables"></a><a name="sharing-rows-or-tables"></a>Sharing rows or tables

![Supported](media/check.png) Business Central Online ![Supported](media/check.png) Business Central On-premises

You can share one or more records in a list. Just select the <kbd>Ctrl</kbd>+<kbd>C</kbd> keyboard shortcut to copy to your clipboard. Then paste what you copied into another application by pressing <kbd>Ctrl</kbd>+<kbd>V</kbd>. For example, copying three sales orders and pasting that into an email will display the orders in a nicely formatted table.

For more information, see [Copy and Paste FAQ](faq-copy-paste.yml).

## <a name="see-also"></a><a name="see-also"></a><a name="see-also"></a>See Also

[Business Central and OneDrive Integration](across-onedrive-overview.md)  
[Managing OneDrive Integration with Business Central](admin-onedrive-integration.md)  
[OneDrive FAQ](admin-onedrive-faq.md)
