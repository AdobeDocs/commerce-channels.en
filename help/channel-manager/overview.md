---
title: 'Introduction to [!DNL Channel Manager]'
description: 'Learn how to install and use [!DNL Channel Manager] to integrate Adobe Commerce and Magento Open Source stores with the Walmart Marketplace and create a sales channel to manage marketplace listings, pricing, inventory, and sales seamlessly from your Commerce Admin.'
role: User
level: Intermediate
exl-id: 91265973-d2ad-4925-aa10-260d7e186f20
---

# Introduction to [!DNL Channel Manager]

[!DNL Channel Manager] helps merchants increase sales, reach new customers, streamline sales operations, and save time by integrating an Adobe Commerce or Magento Open Source product catalog with the [!DNL Walmart Marketplace].

![[!DNL Channel Manager] extension Admin view](assets/channel-manager-home.png)

[!DNL Channel Manager] supports Adobe Commerce or Magento Open Source merchants who want to sell on [!DNL Walmart Marketplace] by extending the [!DNL Commerce] Admin. With [!DNL Channel Manager] installed, store administrators and operations staff can manage [!DNL Walmart Marketplace] sales, inventory, and product pricing seamlessly from the Commerce environment.

The extended Admin streamlines operations because merchants can use the same workflows and processes to manage sales from both [!DNL Commerce] storefronts and the Walmart Marketplace.

After you install and configure [!DNL Channel Manager], you can use the following capabilities to manage Walmart Marketplace sales orders:

* **Listing management**–Easily connect product listings by matching products from your [!DNL Commerce] catalog to existing [!DNL Walmart Marketplace] listings.

* **Inventory management**–Items in the merchant's marketplace seller account are automatically synchronized and updated from [!DNL Commerce] to ensure accurate inventory levels.

* **Pricing updates**—Maintain accurate pricing for marketplace listings with automatic price synchronization. When a price changes in Adobe Commerce, the changes are reflected in the marketplace.

* **Order management**—When new orders are created in the marketplace, [!DNL Channel Manager] synchronizes orders with Adobe Commerce, and sends order acknowledgments to the marketplace. This acknowledgment ensures that inventory is reserved for each order. The final step is to create the corresponding orders in the [!DNL Commerce] Order Management system for processing.

* **Shipping management**—When orders are marked as shipped in Adobe Commerce, the shipment update is sent to the [!DNL Walmart Marketplace]. This notification ensures that sellers meet their fulfillment SLA requirements and that customers receive shipping update notifications for their current orders.

* **Cancellations**—When orders are canceled in Adobe Commerce, [!DNL Channel Manager] sends updated order information to the marketplace to replicate the action for the corresponding marketplace order. After the order cancellation completes, the [!DNL Commerce] stock quantity updates to reflect returned items and inventory updates are synchronized automatically to [!DNL Walmart Marketplace].

* **Returns and Refunds**—When Walmart Marketplace requests a return for items ordered through the Adobe Commerce or Magento Open Source sales channel, [!DNL Channel Manager] sends the return request information to the Commerce sales channel store to replicate the return request. Then, the refund can be processed using the [!DNL Commerce] [refund workflow](https://docs.magento.com/user-guide/sales/credit-memos.html#refund-workflow), offline method. After the refund completes, [!DNL Channel Manager] synchronizes the update to Walmart so that the return status in the marketplace seller account can be updated to reflect the refund.

## Expected latency for [!DNL Channel Manager] operations

The data synchronization processes between [!DNL Channel Manager] and a linked [!DNL Walmart Marketplace] store require some time to complete. Review the expected processing time for [!DNL Channel Manager] operations to help plan sales channel operations work.

**Estimated latency for [!DNL Channel Manager] operations**

| **Operation**                                              | **Description**                                                                                                                                                                                                                                                                                                                                                                                  | **Expected delay**                                                                                                           |
|------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------|
| Add products to [!DNL Channel Manager]                     | Select products from the [!DNL Commerce] product catalog and import them into [!DNL Channel Manager].                                                                                                                                                                                                                                                                                            | **Up to five minutes**–If you select many products, for example, an entire product catalog, the import process takes longer. |
| Match products on [!DNL Walmart Marketplace]               | Select product listings in [!DNL Channel Manager] and send to Walmart for matching.                                                                                                                                                                                                                                                                                                              | **Up to 30 minutes**–If you select many products, the matching process takes longer depending on the quantity selected.      |
| Inventory updates                                          | When inventory quantity changes in Commerce, [!DNL Channel Manager] syncs the update to Walmart.                                                                                                                                                                                                                                                                                                 | **Up to 10 minutes**                                                                                                         |
| Price updates                                              | When a product price changes, [!DNL Channel Manager] syncs the update to Walmart.                                                                                                                                                                                                                                                                                                                | **Up to five minutes**                                                                                                       |
| Order syncs from Walmart to [!DNL Commerce]                | Customer orders a [!DNL Commerce] product on the Walmart Marketplace. Walmart sends the order to [!DNL Channel Manager]. Order displays in order dashboard.                                                                                                                                                                                                                                      | **Up to 30 minutes**                                                                                                         |
| Order created in [!DNL Commerce] Order Management          | [!DNL Channel Manager] creates the [!DNL Commerce] order from the Walmart order and updates the order dashboard to include the [!DNL Commerce] order number.                                                                                                                                                                                                                                     | **Up to five minutes**                                                                                                       |
| Shipping status update in [!DNL Commerce] Order Management | When an order is shipped from Commerce, [!DNL Channel Manager] updates the Shipping status in the order dashboard and send the update to Walmart marketplace so that the customer can be notified.                                                                                                                                                                                               | **Up to five minutes**                                                                                                       |
| Order cancellation update in Commerce Order Management     | When an order is canceled from Commerce, [!DNL Channel Manager] updates the order status in the order dashboard and sends the update to Walmart marketplace so that the customer can be notified. After the order cancellation completes, the [!DNL Commerce] stock quantity updates to reflect returned items. Then, [!DNL Channel Manager] syncs the update to the [!DNL Walmart Marketplace]. | **Up to five minutes**                                                                                                       |


