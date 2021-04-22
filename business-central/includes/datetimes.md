---
author: edupont04
ms.service: dynamics365-business-central
ms.topic: include
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 7ead218d289668d893a659f730a4c64e31195f10
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 03/31/2021
ms.locfileid: "5788675"
---
<span data-ttu-id="5af03-101">When you enter datetimes, which are a date and time combined into one field, you must enter a space between the date and the time.</span><span class="sxs-lookup"><span data-stu-id="5af03-101">When you enter datetimes, which are a date and time combined into one field, you must enter a space between the date and the time.</span></span> <span data-ttu-id="5af03-102">The date part can only contain spaces in the form of the official date separator of your region settings.</span><span class="sxs-lookup"><span data-stu-id="5af03-102">The date part can only contain spaces in the form of the official date separator of your region settings.</span></span> <span data-ttu-id="5af03-103">The time can contain spaces around the AM/PM indicator in relevant regional settings.</span><span class="sxs-lookup"><span data-stu-id="5af03-103">The time can contain spaces around the AM/PM indicator in relevant regional settings.</span></span>

<!--It is also possible to enter only a date in a datetime field, but it is not possible to enter only a time.-->

<span data-ttu-id="5af03-104">The following table lists the various ways in which you can enter datetimes and how they're interpreted.</span><span class="sxs-lookup"><span data-stu-id="5af03-104">The following table lists the various ways in which you can enter datetimes and how they're interpreted.</span></span>  

