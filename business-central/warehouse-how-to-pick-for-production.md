---
title: 'Pick or Move Items for Production, Assembly, or Jobs in Basic Warehouse Configurations'
description: 'When your warehouse location requires that you process picks but not shipments, use the Inventory Pick page to record that components were picked.'
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bholtorf
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.date: 12/16/2022
ms.custom: bap-template
ms.search.forms: '9330, 931, 990008, 89, 900, 902'
---
# <a name="pick-for-production-assembly-or-jobs-in-basic-warehouse-configurations"></a>Pick for Production, Assembly, or Jobs in Basic Warehouse Configurations

How you pick components for production, jobs, or assembly orders depends on how your warehouse is set up as a location. Learn more at [Setting Up Warehouse Management](warehouse-setup-warehouse.md).

In a basic warehouse configuration for the outbound flow (pick), on the **Location Card** page for the location, turn on the **Require Pick** toggle but turn off the **Require Shipment** toggle.

Use the following documents for internal operations:

* Inventory Pick
* Inventory Movement

## <a name="inventory-picks"></a>Inventory picks

* When you register an inventory pick for an internal operation, such as production or a job, the consumption of the picked components is posted at the same time.
* The **Bin Mandatory** toggle on the **Location Card** page is optional.
* When you use inventory picks, the **Bin Code** field on a production order component line or job planning lines defines the *take* bin. Components are decreased in the take bin when you post consumption.

## <a name="inventory-movements"></a>Inventory movements

* Inventory movements require that you turn on the **Bin Mandatory** toggle on the **Location Card** page for the location.
* Inventory movements only work with production order component lines and assembly order lines.
* When you register an inventory movement for an internal operation, you only record the physical movement of the components to a bin in the operation area. You don't post consumption.
* When you use inventory movements, the **Bin Code** field on production order component lines defines the *place* bin in the operation area. The place bin is where warehouse employees must place the components.
* Register the consumption of the picked components separately by posting a consumption journal or assembly order.

>[!NOTE]
> Even if the **Require Pick** toggle is turned off, you can use a **Warehouse Pick** document. Warehouse pick documents are similar to **Inventory Pick** documents. This is useful if you want to use picks in operations and ship in outbound warehouse flows.

### <a name="production"></a>Production

Use **Inventory Pick** documents for picking production components in the flow to production.

