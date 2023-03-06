---
title: Common Order Processing Tasks
description: Use the corresponding [!DNL Commerce] orders created for Amazon orders to manage order activity and processing in the [!UICONTROL Commerce] Admin.
exl-id: a44f36f0-db18-4de5-9c5b-cc68f4793008
---
# Common Order Processing Tasks

[[!DNL Commerce] order processing](https://docs.magento.com/user-guide/sales/order-processing.html){target="_blank"} can manage your Amazon orders, including emailing the buyer, fulfilling the order (shipping), issuing credits/refunds, adding comments, and more. To manage your Amazon orders, your [**Import Amazon Orders**](./order-settings.md) setting must be set to `Enabled` so that corresponding [!DNL Commerce] orders are created when Amazon orders are received. Amazon order information shows in the *[!UICONTROL Recent Orders]* section of the store dashboard.

When enabled, corresponding [!DNL Commerce] orders are created for Amazon orders, and the Amazon order number shows in the _[!UICONTROL Order Number]_ column. If a corresponding [!DNL Commerce] order is created, click the order number to open the order in the [!DNL Commerce] [order processing](https://docs.magento.com/user-guide/sales/order-processing.html){target="_blank"} page. You can manage the order as you do your other [[!DNL Commerce] order processing](https://docs.magento.com/user-guide/sales/order-processing.html){target="_blank"}.

The [!DNL Commerce] order number does not show with the _[!UICONTROL Recent Orders]_ information. The [!DNL Commerce] order number only shows when you click the order number on the store dashboard and open the order in [[!DNL Commerce] order processing](https://docs.magento.com/user-guide/sales/order-processing.html){target="_blank"}. When viewing the [!DNL Commerce] order, the Amazon Order number appears in the *[!UICONTROL Payment & Shipping Method]* section. It also includes options to *[!UICONTROL View or Cancel Amazon Order]* and *[!UICONTROL View all Amazon Orders]*, depending on the order shipping status.

See [cancel an unshipped order](./cancel-unshipped-order.md).

![Amazon Order info in the Commerce order](assets/amazon-order-number-payment-info.png)

When processing an Amazon order, Amazon sales channel updates and syncs the order information with your [!DNL Amazon Seller Central] account. Your cron settings determine how often order information is synced between Amazon and Amazon sales channel.

Common [!DNL Commerce] [order processing](https://docs.magento.com/user-guide/sales/order-processing.html){target="_blank"} tasks include:

- [Order Actions](https://docs.magento.com/user-guide/sales/order-actions.html){target="_blank"}
- [Order Search](https://docs.magento.com/user-guide/sales/orders-search.html){target="_blank"}
- [Process an Order](https://docs.magento.com/user-guide/sales/order-processing.html){target="_blank"}
  - [View an Order](https://docs.magento.com/user-guide/sales/order-processing.html#view-an-order){target="_blank"}
  - [Process an Order](https://docs.magento.com/user-guide/sales/order-processing.html#process-an-order){target="_blank"}
  - [Order and Account Information](https://docs.magento.com/user-guide/sales/order-processing.html#order-and-account-information){target="_blank"}
  - [Address Information](https://docs.magento.com/user-guide/sales/order-processing.html#address-information){target="_blank"}
  - [Payment & Shipping Method](https://docs.magento.com/user-guide/sales/order-processing.html#payment--shipping-method){target="_blank"}
  - [Review items ordered](https://docs.magento.com/user-guide/sales/order-processing.html#review-items-ordered){target="_blank"}
- [Issuing a credit/refund](https://docs.magento.com/user-guide/sales/credit-memo-create.html){target="_blank"}
- [Fulfilling/shipping an order](https://docs.magento.com/user-guide/sales/shipments-create.html){target="_blank"}
- [Create an invoice](https://docs.magento.com/user-guide/sales/invoice-create.html){target="_blank"}
- [Cancel an unshipped order](./cancel-unshipped-order.md)

>[!NOTE]
>
>If an order is in `Unshipped` status, you can [cancel an Amazon order](./cancel-unshipped-order.md) on the [[!UICONTROL Amazon Order Details]](./amazon-order-details.md) page. If an order has been shipped, it cannot be canceled.

See [Commerce Order Management](https://docs.magento.com/user-guide/sales/order-management.html){target="_blank"}.
