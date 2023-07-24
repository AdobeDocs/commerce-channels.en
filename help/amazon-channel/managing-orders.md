---
title: Manage Amazon orders
description: You can enable order import in your Order Settings to more easily manage your Amazon orders from your Commerce Admin.
feature: Sales Channels, Orders
exl-id: 018a8936-2f03-4a2d-b9af-6b72729ca709
---
# Manage Amazon orders

You can view your Amazon order information, as received from Amazon, in the _[!UICONTROL Recent Orders]_ section of the [store dashboard](./amazon-store-dashboard.md) or on the _[!UICONTROL Amazon orders]_ page (also called the _[!UICONTROL All Orders]_ view).

How you manage your Amazon orders depends on whether the order import is enabled or disabled in your [Order Settings](./order-settings.md#configure-order-settings).

## With order import enabled

After [store integration](./store-integration.md), the [**[!UICONTROL Import Amazon Orders]**](./order-settings.md#configure-order-settings) setting is `Enabled` by default. With this setting, corresponding [!DNL Commerce] orders are created for your Amazon orders and can be managed in the [[!DNL Commerce] Orders](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html) workflow.

>[!NOTE]
>
>Regardless of your order import settings, Amazon orders that existed in your [!DNL Amazon Seller Central] account before your [store integration](./store-integration.md) are not imported.

Imported Amazon orders are managed in the [[!DNL Commerce] Orders](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html) workflow, just like your other [!DNL Commerce] stores. Click the Amazon order number in the *[!UICONTROL Order Number]* column to open the order in the [[!DNL Commerce] order process](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order#order-view-descriptions). See [View Amazon Orders](./amazon-orders-all.md).

### Order import process

When an order is placed on Amazon and [order import](./order-settings.md) is enabled, the following process begins.

| Change                                                                                                                                                                                                                     | Actions                                                                                                                                                                                                                                                                                                                                                                                                          |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| An order is placed on Amazon.                                                                                                                                                                                              | <ul><li>Amazon sets the order status to `Pending`.</li><li>Order information is sent to [!DNL Commerce].</li><li>Order is added to [_Amazon orders_ table](./amazon-orders-all.md) with a `Pending` status.</li></ul>                                                                                                                                                                                            |
| Amazon changes the order status to `Unshipped`.                                                                                                                                                                            | <ul><li>The status change is sent to [!DNL Commerce].</li><li>In the [_Amazon orders_ table](./amazon-orders-all.md), the order status changes to `Unshipped`.</li><li>In the [[!DNL Commerce] orders workflow](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html), a corresponding [!DNL Commerce] order is created with a `Processing` status.</li></ul> |
| In [[!DNL Commerce] orders workflow](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html), the [!DNL Commerce] order is processed and the status changes to `Shipped`. | <ul><li>In the [_Amazon orders_ table](./amazon-orders-all.md), the order status changes to `Shipped`.</li><li>On the next cron job, the order status changes to `Complete` in the [[!DNL Commerce] orders workflow](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html).</li></ul>                                                                         |

### Order creation blockers

There are a few scenarios that prevent the creation of the corresponding [!DNL Commerce] order. [!DNL Commerce] orders are not created for orders that are received when any of the following issues occur.

| Scenario                                                | Solution                                                                                                                                                                         |
|---------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| The item does not exist in the [!DNL Commerce] catalog. | [Create the product](./creating-assigning-catalog-products.md) in your [!DNL Commerce] catalog and [manually match](./creating-assigning-catalog-products.md) it to the product. |
| The item in the catalog is disabled.                    | Make sure that the [product status](https://experienceleague.adobe.com/docs/commerce-admin/inventory/configuration/product-options.html) is enabled.                             |
| The ordered item is out of stock.                       | Update or configure the [product options](https://experienceleague.adobe.com/docs/commerce-admin/inventory/configuration/product-options.html) for quantity and source.          |

When orders cannot be imported, a system message similar to the following appears at the top of the screen:

   `Your Amazon store(s) has orders that cannot be imported into [!DNL Commerce]. See Recent Orders in the store dashboard(s): <store name>`

When the issue is resolved, the [!DNL Commerce] order is created on the next sync.

## With order import disabled

If you do not want to import and manage your Amazon orders in [!DNL Commerce], you can change the [**[!UICONTROL Import Amazon Orders]**](./order-settings.md#configure-order-settings) setting to `Disabled`. This setting means that when new orders are received from Amazon, corresponding [!DNL Commerce] orders are not created.

When disabled, order information received from Amazon appears in the _[!UICONTROL Recent Orders]_ section of the store dashboard and in the _[!UICONTROL All Orders]_ view. This order information is view-only, and you must manage these orders in [!DNL Amazon Seller Central]. To open the order details in [!DNL Amazon Seller Central], click the Amazon order number in the _[!UICONTROL Order Number]_ column.

See also [View Amazon Orders](./amazon-orders-all.md), [View Amazon Order Details](./amazon-order-details.md), and [Common Order Processing Tasks](./common-order-processing.md).
