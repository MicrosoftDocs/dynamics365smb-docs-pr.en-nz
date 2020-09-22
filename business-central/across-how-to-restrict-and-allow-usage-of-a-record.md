---
title: How to Restrict and Allow Usage of a Record | Microsoft Docs
description: If you want to restrict a record from being used in certain activities, for example, until the record has been approved, you can incorporate two workflow responses in a workflow that controls the usage of the record.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2020
ms.author: edupont
ms.openlocfilehash: 13a6f57bbdabf93bea74ff6a8c874d457e2234ec
ms.sourcegitcommit: a80afd4e5075018716efad76d82a54e158f1392d
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 09/09/2020
ms.locfileid: "3785137"
---
# <a name="restrict-and-allow-usage-of-a-record"></a><span data-ttu-id="0b41c-103">Restrict and Allow Usage of a Record</span><span class="sxs-lookup"><span data-stu-id="0b41c-103">Restrict and Allow Usage of a Record</span></span>
<span data-ttu-id="0b41c-104">If you want to restrict a record from being used in certain activities, for example, until the record has been approved, you can incorporate two workflow responses in a workflow that controls the usage of the record.</span><span class="sxs-lookup"><span data-stu-id="0b41c-104">If you want to restrict a record from being used in certain activities, for example, until the record has been approved, you can incorporate two workflow responses in a workflow that controls the usage of the record.</span></span> <span data-ttu-id="0b41c-105">One workflow response will restrict usage of the record as defined by the workflow event and conditions.</span><span class="sxs-lookup"><span data-stu-id="0b41c-105">One workflow response will restrict usage of the record as defined by the workflow event and conditions.</span></span> <span data-ttu-id="0b41c-106">Another workflow response will allow usage of the record as defined by the workflow event and conditions.</span><span class="sxs-lookup"><span data-stu-id="0b41c-106">Another workflow response will allow usage of the record as defined by the workflow event and conditions.</span></span> <span data-ttu-id="0b41c-107">Two responses exist in the generic version of [!INCLUDE[d365fin](includes/d365fin_md.md)] for this purpose: **Restrict usage of a record.**</span><span class="sxs-lookup"><span data-stu-id="0b41c-107">Two responses exist in the generic version of [!INCLUDE[d365fin](includes/d365fin_md.md)] for this purpose: **Restrict usage of a record.**</span></span> <span data-ttu-id="0b41c-108">and **Allow usage of a record.**.</span><span class="sxs-lookup"><span data-stu-id="0b41c-108">and **Allow usage of a record.**.</span></span>

> [!NOTE]  
>  <span data-ttu-id="0b41c-109">The generic version of [!INCLUDE[d365fin](includes/d365fin_md.md)] offers support for restricting a record from being posted, from being exported as a payment, and from being printed as a cheque.</span><span class="sxs-lookup"><span data-stu-id="0b41c-109">The generic version of [!INCLUDE[d365fin](includes/d365fin_md.md)] offers support for restricting a record from being posted, from being exported as a payment, and from being printed as a check.</span></span> <span data-ttu-id="0b41c-110">To support other restrictions, a Microsoft partner must customise the application code.</span><span class="sxs-lookup"><span data-stu-id="0b41c-110">To support other restrictions, a Microsoft partner must customize the application code.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="0b41c-111">The workflow functionality to restrict and allow records from being used is not related to the functionality to block item, customer, and vendor records from being posted.</span><span class="sxs-lookup"><span data-stu-id="0b41c-111">The workflow functionality to restrict and allow records from being used is not related to the functionality to block item, customer, and vendor records from being posted.</span></span>

<span data-ttu-id="0b41c-112">The following procedure describes how to restrict purchase orders from being posted until they have been approved.</span><span class="sxs-lookup"><span data-stu-id="0b41c-112">The following procedure describes how to restrict purchase orders from being posted until they have been approved.</span></span> <span data-ttu-id="0b41c-113">The new workflow will be based on the existing Purchase Invoice Approval Workflow workflow template.</span><span class="sxs-lookup"><span data-stu-id="0b41c-113">The new workflow will be based on the existing Purchase Invoice Approval Workflow workflow template.</span></span>  

