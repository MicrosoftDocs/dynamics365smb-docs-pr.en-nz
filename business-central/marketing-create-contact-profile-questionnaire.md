---
title: Use profiles to classify contacts
description: Set up profile questionnaires to help classify your business contacts
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: contacts, profiles
ms.author: edupont
ms.date: 05/09/2018
ms.translationtype: HT
ms.sourcegitcommit: 75501b9402bb1c14fcfeb2fc6e61f055a2247493
ms.openlocfilehash: 00cfce8b467040a4de419c1b59a258c0eacf0b9a
ms.contentlocale: en-nz
ms.lasthandoff: 05/15/2018

---

# <a name="use-profile-questionnaires-to-classify-business-contacts"></a><span data-ttu-id="2d2c2-103">Use Profile Questionnaires to Classify Business Contacts</span><span class="sxs-lookup"><span data-stu-id="2d2c2-103">Use Profile Questionnaires to Classify Business Contacts</span></span>
<span data-ttu-id="2d2c2-104">You can set up profile questionnaires that you want to use when entering information about your contacts' profiles.</span><span class="sxs-lookup"><span data-stu-id="2d2c2-104">You can set up profile questionnaires that you want to use when entering information about your contacts' profiles.</span></span> <span data-ttu-id="2d2c2-105">Within each questionnaire, you can set up the different questions you intend to ask your contacts.</span><span class="sxs-lookup"><span data-stu-id="2d2c2-105">Within each questionnaire, you can set up the different questions you intend to ask your contacts.</span></span>  

<span data-ttu-id="2d2c2-106">You can also run the questionnaire to answer some of the questions based on contact, customer, or vendor data automatically.</span><span class="sxs-lookup"><span data-stu-id="2d2c2-106">You can also run the questionnaire to answer some of the questions based on contact, customer, or vendor data automatically.</span></span>  

## <a name="to-add-a-profile-questionnaire"></a><span data-ttu-id="2d2c2-107">To add a profile questionnaire</span><span class="sxs-lookup"><span data-stu-id="2d2c2-107">To add a profile questionnaire</span></span>
1.  <span data-ttu-id="2d2c2-108">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Questionnaire Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="2d2c2-108">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Questionnaire Setup**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="2d2c2-109">On the **Home** tab, in the **New** group, choose **New**.</span><span class="sxs-lookup"><span data-stu-id="2d2c2-109">On the **Home** tab, in the **New** group, choose **New**.</span></span>  
3.  <span data-ttu-id="2d2c2-110">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="2d2c2-110">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

## <a name="to-add-questions-to-a-profile-questionnaire"></a><span data-ttu-id="2d2c2-111">To add questions to a profile questionnaire</span><span class="sxs-lookup"><span data-stu-id="2d2c2-111">To add questions to a profile questionnaire</span></span>
1.  <span data-ttu-id="2d2c2-112">Choose the relevant profile questionnaire, and then on the **Home** tab, in the **Process** group, choose **Edit Questionnaire Setup**.</span><span class="sxs-lookup"><span data-stu-id="2d2c2-112">Choose the relevant profile questionnaire, and then on the **Home** tab, in the **Process** group, choose **Edit Questionnaire Setup**.</span></span>  
2.  <span data-ttu-id="2d2c2-113">On the first empty line, in the **Type** field, choose **Question** and type your question in the **Description** field.</span><span class="sxs-lookup"><span data-stu-id="2d2c2-113">On the first empty line, in the **Type** field, choose **Question** and type your question in the **Description** field.</span></span> <span data-ttu-id="2d2c2-114">Fill in the other fields on this line.</span><span class="sxs-lookup"><span data-stu-id="2d2c2-114">Fill in the other fields on this line.</span></span>  
3.  <span data-ttu-id="2d2c2-115">On the next empty line, in the **Type** field, choose **Answer** and type your answer in the **Description** field.</span><span class="sxs-lookup"><span data-stu-id="2d2c2-115">On the next empty line, in the **Type** field, choose **Answer** and type your answer in the **Description** field.</span></span>  
4.  <span data-ttu-id="2d2c2-116">In the **Priority** field, select the priority.</span><span class="sxs-lookup"><span data-stu-id="2d2c2-116">In the **Priority** field, select the priority.</span></span> <span data-ttu-id="2d2c2-117">In the **From Value** and **To Value** fields, define a point range.</span><span class="sxs-lookup"><span data-stu-id="2d2c2-117">In the **From Value** and **To Value** fields, define a point range.</span></span> <span data-ttu-id="2d2c2-118">Contacts that receive points within the defined range will get the answer.</span><span class="sxs-lookup"><span data-stu-id="2d2c2-118">Contacts that receive points within the defined range will get the answer.</span></span>  

