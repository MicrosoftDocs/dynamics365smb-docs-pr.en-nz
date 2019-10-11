---
title: Manage, delete, or compress documents | Microsoft Docs
description: Keep your historical data or delete it.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2019
ms.author: edupont
ms.openlocfilehash: e2ef5daf60bd9b2a3b7200001170c2c5e570b674
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 10/01/2019
ms.locfileid: "2304422"
---
# <a name="manage-documents"></a><span data-ttu-id="f977a-103">Manage Documents</span><span class="sxs-lookup"><span data-stu-id="f977a-103">Manage Documents</span></span>
<span data-ttu-id="f977a-104">A central role, such as the application administrator, must regularly deal with accumulating historic documents by deleting or compressing them.</span><span class="sxs-lookup"><span data-stu-id="f977a-104">A central role, such as the application administrator, must regularly deal with accumulating historic documents by deleting or compressing them.</span></span>  

## <a name="delete-documents"></a><span data-ttu-id="f977a-105">Delete Documents</span><span class="sxs-lookup"><span data-stu-id="f977a-105">Delete Documents</span></span>
<span data-ttu-id="f977a-106">In certain situations, you may need to delete invoiced purchase orders that have not been deleted.</span><span class="sxs-lookup"><span data-stu-id="f977a-106">In certain situations, you may need to delete invoiced purchase orders that have not been deleted.</span></span> [!INCLUDE[d365fin](includes/d365fin_md.md)] <span data-ttu-id="f977a-107">checks that you have fully invoiced the deleted purchase orders.</span><span class="sxs-lookup"><span data-stu-id="f977a-107">checks that you have fully invoiced the deleted purchase orders.</span></span> <span data-ttu-id="f977a-108">You cannot delete orders that you have not fully invoiced and received.</span><span class="sxs-lookup"><span data-stu-id="f977a-108">You cannot delete orders that you have not fully invoiced and received.</span></span>  

<span data-ttu-id="f977a-109">Return orders are usually deleted after they are invoiced.</span><span class="sxs-lookup"><span data-stu-id="f977a-109">Return orders are usually deleted after they are invoiced.</span></span> <span data-ttu-id="f977a-110">When you post an invoice, it is transferred to the **Posted Purchase Credit Memo** page.</span><span class="sxs-lookup"><span data-stu-id="f977a-110">When you post an invoice, it is transferred to the **Posted Purchase Credit Memo** page.</span></span> <span data-ttu-id="f977a-111">If you selected the **Return Shipment on Credit Memo** check box on the **Purchases & Payable Setup** page, then the invoice is transferred to the **Posted Return Shipment** page.</span><span class="sxs-lookup"><span data-stu-id="f977a-111">If you selected the **Return Shipment on Credit Memo** check box on the **Purchases & Payable Setup** page, then the invoice is transferred to the **Posted Return Shipment** page.</span></span> <span data-ttu-id="f977a-112">You can delete the documents using the **Delete Invd Purch. Ret. Orders** batch job.</span><span class="sxs-lookup"><span data-stu-id="f977a-112">You can delete the documents using the **Delete Invd Purch. Ret. Orders** batch job.</span></span> <span data-ttu-id="f977a-113">Before deleting, the batch job checks if the purchase return orders are fully shipped and invoiced.</span><span class="sxs-lookup"><span data-stu-id="f977a-113">Before deleting, the batch job checks if the purchase return orders are fully shipped and invoiced.</span></span>  

<span data-ttu-id="f977a-114">Blanket purchase orders are not deleted after you have processed and invoiced all the related purchase orders.</span><span class="sxs-lookup"><span data-stu-id="f977a-114">Blanket purchase orders are not deleted after you have processed and invoiced all the related purchase orders.</span></span> <span data-ttu-id="f977a-115">You can delete blanket orders with the **Delete Invoiced Blanket Purchase Orders** batch job.</span><span class="sxs-lookup"><span data-stu-id="f977a-115">You can delete blanket orders with the **Delete Invoiced Blanket Purchase Orders** batch job.</span></span>  

<span data-ttu-id="f977a-116">Invoiced service orders are usually deleted automatically after having been fully invoiced.</span><span class="sxs-lookup"><span data-stu-id="f977a-116">Invoiced service orders are usually deleted automatically after having been fully invoiced.</span></span> <span data-ttu-id="f977a-117">When an invoice is posted, a corresponding entry is created on the **Posted Service Invoices** page.</span><span class="sxs-lookup"><span data-stu-id="f977a-117">When an invoice is posted, a corresponding entry is created on the **Posted Service Invoices** page.</span></span> <span data-ttu-id="f977a-118">The posted document can be viewed on the **Posted Service Invoice** page.</span><span class="sxs-lookup"><span data-stu-id="f977a-118">The posted document can be viewed on the **Posted Service Invoice** page.</span></span>  

<span data-ttu-id="f977a-119">Service orders are not deleted automatically, however, if the total quantity on the order has been posted not from the service order itself, but from the **Service Invoice** page.</span><span class="sxs-lookup"><span data-stu-id="f977a-119">Service orders are not deleted automatically, however, if the total quantity on the order has been posted not from the service order itself, but from the **Service Invoice** page.</span></span> <span data-ttu-id="f977a-120">Then you may need to delete invoiced orders that were not deleted.</span><span class="sxs-lookup"><span data-stu-id="f977a-120">Then you may need to delete invoiced orders that were not deleted.</span></span> <span data-ttu-id="f977a-121">You can do this by running the **Delete Invoiced Service Orders** batch job.</span><span class="sxs-lookup"><span data-stu-id="f977a-121">You can do this by running the **Delete Invoiced Service Orders** batch job.</span></span>  

## <a name="see-also"></a><span data-ttu-id="f977a-122">See Also</span><span class="sxs-lookup"><span data-stu-id="f977a-122">See Also</span></span>  
[<span data-ttu-id="f977a-123">Administration</span><span class="sxs-lookup"><span data-stu-id="f977a-123">Administration</span></span>](admin-setup-and-administration.md)  
