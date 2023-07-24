---
title: Amazon order settings
description: Use the Order settings to determine how Amazon orders are imported into and processed in your Commerce store.
feature: Sales Channels, Orders, Configuration
exl-id: dc8d0ce1-86a8-4949-b49a-73c5cf62db16
---
# Amazon order settings

Order settings define if and how Amazon orders are imported into and processed in [!DNL Commerce] and can be accessed on the [store dashboard](./amazon-store-dashboard.md).

The order import settings are set to `Enabled` by default, which means that your Amazon orders appear on the store dashboard and create corresponding [!DNL Commerce] orders. Imported orders can be managed in the [!DNL Commerce] [Orders](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html) workflow.

>[!NOTE]
>
>Regardless of your order settings, Amazon orders that existed before your store integration are not imported.

After [store integration](./store-integration.md) is complete, you can change your order settings. If you set your order settings to `Disabled`, Amazon orders are displayed on the store dashboard but must be managed in your [!DNL Amazon Seller Central] account.

When an order is created on Amazon, it is not immediately imported into [!DNL Commerce]. Amazon assigns a `Pending` status to newly created orders. After Amazon verifies the order and payment method, the order's status is changed to `Unshipped`. This status change triggers the order import, and [!DNL Commerce] creates a matching, corresponding order.

Orders imported from Amazon can be managed in the [!DNL Commerce] [orders workflow](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html). See also [Manage Orders](./managing-orders.md).

## Configure order settings {#configure-order-settings}

1. Click **[!UICONTROL Order Settings]** on the store dashboard.

1. For **[!UICONTROL Import Amazon Orders]** (required), choose an option:

    - `Disabled` - Choose when you do not want to create corresponding orders in [!DNL Commerce] when new orders are received from Amazon. When chosen, all other fields on this page are disabled.

    - `Enabled` - (Default) Choose when you want to create corresponding [!DNL Commerce] orders when new orders are received from Amazon. [!DNL Commerce] orders are created based on Amazon status and stock levels.

      >[!NOTE]
      >
      >Import Amazon Orders must be set to `Enabled` to manage Amazon orders in the [!DNL Commerce] [orders](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html) workflow. When set to `Disabled`, your Amazon orders do not have a corresponding [!DNL Commerce] order number and cannot be managed in [!DNL Commerce]. You manage these orders in your [!DNL Amazon Seller Central] account.

1. For **[!UICONTROL Import Amazon Orders Into Magento Store]**, choose which [!DNL Commerce] store the Amazon orders are associated with when the corresponding order is created in [!DNL Commerce].

   This setting defaults to the Store View for the website selected when you [added the Amazon store](./store-integration.md). If you want to change this setting, the list of options depends on the [!DNL Commerce] stores you have set up in your configuration. See [Stores](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/store-views.html).

1. For **[!UICONTROL Customer Creation]**, choose an option:

    - `No Customer Creation (guest)` - (Default) Choose when you do not want to create a customer account in [!DNL Commerce] using the imported customer data from the Amazon order. When chosen, [!DNL Commerce] processes an imported Amazon order the same way it processes a guest checkout in [!DNL Commerce].

    - `Build New Customer Account` - Choose when you want to create a New Customer Account in [!DNL Commerce] using the customer data imported with the Amazon order. This option helps build your customer database from your Amazon orders.

1. For **[!UICONTROL Order Number Source]**, choose an option:

    - `Build Using Magento Order Number` - (Default) Choose when you want to create a unique [!DNL Commerce] order number for the corresponding Amazon order using the [!DNL Commerce] incrementally assigned order ID.

    - `Build Using Amazon Order Number` - Choose when you want to create the [!DNL Commerce] order number using the corresponding Amazon-assigned order number.

    >[!NOTE]
    >
    >After an order is imported, the Amazon order number shows in the _[!UICONTROL Recent Orders]_ list on the store dashboard. The [!DNL Commerce] order number shows when viewing the order details in the [!DNL Commerce] [Orders](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html) workspace.