<span data-ttu-id="2d2c2-119">Repeat these steps to enter all the questions and answers within the profile questionnaire.</span><span class="sxs-lookup"><span data-stu-id="2d2c2-119">Repeat these steps to enter all the questions and answers within the profile questionnaire.</span></span>

<span data-ttu-id="2d2c2-120">After you have created a questionnaire, you must create contact ratings to classify your contacts.</span><span class="sxs-lookup"><span data-stu-id="2d2c2-120">After you have created a questionnaire, you must create contact ratings to classify your contacts.</span></span> <span data-ttu-id="2d2c2-121">You can also set up questions that are rated automatically based on information in the contact card.</span><span class="sxs-lookup"><span data-stu-id="2d2c2-121">You can also set up questions that are rated automatically based on information in the contact card.</span></span>  

> [!NOTE]
> <span data-ttu-id="2d2c2-122">If you enter a question that is automatically answered, choose <STRONG>Line</STRONG>, and then choose <STRONG>Question Details</STRONG>, to enter the criteria to automatically answer the question.</span><span class="sxs-lookup"><span data-stu-id="2d2c2-122">If you enter a question that is automatically answered, choose <STRONG>Line</STRONG>, and then choose <STRONG>Question Details</STRONG>, to enter the criteria to automatically answer the question.</span></span>

## <a name="the-automatic-classification-of-contacts"></a><span data-ttu-id="2d2c2-123">The Automatic Classification of Contacts</span><span class="sxs-lookup"><span data-stu-id="2d2c2-123">The Automatic Classification of Contacts</span></span>
<span data-ttu-id="2d2c2-124">You can automatically classify your contacts according to customer, vendor, and contact information, by setting up automatically answered profile questions in the **Profile Questionnaire Setup** window.</span><span class="sxs-lookup"><span data-stu-id="2d2c2-124">You can automatically classify your contacts according to customer, vendor, and contact information, by setting up automatically answered profile questions in the **Profile Questionnaire Setup** window.</span></span>  

> [!NOTE]
> <span data-ttu-id="2d2c2-125">Only contacts that are recorded as customers can be assigned a classification based on customer data and only contacts that are recorded as vendors can be assigned a classification based on vendor data.</span><span class="sxs-lookup"><span data-stu-id="2d2c2-125">Only contacts that are recorded as customers can be assigned a classification based on customer data and only contacts that are recorded as vendors can be assigned a classification based on vendor data.</span></span> <span data-ttu-id="2d2c2-126">The automatic classification is not updated automatically.</span><span class="sxs-lookup"><span data-stu-id="2d2c2-126">The automatic classification is not updated automatically.</span></span> <span data-ttu-id="2d2c2-127">Consequently, you may want to update the profile questionnaires, after you have updated the customer, vendor or contact data they are based on.</span><span class="sxs-lookup"><span data-stu-id="2d2c2-127">Consequently, you may want to update the profile questionnaires, after you have updated the customer, vendor or contact data they are based on.</span></span>  

<span data-ttu-id="2d2c2-128">After you have set up automatically answered profile questions, if you assign the profile questionnaire containing these questions to a contact, [!INCLUDE[d365fin](includes/d365fin_md.md)] will automatically assign the right answers for the contact.</span><span class="sxs-lookup"><span data-stu-id="2d2c2-128">After you have set up automatically answered profile questions, if you assign the profile questionnaire containing these questions to a contact, [!INCLUDE[d365fin](includes/d365fin_md.md)] will automatically assign the right answers for the contact.</span></span>  

