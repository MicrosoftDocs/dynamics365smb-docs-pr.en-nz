---
title: Using the QuickBooks Migration Extension | Microsoft Docs
description: Describes how to use the extension to migrate customers, vendors, items, and accounts from QuickBooks Online to Business Central.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: extension, migrate, data, QuickBooks, import
ms.date: 10/01/2019
ms.author: bholtorf
ms.openlocfilehash: bbfbb187ff533a2c786d0a5b4aa26a20518f760b
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 10/01/2019
ms.locfileid: "2315436"
---
# <a name="the-quickbooks-online-data-migration-extension"></a><span data-ttu-id="1ad3c-103">The QuickBooks Online Data Migration Extension</span><span class="sxs-lookup"><span data-stu-id="1ad3c-103">The QuickBooks Online Data Migration Extension</span></span>
<span data-ttu-id="1ad3c-104">This extension is included in the **Data Migration** assisted setup guide to help you migrate important business data from QuickBooks Online to [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="1ad3c-104">This extension is included in the **Data Migration** assisted setup guide to help you migrate important business data from QuickBooks Online to [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="1ad3c-105">For example, this is useful when your business is growing, and you've decided to upgrade your business management app by starting to use [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="1ad3c-105">For example, this is useful when your business is growing, and you've decided to upgrade your business management app by starting to use [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>

## <a name="what-data-can-i-import-from-quickbooks-online"></a><span data-ttu-id="1ad3c-106">What data can I import from QuickBooks Online?</span><span class="sxs-lookup"><span data-stu-id="1ad3c-106">What data can I import from QuickBooks Online?</span></span>
<span data-ttu-id="1ad3c-107">You can import the following data from QuickBooks Online to [!INCLUDE[d365fin](includes/d365fin_md.md)]:</span><span class="sxs-lookup"><span data-stu-id="1ad3c-107">You can import the following data from QuickBooks Online to [!INCLUDE[d365fin](includes/d365fin_md.md)]:</span></span>  

* <span data-ttu-id="1ad3c-108">Customers</span><span class="sxs-lookup"><span data-stu-id="1ad3c-108">Customers</span></span>
* <span data-ttu-id="1ad3c-109">Vendors</span><span class="sxs-lookup"><span data-stu-id="1ad3c-109">Vendors</span></span>
* <span data-ttu-id="1ad3c-110">Items</span><span class="sxs-lookup"><span data-stu-id="1ad3c-110">Items</span></span>
* <span data-ttu-id="1ad3c-111">Chart of accounts</span><span class="sxs-lookup"><span data-stu-id="1ad3c-111">Chart of accounts</span></span>
* <span data-ttu-id="1ad3c-112">Beginning balance transaction in the general ledger</span><span class="sxs-lookup"><span data-stu-id="1ad3c-112">Beginning balance transaction in the general ledger</span></span>
* <span data-ttu-id="1ad3c-113">On-hand quantities for inventory items</span><span class="sxs-lookup"><span data-stu-id="1ad3c-113">On-hand quantities for inventory items</span></span>
* <span data-ttu-id="1ad3c-114">Open documents for customers and vendors, such as invoices, credit memos, and payments</span><span class="sxs-lookup"><span data-stu-id="1ad3c-114">Open documents for customers and vendors, such as invoices, credit memos, and payments</span></span>

<span data-ttu-id="1ad3c-115">We migrate only full amounts on sales and purchase documents.</span><span class="sxs-lookup"><span data-stu-id="1ad3c-115">We migrate only full amounts on sales and purchase documents.</span></span> <span data-ttu-id="1ad3c-116">We do not update partially paid amounts.</span><span class="sxs-lookup"><span data-stu-id="1ad3c-116">We do not update partially paid amounts.</span></span> <span data-ttu-id="1ad3c-117">For example, if a customer has paid 300 of a total of 500 dollars on a sales invoice, we migrate the full 500.</span><span class="sxs-lookup"><span data-stu-id="1ad3c-117">For example, if a customer has paid 300 of a total of 500 dollars on a sales invoice, we migrate the full 500.</span></span> <span data-ttu-id="1ad3c-118">If you have received partial payments, you must update these manually, either before or after you migrate data.</span><span class="sxs-lookup"><span data-stu-id="1ad3c-118">If you have received partial payments, you must update these manually, either before or after you migrate data.</span></span> <span data-ttu-id="1ad3c-119">We recommend that you apply outstanding transactions before you migrate, just to make things easier afterward.</span><span class="sxs-lookup"><span data-stu-id="1ad3c-119">We recommend that you apply outstanding transactions before you migrate, just to make things easier afterward.</span></span>

> [!NOTE]  
>   <span data-ttu-id="1ad3c-120">We do not migrate purchase orders or sales orders.</span><span class="sxs-lookup"><span data-stu-id="1ad3c-120">We do not migrate purchase orders or sales orders.</span></span>

## <a name="before-you-start"></a><span data-ttu-id="1ad3c-121">Before you start</span><span class="sxs-lookup"><span data-stu-id="1ad3c-121">Before you start</span></span>
<span data-ttu-id="1ad3c-122">An important part of the migration process is to specify the accounts to migrate transactions to.</span><span class="sxs-lookup"><span data-stu-id="1ad3c-122">An important part of the migration process is to specify the accounts to migrate transactions to.</span></span> <span data-ttu-id="1ad3c-123">It's a good idea to plan this mapping before you migrate data.</span><span class="sxs-lookup"><span data-stu-id="1ad3c-123">It's a good idea to plan this mapping before you migrate data.</span></span> <span data-ttu-id="1ad3c-124">For example, the accounts where you post transactions for:</span><span class="sxs-lookup"><span data-stu-id="1ad3c-124">For example, the accounts where you post transactions for:</span></span>  

* <span data-ttu-id="1ad3c-125">The sale of items or services to customers.</span><span class="sxs-lookup"><span data-stu-id="1ad3c-125">The sale of items or services to customers.</span></span>
* <span data-ttu-id="1ad3c-126">The purchase of items or services from vendors.</span><span class="sxs-lookup"><span data-stu-id="1ad3c-126">The purchase of items or services from vendors.</span></span>  
* <span data-ttu-id="1ad3c-127">Adjustments in the general ledger.</span><span class="sxs-lookup"><span data-stu-id="1ad3c-127">Adjustments in the general ledger.</span></span>  

[!INCLUDE[d365fin](includes/d365fin_md.md)] <span data-ttu-id="1ad3c-128">requires that general ledger accounts have account numbers assigned to them.</span><span class="sxs-lookup"><span data-stu-id="1ad3c-128">requires that general ledger accounts have account numbers assigned to them.</span></span> <span data-ttu-id="1ad3c-129">Make sure that account numbers are assigned to your accounts in QuickBooks Online.</span><span class="sxs-lookup"><span data-stu-id="1ad3c-129">Make sure that account numbers are assigned to your accounts in QuickBooks Online.</span></span>

<span data-ttu-id="1ad3c-130">If transactions in QuickBooks Online have tax amounts, you must set up a tax account for your tax jurisdictions in [!INCLUDE[d365fin](includes/d365fin_md.md)] before you can post transactions.</span><span class="sxs-lookup"><span data-stu-id="1ad3c-130">If transactions in QuickBooks Online have tax amounts, you must set up a tax account for your tax jurisdictions in [!INCLUDE[d365fin](includes/d365fin_md.md)] before you can post transactions.</span></span>

## <a name="how-do-i-start-using-the-extension"></a><span data-ttu-id="1ad3c-131">How do I start using the extension?</span><span class="sxs-lookup"><span data-stu-id="1ad3c-131">How do I start using the extension?</span></span>
<span data-ttu-id="1ad3c-132">Getting started is easy.</span><span class="sxs-lookup"><span data-stu-id="1ad3c-132">Getting started is easy.</span></span> <span data-ttu-id="1ad3c-133">All you need to do is run the **Data Migration** assisted setup guide.</span><span class="sxs-lookup"><span data-stu-id="1ad3c-133">All you need to do is run the **Data Migration** assisted setup guide.</span></span> <span data-ttu-id="1ad3c-134">Here's how:</span><span class="sxs-lookup"><span data-stu-id="1ad3c-134">Here's how:</span></span>

1. <span data-ttu-id="1ad3c-135">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Assisted Setup**, and then choose **Migrate business data**.</span><span class="sxs-lookup"><span data-stu-id="1ad3c-135">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Assisted Setup**, and then choose **Migrate business data**.</span></span>
2. <span data-ttu-id="1ad3c-136">Follow the instructions on each step in the assisted setup guide.</span><span class="sxs-lookup"><span data-stu-id="1ad3c-136">Follow the instructions on each step in the assisted setup guide.</span></span>

## <a name="what-do-i-do-after-i-migrate-data"></a><span data-ttu-id="1ad3c-137">What do I do after I migrate data?</span><span class="sxs-lookup"><span data-stu-id="1ad3c-137">What do I do after I migrate data?</span></span>
<span data-ttu-id="1ad3c-138">After you migrate data, transactions have the status **Unposted**, so you can review them and make adjustments.</span><span class="sxs-lookup"><span data-stu-id="1ad3c-138">After you migrate data, transactions have the status **Unposted**, so you can review them and make adjustments.</span></span> <span data-ttu-id="1ad3c-139">To review the transactions, go to the page where you would normally find them.</span><span class="sxs-lookup"><span data-stu-id="1ad3c-139">To review the transactions, go to the page where you would normally find them.</span></span> <span data-ttu-id="1ad3c-140">For example, to review unposted sales invoices, go to the **Sales Invoices** page.</span><span class="sxs-lookup"><span data-stu-id="1ad3c-140">For example, to review unposted sales invoices, go to the **Sales Invoices** page.</span></span> <span data-ttu-id="1ad3c-141">To review payment journals, go to the **Payment Journals** page.</span><span class="sxs-lookup"><span data-stu-id="1ad3c-141">To review payment journals, go to the **Payment Journals** page.</span></span>   

<span data-ttu-id="1ad3c-142">There are a few things in particular that you should do:</span><span class="sxs-lookup"><span data-stu-id="1ad3c-142">There are a few things in particular that you should do:</span></span>

* <span data-ttu-id="1ad3c-143">If the transactions in QuickBooks Online had markup or discount amounts, you must manually add the amounts to the related transactions in [!INCLUDE[d365fin](includes/d365fin_md.md)] before you post them.</span><span class="sxs-lookup"><span data-stu-id="1ad3c-143">If the transactions in QuickBooks Online had markup or discount amounts, you must manually add the amounts to the related transactions in [!INCLUDE[d365fin](includes/d365fin_md.md)] before you post them.</span></span>
* <span data-ttu-id="1ad3c-144">If you are using value added tax (VAT), you may need to add a business posting group and a product posting group to the posting setup so that you can post VAT amounts.</span><span class="sxs-lookup"><span data-stu-id="1ad3c-144">If you are using value added tax (VAT), you may need to add a business posting group and a product posting group to the posting setup so that you can post VAT amounts.</span></span>
* <span data-ttu-id="1ad3c-145">Verify the beginning balances for accounts in the general ledger.</span><span class="sxs-lookup"><span data-stu-id="1ad3c-145">Verify the beginning balances for accounts in the general ledger.</span></span> <span data-ttu-id="1ad3c-146">QuickBooks Online does not store the current balance for all accounts, so you might need to correct beginning balances.</span><span class="sxs-lookup"><span data-stu-id="1ad3c-146">QuickBooks Online does not store the current balance for all accounts, so you might need to correct beginning balances.</span></span>

## <a name="see-also"></a><span data-ttu-id="1ad3c-147">See Also</span><span class="sxs-lookup"><span data-stu-id="1ad3c-147">See Also</span></span>
[<span data-ttu-id="1ad3c-148">Importing Business Data from Other Finance Systems</span><span class="sxs-lookup"><span data-stu-id="1ad3c-148">Importing Business Data from Other Finance Systems</span></span>](across-import-data-configuration-packages.md)  
<span data-ttu-id="1ad3c-149">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions](ui-extensions.md)</span><span class="sxs-lookup"><span data-stu-id="1ad3c-149">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions](ui-extensions.md)</span></span>  
