---
title: Specify the Layout of a Cheque| Microsoft Docs
description: You can design and print your cheques in different formats to conform with standards.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: print check, customize
ms.date: 04/01/2020
ms.author: edupont
ms.openlocfilehash: 479281e24bffb824f9fc8499bb34ab6b11311a52
ms.sourcegitcommit: 88e4b30eaf6fa32af0c1452ce2f85ff1111c75e2
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 04/01/2020
ms.locfileid: "3183684"
---
# <a name="select-a-check-layout"></a><span data-ttu-id="769bc-103">Select a Cheque Layout</span><span class="sxs-lookup"><span data-stu-id="769bc-103">Select a Check Layout</span></span>
<span data-ttu-id="769bc-104">You can design your cheques to conform with the standards set by the local authorities.</span><span class="sxs-lookup"><span data-stu-id="769bc-104">You can design your checks to conform with the standards set by the local authorities.</span></span> <span data-ttu-id="769bc-105">Cheque images can be printed in English, French, or Spanish.</span><span class="sxs-lookup"><span data-stu-id="769bc-105">Check images can be printed in English, French, or Spanish.</span></span>

<span data-ttu-id="769bc-106">Cheques are designed to print in both the United States and Canadian cheque image formats in either a cheque-stub-cheque format or a stub-stub-cheque format.</span><span class="sxs-lookup"><span data-stu-id="769bc-106">Checks are designed to print in both the United States and Canadian check image formats in either a check-stub-check format or a stub-stub-check format.</span></span>

## <a name="to-select-a-check-layout"></a><span data-ttu-id="769bc-107">To select a cheque layout</span><span class="sxs-lookup"><span data-stu-id="769bc-107">To select a check layout</span></span>
1. <span data-ttu-id="769bc-108">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Report Selections Bank Account**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="769bc-108">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Report Selections Bank Account**, and then choose the related link.</span></span>
2. <span data-ttu-id="769bc-109">On the **Report Selection - Bank Acc.** page, in the **Usage** field, select **Cheque**.</span><span class="sxs-lookup"><span data-stu-id="769bc-109">On the **Report Selection - Bank Acc.** page, in the **Usage** field, select **Check**.</span></span>
3. <span data-ttu-id="769bc-110">Select one of the following report IDs.</span><span class="sxs-lookup"><span data-stu-id="769bc-110">Select one of the following report IDs.</span></span>

| <span data-ttu-id="769bc-111">Report ID</span><span class="sxs-lookup"><span data-stu-id="769bc-111">Report ID</span></span> | <span data-ttu-id="769bc-112">Report Name</span><span class="sxs-lookup"><span data-stu-id="769bc-112">Report Name</span></span> | <span data-ttu-id="769bc-113">Description</span><span class="sxs-lookup"><span data-stu-id="769bc-113">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="769bc-114">1401</span><span class="sxs-lookup"><span data-stu-id="769bc-114">1401</span></span> |<span data-ttu-id="769bc-115">Cheque</span><span class="sxs-lookup"><span data-stu-id="769bc-115">Check</span></span> |<span data-ttu-id="769bc-116">This is the default report.</span><span class="sxs-lookup"><span data-stu-id="769bc-116">This is the default report.</span></span> |
| <span data-ttu-id="769bc-117">10411</span><span class="sxs-lookup"><span data-stu-id="769bc-117">10411</span></span> |<span data-ttu-id="769bc-118">Cheque (Stub/Stub/Cheque)</span><span class="sxs-lookup"><span data-stu-id="769bc-118">Check (Stub/Stub/Check)</span></span> |<span data-ttu-id="769bc-119">This report is designed to print cheques in a stub/stub/cheque format.</span><span class="sxs-lookup"><span data-stu-id="769bc-119">This report is designed to print checks in a stub/stub/check format.</span></span> |
| <span data-ttu-id="769bc-120">10412</span><span class="sxs-lookup"><span data-stu-id="769bc-120">10412</span></span> |<span data-ttu-id="769bc-121">Cheque (Stub/Cheque/Stub)</span><span class="sxs-lookup"><span data-stu-id="769bc-121">Check (Stub/Check/Stub)</span></span> |<span data-ttu-id="769bc-122">This report is designed to print cheques in a stub/cheque/stub format.</span><span class="sxs-lookup"><span data-stu-id="769bc-122">This report is designed to print checks in a stub/check/stub format.</span></span> |
| <span data-ttu-id="769bc-123">10413</span><span class="sxs-lookup"><span data-stu-id="769bc-123">10413</span></span> |<span data-ttu-id="769bc-124">Three Cheques per Page</span><span class="sxs-lookup"><span data-stu-id="769bc-124">Three Checks per Page</span></span> |<span data-ttu-id="769bc-125">This report is designed to print three cheques on each page.</span><span class="sxs-lookup"><span data-stu-id="769bc-125">This report is designed to print three checks on each page.</span></span> |

