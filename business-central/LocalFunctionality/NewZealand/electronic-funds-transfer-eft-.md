---
title: Electronic Funds Transfer (EFT)
description: You can pay vendors using the electronic funds transfer (EFT) system in New Zealand.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2019
ms.author: bholtorf
ms.openlocfilehash: d3f3b9a906d89de87cb77e1f0d8b34f805d1f0f8
ms.sourcegitcommit: cfc92eefa8b06fb426482f54e393f0e6e222f712
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 12/03/2019
ms.locfileid: "2881339"
---
# <a name="electronic-funds-transfer-eft"></a><span data-ttu-id="c22be-103">Electronic Funds Transfer (EFT)</span><span class="sxs-lookup"><span data-stu-id="c22be-103">Electronic Funds Transfer (EFT)</span></span>
<span data-ttu-id="c22be-104">You can pay vendors using the electronic funds transfer (EFT) system in New Zealand.</span><span class="sxs-lookup"><span data-stu-id="c22be-104">You can pay vendors using the electronic funds transfer (EFT) system in New Zealand.</span></span>  

## <a name="setting-up-electronic-funds-transfer-in-included365finincludesd365fin_mdmd"></a><span data-ttu-id="c22be-105">Setting up Electronic Funds Transfer in [!INCLUDE[d365fin](../../includes/d365fin_md.md)]</span><span class="sxs-lookup"><span data-stu-id="c22be-105">Setting up Electronic Funds Transfer in [!INCLUDE[d365fin](../../includes/d365fin_md.md)]</span></span>  
[!INCLUDE[d365fin](../../includes/d365fin_md.md)] <span data-ttu-id="c22be-106">can export EFT files that you can then upload to your bank’s website for additional processing.</span><span class="sxs-lookup"><span data-stu-id="c22be-106">can export EFT files that you can then upload to your bank’s website for additional processing.</span></span> <span data-ttu-id="c22be-107">To submit EFT files, you must set up the following information:</span><span class="sxs-lookup"><span data-stu-id="c22be-107">To submit EFT files, you must set up the following information:</span></span>  

* <span data-ttu-id="c22be-108">You must add EFT information to the bank account or bank accounts that you will use to pay vendors electronically.</span><span class="sxs-lookup"><span data-stu-id="c22be-108">You must add EFT information to the bank account or bank accounts that you will use to pay vendors electronically.</span></span> <span data-ttu-id="c22be-109">The EFT-specific fields are in the **Transfer** FastTab on the **Bank Account** page.</span><span class="sxs-lookup"><span data-stu-id="c22be-109">The EFT-specific fields are in the **Transfer** FastTab on the **Bank Account** page.</span></span>  
* <span data-ttu-id="c22be-110">For those vendors that you want to pay electronically, you must select the **EFT Payment** check box and specify the vendor bank account in the **EFT Vendor Bank Account Code** field on the **Vendor** page.</span><span class="sxs-lookup"><span data-stu-id="c22be-110">For those vendors that you want to pay electronically, you must select the **EFT Payment** check box and specify the vendor bank account in the **EFT Vendor Bank Account Code** field on the **Vendor** page.</span></span>  

<span data-ttu-id="c22be-111">When you have set up bank accounts and vendors, you can create EFT file that are based on entries in the payment journal.</span><span class="sxs-lookup"><span data-stu-id="c22be-111">When you have set up bank accounts and vendors, you can create EFT file that are based on entries in the payment journal.</span></span> <span data-ttu-id="c22be-112">When you create an EFT file, an entry is made in the **EFT Register** table.</span><span class="sxs-lookup"><span data-stu-id="c22be-112">When you create an EFT file, an entry is made in the **EFT Register** table.</span></span> <span data-ttu-id="c22be-113">On the EFT Register page you can drill down to see the vendor ledger entries for the EFT file.</span><span class="sxs-lookup"><span data-stu-id="c22be-113">On the EFT Register page you can drill down to see the vendor ledger entries for the EFT file.</span></span> <span data-ttu-id="c22be-114">On the Payment Journal page,you can also import existing EFT register entries to the payment journal by using the **Transfer EFT Register** batch job.</span><span class="sxs-lookup"><span data-stu-id="c22be-114">On the Payment Journal page,you can also import existing EFT register entries to the payment journal by using the **Transfer EFT Register** batch job.</span></span>

## <a name="see-also"></a><span data-ttu-id="c22be-115">See Also</span><span class="sxs-lookup"><span data-stu-id="c22be-115">See Also</span></span>  
[<span data-ttu-id="c22be-116">Export Payments to a Bank File</span><span class="sxs-lookup"><span data-stu-id="c22be-116">Export Payments to a Bank File</span></span>](../../payables-how-export-payments-bank-file.md)  
[<span data-ttu-id="c22be-117">New Zealand Local Functionality</span><span class="sxs-lookup"><span data-stu-id="c22be-117">New Zealand Local Functionality</span></span>](new-zealand-local-functionality.md)
