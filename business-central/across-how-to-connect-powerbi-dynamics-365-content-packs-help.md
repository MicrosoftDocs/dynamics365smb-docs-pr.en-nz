---
title: How to Connect Power BI to Business Central | Microsoft Docs
description: Getting insight, business intelligence, and KPIs from your Business Central data is easy with Power BI and the Business Central content packs.
author: SusanneWindfeldPedersen
ms.service: dynamics365-business-central
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: account schedule, analysis, reporting, financial report, business intelligence, KPI
ms.date: 03/16/2018
ms.author: solsen
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 315d4b188cdd834e82676a0c5ef77272ad873eb7
ms.contentlocale: en-nz
ms.lasthandoff: 03/22/2018

---
# <a name="connecting-power-bi-to-business-central-content-packs"></a><span data-ttu-id="db187-103">Connecting Power BI to Business Central Content Packs</span><span class="sxs-lookup"><span data-stu-id="db187-103">Connecting Power BI to Business Central Content Packs</span></span>
<span data-ttu-id="db187-104">Getting insights into your Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] data is easy with Power BI and the Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] content packs.</span><span class="sxs-lookup"><span data-stu-id="db187-104">Getting insights into your Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] data is easy with Power BI and the Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] content packs.</span></span> <span data-ttu-id="db187-105">Power BI retrieves your data then builds an out-of-the-box dashboard and reports based on that data.</span><span class="sxs-lookup"><span data-stu-id="db187-105">Power BI retrieves your data then builds an out-of-the-box dashboard and reports based on that data.</span></span>