## <a name="example"></a><span data-ttu-id="2d2c2-129">Example</span><span class="sxs-lookup"><span data-stu-id="2d2c2-129">Example</span></span>
<span data-ttu-id="2d2c2-130">You can classify your contacts according to how much they bought from you:</span><span class="sxs-lookup"><span data-stu-id="2d2c2-130">You can classify your contacts according to how much they bought from you:</span></span>

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="2d2c2-131"><strong>Answer</strong></span><span class="sxs-lookup"><span data-stu-id="2d2c2-131"><strong>Answer</strong></span></span></th>
<th><span data-ttu-id="2d2c2-132"><strong>Applies to</strong></span><span class="sxs-lookup"><span data-stu-id="2d2c2-132"><strong>Applies to</strong></span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><span data-ttu-id="2d2c2-133">A</span><span class="sxs-lookup"><span data-stu-id="2d2c2-133">A</span></span></p></td>
<td><p><span data-ttu-id="2d2c2-134">contacts who bought for 500,000 LCY or more</span><span class="sxs-lookup"><span data-stu-id="2d2c2-134">contacts who bought for 500,000 LCY or more</span></span></p></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="2d2c2-135">B</span><span class="sxs-lookup"><span data-stu-id="2d2c2-135">B</span></span></p></td>
<td><p><span data-ttu-id="2d2c2-136">contacts who bought for 100,000 up to 499,999 LCY</span><span class="sxs-lookup"><span data-stu-id="2d2c2-136">contacts who bought for 100,000 up to 499,999 LCY</span></span></p></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="2d2c2-137">C</span><span class="sxs-lookup"><span data-stu-id="2d2c2-137">C</span></span></p></td>
<td><p><span data-ttu-id="2d2c2-138">contacts who bought for 99,999 LCY or less</span><span class="sxs-lookup"><span data-stu-id="2d2c2-138">contacts who bought for 99,999 LCY or less</span></span></p></td>
</tr>
</tbody>
</table>

<span data-ttu-id="2d2c2-139">To do this, fill in the **Profile Questionnaire Setup** window as follows:</span><span class="sxs-lookup"><span data-stu-id="2d2c2-139">To do this, fill in the **Profile Questionnaire Setup** window as follows:</span></span>


<table>
<colgroup>
<col style="width: 20%" />
<col style="width: 20%" />
<col style="width: 20%" />
<col style="width: 20%" />
<col style="width: 20%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="2d2c2-140"><strong>Type</strong></span><span class="sxs-lookup"><span data-stu-id="2d2c2-140"><strong>Type</strong></span></span></th>
<th><span data-ttu-id="2d2c2-141"><strong>Description</strong></span><span class="sxs-lookup"><span data-stu-id="2d2c2-141"><strong>Description</strong></span></span></th>
<th><span data-ttu-id="2d2c2-142"><strong>Automatic Classification</strong></span><span class="sxs-lookup"><span data-stu-id="2d2c2-142"><strong>Automatic Classification</strong></span></span></th>
<th><span data-ttu-id="2d2c2-143"><strong>From Value</strong></span><span class="sxs-lookup"><span data-stu-id="2d2c2-143"><strong>From Value</strong></span></span></th>
<th><span data-ttu-id="2d2c2-144"><strong>To Value</strong></span><span class="sxs-lookup"><span data-stu-id="2d2c2-144"><strong>To Value</strong></span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><span data-ttu-id="2d2c2-145">Question</span><span class="sxs-lookup"><span data-stu-id="2d2c2-145">Question</span></span></p></td>
<td><p><span data-ttu-id="2d2c2-146">ABC Classification</span><span class="sxs-lookup"><span data-stu-id="2d2c2-146">ABC Classification</span></span></p></td>
<td><p><span data-ttu-id="2d2c2-147">Click to insert a check mark</span><span class="sxs-lookup"><span data-stu-id="2d2c2-147">Click to insert a check mark</span></span></p></td>
<td><p> </p></td>
<td><p> </p></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="2d2c2-148">Answer</span><span class="sxs-lookup"><span data-stu-id="2d2c2-148">Answer</span></span></p></td>
<td><p><span data-ttu-id="2d2c2-149">A</span><span class="sxs-lookup"><span data-stu-id="2d2c2-149">A</span></span></p></td>
<td><p> </p></td>
<td><p><span data-ttu-id="2d2c2-150">500,000</span><span class="sxs-lookup"><span data-stu-id="2d2c2-150">500,000</span></span></p></td>
<td><p> </p></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="2d2c2-151">Answer</span><span class="sxs-lookup"><span data-stu-id="2d2c2-151">Answer</span></span></p></td>
<td><p><span data-ttu-id="2d2c2-152">B</span><span class="sxs-lookup"><span data-stu-id="2d2c2-152">B</span></span></p></td>
<td><p> </p></td>
<td><p><span data-ttu-id="2d2c2-153">100,000</span><span class="sxs-lookup"><span data-stu-id="2d2c2-153">100,000</span></span></p></td>
<td><p><span data-ttu-id="2d2c2-154">499,999</span><span class="sxs-lookup"><span data-stu-id="2d2c2-154">499,999</span></span></p></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="2d2c2-155">Answer</span><span class="sxs-lookup"><span data-stu-id="2d2c2-155">Answer</span></span></p></td>
<td><p><span data-ttu-id="2d2c2-156">C</span><span class="sxs-lookup"><span data-stu-id="2d2c2-156">C</span></span></p></td>
<td><p> </p></td>
<td><p> </p></td>
<td><p><span data-ttu-id="2d2c2-157">99,999</span><span class="sxs-lookup"><span data-stu-id="2d2c2-157">99,999</span></span></p></td>
</tr>
</tbody>
</table>

