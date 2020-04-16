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
ms.date: 04/01/2020
ms.openlocfilehash: 9cf4817cd85951f193ffadbcd3e7ebc971bcca36
ms.sourcegitcommit: 88e4b30eaf6fa32af0c1452ce2f85ff1111c75e2
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 04/01/2020
ms.locfileid: "3181596"
---
# <a name="use-profile-questionnaires-to-classify-business-contacts"></a><span data-ttu-id="48365-103">Use Profile Questionnaires to Classify Business Contacts</span><span class="sxs-lookup"><span data-stu-id="48365-103">Use Profile Questionnaires to Classify Business Contacts</span></span>
<span data-ttu-id="48365-104">You can set up profile questionnaires that you want to use when entering information about your contacts' profiles.</span><span class="sxs-lookup"><span data-stu-id="48365-104">You can set up profile questionnaires that you want to use when entering information about your contacts' profiles.</span></span> <span data-ttu-id="48365-105">Within each questionnaire, you can set up the different questions you intend to ask your contacts.</span><span class="sxs-lookup"><span data-stu-id="48365-105">Within each questionnaire, you can set up the different questions you intend to ask your contacts.</span></span>  

<span data-ttu-id="48365-106">You can also run the questionnaire to answer some of the questions based on contact, customer, or vendor data automatically.</span><span class="sxs-lookup"><span data-stu-id="48365-106">You can also run the questionnaire to answer some of the questions based on contact, customer, or vendor data automatically.</span></span>  

## <a name="to-add-a-profile-questionnaire"></a><span data-ttu-id="48365-107">To add a profile questionnaire</span><span class="sxs-lookup"><span data-stu-id="48365-107">To add a profile questionnaire</span></span>
1.  <span data-ttu-id="48365-108">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Questionnaire Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="48365-108">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Questionnaire Setup**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="48365-109">Choose the **New** Action.</span><span class="sxs-lookup"><span data-stu-id="48365-109">Choose the **New** Action.</span></span>  
3.  <span data-ttu-id="48365-110">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="48365-110">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

## <a name="to-add-questions-to-a-profile-questionnaire"></a><span data-ttu-id="48365-111">To add questions to a profile questionnaire</span><span class="sxs-lookup"><span data-stu-id="48365-111">To add questions to a profile questionnaire</span></span>
1.  <span data-ttu-id="48365-112">Choose the relevant profile questionnaire, and then choose the **Edit Questionnaire Setup** action.</span><span class="sxs-lookup"><span data-stu-id="48365-112">Choose the relevant profile questionnaire, and then choose the **Edit Questionnaire Setup** action.</span></span>  
2.  <span data-ttu-id="48365-113">On the first empty line, in the **Type** field, choose **Question** and type your question in the **Description** field.</span><span class="sxs-lookup"><span data-stu-id="48365-113">On the first empty line, in the **Type** field, choose **Question** and type your question in the **Description** field.</span></span> <span data-ttu-id="48365-114">Fill in the other fields on this line.</span><span class="sxs-lookup"><span data-stu-id="48365-114">Fill in the other fields on this line.</span></span>  
3.  <span data-ttu-id="48365-115">On the next empty line, in the **Type** field, choose **Answer** and type your answer in the **Description** field.</span><span class="sxs-lookup"><span data-stu-id="48365-115">On the next empty line, in the **Type** field, choose **Answer** and type your answer in the **Description** field.</span></span>  
4.  <span data-ttu-id="48365-116">In the **Priority** field, select the priority.</span><span class="sxs-lookup"><span data-stu-id="48365-116">In the **Priority** field, select the priority.</span></span> <span data-ttu-id="48365-117">In the **From Value** and **To Value** fields, define a point range.</span><span class="sxs-lookup"><span data-stu-id="48365-117">In the **From Value** and **To Value** fields, define a point range.</span></span> <span data-ttu-id="48365-118">Contacts that receive points within the defined range will get the answer.</span><span class="sxs-lookup"><span data-stu-id="48365-118">Contacts that receive points within the defined range will get the answer.</span></span>  

<span data-ttu-id="48365-119">Repeat these steps to enter all the questions and answers within the profile questionnaire.</span><span class="sxs-lookup"><span data-stu-id="48365-119">Repeat these steps to enter all the questions and answers within the profile questionnaire.</span></span>

<span data-ttu-id="48365-120">After you have created a questionnaire, you must create contact ratings to classify your contacts.</span><span class="sxs-lookup"><span data-stu-id="48365-120">After you have created a questionnaire, you must create contact ratings to classify your contacts.</span></span> <span data-ttu-id="48365-121">You can also set up questions that are rated automatically based on information in the contact card.</span><span class="sxs-lookup"><span data-stu-id="48365-121">You can also set up questions that are rated automatically based on information in the contact card.</span></span>  