> [!NOTE]  
>  <span data-ttu-id="db187-106">You must have a valid account with [!INCLUDE[d365fin](includes/d365fin_md.md)] and with Power BI.</span><span class="sxs-lookup"><span data-stu-id="db187-106">You must have a valid account with [!INCLUDE[d365fin](includes/d365fin_md.md)] and with Power BI.</span></span> <span data-ttu-id="db187-107">Also, you must download [Power BI Desktop](https://powerbi.microsoft.com/en-us/desktop/).</span><span class="sxs-lookup"><span data-stu-id="db187-107">Also, you must download [Power BI Desktop](https://powerbi.microsoft.com/en-us/desktop/).</span></span>  
>  <span data-ttu-id="db187-108">Power BI content packs require permissions to the tables where data is retrieved from.</span><span class="sxs-lookup"><span data-stu-id="db187-108">Power BI content packs require permissions to the tables where data is retrieved from.</span></span> <span data-ttu-id="db187-109">More details on the requirements are described below.</span><span class="sxs-lookup"><span data-stu-id="db187-109">More details on the requirements are described below.</span></span>  

## <a name="how-to-connect"></a><span data-ttu-id="db187-110">How to Connect</span><span class="sxs-lookup"><span data-stu-id="db187-110">How to Connect</span></span>
1. <span data-ttu-id="db187-111">Select **Get Data** at the bottom of the left navigation pane.</span><span class="sxs-lookup"><span data-stu-id="db187-111">Select **Get Data** at the bottom of the left navigation pane.</span></span>  
<span data-ttu-id="db187-112">![Navigating to Get Data](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-get-data.png)</span><span class="sxs-lookup"><span data-stu-id="db187-112">![Navigating to Get Data](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-get-data.png)</span></span>
2. <span data-ttu-id="db187-113">In the **Services** box, select **Get**.</span><span class="sxs-lookup"><span data-stu-id="db187-113">In the **Services** box, select **Get**.</span></span> <span data-ttu-id="db187-114">This will open a window with the **AppSource** and **Apps for Power BI apps**.</span><span class="sxs-lookup"><span data-stu-id="db187-114">This will open a window with the **AppSource** and **Apps for Power BI apps**.</span></span>  
<span data-ttu-id="db187-115">![Choose content packs from online services](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-online-services-get.png)</span><span class="sxs-lookup"><span data-stu-id="db187-115">![Choose content packs from online services](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-online-services-get.png)</span></span>
3. <span data-ttu-id="db187-116">Select **Apps** from the **Apps for Power BI apps** tab, and choose the **Microsoft Dynamics 365 Business Central** content pack that you want to use, and then select **Get it now**.</span><span class="sxs-lookup"><span data-stu-id="db187-116">Select **Apps** from the **Apps for Power BI apps** tab, and choose the **Microsoft Dynamics 365 Business Central** content pack that you want to use, and then select **Get it now**.</span></span>  
<span data-ttu-id="db187-117">![Select Dynamics 365 Business Central and select Get it now](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-dynamics365-for-financials-get-it-now.png)</span><span class="sxs-lookup"><span data-stu-id="db187-117">![Select Dynamics 365 Business Central and select Get it now](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-dynamics365-for-financials-get-it-now.png)</span></span>
4. <span data-ttu-id="db187-118">When prompted, enter the name of *your company* in [!INCLUDE[d365fin_md](includes/d365fin_long_md.md)].</span><span class="sxs-lookup"><span data-stu-id="db187-118">When prompted, enter the name of *your company* in [!INCLUDE[d365fin_md](includes/d365fin_long_md.md)].</span></span> <span data-ttu-id="db187-119">This is not the display name.</span><span class="sxs-lookup"><span data-stu-id="db187-119">This is not the display name.</span></span>  
<span data-ttu-id="db187-120">![Select Dynamics 365 Business Central and select Get it now](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-connect-to-d365-finance-and-operations-crm.png)</span><span class="sxs-lookup"><span data-stu-id="db187-120">![Select Dynamics 365 Business Central and select Get it now](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-connect-to-d365-finance-and-operations-crm.png)</span></span>
5. <span data-ttu-id="db187-121">Once connected, a dashboard, report and dataset will automatically be loaded into your Power BI workspace.</span><span class="sxs-lookup"><span data-stu-id="db187-121">Once connected, a dashboard, report and dataset will automatically be loaded into your Power BI workspace.</span></span> <span data-ttu-id="db187-122">When completed, the tiles will update with data from your account.</span><span class="sxs-lookup"><span data-stu-id="db187-122">When completed, the tiles will update with data from your account.</span></span>
<span data-ttu-id="db187-123">![Select Dynamics 365 Business Central  and select Get it now](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-workspace-dashboard-report-dataset.png)</span><span class="sxs-lookup"><span data-stu-id="db187-123">![Select Dynamics 365 Business Central  and select Get it now](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-workspace-dashboard-report-dataset.png)</span></span>

## <a name="what-now"></a><span data-ttu-id="db187-124">What Now?</span><span class="sxs-lookup"><span data-stu-id="db187-124">What Now?</span></span>

- <span data-ttu-id="db187-125">[Change the tiles](https://docs.microsoft.com/en-us/power-bi/service-dashboard-edit-tile) in the dashboard.</span><span class="sxs-lookup"><span data-stu-id="db187-125">[Change the tiles](https://docs.microsoft.com/en-us/power-bi/service-dashboard-edit-tile) in the dashboard.</span></span>  
- <span data-ttu-id="db187-126">[Select a tile](https://docs.microsoft.com/en-us/power-bi/service-dashboard-tiles) to open the underlying report.</span><span class="sxs-lookup"><span data-stu-id="db187-126">[Select a tile](https://docs.microsoft.com/en-us/power-bi/service-dashboard-tiles) to open the underlying report.</span></span>  
- <span data-ttu-id="db187-127">While your dataset will be scheduled to refreshed daily, you can change the refresh schedule or try refreshing it on demand using **Refresh Now**.</span><span class="sxs-lookup"><span data-stu-id="db187-127">While your dataset will be scheduled to refreshed daily, you can change the refresh schedule or try refreshing it on demand using **Refresh Now**.</span></span>

## <a name="system-requirements"></a><span data-ttu-id="db187-128">System Requirements</span><span class="sxs-lookup"><span data-stu-id="db187-128">System Requirements</span></span>
<span data-ttu-id="db187-129">To import your [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] data into Power BI, you need to have permissions to the web services used to retrieve data.</span><span class="sxs-lookup"><span data-stu-id="db187-129">To import your [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] data into Power BI, you need to have permissions to the web services used to retrieve data.</span></span> <span data-ttu-id="db187-130">The web services required for each content pack include:</span><span class="sxs-lookup"><span data-stu-id="db187-130">The web services required for each content pack include:</span></span>

<span data-ttu-id="db187-131">**Microsoft Dynamics 365 Business Central – CRM**</span><span class="sxs-lookup"><span data-stu-id="db187-131">**Microsoft Dynamics 365 Business Central – CRM**</span></span>
- <span data-ttu-id="db187-132">SalesOpportunities</span><span class="sxs-lookup"><span data-stu-id="db187-132">SalesOpportunities</span></span>
- <span data-ttu-id="db187-133">ExcelTemplateViewCompany</span><span class="sxs-lookup"><span data-stu-id="db187-133">ExcelTemplateViewCompany</span></span>

<span data-ttu-id="db187-134">**Microsoft Dynamics 365 Business Central – Sales**</span><span class="sxs-lookup"><span data-stu-id="db187-134">**Microsoft Dynamics 365 Business Central – Sales**</span></span>
- <span data-ttu-id="db187-135">ItemSalesbyCustomer</span><span class="sxs-lookup"><span data-stu-id="db187-135">ItemSalesbyCustomer</span></span>
- <span data-ttu-id="db187-136">SalesDashboard</span><span class="sxs-lookup"><span data-stu-id="db187-136">SalesDashboard</span></span>
- <span data-ttu-id="db187-137">ExcelTemplateViewCompany</span><span class="sxs-lookup"><span data-stu-id="db187-137">ExcelTemplateViewCompany</span></span>

<span data-ttu-id="db187-138">**Microsoft Dynamics 365 Business Central – Finance**</span><span class="sxs-lookup"><span data-stu-id="db187-138">**Microsoft Dynamics 365 Business Central – Finance**</span></span>
- <span data-ttu-id="db187-139">PowerBIFinance</span><span class="sxs-lookup"><span data-stu-id="db187-139">PowerBIFinance</span></span>
- <span data-ttu-id="db187-140">ExcelTemplateViewCompany</span><span class="sxs-lookup"><span data-stu-id="db187-140">ExcelTemplateViewCompany</span></span>

<span data-ttu-id="db187-141">**Microsoft Dynamics 365 Business Central – Jobs**</span><span class="sxs-lookup"><span data-stu-id="db187-141">**Microsoft Dynamics 365 Business Central – Jobs**</span></span>
- <span data-ttu-id="db187-142">Job List</span><span class="sxs-lookup"><span data-stu-id="db187-142">Job List</span></span>
- <span data-ttu-id="db187-143">Job Planning Lines</span><span class="sxs-lookup"><span data-stu-id="db187-143">Job Planning Lines</span></span>
- <span data-ttu-id="db187-144">Job Task Lines</span><span class="sxs-lookup"><span data-stu-id="db187-144">Job Task Lines</span></span>

<span data-ttu-id="db187-145">**Microsoft Dynamics 365 Business Central – Customers List**</span><span class="sxs-lookup"><span data-stu-id="db187-145">**Microsoft Dynamics 365 Business Central – Customers List**</span></span>
- <span data-ttu-id="db187-146">ItemSalesbyCustomer</span><span class="sxs-lookup"><span data-stu-id="db187-146">ItemSalesbyCustomer</span></span>
- <span data-ttu-id="db187-147">Power_BI_Item_Purchase_List</span><span class="sxs-lookup"><span data-stu-id="db187-147">Power_BI_Item_Purchase_List</span></span>
- <span data-ttu-id="db187-148">Power_BI_Item_Sales_List</span><span class="sxs-lookup"><span data-stu-id="db187-148">Power_BI_Item_Sales_List</span></span>
- <span data-ttu-id="db187-149">SalesDashboard</span><span class="sxs-lookup"><span data-stu-id="db187-149">SalesDashboard</span></span>
- <span data-ttu-id="db187-150">Power_BI_Customer_List</span><span class="sxs-lookup"><span data-stu-id="db187-150">Power_BI_Customer_List</span></span>
- <span data-ttu-id="db187-151">ExcelTemplateViewCompany</span><span class="sxs-lookup"><span data-stu-id="db187-151">ExcelTemplateViewCompany</span></span>

<span data-ttu-id="db187-152">**Microsoft Dynamics 365 Business Central – Items List**</span><span class="sxs-lookup"><span data-stu-id="db187-152">**Microsoft Dynamics 365 Business Central – Items List**</span></span>
- <span data-ttu-id="db187-153">ItemSalesbyCustomer</span><span class="sxs-lookup"><span data-stu-id="db187-153">ItemSalesbyCustomer</span></span>
- <span data-ttu-id="db187-154">Power_BI_Item_Purchase_List</span><span class="sxs-lookup"><span data-stu-id="db187-154">Power_BI_Item_Purchase_List</span></span>
- <span data-ttu-id="db187-155">Power_BI_Item_Sales_List</span><span class="sxs-lookup"><span data-stu-id="db187-155">Power_BI_Item_Sales_List</span></span>
- <span data-ttu-id="db187-156">Items</span><span class="sxs-lookup"><span data-stu-id="db187-156">Items</span></span>
- <span data-ttu-id="db187-157">SalesDashboard</span><span class="sxs-lookup"><span data-stu-id="db187-157">SalesDashboard</span></span>
- <span data-ttu-id="db187-158">ExcelTemplateViewCompany</span><span class="sxs-lookup"><span data-stu-id="db187-158">ExcelTemplateViewCompany</span></span>

<span data-ttu-id="db187-159">**Microsoft Dynamics 365 Business Central – Vendors List**</span><span class="sxs-lookup"><span data-stu-id="db187-159">**Microsoft Dynamics 365 Business Central – Vendors List**</span></span>
- <span data-ttu-id="db187-160">ItemSalesbyCustomer</span><span class="sxs-lookup"><span data-stu-id="db187-160">ItemSalesbyCustomer</span></span>
- <span data-ttu-id="db187-161">Power_BI_Item_Purchase_List</span><span class="sxs-lookup"><span data-stu-id="db187-161">Power_BI_Item_Purchase_List</span></span>
- <span data-ttu-id="db187-162">Power_BI_Item_Sales_List</span><span class="sxs-lookup"><span data-stu-id="db187-162">Power_BI_Item_Sales_List</span></span>
- <span data-ttu-id="db187-163">Items</span><span class="sxs-lookup"><span data-stu-id="db187-163">Items</span></span>
- <span data-ttu-id="db187-164">SalesDashboard</span><span class="sxs-lookup"><span data-stu-id="db187-164">SalesDashboard</span></span>
- <span data-ttu-id="db187-165">Power_BI_Customer_List</span><span class="sxs-lookup"><span data-stu-id="db187-165">Power_BI_Customer_List</span></span>
- <span data-ttu-id="db187-166">ItemSalesbyCustomer</span><span class="sxs-lookup"><span data-stu-id="db187-166">ItemSalesbyCustomer</span></span>
- <span data-ttu-id="db187-167">Power_BI_Vendor_List</span><span class="sxs-lookup"><span data-stu-id="db187-167">Power_BI_Vendor_List</span></span>
- <span data-ttu-id="db187-168">ExcelTemplateViewCompany</span><span class="sxs-lookup"><span data-stu-id="db187-168">ExcelTemplateViewCompany</span></span>

## <a name="web-services"></a><span data-ttu-id="db187-169">Web Services</span><span class="sxs-lookup"><span data-stu-id="db187-169">Web Services</span></span>
<span data-ttu-id="db187-170">An easy way to find the web services is to search for web services in [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)].</span><span class="sxs-lookup"><span data-stu-id="db187-170">An easy way to find the web services is to search for web services in [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)].</span></span> <span data-ttu-id="db187-171">In the list make sure the Publish box is marked for the web services listed above.</span><span class="sxs-lookup"><span data-stu-id="db187-171">In the list make sure the Publish box is marked for the web services listed above.</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="db187-172">Troubleshooting</span><span class="sxs-lookup"><span data-stu-id="db187-172">Troubleshooting</span></span>
<span data-ttu-id="db187-173">The Power BI dashboard relies on the published web services that are listed above, and it will show data from the demonstration company or your own company if you import data from your current finance solution.</span><span class="sxs-lookup"><span data-stu-id="db187-173">The Power BI dashboard relies on the published web services that are listed above, and it will show data from the demonstration company or your own company if you import data from your current finance solution.</span></span> <span data-ttu-id="db187-174">However, if something goes wrong, this section provides a workaround for the most typical issues.</span><span class="sxs-lookup"><span data-stu-id="db187-174">However, if something goes wrong, this section provides a workaround for the most typical issues.</span></span>

### <a name="incorrect-company-name"></a><span data-ttu-id="db187-175">Incorrect Company Name</span><span class="sxs-lookup"><span data-stu-id="db187-175">Incorrect Company Name</span></span>  
<span data-ttu-id="db187-176">A common mistake is to enter the company display name instead of the company name.</span><span class="sxs-lookup"><span data-stu-id="db187-176">A common mistake is to enter the company display name instead of the company name.</span></span> <span data-ttu-id="db187-177">To find the company name search for **Companies**.</span><span class="sxs-lookup"><span data-stu-id="db187-177">To find the company name search for **Companies**.</span></span> <span data-ttu-id="db187-178">Then use the **Name** field when entering your company name.</span><span class="sxs-lookup"><span data-stu-id="db187-178">Then use the **Name** field when entering your company name.</span></span>

### <a name="incorrect-user-name-and-password"></a><span data-ttu-id="db187-179">Incorrect User Name and Password</span><span class="sxs-lookup"><span data-stu-id="db187-179">Incorrect User Name and Password</span></span>  
<span data-ttu-id="db187-180">The user name and password used to connect will be the same as what is used to connect to your Microsoft Office 365 account.</span><span class="sxs-lookup"><span data-stu-id="db187-180">The user name and password used to connect will be the same as what is used to connect to your Microsoft Office 365 account.</span></span>  

<span data-ttu-id="db187-181">The content packs also require that you have a Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] account.</span><span class="sxs-lookup"><span data-stu-id="db187-181">The content packs also require that you have a Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] account.</span></span> <span data-ttu-id="db187-182">Once you enter your credentials, we will auto discover any Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] tenants you have access to.</span><span class="sxs-lookup"><span data-stu-id="db187-182">Once you enter your credentials, we will auto discover any Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] tenants you have access to.</span></span> <span data-ttu-id="db187-183">If you do not have a licensed or trial Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] account, you will receive an error message.</span><span class="sxs-lookup"><span data-stu-id="db187-183">If you do not have a licensed or trial Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] account, you will receive an error message.</span></span>