|<span data-ttu-id="5af03-105">Entry</span><span class="sxs-lookup"><span data-stu-id="5af03-105">Entry</span></span>|<span data-ttu-id="5af03-106">Interpretation</span><span class="sxs-lookup"><span data-stu-id="5af03-106">Interpretation</span></span>|
|---------------|------------------------|
|<span data-ttu-id="5af03-107">08-01-2022 05:48:12 PM</span><span class="sxs-lookup"><span data-stu-id="5af03-107">08-01-2022 05:48:12 PM</span></span>|<span data-ttu-id="5af03-108">08\-01\-2022 05:48:12 PM</span><span class="sxs-lookup"><span data-stu-id="5af03-108">08\-01\-2022 05:48:12 PM</span></span>|
|<span data-ttu-id="5af03-109">131222 132455</span><span class="sxs-lookup"><span data-stu-id="5af03-109">131222 132455</span></span>|<span data-ttu-id="5af03-110">13-12-22 13:24:55</span><span class="sxs-lookup"><span data-stu-id="5af03-110">13-12-22 13:24:55</span></span>|
|<span data-ttu-id="5af03-111">1-12-22 10</span><span class="sxs-lookup"><span data-stu-id="5af03-111">1-12-22 10</span></span>|<span data-ttu-id="5af03-112">01-12-22 10:00:00</span><span class="sxs-lookup"><span data-stu-id="5af03-112">01-12-22 10:00:00</span></span>|
|<span data-ttu-id="5af03-113">1.12.22 5</span><span class="sxs-lookup"><span data-stu-id="5af03-113">1.12.22 5</span></span>|<span data-ttu-id="5af03-114">01-12-22 05:00:00</span><span class="sxs-lookup"><span data-stu-id="5af03-114">01-12-22 05:00:00</span></span>|
|<span data-ttu-id="5af03-115">1.12.22</span><span class="sxs-lookup"><span data-stu-id="5af03-115">1.12.22</span></span>|<span data-ttu-id="5af03-116">01-12-22 00:00:00</span><span class="sxs-lookup"><span data-stu-id="5af03-116">01-12-22 00:00:00</span></span>|
|<span data-ttu-id="5af03-117">11 12</span><span class="sxs-lookup"><span data-stu-id="5af03-117">11 12</span></span>|<span data-ttu-id="5af03-118">11-current month-current year 12:00:00</span><span class="sxs-lookup"><span data-stu-id="5af03-118">11-current month-current year 12:00:00</span></span>|
|<span data-ttu-id="5af03-119">1112 12</span><span class="sxs-lookup"><span data-stu-id="5af03-119">1112 12</span></span>|<span data-ttu-id="5af03-120">11-12-current year 12:00:00</span><span class="sxs-lookup"><span data-stu-id="5af03-120">11-12-current year 12:00:00</span></span>|
|<span data-ttu-id="5af03-121">t or today</span><span class="sxs-lookup"><span data-stu-id="5af03-121">t or today</span></span>|<span data-ttu-id="5af03-122">today's date 00:00:00</span><span class="sxs-lookup"><span data-stu-id="5af03-122">today's date 00:00:00</span></span>|
|<span data-ttu-id="5af03-123">t time</span><span class="sxs-lookup"><span data-stu-id="5af03-123">t time</span></span>|<span data-ttu-id="5af03-124">today's date actual time</span><span class="sxs-lookup"><span data-stu-id="5af03-124">today's date actual time</span></span>|
|<span data-ttu-id="5af03-125">t 10:30</span><span class="sxs-lookup"><span data-stu-id="5af03-125">t 10:30</span></span>|<span data-ttu-id="5af03-126">today's date 10:30:00</span><span class="sxs-lookup"><span data-stu-id="5af03-126">today's date 10:30:00</span></span>|
|<span data-ttu-id="5af03-127">t 3:3:3</span><span class="sxs-lookup"><span data-stu-id="5af03-127">t 3:3:3</span></span>|<span data-ttu-id="5af03-128">today's date 03:03:03</span><span class="sxs-lookup"><span data-stu-id="5af03-128">today's date 03:03:03</span></span>|
|<span data-ttu-id="5af03-129">w or workdate</span><span class="sxs-lookup"><span data-stu-id="5af03-129">w or workdate</span></span>|<span data-ttu-id="5af03-130">the working date 00:00:00</span><span class="sxs-lookup"><span data-stu-id="5af03-130">the working date 00:00:00</span></span>|
|<span data-ttu-id="5af03-131">m or Monday</span><span class="sxs-lookup"><span data-stu-id="5af03-131">m or Monday</span></span>|<span data-ttu-id="5af03-132">Monday of the current week 00:00:00</span><span class="sxs-lookup"><span data-stu-id="5af03-132">Monday of the current week 00:00:00</span></span>|
|<span data-ttu-id="5af03-133">tu or Tuesday</span><span class="sxs-lookup"><span data-stu-id="5af03-133">tu or Tuesday</span></span>|<span data-ttu-id="5af03-134">Tuesday of the current week 00:00:00</span><span class="sxs-lookup"><span data-stu-id="5af03-134">Tuesday of the current week 00:00:00</span></span>|
|<span data-ttu-id="5af03-135">we or Wednesday</span><span class="sxs-lookup"><span data-stu-id="5af03-135">we or Wednesday</span></span>|<span data-ttu-id="5af03-136">Wednesday of the current week 00:00:00</span><span class="sxs-lookup"><span data-stu-id="5af03-136">Wednesday of the current week 00:00:00</span></span>|
|<span data-ttu-id="5af03-137">th or Thursday</span><span class="sxs-lookup"><span data-stu-id="5af03-137">th or Thursday</span></span>|<span data-ttu-id="5af03-138">Thursday of the current week 00:00:00</span><span class="sxs-lookup"><span data-stu-id="5af03-138">Thursday of the current week 00:00:00</span></span>|
|<span data-ttu-id="5af03-139">f or Friday</span><span class="sxs-lookup"><span data-stu-id="5af03-139">f or Friday</span></span>|<span data-ttu-id="5af03-140">Friday of the current week 00:00:00</span><span class="sxs-lookup"><span data-stu-id="5af03-140">Friday of the current week 00:00:00</span></span>|
|<span data-ttu-id="5af03-141">s or Saturday</span><span class="sxs-lookup"><span data-stu-id="5af03-141">s or Saturday</span></span>|<span data-ttu-id="5af03-142">Saturday of the current week 00:00:00</span><span class="sxs-lookup"><span data-stu-id="5af03-142">Saturday of the current week 00:00:00</span></span>|
|<span data-ttu-id="5af03-143">su or Sunday</span><span class="sxs-lookup"><span data-stu-id="5af03-143">su or Sunday</span></span>|<span data-ttu-id="5af03-144">Sunday of the current week 00:00:00</span><span class="sxs-lookup"><span data-stu-id="5af03-144">Sunday of the current week 00:00:00</span></span>|
|<span data-ttu-id="5af03-145">tu 10:30</span><span class="sxs-lookup"><span data-stu-id="5af03-145">tu 10:30</span></span>|<span data-ttu-id="5af03-146">Tuesday of the current week 10:30:00</span><span class="sxs-lookup"><span data-stu-id="5af03-146">Tuesday of the current week 10:30:00</span></span>|
|<span data-ttu-id="5af03-147">tu 3:3:3</span><span class="sxs-lookup"><span data-stu-id="5af03-147">tu 3:3:3</span></span>|<span data-ttu-id="5af03-148">Tuesday of the current week 03:03:03</span><span class="sxs-lookup"><span data-stu-id="5af03-148">Tuesday of the current week 03:03:03</span></span>|
|<span data-ttu-id="5af03-149">t23 t</span><span class="sxs-lookup"><span data-stu-id="5af03-149">t23 t</span></span>|<span data-ttu-id="5af03-150">Tuesday of week 23 of the work date year, current time of day</span><span class="sxs-lookup"><span data-stu-id="5af03-150">Tuesday of week 23 of the work date year, current time of day</span></span>|
|<span data-ttu-id="5af03-151">t23</span><span class="sxs-lookup"><span data-stu-id="5af03-151">t23</span></span>|<span data-ttu-id="5af03-152">Tuesday of week 23 of the work date year</span><span class="sxs-lookup"><span data-stu-id="5af03-152">Tuesday of week 23 of the work date year</span></span>|
|<span data-ttu-id="5af03-153">t 23</span><span class="sxs-lookup"><span data-stu-id="5af03-153">t 23</span></span>|<span data-ttu-id="5af03-154">Today 23:00:00</span><span class="sxs-lookup"><span data-stu-id="5af03-154">Today 23:00:00</span></span>|
|<span data-ttu-id="5af03-155">t-1</span><span class="sxs-lookup"><span data-stu-id="5af03-155">t-1</span></span>|<span data-ttu-id="5af03-156">Tuesday of week 1 of the work date year</span><span class="sxs-lookup"><span data-stu-id="5af03-156">Tuesday of week 1 of the work date year</span></span>|


