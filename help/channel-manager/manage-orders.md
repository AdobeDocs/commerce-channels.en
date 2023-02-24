---
title: 'View and Manage Orders from [!DNL Channel Manager]'
description: 'View and manage [!DNL Walmart Marketplace] orders with [!DNL Channel Manager] for Adobe Commerce and Magento Open Source.'
exl-id: c2779c72-4793-445c-858a-867ea8389662
---
# View and Track Orders from [!DNL Channel Manager]

[!DNL Walmart Marketplace] order data for [!DNL Commerce] products synchronizes automatically to [!DNL Channel Manager] after [!DNL Walmart] processes the order.

On the [!DNL Commerce] side, a successful synchronization triggers the following actions:

- [!DNL Channel Manager] sends an order acknowledgment to Walmart.

- A corresponding [!DNL Commerce] order is created from the Walmart order.

- The updated order information displays on the [!DNL Channel Manager] Orders dashboard.

In the storefront Admin, you can view order data from [!DNL Channel Manager] by opening the sales channel store and selecting **[!UICONTROL Orders]**.

![Channel Manager Orders view to manage [!DNL Walmart Marketplace] orders](assets/orders-dashboard-view.png)

>[!NOTE]
>
>It can take up to 35 minutes for a [!DNL Walmart Marketplace] order to display in the [!DNL Channel Manager] orders list. [!DNL Walmart] requires approximately 30 minutes to process incoming orders and send them to [!DNL Channel Manager]. After Channel Manager receives the order, it takes approximately five more minutes to create and display the order in Adobe Commerce or Magento Open Source.

## Orders Controls and Column Descriptions

The following tables describe the controls and columns available for Orders.

**Controls for [!UICONTROL Orders]**

<table>
<tr>
<td><strong>Control</strong></td>
<td><strong>Description</strong></td>
</tr>
<tr>
<td>[!UICONTROL Filter orders]</td>
<td>Sort the view by selecting one of the [!UICONTROL Order Status] cards.</td>
</tr>
<tr>
<td>Status Details</td>
<td>Provides information about order errors and return requests. To view return information and refund status for an order, select the <strong>[!UICONTROL Return requested]</strong> text to open the [!UICONTROL Returns] dashboard.</td>
</tr>
<tr>
<td>[!UICONTROL View order detail]</td>
<td>To view order details, select the [!DNL Commerce] order number in the [!UICONTROL Order] table. Then, use [!DNL Commerce] order options to process the order.</td>
</tr>
<tr>
<td>[!UICONTROL Channel Settings]</td>
<td>To modify the channel configuration, select channel Walmart Connection credentials, mapped attributes, or shipping identifiers, settings  select the [!DNL Commerce] order number in the [!UICONTROL Order] table. Then, use [!DNL Commerce] order options to process the order.</td>
</tr>
</table>


**Column descriptions**

