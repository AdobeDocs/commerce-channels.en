---
title: Process Orders
description: 'Instructions for shipping and cancelling [!DNL Walmart Marketplace] orders from Adobe Commerce and Magento Open Source.'
feature: Sales Channelss, Orders, Shipping/Delivery, Customer Service
exl-id: 2fdcb348-5c02-464f-a114-16ec657bed6b
---
# Process Orders

After [!DNL Walmart Marketplace] orders have been acknowledged and successfully sent to [!DNL Channel Manager], you use [Commerce Order Management](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html#orders-workspace) to process the order.

Channel Manager synchronizes updates to [!DNL Walmart Marketplace] to ensure that the order status and shipping information from [!DNL Commerce] matches the data tracked in the [!DNL Walmart Marketplace].

* **Order shipments**–Walmart requires a tracking number for all shipments. If some items are out of stock, you can create partial shipments to send items that are currently available. After you submit the shipment, order updates are synchronized to [!DNL Walmart Marketplace]. Then, Walmart notifies customers about the order status and shipping details.

* **Order cancellations**–When you cancel a [!DNL Walmart Marketplace] order, Walmart requires a cancellation reason which is included in the order cancellation notice sent to the customer. The cancellation reason is also displayed in the [!DNL Commerce] order payments information. After you submit the cancellation, inventory updates are synchronized to [!DNL Walmart Marketplace]. Then, Walmart notifies customers about the order status and shipping details.

  In the storefront, you must cancel the entire order. [!DNL Commerce] does not allow partial cancellations.

* **Refund request**–If a Walmart Marketplace return is requested for a shipped order, the [!UICONTROL Status details] includes a link to the return. Returns and refunds are managed from the [Returns](return-refund-orders.md) dashboard.

When Commerce orders are processed and [!DNL Channel Manager] successfully synchronizes shipment, partial shipment, and cancellation updates to the [!DNL Walmart Marketplace], the order processing is complete. Return requests and refunds for shipped orders are managed from the [Returns](return-refund-orders.md) dashboard.

>[!NOTE]
>
> It can take up to five minutes for order updates to synchronize to [!DNL Walmart Marketplace]. To check the order status, return to the [!DNL Channel Manager] Orders page.

## Ship an order

1. From the Admin, select **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]**.

1. Open the store view by selecting the eye icon for a sales channel store.

1. To view [!DNL Walmart Marketplace] orders, select **[!UICONTROL Orders]**.

1. In the Orders table, open the order to ship by selecting the **[!UICONTROL Commerce Order Number]**.

1. Create and submit a shipment for all or part of an order by selecting **[!UICONTROL Ship]**.

   ![Commerce Order detail view for a [!DNL Walmart Marketplace] order](assets/order-detail-with-external-order-id.png){width="600" zoomable="yes"}

   * Choose a shipping carrier and add a tracking number by selecting **[!UICONTROL Add tracking number]**.

     ![Commerce Order detail view for a [!DNL Walmart Marketplace] order](assets/order-shipment-add-tracking-number.png){width="600" zoomable="yes"}

   * Complete the rest of shipping form as needed. See [[!DNL Shipping an Order]](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-ship.html) for detailed instructions.

1. After submitting the shipment, track the [order status](manage-orders.md#about-order-status) in [!DNL Channel Manager] to verify that updates were sent to [!DNL Walmart Marketplace].

After an order is shipped, you can process full or partial refunds from [!DNL Channel Manager] for items included in the order based on return requests received from [!DNL Walmart Marketplace]. See [Return and refund orders](return-refund-orders.md).

## Cancel an order

1. From the Admin, select **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]**.

1. Open the store view by selecting the eye icon for a sale channel store.

1. To view [!DNL Walmart Marketplace] orders, select *[!UICONTROL Orders]**.

1. In the Orders table, open the [order detail page](manage-orders.md#view-order-detail) by selecting the **[!UICONTROL Commerce Order Number]** for the order to cancel.

   ![Commerce Order detail view for a[!DNL Walmart Marketplace]order](assets/order-detail-with-external-order-id.png){width="600" zoomable="yes"}

1. Cancel the order.

   * Select **Cancel** from the Order Detail menu.

   * On the [!UICONTROL Cancel Order] form, select the **[!UICONTROL Cancellation reason]**.

   ![Commerce Order detail view for a [!DNL Walmart Marketplace] order](assets/cancel-order-reason-selector.png){width="600" zoomable="yes"}

   * Select **[!UICONTROL Cancel Order]**.

1. After submitting the cancellation, track the [order status](manage-orders.md#about-order-status) in [!DNL Channel Manager] to verify that updates were sent to [!DNL Walmart Marketplace].

## Fix order errors

Errors can occur during the order synchronization process from [!DNL Walmart Marketplace], or during the order update process for shipments, partial shipments, and cancellations.

If the synchronization operation for a shipment, partial shipment, or cancellation update fails, the [!DNL Channel Manager] Orders page shows an _Error_ status for the order. To ensure that shipment information and order cancellation information is accurately reflected in Walmart Marketplace account, manually update the order in your [!DNL Walmart Marketplace] store.


