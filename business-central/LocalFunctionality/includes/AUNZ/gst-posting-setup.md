---
author: brentholtorf
ms.topic: include
ms.date: 12/07/2023
ms.author: bholtorf
---

To set up posting details for GST, you must define the posting groups, rate of GST, and the accounts to which GST is to be posted. You can set up this information for a particular combination of business posting groups and product posting groups.  

You must set up GST posting before you generate the BAS report.  

## <a name="to-set-up-goods-and-sales-tax-posting"></a>To set up goods and GST posting
1. Choose the ![Lightbulb that opens the Tell Me feature.](../../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **GST Posting Setup**, and then choose the related link.  
2. Fill in the fields as described in the following table.  

    |Field|Description|  
    |---------------------------------|---------------------------------------|  
    |**GST Bus. Posting Group**|Specifies the GST business posting group code.|  
    |**GST Prod. Posting Group**|Specifies the GST product posting group code.|  
    |**GST Identifier**|Specifies the code that is used to group similar GST setups with similar attributes.<br /><br /> For example, you can group many VAT posting setups that have a common VAT percentage.|  
    |**GST %**|Specifies the GST rate.|  
    |**GST Calculation Type**|Specifies the method that is used to calculate the purchase or sale of items.|  
    |**Sales GST Account**|Specifies the number of the general ledger account to which you want to post the sales GST.<br /><br /> If you select the **Reverse Charge VAT** option in the **VAT Calculation Type** field, then don't enter a value in this field.|  
    |**Purchase GST Account**|Specifies the number of the general ledger account to which you want to post the purchase GST.|  
    |**Reverse Chrg. GST Acc.**|Specifies the number of the general ledger account to which you want to post the reverse charge GST.<br /><br /> You can enter a value in this field only if you select the **Reverse Charge VAT** option in the **VAT Calculation Type** field.|  

3.  Choose the **OK** button.  
