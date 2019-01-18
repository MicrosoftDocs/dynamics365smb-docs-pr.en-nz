---
title: Change the Way a Report Looks by Selecting a Different Layout | Microsoft Docs
description: You can use different layouts for a report, and switch between layouts to change how a report looks.
services: project-madeira
documentationcenter: 
author: jswymer
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: customized report, document layout, logo, personalize
ms.date: 10/01/2018
ms.author: jswymer
ms.translationtype: HT
ms.sourcegitcommit: 33b900f1ac9e295921e7f3d6ea72cc93939d8a1b
ms.openlocfilehash: a68c26e94aa4adda7c1f546e57331a741dcfe94b
ms.contentlocale: en-nz
ms.lasthandoff: 11/26/2018

---
# <a name="change-which-layout-is-currently-used-on-a-report"></a>Change Which Layout is Currently Used on a Report
A report can be set up with more than one report layout, which you can then switch among as needed.

Depending on the layouts that are available for a report, you can choose to use a built-in RDLC report layout, a built-in Word report layout, or a custom layout. For more information about RDLC and Word report layouts, built-in and custom layouts, and more, see [Manage Report Layouts](ui-manage-report-layouts.md).

## <a name="to-change-the-layout-that-is-used-on-a-report"></a>To change the layout that is used on a report
1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Report Layout Selection**, and then choose the related link.  
   The **Report Layout Selection** page lists all the reports that are available for the company that is specified in the Company field at the top of the page. The Selected Layout field specifies the layout that is currently used on the report.
2. Set the **Company** field at the top of the page to the company that includes the report.
3. To change the layout that is used by a report, in the row for the report in the list, set the **Selected Layout** field to one of the following options:
   * RDLC (built-in), uses the built-in RDLC report layout on the report.
   * Word (built-in), uses the built-in Word report layout on the report.
   * Custom, uses a custom layout on the report.  
     You can see which custom layouts are available for the report in the Report Layouts Part FactBox. If there are no custom layouts for the report, then you will have to create one first. If you choose this option, go to the next procedure to specify the custom layout that you want to use.

    > [!NOTE]  
    >   If you choose **RDLC (built-in)** or **Word (built-in)** and you get an error message that the report does not have a layout of the specified type, then you must choose another layout option or create a custom report layout of the type that you want to use.

If you selected a built-in RDLC or Word report layout, then no further action is required and the layout will be used the next time the report is run.

## <a name="to-specify-a-custom-layout-on-a-report"></a>To specify a custom layout on a report
1. You specify which custom layout to use on the report from the **Custom Report Layouts** page. If the **Custom Report Layouts** page is not open, then in the **Report Layout Description** field, choose the lookup button.
2. On the **Custom Report Layouts** page, select the row for custom layout that you want to use, and then close the page.

You return to the **Report Layout Selection** page. The name of the selected custom layout displays in the **Custom Layout Description** field. The custom layout will be used the next time that you run the report.

## <a name="see-also"></a>See Also
[Managing Report Layouts](ui-manage-report-layouts.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

