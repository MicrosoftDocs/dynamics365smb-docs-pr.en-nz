---
title: The Image Analyser Extension
description: This extension lets you analyse images of contact persons and items to find attributes, so you can quickly assign them in Business Central.
author: brentholtorf
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: API, extension, Cognitive Services, image, computer vision, attribute, tag, recognition
ms.date: 05/19/2021
ms.author: bholtorf
ms.openlocfilehash: bbeffd4175751e08043d79f596027a79c88503bc
ms.sourcegitcommit: 5a916b0aa0a2eef0c22b5722a0af041757e6d7c2
ms.translationtype: HT
ms.contentlocale: en-NZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "6074628"
---
# <a name="the-image-analyzer-extension"></a>The Image Analyser Extension

The Image Analyser extension uses powerful image analytics provided by the Computer Vision API for Azure Cognitive Services to detect attributes in the images that you import for items and contact persons, so you can easily review and assign them. For items, attributes could be whether the item is a table or a car, and whether it is red or blue. For contact persons, attributes can be gender or age.

Image Analyser suggests attributes based on tags that the Computer Vision API finds, and a confidence level. By default, it suggests attributes only if it is at least 80% sure that the attribute is correct. You can set another confidence level, if needed. To learn more about how the tags and confidence level are determined, see [Computer Vision API](https://go.microsoft.com/fwlink/?linkid=851476).  

Image Analyzer is free in [!INCLUDE[prod_short](includes/prod_short.md)], but there is a limit to the number of items that you can analyze during a certain period of time. By default, you can analyse 100 images per month.

After you enable the extension, Image Analyser runs each time you import an image to an item or contact person. You will see the attributes, confidence level, and details right away, and can decide what to do with each attribute. If you imported images before you enabled the Image Analyzer extension, you must go to the item or contact cards and choose the **Analyze Picture** action.  

## <a name="privacy-notice"></a>Privacy Notice

This extension uses the Computer Vision API from Azure Cognitive Services, which may have varying levels of compliance commitments than [!INCLUDE[prod_short](includes/prod_short.md)]. When you enable the Image Analyser extension, Customer Data such as a contact image or an item image will be sent to the Computer Vision API. By installing this extension, you agree for this limited set of data to be sent to the Computer Vision API. Note that you may disable, as well as uninstall, the Image Analyser extension at any time to discontinue use of this functionality. For more information, see [Microsoft Trust Center](https://go.microsoft.com/fwlink/?linkid=851463).

## <a name="requirements"></a>Requirements

There are a few requirements for the images:

* Image formats: JPEG, PNG, GIF, BMP  
* Maximum file size: Less than 4 MB  
* Image dimensions: Greater than 50 x 50 pixels  

## <a name="to-enable-image-analyzer"></a>To enable Image Analyser

The Image Analyser extension is built in to [!INCLUDE[prod_short](includes/prod_short.md)]. You just need to turn it on.

> [!NOTE]  
> To enable the Image Analyser extension, you must be an administrator. Make sure that you are assigned the **SUPER** user permission set. For more information, see [Assign Permissions to Users and Groups](ui-define-granular-permissions.md).

To enable the Image Analyser extension, take one of the following actions:

* Open an item or contact card. In the notification bar, choose **Analyze Images**, and then follow the steps in the assisted setup guide.  
* Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Service Connections**, and then choose **Image Analysis Setup**. Choose the **Enable Image Analyzer** check box, and then complete the steps in the assisted setup guide.  

    > [!TIP]  
    > The **Image Analysis Setup** page is also where you can change the degree of confidence for attribute suggestions. For example, if you want to require a greater degree of confidence, you can enter a higher percentage.

## <a name="to-analyze-an-image-of-an-item"></a>To analyse an image of an item

The following steps describe how to analyse an image that was imported before you enabled the Image Analyser extension.  

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.  
2. Choose the item, and then choose the **Analyze Picture** action.  
3. The **Image Analyzer Attributes** page displays the detected attributes, the confidence level, and other details about the attribute. Use the **Action to perform** options to specify what to do with the attribute or choose **Add to item description** to add the name of the attribute to the item description. For example, this can be useful for quickly adding detail. 

The **Action to perform** action has following options:

  * *Ignore*

    No actions will be performed
  * *Use as attribute*

    The value is added to the item attributes. For more information, see [Work with Item Attributes](inventory-how-work-item-attributes.md)
  * *Use as a category*

    The selected value is added as a category. For more information, see [Categorise Items](inventory-how-categorize-items.md)
  * *Add to blacklist*

    If the analysis suggests an attribute that you do not want to see, you can block the attribute. Use caution, however. Blocked attributes are not suggested for other items either. If you regret blocking an attribute, choose **View Blacklisted Attributes**, and then delete the attribute from the list.
  
    > [!NOTE]  
    > By default **Item Attributes** displays attributes where **Confidence Score** is above **Confidence Score Threshold %** defined in the **Image Analyser Setup**. To see all detected attributes, choose the **View All Attributes** action.

## <a name="to-analyze-a-picture-of-a-contact-person"></a>To analyse a picture of a contact person

The following steps describe how to analyse an image that was imported before you enabled the Image Analyser extension.  

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Contacts**, and then choose the related link.  
2. Choose the contact person, and then choose the **Analyze Picture** action.  
3. On the **Profile Questionnaire** FastTab, review the suggestions, and make corrections if needed. For more information, see [Use Profile Questionnaires to Classify Business Contacts](marketing-create-contact-profile-questionnaire.md).  

    > [!NOTE]  
    > 
    > The Computer Vision API returns following attributes:
    > * *age*
    >
    >     An estimated "visual age" in years. It is how old a person looks as opposed to the actual biological age.
    > * *gender*
    >
    >    Male or female.
    > 
    > The Computer Vision API doesn't return confidence level for age and gender attributes.
  
## <a name="to-use-your-own-account-for-the-computer-vision-api"></a>To use your own account for the Computer Vision API

You can also use your own account for the Computer Vision API, for example, if you want to analyse more images than we allow.  

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Image Analyser Setup**, and then choose the related link.  
2. Enter the **API URI** and **API Key** that you received for Computer Vision API.  

    > [!NOTE]  
    > You must add **/analyze** at the end of the API URI, if it isn't already there. For example: ```https://cronus.api.cognitive.microsoft.com/vision/v1.0/analyze```.

## <a name="to-see-how-many-analyses-you-have-left-in-the-current-period"></a>To see how many analyses you have left in the current period

You can view the number of analyses you've done, and how many you can still do, in the current period.  

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Image Analyser Setup**, and then choose the related link.  
2. The **Limit type**, **Limit value**, and **Analyzes performed** provide the usage information.  

## <a name="to-stop-using-the-image-analyzer-extension"></a>To stop using the Image Analyser extension

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Service Connections**, and then choose **Image Analyser Setup**.  
2. Clear the **Enable Image Analyzer** check box.  

Alternatively, uninstall the extension completely. You can always fetch it again from AppSource. For more information, see [Installing and Uninstalling Extensions in Business Central](ui-extensions-install-uninstall.md#uninstalling-an-extension).  

## <a name="see-also"></a>See Also

[Work with Item Attributes](inventory-how-work-item-attributes.md)  
[Categorise Items](inventory-how-categorize-items.md)  
[Use Profile Questionnaires to Classify Business Contacts](marketing-create-contact-profile-questionnaire.md)  
[Customizing [!INCLUDE[prod_short](includes/prod_short.md)] Using Extensions](ui-extensions.md)  
[Getting Ready for Doing Business](ui-get-ready-business.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]