### <a name="the-key-didnt-match-any-rows-in-the-table"></a><span data-ttu-id="db187-184">The Key Didn't Match Any Rows in the Table</span><span class="sxs-lookup"><span data-stu-id="db187-184">The Key Didn't Match Any Rows in the Table</span></span>
<span data-ttu-id="db187-185">If you enter a non valid company name during the connection process, you may get the error message "The key didn't match any rows in the table".</span><span class="sxs-lookup"><span data-stu-id="db187-185">If you enter a non valid company name during the connection process, you may get the error message "The key didn't match any rows in the table".</span></span> <span data-ttu-id="db187-186">Provide the correct company name and try connecting again.</span><span class="sxs-lookup"><span data-stu-id="db187-186">Provide the correct company name and try connecting again.</span></span>

## <a name="see-also"></a><span data-ttu-id="db187-187">See Also</span><span class="sxs-lookup"><span data-stu-id="db187-187">See Also</span></span>
[<span data-ttu-id="db187-188">Get started with Power BI</span><span class="sxs-lookup"><span data-stu-id="db187-188">Get started with Power BI</span></span>](https://docs.microsoft.com/en-us/power-bi/service-get-started)  
<span data-ttu-id="db187-189">[Power BI - Basic Concepts](https://docs.microsoft.com/en-us/power-bi/service-basic-concepts)
[Business Intelligence](bi.md)</span><span class="sxs-lookup"><span data-stu-id="db187-189">[Power BI - Basic Concepts](https://docs.microsoft.com/en-us/power-bi/service-basic-concepts)
[Business Intelligence](bi.md)</span></span>  
<span data-ttu-id="db187-190">[Welcome to [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)</span><span class="sxs-lookup"><span data-stu-id="db187-190">[Welcome to [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)</span></span>  
[<span data-ttu-id="db187-191">Importing Business Data from Other Finance Systems</span><span class="sxs-lookup"><span data-stu-id="db187-191">Importing Business Data from Other Finance Systems</span></span>](upload-data.md)  
<span data-ttu-id="db187-192">[Setting Up [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)</span><span class="sxs-lookup"><span data-stu-id="db187-192">[Setting Up [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)</span></span>  
[<span data-ttu-id="db187-193">Finance</span><span class="sxs-lookup"><span data-stu-id="db187-193">Finance</span></span>](finance.md)  
<span data-ttu-id="db187-194">[Setup Reporting for [!INCLUDE[d365fin](includes/d365fin_md.md)] in Power BI](across-how-use-financials-data-source-powerbi.md)</span><span class="sxs-lookup"><span data-stu-id="db187-194">[Setup Reporting for [!INCLUDE[d365fin](includes/d365fin_md.md)] in Power BI](across-how-use-financials-data-source-powerbi.md)</span></span>  

