---
title: Amazon fulfillment workflows
description: Fulfillment for an order from an Amazon listing follows a specific sequence from order submission to shipping.
exl-id: 30dd9f97-9193-4c98-bded-e5d8d35b0d05
---
# Amazon fulfillment workflows

## Example: fulfilled by merchant

|Step | Description |
|----|----|
|1| **A merchant-fulfilled order is placed on Amazon.** Amazon assigns a status of `Pending` until the customer's credit card information is verified. Orders in `Pending` status automatically import into Amazon sales channel but do not display on the _[!UICONTROL Orders]_ tab.|
|2| **The order is verified by Amazon.** When verified, Amazon changes the status to `Unshipped`. With this status change, the order is updated in Amazon sales channel and appears in the _[!UICONTROL Orders]_ tab.|
|3| **The order details are updated.** Amazon sales channel updates the order details with the price, customer email, and customer name. During this update, the Amazon order creates the corresponding [!DNL Commerce] order in the order management page. The [!DNL Commerce] order number is displayed with the order information on the _[!UICONTROL Orders]_ tab.|
|4| **A new customer account is created.** If configured in your order settings and the customer does not exist in your [!DNL Commerce] database, a new customer is created in your [!DNL Commerce] database using the corresponding customer information from the Amazon order. If you chose `No Customer Creation (guest)` in your order settings, the order follows the [!DNL Commerce] guest process and not create a customer in your database. At this point, if your [!DNL Commerce] system is integrated with an ERP/OMS/WMS, the order is picked up per the integration of a new order being placed and created inside [!DNL Commerce].|
|5| **The order is shipped.** From the [!DNL Commerce] order processing page, you ship the order and add a tracking number. When all items are marked in a `Shipped` status:<ul><li>The status of the [!DNL Commerce] order changes to `Complete`.</li><li>The status of the Amazon sales channel order changes to `Shipped`.</li><li>The tracking number is synced to Amazon, and the status of the order in Amazon changes to `Shipped`.</li><li>Shipping notifications are sent to the customer via Amazon, not from [!DNL Commerce] (per Amazon's policies).|

## Example: fulfilled by Amazon (FBA)

|Step | Description |
|---|---|
|1| **An Amazon-fulfilled order is placed on Amazon.** |
|2| **The order is imported.** The order is not imported into Amazon sales channel until the order is assigned the `Shipped` status by Amazon. Since Amazon has the inventory for this product, it prevents interference with your warehouse/inventory management. |
|3| **The order details are updated.** If configured in your [order settings](./order-settings.md), the Amazon order creates the corresponding [!DNL Commerce] order and be created as an order with a status of `Complete`. |
