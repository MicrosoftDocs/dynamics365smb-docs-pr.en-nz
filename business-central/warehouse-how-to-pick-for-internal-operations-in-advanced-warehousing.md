---
title: Pick for Internal Operations in Advanced Warehouse Configurations
description: 'If your locations use picking and shipping, pick components for production, assembly, and job activities on the Warehouse Pick page.'
author: brentholtorf
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: null
ms.date: 09/02/2022
ms.author: bholtorf
---
# <a name="pick-for-production-assembly-or-jobs-in-advanced-warehouse-configurations" />Pick for Production, Assembly, or Jobs in Advanced Warehouse Configurations

How you pick components for production, jobs, or assembly orders depends on how your warehouse is set up as a location. Learn more at [Setting Up Warehouse Management](warehouse-setup-warehouse.md).

In a advanced warehouse configuration for the outbound flow (pick), turn on the **Require Pick** and **Require Shipment** toggles on the **Location Card** page for the location.

When the location is set up to require warehouse pick processing and warehouse shipment processing, use warehouse pick documents to create and process pick information before you post the usage or consumption of components.  

You can't create a warehouse pick document from scratch. Picks are part of a workflow where a person who is processing an order creates them in a push fashion, or the warehouse employee creates them in a pull fashion:

- In a push fashion, where you use the **Create Pick** action in the **Production Order**, **Assembly Order**, **Job Card** page. Select the lines to pick and prepare the picks by specifying, for example, which bins to take from and place in, and how many units to handle. Bins can be predefined for the warehouse location or resource.
- In a pull fashion, where you release **Production Order**, **Assembly Order**, **Job Card** to warehouse making the items available for picking. Then, on the **Pick Worksheet** page, warehouse employees can use the **Get Warehouse Documents** action to pull their assigned picks.

To pick or move components for source documents in a pull fashion, you must release the source document to make it ready for picking. Release source documents for internal operations in the following ways.  

|Source Document|Release Method|  
|---------------------|--------------------|  
|Production Order|Change the order status to Released or create a released production order right away.|  
|Assembly Order|Change status to Released.|
|Jobs | Change status to Open or create job with status Open right away.|  

## <a name="production" />Production

Use **Warehouse Pick** documents for picking production components in the flow to production.

For a location that uses bins to move items to open shop floor bins, you can use the following methods:

* For a location that uses directed put-away and pick, follow the steps in the [Move Items in advanced warehouse configurations](warehouse-how-to-move-items-in-advanced-warehousing.md) article.
* For other locations, follow the stapes in the [Move Items Unplanned in Basic Warehouse Configurations](warehouse-how-to-move-items-ad-hoc-in-basic-warehousing.md) article.

## <a name="assembly" />Assembly

Use **Warehouse Pick** documents to move assembly components to the assembly area.

