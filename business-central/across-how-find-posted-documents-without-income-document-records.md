---
title: Search for Documents without Attachments| Microsoft Docs
Description: You can search for general ledger entries for posted purchase and sales documents that do not have incoming electronic documents, such as imported invoices.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: electronic document, e-invoice, incoming document, OCR, ecommerce, document exchange, import invoice
ms.date: 04/01/2020
ms.author: sgroespe
ms.openlocfilehash: 0b31d225083d566967b3c9cb7facee564c3d3466
ms.sourcegitcommit: 88e4b30eaf6fa32af0c1452ce2f85ff1111c75e2
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 04/01/2020
ms.locfileid: "3188556"
---
# <a name="find-posted-documents-without-incoming-document-records"></a><span data-ttu-id="35a09-103">Find Posted Documents without Incoming Document Records</span><span class="sxs-lookup"><span data-stu-id="35a09-103">Find Posted Documents without Incoming Document Records</span></span>
<span data-ttu-id="35a09-104">From the **Chart of Accounts** and **General Ledger Entries** pages, you can use a search function to find general ledger entries for posted purchase and sales documents that do not have incoming document records and then centrally link to existing records or create new ones with attached document files.</span><span class="sxs-lookup"><span data-stu-id="35a09-104">From the **Chart of Accounts** and **General Ledger Entries** pages, you can use a search function to find general ledger entries for posted purchase and sales documents that do not have incoming document records and then centrally link to existing records or create new ones with attached document files.</span></span>

## <a name="to-find-posted-documents-without-incoming-document-records"></a><span data-ttu-id="35a09-105">To find posted documents without incoming document records</span><span class="sxs-lookup"><span data-stu-id="35a09-105">To find posted documents without incoming document records</span></span>
1. <span data-ttu-id="35a09-106">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Chart of Accounts**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="35a09-106">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Chart of Accounts**, and then choose the related link.</span></span>
2. <span data-ttu-id="35a09-107">Select a line for a G/L account for whose general ledger entries you want to see posted purchase and sales documents without incoming document records, and then choose the **Posted Documents without Incoming Document** action.</span><span class="sxs-lookup"><span data-stu-id="35a09-107">Select a line for a G/L account for whose general ledger entries you want to see posted purchase and sales documents without incoming document records, and then choose the **Posted Documents without Incoming Document** action.</span></span>
3. <span data-ttu-id="35a09-108">Alternatively, choose the **Ledger Entries** action.</span><span class="sxs-lookup"><span data-stu-id="35a09-108">Alternatively, choose the **Ledger Entries** action.</span></span>
4. <span data-ttu-id="35a09-109">On the **General Ledger Entries** page, choose the **Posted Documents without Incoming Documents** action.</span><span class="sxs-lookup"><span data-stu-id="35a09-109">On the **General Ledger Entries** page, choose the **Posted Documents without Incoming Documents** action.</span></span>

<span data-ttu-id="35a09-110">The **Posted Documents without Incoming Document** page opens showing posted purchase and sales documents without incoming document records represented by general ledger entries on the G/L account that you opened the page for.</span><span class="sxs-lookup"><span data-stu-id="35a09-110">The **Posted Documents without Incoming Document** page opens showing posted purchase and sales documents without incoming document records represented by general ledger entries on the G/L account that you opened the page for.</span></span> <span data-ttu-id="35a09-111">The page can show a maximum of 1000 lines.</span><span class="sxs-lookup"><span data-stu-id="35a09-111">The page can show a maximum of 1000 lines.</span></span> <span data-ttu-id="35a09-112">By default, the **Date Filter** field therefore contains a filter that limits the lines to entries with posting dates from the beginning of the accounting period to the work date.</span><span class="sxs-lookup"><span data-stu-id="35a09-112">By default, the **Date Filter** field therefore contains a filter that limits the lines to entries with posting dates from the beginning of the accounting period to the work date.</span></span>

## <a name="to-connect-found-documents-to-existing-incoming-document-records"></a><span data-ttu-id="35a09-113">To connect found documents to existing incoming document records</span><span class="sxs-lookup"><span data-stu-id="35a09-113">To connect found documents to existing incoming document records</span></span>
1. <span data-ttu-id="35a09-114">On the **Posted Documents without Incoming Document** page, select the line for a posted document that you want to connect to an existing incoming document record, and then choose the **Select Incoming Document** action.</span><span class="sxs-lookup"><span data-stu-id="35a09-114">On the **Posted Documents without Incoming Document** page, select the line for a posted document that you want to connect to an existing incoming document record, and then choose the **Select Incoming Document** action.</span></span>
2. <span data-ttu-id="35a09-115">On the **Incoming Documents** page, select the incoming document record that you want to connect to posted document found, and then choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="35a09-115">On the **Incoming Documents** page, select the incoming document record that you want to connect to posted document found, and then choose the **OK** button.</span></span>
3. <span data-ttu-id="35a09-116">On the **Posted Documents without Incoming Document** page, the selected incoming document record is now connected to the posted document, as you can see in the **Incoming Document Files** FactBox.</span><span class="sxs-lookup"><span data-stu-id="35a09-116">On the **Posted Documents without Incoming Document** page, the selected incoming document record is now connected to the posted document, as you can see in the **Incoming Document Files** FactBox.</span></span>

<span data-ttu-id="35a09-117">If a relevant incoming document record does not exist on the **Incoming Documents** page, then you can create it.</span><span class="sxs-lookup"><span data-stu-id="35a09-117">If a relevant incoming document record does not exist on the **Incoming Documents** page, then you can create it.</span></span> <span data-ttu-id="35a09-118">For more information, see [Create Incoming Document Records](across-how-create-income-document-records.md).</span><span class="sxs-lookup"><span data-stu-id="35a09-118">For more information, see [Create Incoming Document Records](across-how-create-income-document-records.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="35a09-119">See Also</span><span class="sxs-lookup"><span data-stu-id="35a09-119">See Also</span></span>
[<span data-ttu-id="35a09-120">Process Incoming Documents</span><span class="sxs-lookup"><span data-stu-id="35a09-120">Process Incoming Documents</span></span>](across-process-income-documents.md)  
[<span data-ttu-id="35a09-121">Incoming Documents</span><span class="sxs-lookup"><span data-stu-id="35a09-121">Incoming Documents</span></span>](across-income-documents.md)  
[<span data-ttu-id="35a09-122">Purchasing</span><span class="sxs-lookup"><span data-stu-id="35a09-122">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="35a09-123">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="35a09-123">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