<span data-ttu-id="769bc-126">When you have set up cheque layouts, you can print cheques from the **Payment Journal** page.</span><span class="sxs-lookup"><span data-stu-id="769bc-126">When you have set up check layouts, you can print checks from the **Payment Journal** page.</span></span> <span data-ttu-id="769bc-127">For more information, see [Work with Cheques](payables-how-work-checks.md).</span><span class="sxs-lookup"><span data-stu-id="769bc-127">For more information, see [Work with Checks](payables-how-work-checks.md).</span></span>

<span data-ttu-id="769bc-128">To change one of these default cheque layouts, use either the Word or the RDLC integration to do so.</span><span class="sxs-lookup"><span data-stu-id="769bc-128">To change one of these default check layouts, use either the Word or the RDLC integration to do so.</span></span> <span data-ttu-id="769bc-129">For more information, see [Create and Modify Custom Report Layouts](ui-how-create-custom-report-layout.md).</span><span class="sxs-lookup"><span data-stu-id="769bc-129">For more information, see [Create and Modify Custom Report Layouts](ui-how-create-custom-report-layout.md).</span></span>

## <a name="using-micr-and-security-fonts"></a><span data-ttu-id="769bc-130">Using MICR and Security Fonts</span><span class="sxs-lookup"><span data-stu-id="769bc-130">Using MICR and Security Fonts</span></span>
<span data-ttu-id="769bc-131">The online version of [!INCLUDE[d365fin](includes/d365fin_md.md)] contains pre-installed fonts on the servers that can be used when defining cheque layouts.</span><span class="sxs-lookup"><span data-stu-id="769bc-131">The online version of [!INCLUDE[d365fin](includes/d365fin_md.md)] contains pre-installed fonts on the servers that can be used when defining check layouts.</span></span> <span data-ttu-id="769bc-132">The following outlines which fonts are available and has links to detailed information by the 3rd-party suppliers of the fonts.</span><span class="sxs-lookup"><span data-stu-id="769bc-132">The following outlines which fonts are available and has links to detailed information by the 3rd-party suppliers of the fonts.</span></span>