<span data-ttu-id="2d2c2-158">Then fill in the **Profile Question Details** window as follows:</span><span class="sxs-lookup"><span data-stu-id="2d2c2-158">Then fill in the **Profile Question Details** window as follows:</span></span>
<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="2d2c2-159"><strong>Field</strong></span><span class="sxs-lookup"><span data-stu-id="2d2c2-159"><strong>Field</strong></span></span></th>
<th><span data-ttu-id="2d2c2-160"><strong>Value</strong></span><span class="sxs-lookup"><span data-stu-id="2d2c2-160"><strong>Value</strong></span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="2d2c2-161"><strong>Customer Classification Field</strong></span><span class="sxs-lookup"><span data-stu-id="2d2c2-161"><strong>Customer Classification Field</strong></span></span></td>
<td><span data-ttu-id="2d2c2-162"><emphasis>Sales (LCY)</emphasis></span><span class="sxs-lookup"><span data-stu-id="2d2c2-162"><emphasis>Sales (LCY)</emphasis></span></span></td>
</tr>
<tr>
<td><span data-ttu-id="2d2c2-163"><strong>Classification Method</strong></span><span class="sxs-lookup"><span data-stu-id="2d2c2-163"><strong>Classification Method</strong></span></span></td>
<td><span data-ttu-id="2d2c2-164"><emphasis>Defined Value</emphasis></span><span class="sxs-lookup"><span data-stu-id="2d2c2-164"><emphasis>Defined Value</emphasis></span></span></td>
</tr>
</tbody>
</table>

<span data-ttu-id="2d2c2-165">When you assign the profile questionnaire containing this question to a contact, the program automatically enters the relevant answer for this contact on the profile lines of the contact card.</span><span class="sxs-lookup"><span data-stu-id="2d2c2-165">When you assign the profile questionnaire containing this question to a contact, the program automatically enters the relevant answer for this contact on the profile lines of the contact card.</span></span>

## <a name="see-also"></a><span data-ttu-id="2d2c2-166">See Also</span><span class="sxs-lookup"><span data-stu-id="2d2c2-166">See Also</span></span>
[<span data-ttu-id="2d2c2-167">Creating Contact Persons</span><span class="sxs-lookup"><span data-stu-id="2d2c2-167">Creating Contact Persons</span></span>](marketing-create-contact-persons.md)  
[<span data-ttu-id="2d2c2-168">Create Contact Persons</span><span class="sxs-lookup"><span data-stu-id="2d2c2-168">Create Contact Persons</span></span>](marketing-how-create-contact-persons.md)  
[<span data-ttu-id="2d2c2-169">Creating Contact Companies</span><span class="sxs-lookup"><span data-stu-id="2d2c2-169">Creating Contact Companies</span></span>](marketing-create-contact-companies.md)  