> [!NOTE]
> <span data-ttu-id="48365-122">If you enter a question that is automatically answered, choose <STRONG>Line</STRONG>, and then choose <STRONG>Question Details</STRONG>, to enter the criteria to automatically answer the question.</span><span class="sxs-lookup"><span data-stu-id="48365-122">If you enter a question that is automatically answered, choose <STRONG>Line</STRONG>, and then choose <STRONG>Question Details</STRONG>, to enter the criteria to automatically answer the question.</span></span>

## <a name="the-automatic-classification-of-contacts"></a><span data-ttu-id="48365-123">The Automatic Classification of Contacts</span><span class="sxs-lookup"><span data-stu-id="48365-123">The Automatic Classification of Contacts</span></span>
<span data-ttu-id="48365-124">You can automatically classify your contacts according to customer, vendor, and contact information, by setting up automatically answered profile questions on the **Profile Questionnaire Setup** page.</span><span class="sxs-lookup"><span data-stu-id="48365-124">You can automatically classify your contacts according to customer, vendor, and contact information, by setting up automatically answered profile questions on the **Profile Questionnaire Setup** page.</span></span>  

> [!NOTE]
> <span data-ttu-id="48365-125">Only contacts that are recorded as customers can be assigned a classification based on customer data and only contacts that are recorded as vendors can be assigned a classification based on vendor data.</span><span class="sxs-lookup"><span data-stu-id="48365-125">Only contacts that are recorded as customers can be assigned a classification based on customer data and only contacts that are recorded as vendors can be assigned a classification based on vendor data.</span></span> <span data-ttu-id="48365-126">The automatic classification is not updated automatically.</span><span class="sxs-lookup"><span data-stu-id="48365-126">The automatic classification is not updated automatically.</span></span> <span data-ttu-id="48365-127">Consequently, you may want to update the profile questionnaires, after you have updated the customer, vendor or contact data they are based on.</span><span class="sxs-lookup"><span data-stu-id="48365-127">Consequently, you may want to update the profile questionnaires, after you have updated the customer, vendor or contact data they are based on.</span></span>  

<span data-ttu-id="48365-128">After you have set up automatically answered profile questions, if you assign the profile questionnaire containing these questions to a contact, [!INCLUDE[d365fin](includes/d365fin_md.md)] will automatically assign the right answers for the contact.</span><span class="sxs-lookup"><span data-stu-id="48365-128">After you have set up automatically answered profile questions, if you assign the profile questionnaire containing these questions to a contact, [!INCLUDE[d365fin](includes/d365fin_md.md)] will automatically assign the right answers for the contact.</span></span>  

## <a name="example"></a><span data-ttu-id="48365-129">Example</span><span class="sxs-lookup"><span data-stu-id="48365-129">Example</span></span>
<span data-ttu-id="48365-130">You can classify your contacts according to how much they bought from you:</span><span class="sxs-lookup"><span data-stu-id="48365-130">You can classify your contacts according to how much they bought from you:</span></span>

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="48365-131"><strong>Answer</strong></span><span class="sxs-lookup"><span data-stu-id="48365-131"><strong>Answer</strong></span></span></th>
<th><span data-ttu-id="48365-132"><strong>Applies to</strong></span><span class="sxs-lookup"><span data-stu-id="48365-132"><strong>Applies to</strong></span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><span data-ttu-id="48365-133">A</span><span class="sxs-lookup"><span data-stu-id="48365-133">A</span></span></p></td>
<td><p><span data-ttu-id="48365-134">contacts who bought for 500,000 LCY or more</span><span class="sxs-lookup"><span data-stu-id="48365-134">contacts who bought for 500,000 LCY or more</span></span></p></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="48365-135">B</span><span class="sxs-lookup"><span data-stu-id="48365-135">B</span></span></p></td>
<td><p><span data-ttu-id="48365-136">contacts who bought for 100,000 up to 499,999 LCY</span><span class="sxs-lookup"><span data-stu-id="48365-136">contacts who bought for 100,000 up to 499,999 LCY</span></span></p></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="48365-137">C</span><span class="sxs-lookup"><span data-stu-id="48365-137">C</span></span></p></td>
<td><p><span data-ttu-id="48365-138">contacts who bought for 99,999 LCY or less</span><span class="sxs-lookup"><span data-stu-id="48365-138">contacts who bought for 99,999 LCY or less</span></span></p></td>
</tr>
</tbody>
</table>