1. For **[!UICONTROL Order Status]** (required), choose an option:

    - `Default Order Status` - (Default) Choose when you want newly created orders imported from Amazon to be assigned your defined default order status for new orders. The default status for new orders (unless you have created a custom order status for new orders) is `Pending`. See [Processing Orders](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order).

    - `Custom Order Status` - Choose when you want newly created orders imported from Amazon to be assigned a status other than the default.

    - `Processing Order Status` - Enabled when **[!UICONTROL Order Status]** is set to `Custom Order Status`. Choose the status you want to use for newly created orders imported from Amazon. The options in this field are based on the default status options in [!DNL Commerce]. See [Order Status](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-status.html). You can also create a custom order status to show here for selection. To create a custom order status, see [Custom Order Status](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-status.html#custom-order-status).

1. When complete, click **[!UICONTROL Save order settings]**.

![Order settings](assets/amazon-order-settings.png){width="600" zoomable="yes"}

| Field                                                | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
|------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Import Amazon Orders]                    | Options:<ul><li>**[!UICONTROL Disabled]** - Choose when you do not want to create corresponding orders in [!DNL Commerce] when new orders are received from Amazon. When chosen, all other fields on this page are disabled.</li><li>**[!UICONTROL Enabled]** - (Default) Choose when you want to create corresponding [!DNL Commerce] orders when new orders are received from Amazon. [!DNL Commerce] orders are created based on Amazon status and stock levels.</li></ul><br><br>`Enabled` must be chosen to manage Amazon orders in [!DNL Commerce]. When `Disabled` is chosen, your Amazon orders are displayed on the store dashboard, but the orders must be managed in your [!DNL Amazon Seller Central] account.                                                                                  |
| [!UICONTROL Import Amazon Orders Into Magento Store] | Choose which [!DNL Commerce] store the Amazon orders are associated with when they are created in the [!DNL Commerce] [Orders](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html) workspace. This setting defaults to the Store View for the [!DNL Commerce] website selected when you [added the Amazon store](./store-integration.md). If you want to change this setting, the list of options depends on the [!DNL Commerce] stores you have set up in your configuration. See [Stores](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/stores.html).                                                                                                                                                               |
| [!UICONTROL Customer Creation]                       | Options:<ul><li>**[!UICONTROL No Customer Creation (guest)]** - (Default) Choose when you do not want to create a customer account in [!DNL Commerce] using the imported customer data from the Amazon order. When chosen, this option tells [!DNL Commerce] to process an imported Amazon order the same way it processes a guest checkout.</li><li>**[!UICONTROL Build New Customer Account]** - Choose when you want to create a New Customer Account in your [!DNL Commerce] customer database using the customer data imported with the Amazon order. This option helps build your [!DNL Commerce] customer database from your Amazon orders.</li></ul>                                                                                                                                                |
| Order Number Source                                  | Options:<ul><li>**[!UICONTROL Build Using Magento Order Number]** - (Default) Choose when you want to create a unique [!DNL Commerce] order number for the corresponding Amazon order using the [!DNL Commerce] incrementally assigned order ID. </li><li>**Build Using Amazon Order Number** - Choose when you want to create the [!DNL Commerce] order number using the corresponding Amazon-assigned order number.</li></ul>                                                                                                                                                                                                                                                                                                                                                                             |
| Pending Orders                                       | Options:<ul><li>**[!UICONTROL Do Not Reserve Quantity]** - Choose when you do not want your [!DNL Commerce] stock quantity affected by your Amazon orders. Choose if you use Amazon for your fulfillment process (FBA). When chosen and you receive an Amazon order, the quantity ordered does not affect your [!DNL Commerce] stock quantity.</li><li>**[!UICONTROL Reserve Quantity]** - Choose when you want the order quantity in the Amazon order to be "reserved" in your [!DNL Commerce] stock quantity. When chosen and you receive an Amazon order, the quantity ordered will "reserve" in your [!DNL Commerce] stock quantity to prevent your [!DNL Commerce] stock from "over selling." The "reserved" quantity is not available for purchase through your [!DNL Commerce] storefront.</li></ul> |
| [!UICONTROL Order Status]                            | Options:<ul><li>**[!UICONTROL Default Order Status]** - (Default) Choose when you want newly created orders imported from Amazon to be assigned your default order status for new orders. The default status for new orders (unless you have created a custom order status for new orders) is `Pending`. See [Processing Orders](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order).</li><li>**[!UICONTROL Custom Order Status]** - Choose when you want newly created orders imported from Amazon to be assigned a status other than the default. When chosen, **[!UICONTROL Processing Order Status]** enables for you to choose the status you want to use for newly created orders imported from Amazon.</li></ul>    |
| [!UICONTROL Processing Orders Status]                | Enabled when _[!UICONTROL Order Status]_ is set to `Custom Order Status`. Choose the order status you want to assign to new orders. The options in this field depend on the default status options in [!DNL Commerce]. See [Order Status](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-status.html). You can also create a custom order status to show here. To create a custom order status, see [Custom Order Status] |                                                                       