<table>
<tr>
<td>Field</td>
<td>Description</td>
</tr>
<tr>
<td>[!UICONTROL Walmart Order #]</td>
<td>The purchase order number assigned to the order in the [!DNL Walmart Marketplace]. When an order is initially imported to [!DNL Channel Manager], only the [!DNL Walmart] order number displays. When the [!DNL Commerce] order is created, the [!DNL Walmart] order number is stored in the [!UICONTROL External ID] product attribute.</td>
</tr>
<tr>
<td>[!DNL Commerce] Order #</td>
<td>The number assigned to the [!DNL Commerce] order created from the [!DNL Walmart Marketplace] order.</td>
</tr>
<tr>
<td>Items</td>
<td>Number of items ordered on [!DNL Walmart Marketplace].</td>
</tr>
<tr>
<td>[!UICONTROL Order Value]</td>
<td>Total cost of the ordered items.</td>
</tr>
<tr>
<td>[!UICONTROL Ordered]</td>
<td>The date the order was submitted to the [!DNL Walmart Marketplace] converted to the local timezone.</td>
</tr>
<tr>
<td>[!UICONTROL Ship By (timezone)]</td>
<td>The date the order must be shipped by to meet [!DNL Walmart Marketplace] requirements converted to the local timezone.
</td>
</tr>
<tr>
<td>[!UICONTROL Deliver By (timezone)]</td>
<td>The date the order must be delivered to customer to meet [!DNL Walmart Marketplace] requirements converted to the local timezone.</td>
</tr>
<tr>
<td>[!UICONTROL Ship Method]</td>
<td>The [[!DNL Walmart Marketplace] Shipping Method](https://sellerhelp.walmart.com/s/guide?language=en_US&article=000007893%29 selected for the order.</td>
</tr>
<tr>
<td>[!UICONTROL Last Update]</td>
<td>Timestamp indicating the last time the order data was updated in [!DNL Channel Manager] converted to local time zone.</td>
</tr>
<tr>
<td>[!UICONTROL Status]</td>
<td>Indicates the current order status in the [!DNL Commerce] order workflow. The initial status for an order imported from [!DNL Walmart Marketplace] is _Open_. Additional status updates occur when [!DNL Commerce] orders are processed and [!DNL Channel Manager] successfully synchronizes shipment, partial shipment, and cancellation updates to the [!DNL Walmart Marketplace].</td>
</tr>
<tr>
<td>[!UICONTROL Status Details]</td>
<td>Provides more detailed information about orders with errors or refund requests.</td>
</tr>
</table>

## Order Status

[!UICONTROL Order Status] provides information about the current state of [!DNL Walmart Marketplace] orders managed from Adobe Commerce or Magento Open Source. Order status updates occur when [!DNL Channel Manager] receives updated order information from either the [!DNL Walmart Marketplace] or the [!DNL Commerce] order system. Orders can have the following statuses:           

- **[!UICONTROL Shipped]**—Orders that have been shipped from the [!DNL Commerce] store. When the order ships, [!DNL Channel Manager] sends an update to [!DNL Walmart Marketplace] to update the shipping status on Walmart and provide the order tracking number for the shipment. After an order has been shipped, order items can be partially or fully refunded if Walmart issues a Return Merchandise Authorization form. See [Returns and Refunds](return-refund-orders.md).

- **[!UICONTROL Partially Shipped]**—Orders that have some items marked as shipped, and others waiting to be shipped. When items in the order ship, [!DNL Channel Manager] sends an update to [!DNL Walmart Marketplace] to update the shipping status to _[!DNL Partially Shipped]_ on Walmart and provide the order tracking number for the shipment. 

- **[!UICONTROL Canceled]**—Orders that have been canceled from the [!DNL Commerce] store.

  After the order cancellation completes, the [!DNL Commerce] stock quantity updates to reflect returned items. Then, [!DNL Channel Manager] syncs the update to the [!DNL Walmart Marketplace].

- **[!UICONTROL Return requested]**—If Walmart Marketplace requests a return for order items that have been shipped, a `Return requested` link displays in the [!UICONTROL Status details] column. Selecting the link opens the [!UICONTROL Returns] dashboard to view the return and manage the refund process.

- **[!UICONTROL Error]**—Orders that have errors. Errors can occur when an order update operation fails. For example, errors occur if [!DNL Channel Manager] cannot receive a new order from Walmart. They can also occur if [!DNL Channel Manager] cannot send an order shipment or cancellation update to the [!DNL Walmart Marketplace]. If an operation fails, the Orders page shows an _Error_ status for the order. For details, see [Fix order errors](process-orders.md#fix-shipping-and-cancellation- errors). 

- **[!UICONTROL Status details]**–Provides more information about order errors that occur due to issues like missing information or invalid values, incorrect shipment details, or a failed order cancellation. The description helps determine whether error occurred on the [!DNL Commerce] instance or on the [!DNL Walmart Marketplace].

>[!NOTE]
>
>If order items are sent in multiple shipments, the order status in [!DNL Channel Manager] reflects the last order status available. For example, if the first item ships and no errors are returned when order updates are synchronized to [!DNL Channel Manager] and [!DNL Walmart Marketplace], the [!DNL Channel Manager] order status is _[!UICONTROL Partially Shipped]_. If a second item is shipped and [!DNL Channel Manager] returns an error, the order status updates to _[!UICONTROL Error]_.

## Review Orders

1. From the Admin, select **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]** to open the [!UICONTROL Channel Manager Marketplace Stores] page.

1. Open the store view by selecting the eye icon in a store entry row.

1. To view order information, select *[!UICONTROL *Orders]**.

1. Get information about the order and determine next steps by checking the **[Status](#order-status)** column.

## Review Order Detail

After an order is received from the marketplace and imported into your sales channel store, use the [!DNL Commerce] Order ID to view the order detail in Adobe Commerce.

From **[!UICONTROL Orders]**, select the **[!UICONTROL Commerce Order Number]** to open the [!DNL Commerce] order detail.

![Commerce Order detail view for a [!DNL Walmart Marketplace] order](assets/order-detail-with-external-order-id.png)

In the Commerce storefront, orders imported from [!DNL Walmart Marketplace] have the following additional information included in the order data:

- **Payment Information & Shipping Method**–Orders imported from Walmart include following values for payment and shipping fields:

  - **[!UICONTROL Offline Channel Payment]**—Indicates that order payment is processed offline by [!DNL Walmart Marketplace].

  - **[!UICONTROL External Order Number]**—Displays the [!DNL Walmart Marketplace] order number.

  - **[!UICONTROL Channel Shipping - Value]**–Indicates that shipping charges are handled through [!DNL Walmart Marketplace].

  - **[!UICONTROL Cancellation Reason]**–This field displays only if an order imported from [!DNL Walmart Marketplace] is canceled. Cancellation reasons include:

    - [!UICONTROL Price or other listing errors.]
    - [!UICONTROL The item is out of stock.]
    - [!UICONTROL Unavailable carrier or shipping information.]
    - [!UICONTROL Additional information is required by our Credit or Fraud Avoidance department.]

- **Items Ordered**—This section lists the order items on all Commerce orders. The [!UICONTROL Qty] column provides the status history for order items. For example if an order has been invoiced, shipped, and refunded, you can see the status transitions.

  ![Order Detail ordered item status history [!DNL Walmart Marketplace] orders](assets/order-detail-status-history.png)

 View item invoice and refund details by selecting the [!UICONTROL Invoice] and [!UICONTROL Credit Memo] options from the navigation menu. You can also access the Credit Memo directly from the [[!UICONTROL Returns]](return-refund-orders.md) dashboard in your sales channel store.