[!INCLUDE [prod_short](includes/prod_short.md)] supports assemble-to-stock and assemble-to-order types of assembly flows. To learn more about assemble-to-order in the outbound warehouse flow, go to [Handling Assemble-to-Order Items in Warehouse Shipments](warehouse-how-ship-items.md#handling-assemble-to-order-items-in-warehouse-shipments).

## <a name="project-management" />Project management

Use **Warehouse Pick** documents to pick job components in the flow to project management.

> [!NOTE]
> The ability to pick components for job planning lines was added to [!INCLUDE[d365fin](includes/d365fin_md.md)] in 2022 release wave 2. To start using the capability, an administrator must turn on **Feature Update: Enable inventory and warehouse pick from Jobs** on the **Feature Management** page.
>
> Jobs don't support advanced configurations where the **Directed pick and Put-away** toggle is turned on.

## <a name="to-create-pick-documents-in-bulk-with-the-pick-worksheet" />To create pick documents in bulk with the pick worksheet

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Pick Worksheet**, and then choose the related link.  

2. Choose the **Get Warehouse Documents** action.  

    The list will show the released production, jobs, assembly orders that have been forwarded to the pick function. The orders include those for which pick instructions have already been created. Documents with pick lines that have been completely picked and registered are not shown on this list.  
3. Select the orders for which you want to prepare a pick.

    > [!NOTE]  
    > If you select a document that already has instructions for all its lines, [!INCLUDE [prod_short](includes/prod_short.md)] informs you that there is nothing to handle. To combine the already created warehouse pick instructions into one pick instruction, delete the individual warehouse picks first.

4. Fill in the **Sorting Method** field to sort the lines the way you prefer.  

    > [!NOTE]  
    > The way the lines are sorted in the worksheet doesn't automatically carry through to the pick instruction. However, the same sorting tools are available, along with bin ranking. You can easily recreate the order of the lines you plan in the worksheet when you create the pick instructions or by sorting in the pick instructions.

5. Fill in the **Qty. to Handle** field. Choose the **Autofill Qty.to Handle** action, or fill in the fields manually.  

    The page shows the quantities available in cross-dock bins, which is useful for planning work assignments in cross-docking situations. [!INCLUDE[prod_short](includes/prod_short.md)] will always propose a pick from a cross-dock bin first.

6. If needed, edit the lines manually. You can also delete some of the lines to make the pick more efficient. For example, if there are multiple lines with items that are in cross-dock bins, you might create a pick for all of the lines. The cross-docked items will be picked with the other items on the source document, and the cross-dock bins will have space for more incoming items.

    > [!NOTE]  
    >  The lines are only deleted from this worksheet, not from the pick selection list.  

7. Choose the **Create Pick** action. The **Create Pick** page opens, where you can add more information to the pick.  

    Specify how to combine pick lines in the pick documents by selecting one of the following options.  

    |Option|Description|
    |-|-|
    |Per Whse. Document|Creates separate pick documents for worksheet lines with the same warehouse source document.|
    |Per Cust./Vend./Loc.|Creates separate pick documents for each customer (jobs)|
    |Per Item|Creates separate pick documents for each item in the pick worksheet.|
    |Per From Zone|Creates separate pick documents for each zone that you'll take the items from.|
    |Per Bin|Creates separate pick documents for each bin that you'll take the items from.|
    |Per Due Date|Creates separate pick documents for source documents that have the same due date.|

    Specify how to create the pick documents by selecting from the following options.  

    |Option|Description|
    |-|-|
    |Max. No. of Pick Lines|Creates pick documents that have no more than the specified number of lines in each document.|
    |Max. No. of Pick Source Docs.|Creates pick documents that cover up to the specified number of source documents.|
    |Assigned User ID|Creates pick documents only for worksheet lines that are assigned to the selected warehouse employee.|
    |Sorting Method for Pick Lines|Select from the available options to sort lines in the created pick document.|
    |Set Breakbulk Filter|Hides intermediate breakbulk pick lines when a larger unit of measure is converted to a smaller unit of measure and completely picked.|
    |Do Not Fill Qty. to Handle|Leaves the **Qty. to Handle** field empty on the created pick lines.|
    |Print Pick|Prints the pick documents when they're created. You can also print from the created pick documents.|

8. Choose the **OK** button.  

## <a name="to-pick-items-for-a-productions-order-assembly-order-job" />To pick items for a productions order, assembly order, job

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Picks**, and then choose the related link.  

    If you need to work on a particular pick, select the pick from the list or filter the list to find the picks that have been assigned to you. Open the pick card.  
2. If the **Assigned User ID** field is empty, enter your ID to identify yourself, if needed.  
3. Pick the items.  

    If the warehouse is set up to use bins, the items’ default bins are used to suggest where to take the items from. The instructions contain at least two separate lines for Take and Place actions.  

    Operation areas such as production shop floors might have a default bin for the components they require. If so, the default bin code is added to the warehouse pick document to indicate where to put the items. For more information, refer to the tooltips for the **To-Production Bin Code**, the **To-Assembly Bin Code**, the **To-Job Bin Code** fields.

    If the warehouse is set up to use directed put-away and pick, the bin rankings are used to calculate the best bins to pick from. Those bins are suggested on the pick lines. The instructions contain at least two separate lines for Take and Place actions.  

    * The first line, with **Take** in the **Action Type** field, indicates where the items are located in the picking area. If you're shipping a large number of items on one shipment line, you might have to pick the items in several bins, so there's a Take line for each bin.
    * The next line, with **Place** in the **Action Type** field, shows where you must place the items in the warehouse. You can't change the zone and bin on this line.

    > [!NOTE]
    > If you must pick or place the items for one line in more than one bin, for example because the designated bin is full, use the **Split Line** action on the **Lines** FastTab. The action creates a line for the remaining quantity to handle.

4. After you pick and place the items in the production, assembly or job area or bin, choose the **Register Pick** action.  

    You can now bring the items to the respective area and post the usage or consumption of the picked components by posting consumption journal, assembly order, or job journal. The following articles provide more information:

    * [Register Consumption and Output for One Released Production order line](production-how-to-register-consumption-and-output.md)
    * [Assemble Items](assembly-how-to-assemble-items.md)
    * [Record Consumption or Usage for Jobs](projects-how-record-job-usage.md)

## <a name="flushing-production-components-in-a-advanced-warehouse-configuration" />Flushing production components in a advanced warehouse configuration

Flushing methods affect the flow of components in production. Learn more at [Flush Components According to Operation Output](production-how-to-flush-components-according-to-operation-output.md). Depending on the selected flushing method, you can pick components for production om the following ways:

* Use a **Warehouse Pick** document to record the pick for items that use the **Manual** flushing method. You'll need to register consumption separately. Learn more at [Batch Post Production Consumption](production-how-to-post-consumption.md).
* Use a **Warehouse Pick** document to record the pick for items that use the **Pick + Forward**, **Pick + Backward** flushing method. Consumption of the components will happen automatically either when you change the status of the production order or by starting or ending an operation. All required components must be available. Otherwise, posting flushed consumption stop for that component.
* Use a **Warehouse Movement** document without a reference to a source document or other ways to record the movement of components that use the **Forward** or **Backward** flushing method. Components are automatically consumed either when you change of status of the production order or start or end an operation. All required components must be available. Otherwise, posting flushed consumption stops for that component. Learn more at [Move Items](warehouse-move-items.md).

### <a name="example" />Example

You have a production order for 15 PCS of item SP-SCM1004. Some of the items on the component list must be flushed manually in a consumption journal. Other items can be picked and flushed automatically using the **Pick + Backward** flushing method.  

The following steps describe the actions that different people take and the related response:  

1. The shop floor supervisor releases the production order. Items with **Forward** flushing method and no routing link are deducted from the open shop floor bin.  
2. The shop floor supervisor chooses the **Create Warehouse Pick** action on the production order. A warehouse pick document is created pick for items with **Manual**, **Pick + Backward**, and **Pick + Forward** flushing methods. These items are placed in the To-Production bin.  
3. The warehouse manager assigns the picks to a warehouse employee.  
4. The warehouse employee picks the items from the appropriate bins and places them in the To-Production bin or in the bin specified on the warehouse pick. The bin may be a work centre or machine centre bin.
5. The warehouse employee registers the pick. The quantity is transferred from the pick bin to the consumption bin. The **Qty. Picked** field on the component list for all picked items is updated.

    > [!NOTE]  
    >  Only the quantity picked can be consumed.  
6. The machine operator informs the production manager that the end items are finished.
7. The shop floor supervisor uses the consumption journal or production journal to post the consumption of component items that use either **Manual** flushing method.
8. The shop floor supervisor uses the output journal or production journal to post the output. The quantity of component items that use **Pick + Forward** or **Pick + Backward** flushing methods with routing links is deducted from the To-Production bin.
9. The production manager changes the status of the production order to **Finished**. The quantity of component items that use **Backward** flushing method is deducted from the open shop floor bin, and the quantity of component items that use **Pick + Backward** flushing method and no routing link is deducted from the To-Production bin.  

The following illustration shows when the **Bin Code** field on the component list is filled according to your location or machine/work centre setup.  

:::image type="content" source="media/binflow.png" alt-text="Overview of when and how the Bin Code field is filled in.":::

## <a name="see-related-microsoft-trainingtrainingpathspick-ship-items-business-central" />See related [Microsoft training](/training/paths/pick-ship-items-business-central/)

## <a name="see-also" />See also

[Inventory](inventory-manage-inventory.md)  
[Setting Up Warehouse Management](warehouse-setup-warehouse.md)  
[Assembly Management](assembly-assemble-items.md)  
[Warehouse Management Overview](design-details-warehouse-management.md)
[Work with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]