## <a name="to-create-a-workflow-step-that-restricts-posting-of-unapproved-purchase-orders"></a><span data-ttu-id="0b41c-114">To create a workflow step that restricts posting of unapproved purchase orders</span><span class="sxs-lookup"><span data-stu-id="0b41c-114">To create a workflow step that restricts posting of unapproved purchase orders</span></span>  
1. <span data-ttu-id="0b41c-115">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Workflows**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="0b41c-115">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Workflows**, and then choose the related link.</span></span>  
2. <span data-ttu-id="0b41c-116">On the **Workflows** page, create a new workflow named Purchase Order Approval Workflow.</span><span class="sxs-lookup"><span data-stu-id="0b41c-116">On the **Workflows** page, create a new workflow named Purchase Order Approval Workflow.</span></span> <span data-ttu-id="0b41c-117">For more information, see [Create Workflows](across-how-to-create-workflows.md).</span><span class="sxs-lookup"><span data-stu-id="0b41c-117">For more information, see [Create Workflows](across-how-to-create-workflows.md).</span></span>  
3. <span data-ttu-id="0b41c-118">Choose the **Copy From Workflow Template** action.</span><span class="sxs-lookup"><span data-stu-id="0b41c-118">Choose the **Copy From Workflow Template** action.</span></span>  
4. <span data-ttu-id="0b41c-119">Choose the **Source Workflow Code** field, and then, on the **Workflow Templates** page, choose the Purchase Invoice Approval Workflow workflow template.</span><span class="sxs-lookup"><span data-stu-id="0b41c-119">Choose the **Source Workflow Code** field, and then, on the **Workflow Templates** page, choose the Purchase Invoice Approval Workflow workflow template.</span></span>  

     <span data-ttu-id="0b41c-120">Notice that the first two workflow steps are about restricting and then allowing usage of purchase invoices.</span><span class="sxs-lookup"><span data-stu-id="0b41c-120">Notice that the first two workflow steps are about restricting and then allowing usage of purchase invoices.</span></span> <span data-ttu-id="0b41c-121">Proceed to change the event condition on the first step of the new workflow to specify that it applies to purchase orders.</span><span class="sxs-lookup"><span data-stu-id="0b41c-121">Proceed to change the event condition on the first step of the new workflow to specify that it applies to purchase orders.</span></span>  
5. <span data-ttu-id="0b41c-122">On the **Workflow Steps** FastTab, choose the **Event Conditions** field, and then, for the **Document Type** filter, select **Order**.</span><span class="sxs-lookup"><span data-stu-id="0b41c-122">On the **Workflow Steps** FastTab, choose the **Event Conditions** field, and then, for the **Document Type** filter, select **Order**.</span></span>  
6. <span data-ttu-id="0b41c-123">Proceed to edit, delete, or add other workflow steps to fit a business process that begins by restricting unapproved purchase orders from being posted.</span><span class="sxs-lookup"><span data-stu-id="0b41c-123">Proceed to edit, delete, or add other workflow steps to fit a business process that begins by restricting unapproved purchase orders from being posted.</span></span>  

## <a name="see-also"></a><span data-ttu-id="0b41c-124">See Also</span><span class="sxs-lookup"><span data-stu-id="0b41c-124">See Also</span></span>  
<span data-ttu-id="0b41c-125">[Create Workflows](across-how-to-create-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="0b41c-125">[Create Workflows](across-how-to-create-workflows.md) </span></span>  
[<span data-ttu-id="0b41c-126">Workflow</span><span class="sxs-lookup"><span data-stu-id="0b41c-126">Workflow</span></span>](across-workflow.md)   
