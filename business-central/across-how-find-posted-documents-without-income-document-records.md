---
title: Search for Documents without Attachments| Microsoft Docs
Description: You can search for general ledger entries for posted purchase and sales documents that do not have incoming electronic documents, such as imported invoices.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: electronic document, e-invoice, incoming document, OCR, ecommerce, document exchange, import invoice
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 33b900f1ac9e295921e7f3d6ea72cc93939d8a1b
ms.openlocfilehash: 34bbc67c0f2bcc5afe408e75a7d3ceb582160d87
ms.contentlocale: en-nz
ms.lasthandoff: 11/26/2018

---
# <a name="find-posted-documents-without-incoming-document-records"></a><span data-ttu-id="4d8b4-102">Find Posted Documents without Incoming Document Records</span><span class="sxs-lookup"><span data-stu-id="4d8b4-102">Find Posted Documents without Incoming Document Records</span></span>
<span data-ttu-id="4d8b4-103">From the **Chart of Accounts** and **General Ledger Entries** pages, you can use a search function to find general ledger entries for posted purchase and sales documents that do not have incoming document records and then centrally link to existing records or create new ones with attached document files.</span><span class="sxs-lookup"><span data-stu-id="4d8b4-103">From the **Chart of Accounts** and **General Ledger Entries** pages, you can use a search function to find general ledger entries for posted purchase and sales documents that do not have incoming document records and then centrally link to existing records or create new ones with attached document files.</span></span>

## <a name="to-find-posted-documents-without-incoming-document-records"></a><span data-ttu-id="4d8b4-104">To find posted documents without incoming document records</span><span class="sxs-lookup"><span data-stu-id="4d8b4-104">To find posted documents without incoming document records</span></span>
1. <span data-ttu-id="4d8b4-105">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Chart of Accounts**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="4d8b4-105">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Chart of Accounts**, and then choose the related link.</span></span>
2. <span data-ttu-id="4d8b4-106">Select a line for a G/L account for whose general ledger entries you want to see posted purchase and sales documents without incoming document records, and then choose the **Posted Documents without Incoming Document** action.</span><span class="sxs-lookup"><span data-stu-id="4d8b4-106">Select a line for a G/L account for whose general ledger entries you want to see posted purchase and sales documents without incoming document records, and then choose the **Posted Documents without Incoming Document** action.</span></span>
3. <span data-ttu-id="4d8b4-107">Alternatively, choose the **Ledger Entries** action.</span><span class="sxs-lookup"><span data-stu-id="4d8b4-107">Alternatively, choose the **Ledger Entries** action.</span></span>
4. <span data-ttu-id="4d8b4-108">On the **General Ledger Entries** page, choose the **Posted Documents without Incoming Documents** action.</span><span class="sxs-lookup"><span data-stu-id="4d8b4-108">On the **General Ledger Entries** page, choose the **Posted Documents without Incoming Documents** action.</span></span>

<span data-ttu-id="4d8b4-109">The **Posted Documents without Incoming Document** page opens showing posted purchase and sales documents without incoming document records represented by general ledger entries on the G/L account that you opened the page for.</span><span class="sxs-lookup"><span data-stu-id="4d8b4-109">The **Posted Documents without Incoming Document** page opens showing posted purchase and sales documents without incoming document records represented by general ledger entries on the G/L account that you opened the page for.</span></span> <span data-ttu-id="4d8b4-110">The page can show a maximum of 1000 lines.</span><span class="sxs-lookup"><span data-stu-id="4d8b4-110">The page can show a maximum of 1000 lines.</span></span> <span data-ttu-id="4d8b4-111">By default, the **Date Filter** field therefore contains a filter that limits the lines to entries with posting dates from the beginning of the accounting period to the work date.</span><span class="sxs-lookup"><span data-stu-id="4d8b4-111">By default, the **Date Filter** field therefore contains a filter that limits the lines to entries with posting dates from the beginning of the accounting period to the work date.</span></span>

## <a name="to-connect-found-documents-to-existing-incoming-document-records"></a><span data-ttu-id="4d8b4-112">To connect found documents to existing incoming document records</span><span class="sxs-lookup"><span data-stu-id="4d8b4-112">To connect found documents to existing incoming document records</span></span>
1. <span data-ttu-id="4d8b4-113">On the **Posted Documents without Incoming Document** page, select the line for a posted document that you want to connect to an existing incoming document record, and then choose the **Select Incoming Document** action.</span><span class="sxs-lookup"><span data-stu-id="4d8b4-113">On the **Posted Documents without Incoming Document** page, select the line for a posted document that you want to connect to an existing incoming document record, and then choose the **Select Incoming Document** action.</span></span>
2. <span data-ttu-id="4d8b4-114">On the **Incoming Documents** page, select the incoming document record that you want to connect to posted document found, and then choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="4d8b4-114">On the **Incoming Documents** page, select the incoming document record that you want to connect to posted document found, and then choose the **OK** button.</span></span>
3. <span data-ttu-id="4d8b4-115">On the **Posted Documents without Incoming Document** page, the selected incoming document record is now connected to the posted document, as you can see in the **Incoming Document Files** FactBox.</span><span class="sxs-lookup"><span data-stu-id="4d8b4-115">On the **Posted Documents without Incoming Document** page, the selected incoming document record is now connected to the posted document, as you can see in the **Incoming Document Files** FactBox.</span></span>

<span data-ttu-id="4d8b4-116">If a relevant incoming document record does not exist on the **Incoming Documents** page, then you can create it.</span><span class="sxs-lookup"><span data-stu-id="4d8b4-116">If a relevant incoming document record does not exist on the **Incoming Documents** page, then you can create it.</span></span> <span data-ttu-id="4d8b4-117">For more information, see [Create Incoming Document Records](across-how-create-income-document-records.md).</span><span class="sxs-lookup"><span data-stu-id="4d8b4-117">For more information, see [Create Incoming Document Records](across-how-create-income-document-records.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="4d8b4-118">See Also</span><span class="sxs-lookup"><span data-stu-id="4d8b4-118">See Also</span></span>
[<span data-ttu-id="4d8b4-119">Process Incoming Documents</span><span class="sxs-lookup"><span data-stu-id="4d8b4-119">Process Incoming Documents</span></span>](across-process-income-documents.md)  
[<span data-ttu-id="4d8b4-120">Incoming Documents</span><span class="sxs-lookup"><span data-stu-id="4d8b4-120">Incoming Documents</span></span>](across-income-documents.md)  
[<span data-ttu-id="4d8b4-121">Purchasing</span><span class="sxs-lookup"><span data-stu-id="4d8b4-121">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="4d8b4-122">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="4d8b4-122">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