<span data-ttu-id="48365-139">To do this, fill on the **Profile Questionnaire Setup** page as follows:</span><span class="sxs-lookup"><span data-stu-id="48365-139">To do this, fill on the **Profile Questionnaire Setup** page as follows:</span></span>


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
<th><span data-ttu-id="48365-140"><strong>Type</strong></span><span class="sxs-lookup"><span data-stu-id="48365-140"><strong>Type</strong></span></span></th>
<th><span data-ttu-id="48365-141"><strong>Description</strong></span><span class="sxs-lookup"><span data-stu-id="48365-141"><strong>Description</strong></span></span></th>
<th><span data-ttu-id="48365-142"><strong>Automatic Classification</strong></span><span class="sxs-lookup"><span data-stu-id="48365-142"><strong>Automatic Classification</strong></span></span></th>
<th><span data-ttu-id="48365-143"><strong>From Value</strong></span><span class="sxs-lookup"><span data-stu-id="48365-143"><strong>From Value</strong></span></span></th>
<th><span data-ttu-id="48365-144"><strong>To Value</strong></span><span class="sxs-lookup"><span data-stu-id="48365-144"><strong>To Value</strong></span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><span data-ttu-id="48365-145">Question</span><span class="sxs-lookup"><span data-stu-id="48365-145">Question</span></span></p></td>
<td><p><span data-ttu-id="48365-146">ABC Classification</span><span class="sxs-lookup"><span data-stu-id="48365-146">ABC Classification</span></span></p></td>
<td><p><span data-ttu-id="48365-147">Click to insert a check mark</span><span class="sxs-lookup"><span data-stu-id="48365-147">Click to insert a check mark</span></span></p></td>
<td><p> </p></td>
<td><p> </p></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="48365-148">Answer</span><span class="sxs-lookup"><span data-stu-id="48365-148">Answer</span></span></p></td>
<td><p><span data-ttu-id="48365-149">A</span><span class="sxs-lookup"><span data-stu-id="48365-149">A</span></span></p></td>
<td><p> </p></td>
<td><p><span data-ttu-id="48365-150">500,000</span><span class="sxs-lookup"><span data-stu-id="48365-150">500,000</span></span></p></td>
<td><p> </p></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="48365-151">Answer</span><span class="sxs-lookup"><span data-stu-id="48365-151">Answer</span></span></p></td>
<td><p><span data-ttu-id="48365-152">B</span><span class="sxs-lookup"><span data-stu-id="48365-152">B</span></span></p></td>
<td><p> </p></td>
<td><p><span data-ttu-id="48365-153">100,000</span><span class="sxs-lookup"><span data-stu-id="48365-153">100,000</span></span></p></td>
<td><p><span data-ttu-id="48365-154">499,999</span><span class="sxs-lookup"><span data-stu-id="48365-154">499,999</span></span></p></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="48365-155">Answer</span><span class="sxs-lookup"><span data-stu-id="48365-155">Answer</span></span></p></td>
<td><p><span data-ttu-id="48365-156">C</span><span class="sxs-lookup"><span data-stu-id="48365-156">C</span></span></p></td>
<td><p> </p></td>
<td><p> </p></td>
<td><p><span data-ttu-id="48365-157">99,999</span><span class="sxs-lookup"><span data-stu-id="48365-157">99,999</span></span></p></td>
</tr>
</tbody>
</table>

<span data-ttu-id="48365-158">Then fill on the **Profile Question Details** page as follows:</span><span class="sxs-lookup"><span data-stu-id="48365-158">Then fill on the **Profile Question Details** page as follows:</span></span>
<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="48365-159"><strong>Field</strong></span><span class="sxs-lookup"><span data-stu-id="48365-159"><strong>Field</strong></span></span></th>
<th><span data-ttu-id="48365-160"><strong>Value</strong></span><span class="sxs-lookup"><span data-stu-id="48365-160"><strong>Value</strong></span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="48365-161"><strong>Customer Classification Field</strong></span><span class="sxs-lookup"><span data-stu-id="48365-161"><strong>Customer Classification Field</strong></span></span></td>
<td><span data-ttu-id="48365-162"><emphasis>Sales (LCY)</emphasis></span><span class="sxs-lookup"><span data-stu-id="48365-162"><emphasis>Sales (LCY)</emphasis></span></span></td>
</tr>
<tr>
<td><span data-ttu-id="48365-163"><strong>Classification Method</strong></span><span class="sxs-lookup"><span data-stu-id="48365-163"><strong>Classification Method</strong></span></span></td>
<td><span data-ttu-id="48365-164"><emphasis>Defined Value</emphasis></span><span class="sxs-lookup"><span data-stu-id="48365-164"><emphasis>Defined Value</emphasis></span></span></td>
</tr>
</tbody>
</table>

<span data-ttu-id="48365-165">When you assign the profile questionnaire containing this question to a contact, application automatically enters the relevant answer for this contact on the profile lines of the contact card.</span><span class="sxs-lookup"><span data-stu-id="48365-165">When you assign the profile questionnaire containing this question to a contact, application automatically enters the relevant answer for this contact on the profile lines of the contact card.</span></span>

## <a name="see-also"></a><span data-ttu-id="48365-166">See Also</span><span class="sxs-lookup"><span data-stu-id="48365-166">See Also</span></span>
[<span data-ttu-id="48365-167">Creating Contacts</span><span class="sxs-lookup"><span data-stu-id="48365-167">Creating Contacts</span></span>](marketing-create-contact-companies.md)  
