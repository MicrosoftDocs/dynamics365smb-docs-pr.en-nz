---
title: Electronic Funds Transfer (EFT)
description: You can pay vendors using the electronic funds transfer (EFT) system in New Zealand.
services: project-madeira
documentationcenter: 
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 10/01/2018
ms.author: bholtorf
ms.translationtype: HT
ms.sourcegitcommit: 78cb55d0c53db5b0a8252ffae6316a537be25459
ms.openlocfilehash: 9d3c713a649cd0a66a18c892123a90b85cf2aefd
ms.contentlocale: en-nz
ms.lasthandoff: 10/15/2018

---
# <a name="electronic-funds-transfer-eft"></a><span data-ttu-id="053f1-103">Electronic Funds Transfer (EFT)</span><span class="sxs-lookup"><span data-stu-id="053f1-103">Electronic Funds Transfer (EFT)</span></span>
<span data-ttu-id="053f1-104">You can pay vendors using the electronic funds transfer (EFT) system in New Zealand.</span><span class="sxs-lookup"><span data-stu-id="053f1-104">You can pay vendors using the electronic funds transfer (EFT) system in New Zealand.</span></span>  

## <a name="setting-up-electronic-funds-transfer-in-included365finincludesd365finmdmd"></a><span data-ttu-id="053f1-105">Setting up Electronic Funds Transfer in [!INCLUDE[d365fin](../../includes/d365fin_md.md)]</span><span class="sxs-lookup"><span data-stu-id="053f1-105">Setting up Electronic Funds Transfer in [!INCLUDE[d365fin](../../includes/d365fin_md.md)]</span></span>  
[!INCLUDE[d365fin](../../includes/d365fin_md.md)] <span data-ttu-id="053f1-106">can export EFT files that you can then upload to your bank’s website for additional processing.</span><span class="sxs-lookup"><span data-stu-id="053f1-106">can export EFT files that you can then upload to your bank’s website for additional processing.</span></span> <span data-ttu-id="053f1-107">To submit EFT files, you must set up the following information:</span><span class="sxs-lookup"><span data-stu-id="053f1-107">To submit EFT files, you must set up the following information:</span></span>  

* <span data-ttu-id="053f1-108">You must add EFT information to the bank account or bank accounts that you will use to pay vendors electronically.</span><span class="sxs-lookup"><span data-stu-id="053f1-108">You must add EFT information to the bank account or bank accounts that you will use to pay vendors electronically.</span></span> <span data-ttu-id="053f1-109">The EFT-specific fields are in the **Transfer** FastTab in the **Bank Account** window.</span><span class="sxs-lookup"><span data-stu-id="053f1-109">The EFT-specific fields are in the **Transfer** FastTab in the **Bank Account** window.</span></span>  
* <span data-ttu-id="053f1-110">For those vendors that you want to pay electronically, you must select the **EFT Payment** check box and specify the vendor bank account in the **EFT Vendor Bank Account Code** field in the **Vendor** window.</span><span class="sxs-lookup"><span data-stu-id="053f1-110">For those vendors that you want to pay electronically, you must select the **EFT Payment** check box and specify the vendor bank account in the **EFT Vendor Bank Account Code** field in the **Vendor** window.</span></span>  

<span data-ttu-id="053f1-111">When you have set up bank accounts and vendors, you can create EFT file that are based on entries in the payment journal.</span><span class="sxs-lookup"><span data-stu-id="053f1-111">When you have set up bank accounts and vendors, you can create EFT file that are based on entries in the payment journal.</span></span> <span data-ttu-id="053f1-112">When you create an EFT file, an entry is made in the **EFT Register** table.</span><span class="sxs-lookup"><span data-stu-id="053f1-112">When you create an EFT file, an entry is made in the **EFT Register** table.</span></span> <span data-ttu-id="053f1-113">On the EFT Register page you can drill down to see the vendor ledger entries for the EFT file.</span><span class="sxs-lookup"><span data-stu-id="053f1-113">On the EFT Register page you can drill down to see the vendor ledger entries for the EFT file.</span></span> <span data-ttu-id="053f1-114">On the Payment Journal page,you can also import existing EFT register entries to the payment journal by using the **Transfer EFT Register** batch job.</span><span class="sxs-lookup"><span data-stu-id="053f1-114">On the Payment Journal page,you can also import existing EFT register entries to the payment journal by using the **Transfer EFT Register** batch job.</span></span>

## <a name="see-also"></a><span data-ttu-id="053f1-115">See Also</span><span class="sxs-lookup"><span data-stu-id="053f1-115">See Also</span></span>  
[<span data-ttu-id="053f1-116">Export Payments to a Bank File</span><span class="sxs-lookup"><span data-stu-id="053f1-116">Export Payments to a Bank File</span></span>](../../payables-how-export-payments-bank-file.md)  
[<span data-ttu-id="053f1-117">New Zealand Local Functionality</span><span class="sxs-lookup"><span data-stu-id="053f1-117">New Zealand Local Functionality</span></span>](new-zealand-local-functionality.md)