## [!DNL Commerce] order creation

[!DNL Commerce] orders are created for Amazon orders based on the following status and inventory conditions.

### Order creation with Inventory Management

>[!NOTE]
>
>Supported in Adobe Commerce and Magento Open Source 2.3.x integrations only.

| Fulfillment Channel | [!DNL Commerce] Inventory Status          | Amazon Order Status | [!UICONTROL Create Magento Order] Setting | Inventory Reserved |
|---------------------|-------------------------------------------|---------------------|-------------------------------------------|--------------------|
| FBA                 | In-stock<br>Out-of-stock<br>Do Not Manage | Pending             | No                                        | No                 |
| FBA                 | In-stock<br>Out-of-stock<br>Do Not Manage | PendingAvailability | No                                        | No                 |
| FBA                 | In-stock<br>Out-of-stock<br>Do Not Manage | Canceled            | No                                        | No                 |
| FBA                 | In-stock<br>Out-of-stock<br>Do Not Manage | Error               | No                                        | No                 |
| FBA                 | In-stock<br>Out-of-stock<br>Do Not Manage | Unshipped           | No                                        | No                 |
| FBA                 | In-stock<br>Out-of-stock<br>Do Not Manage | PartiallyShipped    | No                                        | No                 |
| FBA                 | In-stock<br>Do Not Manage                 | Shipped             | Yes                                       | No                 |
| FBA                 | Out-of-stock                              | Shipped             | No                                        | No                 |
| FBM                 | In-stock<br>Out-of-stock<br>Do Not Manage | Pending             | No                                        | No                 |
| FBM                 | In-stock<br>Out-of-stock<br>Do Not Manage | PendingAvailability | No                                        | No                 |
| FBM                 | In-stock<br>Out-of-stock<br>Do Not Manage | Canceled            | No                                        | No                 |
| FBM                 | In-stock<br>Out-of-stock<br>Do Not Manage | Error               | No                                        | No                 |
| FBM                 | In-stock<br>Do Not Manage                 | Unshipped           | Yes                                       | Yes                |
| FBM                 | Out-of-stock                              | Unshipped           | No                                        | No                 |
| FBM                 | In-stock<br>Do Not Manage                 | PartiallyShipped    | Yes                                       | Yes                |
| FBM                 | Out-of-stock                              | PartiallyShipped    | No                                        | No                 |
| FBM                 | In-stock<br>Do Not Manage                 | Shipped             | Yes                                       | Yes                |
| FBM                 | Out-of-stock                              | Shipped             | No                                        | No                 |

>[!NOTE]
>If an Amazon order is imported in a `Partially Shipped` or `Shipped` status, the inventory reservation that is created is for all items in the order. Amazon sales channel does not compensate for items that have been previously shipped.
>
>If an order is Fulfilled by Amazon (FBA) but an item is in `out of stock` status, [!DNL Commerce] is unable to create a corresponding order. This is a limitation of Inventory Management integrations.
