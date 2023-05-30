---
title: Common Order Processing Tasks
description: Use the corresponding [!DNL Commerce] orders created for Amazon orders to manage order activity and processing in the [!UICONTROL Commerce] Admin.
exl-id: a44f36f0-db18-4de5-9c5b-cc68f4793008
---
# Common Order Processing Tasks

[[!DNL Commerce] order processing](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order) can manage your Amazon orders, including emailing the buyer, fulfilling the order (shipping), issuing credits/refunds, adding comments, and more. To manage your Amazon orders, your [**Import Amazon Orders**](./order-settings.md) setting must be set to `Enabled` so that corresponding [!DNL Commerce] orders are created when Amazon orders are received. Amazon order information shows in the *[!UICONTROL Recent Orders]* section of the store dashboard.

When enabled, corresponding [!DNL Commerce] orders are created for Amazon orders, and the Amazon order number shows in the _[!UICONTROL Order Number]_ column. If a corresponding [!DNL Commerce] order is created, click the order number to open the order in the [!DNL Commerce] [order processing](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order) page. You can manage the order as you do your other [[!DNL Commerce] order processing](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order).

The [!DNL Commerce] order number does not show with the _[!UICONTROL Recent Orders]_ information. The [!DNL Commerce] order number only shows when you click the order number on the store dashboard and open the order in [[!DNL Commerce] order processing](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order). When viewing the [!DNL Commerce] order, the Amazon Order number appears in the *[!UICONTROL Payment & Shipping Method]* section. It also includes options to *[!UICONTROL View or Cancel Amazon Order]* and *[!UICONTROL View all Amazon Orders]*, depending on the order shipping status.

See [cancel an unshipped order](./cancel-unshipped-order.md).

![Amazon Order info in the Commerce order](assets/amazon-order-number-payment-info.png){width="500"}

When processing an Amazon order, Amazon sales channel updates and syncs the order information with your [!DNL Amazon Seller Central] account. Your cron settings determine how often order information is synced between Amazon and Amazon sales channel.

Common [!DNL Commerce] [order processing](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order) tasks include:

- [Order Actions](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html#actions)
- [Order Search](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html#order-search)
- [Process an Order](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order)
  - [View an Order](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order#view-an-order)
  - [Process an Order](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order#process-an-order)
  - [Order and Account Information](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order#order-and-account-information)
  - [Address Information](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order#address-information)
  - [Payment & Shipping Method](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order#payment--shipping-method)
  - [Review items ordered](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order#review-items-ordered)
- [Issuing a credit/refund](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/credit-memos/credit-memo-create.html)
- [Fulfilling/shipping an order](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/shipments.html#create-a-shipment)
- [Create an invoice](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/invoices.html#create-an-invoice)
- [Cancel an unshipped order](./cancel-unshipped-order.md)

>[!NOTE]
>
>If an order is in `Unshipped` status, you can [cancel an Amazon order](./cancel-unshipped-order.md) on the [[!UICONTROL Amazon Order Details]](./amazon-order-details.md) page. If an order has been shipped, it cannot be canceled.

See [Commerce Order Management](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/introduction.html#order-management-and-operations).