For a location that uses bins, you can extend the flow to production by using **Inventory Movement** documents. Inventory movements are especially useful for component flushing. To learn more about how component consumption is flushed from the To-Production or Open Shop Floor Bins, go to [Flushing Production Components in a Basic Warehouse Configuration](#flushing-production-components-in-a-basic-warehouse-configuration).

### <a name="assembly"></a>Assembly

Use **Inventory Movement** documents to move assembly components to the assembly area.

> [!NOTE]
> **Inventory Movement** documents require bins.

[!INCLUDE [prod_short](includes/prod_short.md)] supports assemble-to-stock and assemble-to-order types of assembly flows. To learn more about assemble-to-order in the outbound warehouse flow, go to [Handling Assemble-to-Order Items with Inventory Picks](warehouse-how-to-pick-items-with-inventory-picks.md#handling-assemble-to-order-items-with-inventory-picks).

### <a name="project-management"></a>Project management

Use **Inventory Pick** documents to pick job components in the flow to project management.

For locations that use bins, you can extend the flow to jobs with **Inventory Movement** documents.

> [!NOTE]
> The ability to pick components for job planning lines was added to [!INCLUDE[d365fin](includes/d365fin_md.md)] in 2022 release wave 2. To start using the capability, an administrator must turn on **Feature Update: Enable inventory and warehouse pick from Jobs** on the **Feature Management** page.
>
> [!INCLUDE[prod_short](includes/prod_short.md)] uses the value in the **Remaining Quantity** field on the job planning line when it creates inventory picks. To use inventory picks for jobs, you must turn on the **Apply Usage Link** toggle on the **Job Card** page for the job. This lets you track usage against your plan. If you don't turn on the toggle, the remaining quantity will stay at **0** and the inventory pick won't be created. Learn more at [To set up job usage tracking](projects-how-setup-jobs.md?tabs=current-experience#to-set-up-job-usage-tracking).

## <a name="pick-or-move-for-production-assembly-and-jobs-in-a-basic-warehouse-configuration"></a>Pick or move for production, assembly, and jobs in a basic warehouse configuration

You can create an inventory pick or inventory movement in three ways:  

* From the source document itself.  
* For several source documents at the same time by using a batch job.  
* In two steps. Release the source document to make the source document ready for picking. Create the inventory pick or movement from the **Inventory Pick** or **Inventory Movement** documents. The inventory pick or movement are based on the source document.  

### <a name="to-create-an-inventory-pick-from-the-source-document"></a>To create an inventory pick from the source document

1. On the source document, which can be a production order or job, choose the **Create Inventory Put-away/Pick** action.  
2. Select the **Create Invt. Pick** checkbox.
3. Choose the **OK** button.

### <a name="to-create-an-inventory-movement-from-the-source-document"></a>To create an inventory movement from the source document

1. On the source document, which can be a production order, assembly order, or job, choose the **Create Inventory Put-away/Pick** action.  
2. Select the **Create Invt. Movement** checkbox.
3. Choose the **OK** button.

### <a name="to-create-multiple-inventory-picks-or-movements-with-a-batch-job"></a>To create multiple inventory picks or movements with a batch job

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Create Inventory Put-away/Pick/Movement**, and then choose the related link.  
2. On the **Warehouse Request** FastTab, use the **Source Document** and **Source No.** fields to filter on types of documents or ranges of document numbers. For example, you might create picks only for productions orders.
3. On the **Options** FastTab, turn on the **Create Invt. Pick** or **Create Invt. Movement** toggles.
4. Choose the **OK** button.

### <a name="to-create-inventory-picks-or-movements-in-two-steps"></a>To create inventory picks or movements in two steps

To pick or move components for source documents in two steps, you must release the source document to make it ready for picking. Release source documents for internal operations in the following ways.  

|Source Document|Release Method|  
|---------------------|--------------------|  
|Production Order|On the **Planned Production Order** page, change the status of an order to **Released**, or use the **Released Production Order** page to create a released production order.|  
|Assembly Order|Change status of an assembly order to **Released**.|
|Jobs | Change a job's status to **Open**, or create job with status Open right away.|  

A warehouse employee assigned to picking items can create an inventory put-away document for the source document.  

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Inventory Picks** or **Inventory Movement**, and then choose the related link.  
2. Choose the **New** action.  
3. In the **Source Document** field, select the type of source document that the put-away is for.

    > [!NOTE]
    > You can't use **Inventory Pick** documents for picking assembly components.
4. In the **Source No.** field, select the source document.  
5. Alternatively, choose the **Get Source Document** action to select the document from a list of inbound source documents that are ready for picking at the location.  
6. Choose the **OK** button to fill the pick or movement lines according to the selected source document.  

## <a name="to-record-the-inventory-pick"></a>To record the inventory pick

1. On the **Inventory Pick** page, open the document to record a pick for.  
2. In the **Bin Code** field on the pick lines, the bin where the items must be picked from the bin where the item is available. You can change the bin if needed.
3. Perform the pick, and then enter the pick quantity in the **Qty. to Handle** field.

    If you must pick the items for a line from more than one bin, for example because a bin doesn't contain the full quantity, use the **Split Line** action on the **Lines** FastTab. The action creates a line for the remaining quantity to handle.  
4. Choose the **Post** action.  

The following happens during the posting process:

* Post the consumption of the source document lines that were picked.
* If the location uses bins, posting will create warehouse entries to post the changes to the bin quantity.

[!INCLUDE [preview-posting-warehouse](includes/preview-posting-warehouse.md)]

## <a name="to-record-the-inventory-movement"></a>To record the inventory movement

1. On the **Inventory Movement** page, open the document to record a movement for.  
2. In the **Bin Code** field on the movement lines, the bin to pick from is suggested based on the item's default bin and availability. You can change the bin if needed.  
3. Perform the move, and then enter the moved quantity in the **Qty. to Handle** field. The value on the Take and the Place lines must be the same. Otherwise, you can't register the movement.

    If you must take the items for a line from more than one bin, for example because a bin doesn't contain the full quantity, use the **Split Line** action on the **Lines** FastTab. The action creates a line for the remaining quantity to handle.  
4. Choose the **Register Invt. Movement** action.  

The following happens during the posting process:

* Warehouse entries now indicate that the components are in the bins specified on the source document order lines. For example, the assembly order, production component, or job planning line.

>[!NOTE]
> Unlike when you move components with inventory picks, consumption isn't posted when you register an inventory movement. You register consumption as a separate step by posting the source document.

## <a name="flushing-production-components-in-a-basic-warehouse-configuration"></a>Flushing production components in a basic warehouse configuration

Flushing methods affect the flow of components in production. Learn more at [Flush Components According to Operation Output](production-how-to-flush-components-according-to-operation-output.md). Depending on the flushing method you select, you can pick components for production om the following ways:

* Use an **Inventory Pick** document to record the pick for items that use the **Manual** flushing method. When you register an inventory pick, the consumption of the picked components is posted. 
* Use an **Inventory Movement** document with a reference to a source document to record picks for components that use the **Manual** flushing method. You'll need to register consumption separately. Learn more at [Batch Post Production Consumption](production-how-to-post-consumption.md). 
* Use an **Inventory Movement** document with a reference to a source document to record picks for components that use the **Pick + Forward**, **Pick + Backward** flushing method. Consumption of the components will happen automatically either when you change the status of the production order or by starting or ending an operation. All required components must be available. Otherwise, posting flushed consumption stop for that component.
* Use an **Inventory Movement** document without a reference to a source document or other ways to record the movement of components that use the **Forward** or **Backward** flushing method. Consumption of the components will happen automatically either when you change of status of the production order or start or end an operation. All required components must be available. Otherwise, posting flushed consumption stops for that component. Learn more at [Move Items Internally in Basic Warehouse Configurations](warehouse-how-to-move-items-ad-hoc-in-basic-warehousing.md).

### <a name="example"></a>Example

You have a production order for 15 PCS of item SP-SCM1004. Some of the items on the component list must be flushed manually in a consumption journal, and other items can be picked and flushed automatically using the **Pick + Backward** flushing method.  

The following steps provide an example of the actions that different people take and the related responses:  

1. The shop floor supervisor releases the production order. Items with **Forward** flushing method and no routing link are deducted from the open shop floor bin.  
2. The shop floor supervisor chooses the **Create Inventory Put-away/Pick** action on the production order and turns on the **Create Invt. Pick** and **Create Invt. Movement** toggles. An inventory pick document is created for items with **Manual** flushing method, and an inventory movement is created for items with **Pick + Backward** and **Pick + Forward** flushing methods.
3. The warehouse manager assigns the picks and movements to a warehouse employee.
4. The warehouse employee picks the items from the appropriate bins and places them in the To-Production bin or in the bin specified on the inventory movement. The bin can be a work centre or machine centre bin.  
5. The warehouse employee posts the pick. The quantity is deducted from the bins.
6. The warehouse employee posts the movement. The quantity is deducted from the pick bins and added to the consumption bin. The **Qty. Picked** field on the component list for all picked items is updated.  
7. The machine operator informs the production manager that the end items are finished.  
8. The shop floor supervisor uses the output journal or production journal to post the output. The quantity of component items that use **Pick + Forward** or **Pick + Backward** flushing methods with routing links is deducted from the To-Production bin.
9. The production manager changes the status of the production order to **Finished**. The quantity of component items that use **Backward** flushing method is deducted from the open shop floor bin, and the quantity of component items that use **Pick + Backward** flushing method and no routing link is deducted from the To-Production bin.  

 The following illustration shows when the **Bin Code** field on the component list is filled according to your location or machine/work centre setup.  

:::image type="content" source="media/binflow.png" alt-text="Overview of when and how the Bin Code field is filled in.":::

## <a name="see-related-microsoft-training"></a>See related [Microsoft training](/training/paths/pick-ship-items-business-central/)

## <a name="see-also"></a>See also

[Inventory](inventory-manage-inventory.md)  
[Setting Up Warehouse Management](warehouse-setup-warehouse.md)  
[Assembly Management](assembly-assemble-items.md)  
[Warehouse Management Overview](design-details-warehouse-management.md)
[Work with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]
