---
title: QuickBooks Online Migration Extension | Microsoft Docs
description: Describes how to use the extension to migrate customers, vendors, items, and accounts from QuickBooks Online to Business Central.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: extension, migrate, data, QuickBooks, import
ms.date: 04/01/2021
ms.author: bholtorf
ms.openlocfilehash: 6481eeb46116d02240c6f6a0201cb633f572822a
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 03/31/2021
ms.locfileid: "5785026"
---
# <a name="the-quickbooks-online-data-migration-extension"></a><span data-ttu-id="64abd-103">The QuickBooks Online Data Migration Extension</span><span class="sxs-lookup"><span data-stu-id="64abd-103">The QuickBooks Online Data Migration Extension</span></span>

<span data-ttu-id="64abd-104">This extension is included in the **Data Migration** assisted setup guide to help you migrate important business data from QuickBooks Online to [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="64abd-104">This extension is included in the **Data Migration** assisted setup guide to help you migrate important business data from QuickBooks Online to [!INCLUDE[prod_short](includes/prod_short.md)].</span></span> <span data-ttu-id="64abd-105">For example, this is useful when your business is growing, and you've decided to upgrade your business management app by starting to use [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="64abd-105">For example, this is useful when your business is growing, and you've decided to upgrade your business management app by starting to use [!INCLUDE[prod_short](includes/prod_short.md)].</span></span>

## <a name="what-data-can-i-import-from-quickbooks-online"></a><span data-ttu-id="64abd-106">What data can I import from QuickBooks Online?</span><span class="sxs-lookup"><span data-stu-id="64abd-106">What data can I import from QuickBooks Online?</span></span>

<span data-ttu-id="64abd-107">You can import the following data from QuickBooks Online to [!INCLUDE[prod_short](includes/prod_short.md)]:</span><span class="sxs-lookup"><span data-stu-id="64abd-107">You can import the following data from QuickBooks Online to [!INCLUDE[prod_short](includes/prod_short.md)]:</span></span>  

* <span data-ttu-id="64abd-108">Customers</span><span class="sxs-lookup"><span data-stu-id="64abd-108">Customers</span></span>
* <span data-ttu-id="64abd-109">Vendors</span><span class="sxs-lookup"><span data-stu-id="64abd-109">Vendors</span></span>
* <span data-ttu-id="64abd-110">Items</span><span class="sxs-lookup"><span data-stu-id="64abd-110">Items</span></span>
* <span data-ttu-id="64abd-111">Chart of accounts</span><span class="sxs-lookup"><span data-stu-id="64abd-111">Chart of accounts</span></span>
* <span data-ttu-id="64abd-112">Beginning balance transaction in the general ledger</span><span class="sxs-lookup"><span data-stu-id="64abd-112">Beginning balance transaction in the general ledger</span></span>
* <span data-ttu-id="64abd-113">On-hand quantities for inventory items</span><span class="sxs-lookup"><span data-stu-id="64abd-113">On-hand quantities for inventory items</span></span>
* <span data-ttu-id="64abd-114">Open documents for customers and vendors, such as invoices, credit memos, and payments</span><span class="sxs-lookup"><span data-stu-id="64abd-114">Open documents for customers and vendors, such as invoices, credit memos, and payments</span></span>

<span data-ttu-id="64abd-115">We migrate only full amounts on sales and purchase documents.</span><span class="sxs-lookup"><span data-stu-id="64abd-115">We migrate only full amounts on sales and purchase documents.</span></span> <span data-ttu-id="64abd-116">We do not update partially paid amounts.</span><span class="sxs-lookup"><span data-stu-id="64abd-116">We do not update partially paid amounts.</span></span> <span data-ttu-id="64abd-117">For example, if a customer has paid 300 of a total of 500 dollars on a sales invoice, we migrate the full 500.</span><span class="sxs-lookup"><span data-stu-id="64abd-117">For example, if a customer has paid 300 of a total of 500 dollars on a sales invoice, we migrate the full 500.</span></span> <span data-ttu-id="64abd-118">If you have received partial payments, you must update these manually, either before or after you migrate data.</span><span class="sxs-lookup"><span data-stu-id="64abd-118">If you have received partial payments, you must update these manually, either before or after you migrate data.</span></span> <span data-ttu-id="64abd-119">We recommend that you apply outstanding transactions before you migrate, just to make things easier afterward.</span><span class="sxs-lookup"><span data-stu-id="64abd-119">We recommend that you apply outstanding transactions before you migrate, just to make things easier afterward.</span></span>

> [!NOTE]  
> <span data-ttu-id="64abd-120">We do not migrate purchase orders or sales orders.</span><span class="sxs-lookup"><span data-stu-id="64abd-120">We do not migrate purchase orders or sales orders.</span></span>

## <a name="before-you-start"></a><span data-ttu-id="64abd-121">Before you start</span><span class="sxs-lookup"><span data-stu-id="64abd-121">Before you start</span></span>

<span data-ttu-id="64abd-122">An important part of the migration process is to specify the accounts to migrate transactions to.</span><span class="sxs-lookup"><span data-stu-id="64abd-122">An important part of the migration process is to specify the accounts to migrate transactions to.</span></span> <span data-ttu-id="64abd-123">It's a good idea to plan this mapping before you migrate data.</span><span class="sxs-lookup"><span data-stu-id="64abd-123">It's a good idea to plan this mapping before you migrate data.</span></span> <span data-ttu-id="64abd-124">For example, the accounts where you post transactions for:</span><span class="sxs-lookup"><span data-stu-id="64abd-124">For example, the accounts where you post transactions for:</span></span>  

* <span data-ttu-id="64abd-125">The sale of items or services to customers.</span><span class="sxs-lookup"><span data-stu-id="64abd-125">The sale of items or services to customers.</span></span>
* <span data-ttu-id="64abd-126">The purchase of items or services from vendors.</span><span class="sxs-lookup"><span data-stu-id="64abd-126">The purchase of items or services from vendors.</span></span>  
* <span data-ttu-id="64abd-127">Adjustments in the general ledger.</span><span class="sxs-lookup"><span data-stu-id="64abd-127">Adjustments in the general ledger.</span></span>  

[!INCLUDE[prod_short](includes/prod_short.md)] <span data-ttu-id="64abd-128">requires that general ledger accounts have account numbers assigned to them.</span><span class="sxs-lookup"><span data-stu-id="64abd-128">requires that general ledger accounts have account numbers assigned to them.</span></span> <span data-ttu-id="64abd-129">Make sure that account numbers are assigned to your accounts in QuickBooks Online.</span><span class="sxs-lookup"><span data-stu-id="64abd-129">Make sure that account numbers are assigned to your accounts in QuickBooks Online.</span></span>

<span data-ttu-id="64abd-130">If transactions in QuickBooks Online have tax amounts, you must set up a tax account for your tax jurisdictions in [!INCLUDE[prod_short](includes/prod_short.md)] before you can post transactions.</span><span class="sxs-lookup"><span data-stu-id="64abd-130">If transactions in QuickBooks Online have tax amounts, you must set up a tax account for your tax jurisdictions in [!INCLUDE[prod_short](includes/prod_short.md)] before you can post transactions.</span></span>

## <a name="how-do-i-start-using-the-extension"></a><span data-ttu-id="64abd-131">How do I start using the extension?</span><span class="sxs-lookup"><span data-stu-id="64abd-131">How do I start using the extension?</span></span>

<span data-ttu-id="64abd-132">Getting started is easy.</span><span class="sxs-lookup"><span data-stu-id="64abd-132">Getting started is easy.</span></span> <span data-ttu-id="64abd-133">All you need to do is run the **Data Migration** assisted setup guide.</span><span class="sxs-lookup"><span data-stu-id="64abd-133">All you need to do is run the **Data Migration** assisted setup guide.</span></span> <span data-ttu-id="64abd-134">Here's how:</span><span class="sxs-lookup"><span data-stu-id="64abd-134">Here's how:</span></span>

1. <span data-ttu-id="64abd-135">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Assisted Setup**, and then choose **Migrate business data**.</span><span class="sxs-lookup"><span data-stu-id="64abd-135">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Assisted Setup**, and then choose **Migrate business data**.</span></span>
2. <span data-ttu-id="64abd-136">Follow the instructions on each step in the assisted setup guide.</span><span class="sxs-lookup"><span data-stu-id="64abd-136">Follow the instructions on each step in the assisted setup guide.</span></span>

## <a name="what-do-i-do-after-i-migrate-data"></a><span data-ttu-id="64abd-137">What do I do after I migrate data?</span><span class="sxs-lookup"><span data-stu-id="64abd-137">What do I do after I migrate data?</span></span>

<span data-ttu-id="64abd-138">After you migrate data, transactions have the status **Unposted**, so you can review them and make adjustments.</span><span class="sxs-lookup"><span data-stu-id="64abd-138">After you migrate data, transactions have the status **Unposted**, so you can review them and make adjustments.</span></span> <span data-ttu-id="64abd-139">To review the transactions, go to the page where you would normally find them.</span><span class="sxs-lookup"><span data-stu-id="64abd-139">To review the transactions, go to the page where you would normally find them.</span></span> <span data-ttu-id="64abd-140">For example, to review unposted sales invoices, go to the **Sales Invoices** page.</span><span class="sxs-lookup"><span data-stu-id="64abd-140">For example, to review unposted sales invoices, go to the **Sales Invoices** page.</span></span> <span data-ttu-id="64abd-141">To review payment journals, go to the **Payment Journals** page.</span><span class="sxs-lookup"><span data-stu-id="64abd-141">To review payment journals, go to the **Payment Journals** page.</span></span>  

<span data-ttu-id="64abd-142">There are a few things in particular that you should do:</span><span class="sxs-lookup"><span data-stu-id="64abd-142">There are a few things in particular that you should do:</span></span>

* <span data-ttu-id="64abd-143">If the transactions in QuickBooks Online had markup or discount amounts, you must manually add the amounts to the related transactions in [!INCLUDE[prod_short](includes/prod_short.md)] before you post them.</span><span class="sxs-lookup"><span data-stu-id="64abd-143">If the transactions in QuickBooks Online had markup or discount amounts, you must manually add the amounts to the related transactions in [!INCLUDE[prod_short](includes/prod_short.md)] before you post them.</span></span>
* <span data-ttu-id="64abd-144">If you are using value added tax (VAT), you may need to add a business posting group and a product posting group to the posting setup so that you can post VAT amounts.</span><span class="sxs-lookup"><span data-stu-id="64abd-144">If you are using value added tax (VAT), you may need to add a business posting group and a product posting group to the posting setup so that you can post VAT amounts.</span></span>
* <span data-ttu-id="64abd-145">Verify the beginning balances for accounts in the general ledger.</span><span class="sxs-lookup"><span data-stu-id="64abd-145">Verify the beginning balances for accounts in the general ledger.</span></span> <span data-ttu-id="64abd-146">QuickBooks Online does not store the current balance for all accounts, so you might need to correct beginning balances.</span><span class="sxs-lookup"><span data-stu-id="64abd-146">QuickBooks Online does not store the current balance for all accounts, so you might need to correct beginning balances.</span></span>

## <a name="see-also"></a><span data-ttu-id="64abd-147">See Also</span><span class="sxs-lookup"><span data-stu-id="64abd-147">See Also</span></span>

[<span data-ttu-id="64abd-148">Importing Business Data from Other Finance Systems</span><span class="sxs-lookup"><span data-stu-id="64abd-148">Importing Business Data from Other Finance Systems</span></span>](across-import-data-configuration-packages.md)  
<span data-ttu-id="64abd-149">[Customizing [!INCLUDE[prod_short](includes/prod_short.md)] Using Extensions](ui-extensions.md)</span><span class="sxs-lookup"><span data-stu-id="64abd-149">[Customizing [!INCLUDE[prod_short](includes/prod_short.md)] Using Extensions](ui-extensions.md)</span></span>  


[!INCLUDE[footer-include](includes/footer-banner.md)]