> [!Important]
> <span data-ttu-id="769bc-133">MICR and cheque security fonts in Microsoft Dynamics [!INCLUDE[d365fin](includes/d365fin_md.md)] are licensed in a font package from IDAutomation.com, Inc. These products may only be used as part of and in connection with Microsoft Dynamics [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="769bc-133">MICR and check security fonts in Microsoft Dynamics [!INCLUDE[d365fin](includes/d365fin_md.md)] are licensed in a font package from IDAutomation.com, Inc. These products may only be used as part of and in connection with Microsoft Dynamics [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>

<span data-ttu-id="769bc-134">In update 15.3 and newer, Magnetic Ink Character Recognition (MICR) fonts are installed and available to use.</span><span class="sxs-lookup"><span data-stu-id="769bc-134">In update 15.3 and newer, Magnetic Ink Character Recognition (MICR) fonts are installed and available to use.</span></span> <span data-ttu-id="769bc-135">Both the E-13B and the CMC-7 standards are supported.</span><span class="sxs-lookup"><span data-stu-id="769bc-135">Both the E-13B and the CMC-7 standards are supported.</span></span> <span data-ttu-id="769bc-136">In addition to MICR fonts, special security fonts are available to generate text, names, amounts, and the currency symbols Dollar, Euro, Pound, and Yen, which are hard to tamper with once a cheque has been printed.</span><span class="sxs-lookup"><span data-stu-id="769bc-136">In addition to MICR fonts, special security fonts are available to generate text, names, amounts, and the currency symbols Dollar, Euro, Pound, and Yen, which are hard to tamper with once a check has been printed.</span></span>

> [!NOTE]
> <span data-ttu-id="769bc-137">For security and legal reasons, you cannot upload custom fonts to the [!INCLUDE[d365fin](includes/d365fin_md.md)] environment.</span><span class="sxs-lookup"><span data-stu-id="769bc-137">For security and legal reasons, you cannot upload custom fonts to the [!INCLUDE[d365fin](includes/d365fin_md.md)] environment.</span></span>

### <a name="micr-e-13b-specifications"></a><span data-ttu-id="769bc-138">MICR E-13B Specifications</span><span class="sxs-lookup"><span data-stu-id="769bc-138">MICR E-13B Specifications</span></span>
<span data-ttu-id="769bc-139">The following summarises specifications for the MICR E-13B fonts that may be useful when calibrating fonts to be on cheque layouts with specific MICR printers.</span><span class="sxs-lookup"><span data-stu-id="769bc-139">The following summarizes specifications for the MICR E-13B fonts that may be useful when calibrating fonts to be on check layouts with specific MICR printers.</span></span>

<span data-ttu-id="769bc-140">![MICR E-13B Specifications](media/font_MICR_E-13B_Specifications.png "MICR E-13B Specifications")</span><span class="sxs-lookup"><span data-stu-id="769bc-140">![MICR E-13B Specifications](media/font_MICR_E-13B_Specifications.png "MICR E-13B Specifications")</span></span>

<span data-ttu-id="769bc-141">The full specification of MICR E-13B fonts can be found in the supplier's documentation here: (https://www.idautomation.com/micr-fonts/e13b/).</span><span class="sxs-lookup"><span data-stu-id="769bc-141">The full specification of MICR E-13B fonts can be found in the supplier's documentation here: (https://www.idautomation.com/micr-fonts/e13b/).</span></span>

### <a name="micr-cmc-7-specifications"></a><span data-ttu-id="769bc-142">MICR CMC-7 Specifications</span><span class="sxs-lookup"><span data-stu-id="769bc-142">MICR CMC-7 Specifications</span></span>
<span data-ttu-id="769bc-143">The following CMC-7 fonts are available in [!INCLUDE[d365fin](includes/d365fin_md.md)] online:</span><span class="sxs-lookup"><span data-stu-id="769bc-143">The following CMC-7 fonts are available in [!INCLUDE[d365fin](includes/d365fin_md.md)] online:</span></span>

- <span data-ttu-id="769bc-144">IDAutomationCMC7</span><span class="sxs-lookup"><span data-stu-id="769bc-144">IDAutomationCMC7</span></span>
- <span data-ttu-id="769bc-145">IDAutomationCMC7n10</span><span class="sxs-lookup"><span data-stu-id="769bc-145">IDAutomationCMC7n10</span></span>
- <span data-ttu-id="769bc-146">IDAutomationCMC7n25</span><span class="sxs-lookup"><span data-stu-id="769bc-146">IDAutomationCMC7n25</span></span>
-   <span data-ttu-id="769bc-147">IDAutomationCMC7n40</span><span class="sxs-lookup"><span data-stu-id="769bc-147">IDAutomationCMC7n40</span></span>

<span data-ttu-id="769bc-148">The following summarises specifications for the MICR CMC-7 fonts that may be useful when calibrating fonts to be on cheque layouts with specific MICR printers.</span><span class="sxs-lookup"><span data-stu-id="769bc-148">The following summarizes specifications for the MICR CMC-7 fonts that may be useful when calibrating fonts to be on check layouts with specific MICR printers.</span></span>

<span data-ttu-id="769bc-149">![MICR CMC-7 Specifications](media/font_MICR_CMC-7_Specifications.png "MICR CMC-7 Specifications")</span><span class="sxs-lookup"><span data-stu-id="769bc-149">![MICR CMC-7 Specifications](media/font_MICR_CMC-7_Specifications.png "MICR CMC-7 Specifications")</span></span>

<span data-ttu-id="769bc-150">The full specification of MICR CMC-7 fonts can be found in the supplier's documentation here: (http://www.idautomation.com/micr-fonts/cmc7/).</span><span class="sxs-lookup"><span data-stu-id="769bc-150">The full specification of MICR CMC-7 fonts can be found in the supplier's documentation here: (http://www.idautomation.com/micr-fonts/cmc7/).</span></span>

### <a name="secure-font-specifications"></a><span data-ttu-id="769bc-151">Secure Font Specifications</span><span class="sxs-lookup"><span data-stu-id="769bc-151">Secure Font Specifications</span></span>
<span data-ttu-id="769bc-152">The following Summarises specifications for cheque security fonts that may be useful when calibrating fonts to be on cheque layouts with specific MICR printers.</span><span class="sxs-lookup"><span data-stu-id="769bc-152">The following summarizes specifications for check security fonts that may be useful when calibrating fonts to be on check layouts with specific MICR printers.</span></span>

<span data-ttu-id="769bc-153">![Cheque Security Font Specifications](media/font_check-security-font_Specifications.png "Cheque Security Font Specifications")</span><span class="sxs-lookup"><span data-stu-id="769bc-153">![Check Security Font Specifications](media/font_check-security-font_Specifications.png "Check Security Font Specifications")</span></span>

<span data-ttu-id="769bc-154">The full specification of cheque security fonts can be found in the supplier's documentation here: (https://www.idautomation.com/security-fonts/).</span><span class="sxs-lookup"><span data-stu-id="769bc-154">The full specification of check security fonts can be found in the supplier's documentation here: (https://www.idautomation.com/security-fonts/).</span></span>

<span data-ttu-id="769bc-155">Fonts for other purposes are also available in [!INCLUDE[prodshort](includes/prodshort.md)].</span><span class="sxs-lookup"><span data-stu-id="769bc-155">Fonts for other purposes are also available in [!INCLUDE[prodshort](includes/prodshort.md)].</span></span> <span data-ttu-id="769bc-156">For more information, see [Available Fonts](ui-fonts.md)</span><span class="sxs-lookup"><span data-stu-id="769bc-156">For more information, see [Available Fonts](ui-fonts.md)</span></span>

## <a name="see-also"></a><span data-ttu-id="769bc-157">See Also</span><span class="sxs-lookup"><span data-stu-id="769bc-157">See Also</span></span>
[<span data-ttu-id="769bc-158">Create and Modify Custom Report Layouts</span><span class="sxs-lookup"><span data-stu-id="769bc-158">Create and Modify Custom Report Layouts</span></span>](ui-how-create-custom-report-layout.md)  
[<span data-ttu-id="769bc-159">Fonts in Business Central</span><span class="sxs-lookup"><span data-stu-id="769bc-159">Fonts in Business Central</span></span>](ui-fonts.md)  
[<span data-ttu-id="769bc-160">Managing Payables</span><span class="sxs-lookup"><span data-stu-id="769bc-160">Managing Payables</span></span>](payables-manage-payables.md)  
<span data-ttu-id="769bc-161">[Reconciling Bank Accounts](bank-manage-bank-accounts.md) </span><span class="sxs-lookup"><span data-stu-id="769bc-161">[Reconciling Bank Accounts](bank-manage-bank-accounts.md) </span></span>  
[<span data-ttu-id="769bc-162">Completing Period-End Processes</span><span class="sxs-lookup"><span data-stu-id="769bc-162">Completing Period-End Processes</span></span>](year-how-complete-period-end-processes.md)  
<span data-ttu-id="769bc-163">[Working with [!INCLUDE[prodshort](includes/prodshort.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="769bc-163">[Working with [!INCLUDE[prodshort](includes/prodshort.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="769bc-164">General Business Functionality</span><span class="sxs-lookup"><span data-stu-id="769bc-164">General Business Functionality</span></span>](ui-across-business-areas.md)
